# Comparing `tmp/python-automation-framework-0.0.3.tar.gz` & `tmp/python-automation-framework-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-automation-framework-0.0.3.tar", last modified: Thu Apr 27 13:58:49 2023, max compression
+gzip compressed data, was "python-automation-framework-0.0.4.tar", last modified: Fri Apr 28 06:24:32 2023, max compression
```

## Comparing `python-automation-framework-0.0.3.tar` & `python-automation-framework-0.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-27 13:58:49.241523 python-automation-framework-0.0.3/
--rw-r--r--   0 mikereiche   (502) staff       (20)     3142 2023-04-27 13:58:49.241405 python-automation-framework-0.0.3/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)     2892 2023-04-27 13:56:48.000000 python-automation-framework-0.0.3/README.md
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-27 13:58:49.239939 python-automation-framework-0.0.3/paf/
--rw-r--r--   0 mikereiche   (502) staff       (20)     5681 2023-04-27 06:57:02.000000 python-automation-framework-0.0.3/paf/assertion.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2567 2023-04-27 06:43:23.000000 python-automation-framework-0.0.3/paf/common.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2242 2023-04-19 16:02:07.000000 python-automation-framework-0.0.3/paf/component.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      309 2023-04-25 06:43:36.000000 python-automation-framework-0.0.3/paf/config.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2430 2023-04-26 13:34:30.000000 python-automation-framework-0.0.3/paf/control.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      104 2023-04-14 17:12:01.000000 python-automation-framework-0.0.3/paf/dom.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1913 2023-04-20 08:51:37.000000 python-automation-framework-0.0.3/paf/javascript.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2476 2023-04-17 22:07:55.000000 python-automation-framework-0.0.3/paf/locator.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     4067 2023-04-24 14:19:04.000000 python-automation-framework-0.0.3/paf/manager.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2737 2023-04-27 09:49:20.000000 python-automation-framework-0.0.3/paf/page.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2476 2023-04-25 06:48:40.000000 python-automation-framework-0.0.3/paf/request.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      209 2023-04-19 09:45:36.000000 python-automation-framework-0.0.3/paf/types.py
--rw-r--r--   0 mikereiche   (502) staff       (20)    11207 2023-04-27 13:10:54.000000 python-automation-framework-0.0.3/paf/uielement.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     6570 2023-04-27 13:27:22.000000 python-automation-framework-0.0.3/paf/xpath.py
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-27 13:58:49.240508 python-automation-framework-0.0.3/python_automation_framework.egg-info/
--rw-r--r--   0 mikereiche   (502) staff       (20)     3142 2023-04-27 13:58:49.000000 python-automation-framework-0.0.3/python_automation_framework.egg-info/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)      630 2023-04-27 13:58:49.000000 python-automation-framework-0.0.3/python_automation_framework.egg-info/SOURCES.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-04-27 13:58:49.000000 python-automation-framework-0.0.3/python_automation_framework.egg-info/dependency_links.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       46 2023-04-27 13:58:49.000000 python-automation-framework-0.0.3/python_automation_framework.egg-info/requires.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)        4 2023-04-27 13:58:49.000000 python-automation-framework-0.0.3/python_automation_framework.egg-info/top_level.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-04-27 13:58:49.241554 python-automation-framework-0.0.3/setup.cfg
--rw-r--r--   0 mikereiche   (502) staff       (20)      587 2023-04-27 13:58:47.000000 python-automation-framework-0.0.3/setup.py
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-27 13:58:49.241252 python-automation-framework-0.0.3/test/
--rw-r--r--   0 mikereiche   (502) staff       (20)     1065 2023-04-20 13:21:10.000000 python-automation-framework-0.0.3/test/test_components.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      569 2023-04-19 16:18:15.000000 python-automation-framework-0.0.3/test/test_javascript.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1383 2023-04-24 14:20:50.000000 python-automation-framework-0.0.3/test/test_page.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1435 2023-04-24 13:08:49.000000 python-automation-framework-0.0.3/test/test_request.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     3174 2023-04-27 13:24:00.000000 python-automation-framework-0.0.3/test/test_uielement.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      456 2023-04-21 09:51:14.000000 python-automation-framework-0.0.3/test/test_webdriver.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1148 2023-04-27 13:25:36.000000 python-automation-framework-0.0.3/test/test_xpath.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 06:24:32.077359 python-automation-framework-0.0.4/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3115 2023-04-28 06:24:32.077209 python-automation-framework-0.0.4/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2865 2023-04-27 14:24:03.000000 python-automation-framework-0.0.4/README.md
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 06:24:32.075389 python-automation-framework-0.0.4/paf/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     5741 2023-04-27 19:14:21.000000 python-automation-framework-0.0.4/paf/assertion.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2567 2023-04-27 06:43:23.000000 python-automation-framework-0.0.4/paf/common.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2283 2023-04-28 06:10:19.000000 python-automation-framework-0.0.4/paf/component.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      309 2023-04-25 06:43:36.000000 python-automation-framework-0.0.4/paf/config.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2430 2023-04-26 13:34:30.000000 python-automation-framework-0.0.4/paf/control.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      104 2023-04-14 17:12:01.000000 python-automation-framework-0.0.4/paf/dom.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1913 2023-04-20 08:51:37.000000 python-automation-framework-0.0.4/paf/javascript.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2544 2023-04-27 19:06:53.000000 python-automation-framework-0.0.4/paf/locator.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     4249 2023-04-27 19:41:20.000000 python-automation-framework-0.0.4/paf/manager.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2737 2023-04-27 09:49:20.000000 python-automation-framework-0.0.4/paf/page.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2476 2023-04-25 06:48:40.000000 python-automation-framework-0.0.4/paf/request.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      209 2023-04-19 09:45:36.000000 python-automation-framework-0.0.4/paf/types.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)    11014 2023-04-28 06:15:37.000000 python-automation-framework-0.0.4/paf/uielement.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     6570 2023-04-27 13:27:22.000000 python-automation-framework-0.0.4/paf/xpath.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 06:24:32.076044 python-automation-framework-0.0.4/python_automation_framework.egg-info/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3115 2023-04-28 06:24:32.000000 python-automation-framework-0.0.4/python_automation_framework.egg-info/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)      631 2023-04-28 06:24:32.000000 python-automation-framework-0.0.4/python_automation_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-04-28 06:24:32.000000 python-automation-framework-0.0.4/python_automation_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       46 2023-04-28 06:24:32.000000 python-automation-framework-0.0.4/python_automation_framework.egg-info/requires.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)        4 2023-04-28 06:24:32.000000 python-automation-framework-0.0.4/python_automation_framework.egg-info/top_level.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-04-28 06:24:32.077400 python-automation-framework-0.0.4/setup.cfg
+-rw-r--r--   0 mikereiche   (502) staff       (20)      587 2023-04-28 06:24:24.000000 python-automation-framework-0.0.4/setup.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 06:24:32.077015 python-automation-framework-0.0.4/test/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1060 2023-04-28 06:09:33.000000 python-automation-framework-0.0.4/test/test_component.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      569 2023-04-19 16:18:15.000000 python-automation-framework-0.0.4/test/test_javascript.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1292 2023-04-27 18:53:01.000000 python-automation-framework-0.0.4/test/test_locator.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1440 2023-04-27 19:24:35.000000 python-automation-framework-0.0.4/test/test_page.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1673 2023-04-27 19:37:23.000000 python-automation-framework-0.0.4/test/test_request.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     5537 2023-04-28 06:07:23.000000 python-automation-framework-0.0.4/test/test_uielement.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      844 2023-04-27 19:22:39.000000 python-automation-framework-0.0.4/test/test_webdriver.py
```

### Comparing `python-automation-framework-0.0.3/PKG-INFO` & `python-automation-framework-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,24 @@
 Metadata-Version: 2.1
 Name: python-automation-framework
-Version: 0.0.3
+Version: 0.0.4
 Summary: Automation framework for the WebDriver API
 Home-page: https://github.com/mreiche/python-automation-framework
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 
 # PAF - Python Automation Framework
 
 Python implementation of [Testerra](https://github.com/telekom/testerra) API.
 
 It is basically a wrapper for Selenium *WebDriver* and *WebElement* which bring some more comfort features.
 This is not a test framework, but it implements some assertion features anyway.
 
 The basic concept is, to identify *WebElements* on every action or property accessor to prevent `StaleElementExceptions`.
 
-## Prerequisites
-
-You need at least a local *WebDriver* installed.
-
-**MacOS**
-```shell
-brew install chromedriver
-```
-
-**Windows**
-```shell
-choco install chromedriver
-```
-**Linux**
-```shell
-apt install chromedriver
-```
-
 ## Quick start
 
 ```python
 import inject
 import paf.config
 from paf.locator import By
 from paf.page import FinderPage, PageFactory
@@ -50,31 +32,40 @@
 # Create a simple finder page
 page = page_factory.create_page(FinderPage)
 
 # Visit URL
 page.open("https://google.com")
 
 # Find element
-element = page.find(By.id("q"))
+element = page.find("#q")
 
 # Perform actions
 element.type("Search")
 
 # Perform assertions
 element.expect.text.be("Search")
 ```
 
+### Prerequisites
+
+- You need at least a local *WebDriver* installed.
+   ```shell
+   brew|choco|apt install chromedriver
+   ```
+
+- Python 3.10 (or higher).
 
 ## Feature list
 
 - [UiElements](doc/uielement.md)
 - [Locators](doc/locators.md)
 - [Page objects](doc/pages.md)
 - [Components](doc/components.md)
 - [Managing WebDrivers](doc/webdriver.md)
+- [Execution controlling](doc/control.md)
 
 ### Missing features (todos)
 
 - Rect assertions
 - ContextClick/DoubleClick actions
 - Frames/ShadowRoot support
```

### Comparing `python-automation-framework-0.0.3/README.md` & `python-automation-framework-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,32 +3,14 @@
 Python implementation of [Testerra](https://github.com/telekom/testerra) API.
 
 It is basically a wrapper for Selenium *WebDriver* and *WebElement* which bring some more comfort features.
 This is not a test framework, but it implements some assertion features anyway.
 
 The basic concept is, to identify *WebElements* on every action or property accessor to prevent `StaleElementExceptions`.
 
-## Prerequisites
-
-You need at least a local *WebDriver* installed.
-
-**MacOS**
-```shell
-brew install chromedriver
-```
-
-**Windows**
-```shell
-choco install chromedriver
-```
-**Linux**
-```shell
-apt install chromedriver
-```
-
 ## Quick start
 
 ```python
 import inject
 import paf.config
 from paf.locator import By
 from paf.page import FinderPage, PageFactory
@@ -42,31 +24,40 @@
 # Create a simple finder page
 page = page_factory.create_page(FinderPage)
 
 # Visit URL
 page.open("https://google.com")
 
 # Find element
-element = page.find(By.id("q"))
+element = page.find("#q")
 
 # Perform actions
 element.type("Search")
 
 # Perform assertions
 element.expect.text.be("Search")
 ```
 
+### Prerequisites
+
+- You need at least a local *WebDriver* installed.
+   ```shell
+   brew|choco|apt install chromedriver
+   ```
+
+- Python 3.10 (or higher).
 
 ## Feature list
 
 - [UiElements](doc/uielement.md)
 - [Locators](doc/locators.md)
 - [Page objects](doc/pages.md)
 - [Components](doc/components.md)
 - [Managing WebDrivers](doc/webdriver.md)
+- [Execution controlling](doc/control.md)
 
 ### Missing features (todos)
 
 - Rect assertions
 - ContextClick/DoubleClick actions
 - Frames/ShadowRoot support
```

### Comparing `python-automation-framework-0.0.3/paf/assertion.py` & `python-automation-framework-0.0.4/paf/assertion.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,37 +10,39 @@
 class Format:
     @staticmethod
     def param(value: any):
         if value is None:
             return "[null]"
         else:
             return f"[{value}]"
-
-    @staticmethod
-    def separate(*args):
-        return " ".join(map(str, args))
+    #
+    # @staticmethod
+    # def separate(*args):
+    #     return " ".join(map(str, args))
 
 
 class AbstractPropertyAssertion:
     def __init__(
         self,
         parent: None | object,
         actual: Supplier[any],
         subject: Supplier[str],
         raise_exception: bool = True,
         failed: Callable = None,
         passed: Callable = None,
         failed_finally: Callable = None
     ):
+        self._raise = raise_exception
+
         if parent:
             assert isinstance(parent, AbstractPropertyAssertion)
+            self._raise = parent._raise
 
         self._parent = parent
         self._actual = actual
-        self._raise = raise_exception
         self._subject = subject
         self._failed = failed
         self._passed = passed
         self._failed_finally = failed_finally
 
     def _test_sequence(
         self,
@@ -156,15 +158,15 @@
     def matches(self, regex: str | re.Pattern):
         if not isinstance(regex, re.Pattern):
             regex = re.compile(regex, re.MULTILINE | re.IGNORECASE | re.UNICODE)
 
         return BinaryAssertion(
             parent=self,
             actual=lambda: regex.search(self._actual()) is not None,
-            subject=lambda: f"matches {Format.param(regex)}",
+            subject=lambda: f"matches {Format.param(regex.pattern)}",
         )
 
     def has_words(self, *words: any):
         if not isinstance(words, Iterable):
             words = [words]
 
         pattern = "|".join(words)
```

### Comparing `python-automation-framework-0.0.3/paf/common.py` & `python-automation-framework-0.0.4/paf/common.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.3/paf/component.py` & `python-automation-framework-0.0.4/paf/component.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from typing import TypeVar, Generic, List
 
 from selenium.webdriver.remote.webelement import WebElement
+from selenium.webdriver.support.color import Color
 
 from paf.common import HasParent, Locator, Point
 from paf.uielement import UiElement, UiElementActions, PageObject, TestableUiElement, PageObjectList
 
 T = TypeVar("T")
 
 
-class Component(Generic[T], HasParent, UiElementActions, TestableUiElement, PageObject[T]):
+class Component(Generic[T], HasParent, UiElementActions, TestableUiElement, PageObject[T], PageObjectList[T]):
+
+    def highlight(self, color: Color = Color.from_string("#0f0"), seconds: float = 2):
+        self._ui_element.highlight(color, seconds)
+        return self
 
     def __init__(self, ui_element: UiElement):
         self._ui_element = ui_element
         ui_element._parent = self
 
     def click(self):
         self._ui_element.click()
@@ -38,17 +43,17 @@
     @property
     def name(self):
         return f"{self.__class__.__name__}({self._ui_element.name})"
 
     def __str__(self):
         return self.name
 
-    @property
-    def list(self):
-        return ComponentList[T](self)
+    # @property
+    # def list(self):
+    #     return ComponentList[T](self)
 
     @property
     def expect(self):
         return self._ui_element.expect
 
     @property
     def wait_for(self):
@@ -56,27 +61,21 @@
 
     def scroll_into_view(self, offset: Point = Point()):
         self._ui_element.scroll_into_view(offset)
 
     def scroll_to_top(self, offset: Point = Point()):
         self._ui_element.scroll_to_top(offset)
 
-
-class ComponentList(PageObjectList[T]):
-
-    def __init__(self, component: Component[T]):
-        self._component = component
-
     def __iter__(self):
-        for i in range(self._component._ui_element._count_elements()):
+        for i in range(self._ui_element._count_elements()):
             yield self.__getitem__(i)
 
     def __getitem__(self, index: int) -> T:
         ui_element = UiElement(
-            ui_element=self._component._ui_element._ui_element,
-            webdriver=self._component._ui_element._webdriver,
-            by=self._component._ui_element._by,
+            ui_element=self._ui_element._ui_element,
+            webdriver=self._ui_element._webdriver,
+            by=self._ui_element._by,
             index=index
         )
-        component = self._component.__class__(ui_element)
-        component._parent = self._component._parent
+        component = self.__class__(ui_element)
+        component._parent = self._parent
         return component
```

### Comparing `python-automation-framework-0.0.3/paf/control.py` & `python-automation-framework-0.0.4/paf/control.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.3/paf/javascript.py` & `python-automation-framework-0.0.4/paf/javascript.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.3/paf/locator.py` & `python-automation-framework-0.0.4/paf/locator.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,19 +80,19 @@
         if self._filter:
             id += " filtered"
         return id
 
     def to_xpath(self):
         from paf.xpath import XPath
 
-        if self._by.XPATH:
+        if self._by == SeleniumBy.XPATH:
             return XPath.at(self._value)
-        elif self._by.NAME:
+        elif self._by == SeleniumBy.NAME:
             return XPath.at("//*").attribute(Attribute.NAME).be(self._value)
-        elif self._by.CLASS_NAME:
+        elif self._by == SeleniumBy.CLASS_NAME:
             return XPath.at("//*").attribute(Attribute.CLASS).be(self._value)
-        elif self._by.ID:
+        elif self._by == SeleniumBy.ID:
             return XPath.at("//*").attribute(Attribute.ID).be(self._value)
-        elif self._by.CLASS_NAME:
+        elif self._by == SeleniumBy.TAG_NAME:
             return XPath.at(self._value)
         else:
             raise Exception(f"By type '{self.by}' not supported (yet)")
```

### Comparing `python-automation-framework-0.0.3/paf/manager.py` & `python-automation-framework-0.0.4/paf/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import logging
 import os
-import threading
+from datetime import datetime
 from pathlib import Path
 from typing import Type, TypeVar, Iterable
-from datetime import datetime
 
 import inject
 from is_empty import empty
 from selenium.webdriver import Chrome, Firefox, Edge, Safari, Remote, ChromeOptions, EdgeOptions, FirefoxOptions, WPEWebKitOptions
 from selenium.webdriver.common.options import BaseOptions
 from selenium.webdriver.remote.webdriver import WebDriver, BaseWebDriver
 
-from paf.common import Property
+from paf.common import Property, Formatter
 from paf.request import WebDriverRequest
-from paf.types import Consumer
 
 OPTION = TypeVar("OPTION")
 
 LOG = logging.getLogger(__name__)
 
 
 class WebDriverManager:
@@ -76,15 +74,18 @@
         if request.window_size:
             LOG.info(f"Set window size: {request.window_size}")
             webdriver.set_window_rect(0, 0, request.window_size.width, request.window_size.height)
 
         return webdriver
 
     def shutdown_session(self, session_key):
-        pass
+        if session_key in self._session_driver_map:
+            self.shutdown(self._session_driver_map[session_key])
+        else:
+            raise Exception(f"Unknown session: {session_key}")
 
     def shutdown(self, webdriver: WebDriver):
         webdriver.quit()
         webdrivers = list(self._session_driver_map.values())
         index = webdrivers.index(webdriver)
 
         session_keys = list(self._session_driver_map.keys())
@@ -97,15 +98,17 @@
 
     def take_screenshot(self, webdriver: WebDriver) -> Path|None:
         dir = Path(os.getenv(Property.PAF_SCREENSHOTS_DIR.name, Property.PAF_SCREENSHOTS_DIR.value))
         title = webdriver.title
         if empty(title):
             title = webdriver.current_url
 
-        file_name = f"{title}-{datetime.now().strftime('%Y-%m-%d-%H:%M:%S')}.png"
+        formatter = inject.instance(Formatter)
+
+        file_name = f"{title}-{formatter.datetime(datetime.now())}.png"
         dir.mkdir(parents=True, exist_ok=True)
         path = dir/file_name
         if webdriver.save_screenshot(dir / file_name):
             return path
         else:
             return None
```

### Comparing `python-automation-framework-0.0.3/paf/page.py` & `python-automation-framework-0.0.4/paf/page.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.3/paf/request.py` & `python-automation-framework-0.0.4/paf/request.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.3/paf/uielement.py` & `python-automation-framework-0.0.4/paf/uielement.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from selenium.webdriver.common.by import By as SeleniumBy
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support.color import Color
 
 import paf.javascript as script
 from paf.assertion import StringAssertion, Format, BinaryAssertion, QuantityAssertion
-from paf.common import HasParent, Locator, Point, Rect, Property
+from paf.common import HasParent, Locator, Point, Rect, Property, Formatter
 from paf.control import Control
 from paf.locator import By
 from paf.types import Mapper, Consumer, R
 from paf.xpath import XPath
 
 
 class UiElementActions:
@@ -56,18 +56,14 @@
 
     @property
     def last(self) -> T:
         return self.__getitem__(-1)
 
 
 class PageObject(Generic[T]):
-    @property
-    @abstractmethod
-    def list(self) -> PageObjectList[T]:
-        pass
 
     @abstractmethod
     def scroll_into_view(self, offset: Point = Point()):
         pass
 
     @abstractmethod
     def scroll_to_top(self, offset: Point = Point()):
@@ -90,15 +86,15 @@
         pass
 
 
 class InteractiveUiElement(TestableUiElement, UiElementActions, PageObject["InteractiveUiElement"], ABC):
     pass
 
 
-class UiElement(InteractiveUiElement, HasParent):
+class UiElement(InteractiveUiElement, HasParent, PageObjectList["UiElement"]):
 
     def __init__(
         self,
         by: Locator,
         ui_element: "UiElement" = None,
         webdriver: WebDriver = None,
         parent: object = None,
@@ -126,15 +122,15 @@
             ui_element=self,
             webdriver=self._webdriver,
             parent=self
         )
 
     def __relative_selector(self, by: By):
         if by.by == SeleniumBy.XPATH:
-            return by.value.replace("/", "./", 1)
+            return by.value.replace("/", "./", 0)
         else:
             return by.value
 
     def _find_web_elements(self, consumer: Mapper[List[WebElement], R]) -> R:
         if self._ui_element:
             def _handle(web_element: WebElement):
                 value = self.__relative_selector(self._by)
@@ -178,18 +174,19 @@
         self._action_sequence(lambda web_element: web_element.click())
         return self
 
     def send_keys(self, value: str):
         self._action_sequence(lambda web_element: web_element.send_keys(value))
         return self
 
-    def take_screenshot(self) -> Path|None:
+    def take_screenshot(self) -> Path | None:
         def _handle(web_element: WebElement):
             dir = Path(Property.env(Property.PAF_SCREENSHOTS_DIR))
-            file_name = f"{self.name}-{datetime.now().strftime('%Y-%m-%d-%H:%M:%S')}.png"
+            formatter = inject.instance(Formatter)
+            file_name = f"{self.name}-{formatter.datetime(datetime.now())}.png"
             dir.mkdir(parents=True, exist_ok=True)
             path = dir / file_name
             if web_element.screenshot(str(path)):
                 return path
             else:
                 return None
 
@@ -219,17 +216,17 @@
     def __str__(self):
         return self.name
 
     @property
     def name(self):
         return f"UiElement({self._by.__str__()})[{self._index}]"
 
-    @property
-    def list(self) -> "UiElementList":
-        return UiElementList(self)
+    # @property
+    # def list(self) -> "UiElementList":
+    #     return UiElementList(self)
 
     def scroll_into_view(self, offset: Point = Point()):
         self._action_sequence(lambda web_element: script.scroll_to_center(self._webdriver, web_element, offset))
 
     def scroll_to_top(self, offset: Point = Point()):
         self._action_sequence(lambda web_element: script.scroll_to_top(self._webdriver, web_element, offset))
 
@@ -241,34 +238,28 @@
             count = len(web_elements)
 
         self._find_web_elements(_count)
         return count
 
     def highlight(self, color: Color = Color.from_string("#0f0"), seconds: float = 2):
         def _handle(web_element: WebElement):
-            script.highlight(self._webdriver, web_element, color, math.floor(seconds*1000))
+            script.highlight(self._webdriver, web_element, color, math.floor(seconds * 1000))
 
         self.find_web_element(_handle)
 
-
-class UiElementList(PageObjectList[UiElement]):
-
-    def __init__(self, ui_element: UiElement):
-        self._ui_element = ui_element
-
     def __iter__(self):
-        for i in range(self._ui_element._count_elements()):
+        for i in range(self._count_elements()):
             yield self.__getitem__(i)
 
     def __getitem__(self, index: int):
         return UiElement(
-            ui_element=self._ui_element._ui_element,
-            webdriver=self._ui_element._webdriver,
-            by=self._ui_element._by,
-            parent=self._ui_element._parent,
+            ui_element=self._ui_element,
+            webdriver=self._webdriver,
+            by=self._by,
+            parent=self._parent,
             index=index
         )
 
 
 A = TypeVar('A')
```

### Comparing `python-automation-framework-0.0.3/paf/xpath.py` & `python-automation-framework-0.0.4/paf/xpath.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.3/python_automation_framework.egg-info/PKG-INFO` & `python-automation-framework-0.0.4/python_automation_framework.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,24 @@
 Metadata-Version: 2.1
 Name: python-automation-framework
-Version: 0.0.3
+Version: 0.0.4
 Summary: Automation framework for the WebDriver API
 Home-page: https://github.com/mreiche/python-automation-framework
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 
 # PAF - Python Automation Framework
 
 Python implementation of [Testerra](https://github.com/telekom/testerra) API.
 
 It is basically a wrapper for Selenium *WebDriver* and *WebElement* which bring some more comfort features.
 This is not a test framework, but it implements some assertion features anyway.
 
 The basic concept is, to identify *WebElements* on every action or property accessor to prevent `StaleElementExceptions`.
 
-## Prerequisites
-
-You need at least a local *WebDriver* installed.
-
-**MacOS**
-```shell
-brew install chromedriver
-```
-
-**Windows**
-```shell
-choco install chromedriver
-```
-**Linux**
-```shell
-apt install chromedriver
-```
-
 ## Quick start
 
 ```python
 import inject
 import paf.config
 from paf.locator import By
 from paf.page import FinderPage, PageFactory
@@ -50,31 +32,40 @@
 # Create a simple finder page
 page = page_factory.create_page(FinderPage)
 
 # Visit URL
 page.open("https://google.com")
 
 # Find element
-element = page.find(By.id("q"))
+element = page.find("#q")
 
 # Perform actions
 element.type("Search")
 
 # Perform assertions
 element.expect.text.be("Search")
 ```
 
+### Prerequisites
+
+- You need at least a local *WebDriver* installed.
+   ```shell
+   brew|choco|apt install chromedriver
+   ```
+
+- Python 3.10 (or higher).
 
 ## Feature list
 
 - [UiElements](doc/uielement.md)
 - [Locators](doc/locators.md)
 - [Page objects](doc/pages.md)
 - [Components](doc/components.md)
 - [Managing WebDrivers](doc/webdriver.md)
+- [Execution controlling](doc/control.md)
 
 ### Missing features (todos)
 
 - Rect assertions
 - ContextClick/DoubleClick actions
 - Frames/ShadowRoot support
```

### Comparing `python-automation-framework-0.0.3/python_automation_framework.egg-info/SOURCES.txt` & `python-automation-framework-0.0.4/python_automation_framework.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 paf/uielement.py
 paf/xpath.py
 python_automation_framework.egg-info/PKG-INFO
 python_automation_framework.egg-info/SOURCES.txt
 python_automation_framework.egg-info/dependency_links.txt
 python_automation_framework.egg-info/requires.txt
 python_automation_framework.egg-info/top_level.txt
-test/test_components.py
+test/test_component.py
 test/test_javascript.py
+test/test_locator.py
 test/test_page.py
 test/test_request.py
 test/test_uielement.py
-test/test_webdriver.py
-test/test_xpath.py
+test/test_webdriver.py
```

### Comparing `python-automation-framework-0.0.3/setup.py` & `python-automation-framework-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="python-automation-framework",
     description="Automation framework for the WebDriver API",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.0.3",
+    version="0.0.4",
     url="https://github.com/mreiche/python-automation-framework",
     author="Mike Reiche",
     packages=["paf"],
     install_requires=["inject>=4.3.1", "selenium>=4.8.3", "is-empty>=1.0.1"],
 )
```

### Comparing `python-automation-framework-0.0.3/test/test_components.py` & `python-automation-framework-0.0.4/test/test_component.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,12 +27,12 @@
     page = page_factory.create_page(MyPage)
     assert page.custom_component.type.name_path == "MyPage > MyComponent(UiElement(By.tag name(body))[0]) > UiElement(By.id(input))[0]"
 
 
 def test_component_list():
     page_factory = inject.instance(PageFactory)
     page = page_factory.create_page(MyPage)
-    assert page.custom_component.list.last.name_path == "MyPage > MyComponent(UiElement(By.tag name(body))[-1])"
+    assert page.custom_component.last.name_path == "MyPage > MyComponent(UiElement(By.tag name(body))[-1])"
 
 
 def teardown_module():
     inject.instance(WebDriverManager).shutdown_all()
```

### Comparing `python-automation-framework-0.0.3/test/test_javascript.py` & `python-automation-framework-0.0.4/test/test_javascript.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.3/test/test_page.py` & `python-automation-framework-0.0.4/test/test_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 
 def test_page():
     page = page_factory.create_page(Page, create_webdriver())
     page.open("https://testpages.herokuapp.com")
     page.expect.title.be("Selenium Test Pages")
     page.expect.url.be("https://testpages.herokuapp.com/styled/index.html")
+    assert page.webdriver.title == "Selenium Test Pages"
 
 # def test_yahoo():
 #     class YahooStartPage(Page):
 #         @property
 #         def cookie_btn(self) -> InteractiveUiElement:
 #             return self._find(By.name("agree").displayed)
 #
```

### Comparing `python-automation-framework-0.0.3/test/test_request.py` & `python-automation-framework-0.0.4/test/test_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,30 @@
+from urllib.parse import ParseResult
+
 from paf.manager import WebDriverManager
 from paf.request import WebDriverRequest
 from selenium.webdriver import ChromeOptions, Remote
 import inject
 
+
 def test_browser(monkeypatch):
     monkeypatch.setenv('PAF_BROWSER_SETTING', 'firefox')
     request = WebDriverRequest()
     assert request.browser == "firefox"
 
 
 def test_browser_version(monkeypatch):
     monkeypatch.setenv('PAF_BROWSER_SETTING', 'firefox:64')
     request = WebDriverRequest()
     assert request.browser == "firefox"
     assert request.browser_version == "64"
 
+    request.browser_version = "99"
+    assert request.browser_version == "99"
+
 
 def test_window_size(monkeypatch):
     monkeypatch.setenv('PAF_WINDOW_SIZE', '1024x768')
     request = WebDriverRequest()
     assert request.window_size.width == 1024
     assert request.window_size.height == 768
 
@@ -28,19 +34,21 @@
     request.browser = "chrome"
     request.options = ChromeOptions()
     manager = inject.instance(WebDriverManager)
     webdriver = manager.get_webdriver(request)
     assert webdriver.name == request.browser
 
 
-def test_remote_webdriver():
+def test_remote_webdriver(monkeypatch):
+    server_url = "http://127.0.0.1:4444"
+    monkeypatch.setenv('PAF_SELENIUM_SERVER_URL', server_url)
     request = WebDriverRequest()
     request.browser = "chrome"
     request.options = ChromeOptions()
-    request.server_url = "http://127.0.0.1:4444"
+    assert isinstance(request.server_url, ParseResult)
     manager = inject.instance(WebDriverManager)
     webdriver = manager.get_webdriver(request)
     assert webdriver.name == request.browser
 
 
 def teardown_module():
     manager = inject.instance(WebDriverManager)
```

### Comparing `python-automation-framework-0.0.3/test/test_uielement.py` & `python-automation-framework-0.0.4/test/test_uielement.py`

 * *Files 25% similar despite different names*

```diff
@@ -18,50 +18,76 @@
 
 def test_finder_page():
     finder = page_factory.create_page(FinderPage, create_webdriver())
     finder.open("https://testpages.herokuapp.com/styled/basic-web-page-test.html")
 
     p = finder.find(By.id("para1"))
     assert p.name_path == 'UiElement(By.id(para1))[0]'
+    assert p.name == p.name_path
 
 
 # def test_rect():
 #     finder = page_factory.create_page(FinderPage, create_webdriver())
 #     finder.open("https://testpages.herokuapp.com/styled/basic-web-page-test.html")
 #
 #     p = finder.find(By.id("para1"))
 #     rect = p._get_bounds()
 #     assert isinstance(rect, Rect)
 #     assert rect.width == 962
 #     assert rect.height == 27
 
-def test_assertions():
+def test_text_assertions():
     finder = page_factory.create_page(FinderPage, create_webdriver())
     finder.open("https://testpages.herokuapp.com/styled/basic-web-page-test.html")
 
     p = finder.find("#para1")
 
     p.expect.tag_name.be("p")
 
     text = p.expect.text
     text.be("A paragraph of text")
     text.contains("paragraph").be(True)
     text.has_words("paragraph", "text").be(True)
+    text.starts_with("A").be(True)
+    text.ends_with("text").be(True)
     text.matches("hello").be(False)
+    assert text.actual == "A paragraph of text"
 
     length = p.expect.text.length
     length.be(19)
     length.greater_than(1).be(True)
     length.greater_equal_than(10).be(True)
     length.lower_than(20).be(True)
     length.lower_equal_than(30).be(True)
     length.between(18, 20).be(True)
     length.not_be(30)
 
 
+def test_wait():
+    finder = page_factory.create_page(FinderPage, create_webdriver())
+    finder.open("https://testpages.herokuapp.com/styled/basic-web-page-test.html")
+
+    p = finder.find("#para1")
+
+    assert p.wait_for.tag_name.be("p") is True
+    assert p.wait_for.tag_name.be("b") is False
+
+
+def test_displayed():
+    finder = page_factory.create_page(FinderPage, create_webdriver())
+    finder.open("https://testpages.herokuapp.com/styled/alerts/fake-alert-test.html")
+
+    ok = finder.find("#dialog-ok")
+    btn = finder.find("#fakealert")
+
+    ok.expect.displayed.be(False)
+    btn.click()
+    ok.expect.displayed.be(True)
+
+
 def test_highlight():
     finder = page_factory.create_page(FinderPage, create_webdriver())
     finder.open("https://testpages.herokuapp.com/styled/basic-web-page-test.html")
 
     p = finder.find(By.id("para1"))
     p.highlight(color=Color.from_string("#0f0"))
     p.expect.css("outline").be("rgb(0, 255, 0) solid 5px")
@@ -73,14 +99,63 @@
 
     p = finder.find(By.id("pre1").unique)
     p.expect.visible.be(False)
     p.scroll_into_view()
     p.expect.visible.be(True)
     p.expect.fully_visible.be(True)
 
+    first = finder.find("#p1")
+    first.expect.visible.be(False)
+    first.scroll_to_top()
+    first.expect.visible.be(True)
+    p.expect.visible.be(False)
+
+
+def test_find_sub_elements_list():
+    finder = page_factory.create_page(FinderPage, create_webdriver())
+    finder.open("https://testpages.herokuapp.com/styled/find-by-playground-test.html")
+
+    # Sub elements
+    div = finder.find("#div1")
+    p = div.find("p")
+    p.expect.attribute("name").be("pName1")
+
+    # Correct XPAth
+    div.find(By.xpath("//p")).expect.attribute("name").be("pName1")
+    div.find(By.xpath("./p")).expect.attribute("name").be("pName1")
+
+    # List
+    p.first.expect.attribute("name").be("pName1")
+    p[1].expect.attribute("name").be("pName2")
+    p.last.expect.attribute("name").be("pName41")
+
+    for item in p:
+        item.expect.attribute("name").be("pName1")
+        break
+
+
+def test_form():
+    finder = page_factory.create_page(FinderPage, create_webdriver())
+    finder.open("https://testpages.herokuapp.com/styled/basic-html-form-test.html")
+
+    checkbox = finder.find(XPath.at("input").name("checkboxes[]").attribute("value").be("cb3"))
+    checkbox.expect.selected.be(True)
+
+    textarea = finder.find(By.name("comments"))
+    textarea.expect.value.be("Comments...")
+    textarea.type("Hello World")
+    textarea.expect.value.be("Hello World")
+
+    username = finder.find(By.name("username"))
+    username.expect.enabled.be(True)
+    username.send_keys("My Name")
+    username.expect.value.be("My Name")
+    username.clear()
+    username.expect.value.be("")
+
 
 def test_screenshot():
     finder = page_factory.create_page(FinderPage, create_webdriver())
     finder.open("https://testpages.herokuapp.com/styled/find-by-playground-test.html")
     p = finder.find(By.id("pre1").unique)
     path = p.take_screenshot()
     assert path
@@ -90,12 +165,12 @@
     finder = page_factory.create_page(FinderPage, create_webdriver())
     finder.open("https://testpages.herokuapp.com/styled/key-click-display-test.html")
     btn = finder.find(By.id("button").unique)
     clicks = finder.find(XPath.at("div").id("events").select("p"))
 
     control = inject.instance(Control)
     btn.click()
-    control.retry(lambda: clicks.expect.count.be(3), lambda: btn.click(), wait_after_fail=0)
+    control.retry(lambda: clicks.expect.count.be(3), lambda: btn.click(), wait_after_fail=0, count=3)
 
 
 def teardown_module():
     inject.instance(WebDriverManager).shutdown_all()
```

### Comparing `python-automation-framework-0.0.3/test/test_xpath.py` & `python-automation-framework-0.0.4/test/test_locator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from paf.locator import By
 from paf.xpath import XPath
 
 
 def test_text_functions():
     assert str(XPath.at("myElement").text.be("Exakt")) == "//myElement[.//text()='Exakt']"
     assert str(XPath.at("myElement").text.contains("Contains")) == "//myElement[contains(.//text(),'Contains')]"
     assert str(XPath.at("myElement").text.starts_with("Start")) == "//myElement[starts-with(.//text(),'Start')]"
@@ -11,14 +12,16 @@
 def test_deep_selection():
     assert str(XPath.at("button").attribute("data-qa").present.encloses("span").text.be("Klick mich")) == "//button[@data-qa and descendant::span[.//text()='Klick mich']]"
 
 
 def test_XPath_with_XPath():
     assert str(XPath.at("body").encloses(XPath.at("div"))) == "//body[descendant::div]"
 
+def test_XPath_with_By():
+    assert str(XPath.at("body").encloses(By.tag_name("div"))) == "//body[descendant::div]"
 
 def test_select_sibling():
     assert str(XPath.at("body").select("dd").text.be("Title").following("/dt")) == "//body//dd[.//text()='Title']/following-sibling::dt"
 
 
 def test_class_selection():
     assert str(XPath.at("body").select("nav").classes("container")) == "//body//nav[contains(concat(' ', normalize-space(@class), ' '), ' container ')]"
```

