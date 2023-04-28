# Comparing `tmp/python-automation-framework-0.0.4.tar.gz` & `tmp/python-automation-framework-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-automation-framework-0.0.4.tar", last modified: Fri Apr 28 06:24:32 2023, max compression
+gzip compressed data, was "python-automation-framework-0.0.5.tar", last modified: Fri Apr 28 06:54:29 2023, max compression
```

## Comparing `python-automation-framework-0.0.4.tar` & `python-automation-framework-0.0.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 06:24:32.077359 python-automation-framework-0.0.4/
--rw-r--r--   0 mikereiche   (502) staff       (20)     3115 2023-04-28 06:24:32.077209 python-automation-framework-0.0.4/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)     2865 2023-04-27 14:24:03.000000 python-automation-framework-0.0.4/README.md
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 06:24:32.075389 python-automation-framework-0.0.4/paf/
--rw-r--r--   0 mikereiche   (502) staff       (20)     5741 2023-04-27 19:14:21.000000 python-automation-framework-0.0.4/paf/assertion.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2567 2023-04-27 06:43:23.000000 python-automation-framework-0.0.4/paf/common.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2283 2023-04-28 06:10:19.000000 python-automation-framework-0.0.4/paf/component.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      309 2023-04-25 06:43:36.000000 python-automation-framework-0.0.4/paf/config.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2430 2023-04-26 13:34:30.000000 python-automation-framework-0.0.4/paf/control.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      104 2023-04-14 17:12:01.000000 python-automation-framework-0.0.4/paf/dom.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1913 2023-04-20 08:51:37.000000 python-automation-framework-0.0.4/paf/javascript.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2544 2023-04-27 19:06:53.000000 python-automation-framework-0.0.4/paf/locator.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     4249 2023-04-27 19:41:20.000000 python-automation-framework-0.0.4/paf/manager.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2737 2023-04-27 09:49:20.000000 python-automation-framework-0.0.4/paf/page.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2476 2023-04-25 06:48:40.000000 python-automation-framework-0.0.4/paf/request.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      209 2023-04-19 09:45:36.000000 python-automation-framework-0.0.4/paf/types.py
--rw-r--r--   0 mikereiche   (502) staff       (20)    11014 2023-04-28 06:15:37.000000 python-automation-framework-0.0.4/paf/uielement.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     6570 2023-04-27 13:27:22.000000 python-automation-framework-0.0.4/paf/xpath.py
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 06:24:32.076044 python-automation-framework-0.0.4/python_automation_framework.egg-info/
--rw-r--r--   0 mikereiche   (502) staff       (20)     3115 2023-04-28 06:24:32.000000 python-automation-framework-0.0.4/python_automation_framework.egg-info/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)      631 2023-04-28 06:24:32.000000 python-automation-framework-0.0.4/python_automation_framework.egg-info/SOURCES.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-04-28 06:24:32.000000 python-automation-framework-0.0.4/python_automation_framework.egg-info/dependency_links.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       46 2023-04-28 06:24:32.000000 python-automation-framework-0.0.4/python_automation_framework.egg-info/requires.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)        4 2023-04-28 06:24:32.000000 python-automation-framework-0.0.4/python_automation_framework.egg-info/top_level.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-04-28 06:24:32.077400 python-automation-framework-0.0.4/setup.cfg
--rw-r--r--   0 mikereiche   (502) staff       (20)      587 2023-04-28 06:24:24.000000 python-automation-framework-0.0.4/setup.py
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 06:24:32.077015 python-automation-framework-0.0.4/test/
--rw-r--r--   0 mikereiche   (502) staff       (20)     1060 2023-04-28 06:09:33.000000 python-automation-framework-0.0.4/test/test_component.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      569 2023-04-19 16:18:15.000000 python-automation-framework-0.0.4/test/test_javascript.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1292 2023-04-27 18:53:01.000000 python-automation-framework-0.0.4/test/test_locator.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1440 2023-04-27 19:24:35.000000 python-automation-framework-0.0.4/test/test_page.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1673 2023-04-27 19:37:23.000000 python-automation-framework-0.0.4/test/test_request.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     5537 2023-04-28 06:07:23.000000 python-automation-framework-0.0.4/test/test_uielement.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      844 2023-04-27 19:22:39.000000 python-automation-framework-0.0.4/test/test_webdriver.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 06:54:29.671743 python-automation-framework-0.0.5/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3106 2023-04-28 06:54:29.671571 python-automation-framework-0.0.5/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2856 2023-04-28 06:45:27.000000 python-automation-framework-0.0.5/README.md
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 06:54:29.668954 python-automation-framework-0.0.5/paf/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     5741 2023-04-27 19:14:21.000000 python-automation-framework-0.0.5/paf/assertion.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2567 2023-04-27 06:43:23.000000 python-automation-framework-0.0.5/paf/common.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2283 2023-04-28 06:10:19.000000 python-automation-framework-0.0.5/paf/component.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      309 2023-04-25 06:43:36.000000 python-automation-framework-0.0.5/paf/config.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2430 2023-04-26 13:34:30.000000 python-automation-framework-0.0.5/paf/control.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      104 2023-04-14 17:12:01.000000 python-automation-framework-0.0.5/paf/dom.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1913 2023-04-20 08:51:37.000000 python-automation-framework-0.0.5/paf/javascript.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2544 2023-04-27 19:06:53.000000 python-automation-framework-0.0.5/paf/locator.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     4249 2023-04-27 19:41:20.000000 python-automation-framework-0.0.5/paf/manager.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2737 2023-04-27 09:49:20.000000 python-automation-framework-0.0.5/paf/page.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2476 2023-04-25 06:48:40.000000 python-automation-framework-0.0.5/paf/request.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      209 2023-04-19 09:45:36.000000 python-automation-framework-0.0.5/paf/types.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)    12665 2023-04-28 06:51:28.000000 python-automation-framework-0.0.5/paf/uielement.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     6570 2023-04-27 13:27:22.000000 python-automation-framework-0.0.5/paf/xpath.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 06:54:29.669851 python-automation-framework-0.0.5/python_automation_framework.egg-info/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3106 2023-04-28 06:54:29.000000 python-automation-framework-0.0.5/python_automation_framework.egg-info/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)      631 2023-04-28 06:54:29.000000 python-automation-framework-0.0.5/python_automation_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-04-28 06:54:29.000000 python-automation-framework-0.0.5/python_automation_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       46 2023-04-28 06:54:29.000000 python-automation-framework-0.0.5/python_automation_framework.egg-info/requires.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)        4 2023-04-28 06:54:29.000000 python-automation-framework-0.0.5/python_automation_framework.egg-info/top_level.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-04-28 06:54:29.671788 python-automation-framework-0.0.5/setup.cfg
+-rw-r--r--   0 mikereiche   (502) staff       (20)      587 2023-04-28 06:54:24.000000 python-automation-framework-0.0.5/setup.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 06:54:29.671373 python-automation-framework-0.0.5/test/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1060 2023-04-28 06:09:33.000000 python-automation-framework-0.0.5/test/test_component.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      569 2023-04-19 16:18:15.000000 python-automation-framework-0.0.5/test/test_javascript.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1292 2023-04-27 18:53:01.000000 python-automation-framework-0.0.5/test/test_locator.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1440 2023-04-27 19:24:35.000000 python-automation-framework-0.0.5/test/test_page.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1673 2023-04-27 19:37:23.000000 python-automation-framework-0.0.5/test/test_request.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     6986 2023-04-28 06:51:10.000000 python-automation-framework-0.0.5/test/test_uielement.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      844 2023-04-27 19:22:39.000000 python-automation-framework-0.0.5/test/test_webdriver.py
```

### Comparing `python-automation-framework-0.0.4/PKG-INFO` & `python-automation-framework-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-automation-framework
-Version: 0.0.4
+Version: 0.0.5
 Summary: Automation framework for the WebDriver API
 Home-page: https://github.com/mreiche/python-automation-framework
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 
 # PAF - Python Automation Framework
 
@@ -62,16 +62,16 @@
 - [Components](doc/components.md)
 - [Managing WebDrivers](doc/webdriver.md)
 - [Execution controlling](doc/control.md)
 
 ### Missing features (todos)
 
 - Rect assertions
-- ContextClick/DoubleClick actions
 - Frames/ShadowRoot support
+- Drag & Drop over frames
 
 ## Environment variables
 
 * `PAF_BROWSER_SETTING=chrome:90`: Sets the requested browser name and it's version.
 * `PAF_WINDOW_SIZE=1920x1080`: Sets the browsers default window size.
 * `PAF_SCREENSHOTS_DIR=screenshots`: Sets the screenshots' directory.
 * `PAF_SEQUENCE_WAIT_AFTER_FAIL=0.3`: Wait in seconds whenever a sequence action fails.
```

### Comparing `python-automation-framework-0.0.4/README.md` & `python-automation-framework-0.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 - [Components](doc/components.md)
 - [Managing WebDrivers](doc/webdriver.md)
 - [Execution controlling](doc/control.md)
 
 ### Missing features (todos)
 
 - Rect assertions
-- ContextClick/DoubleClick actions
 - Frames/ShadowRoot support
+- Drag & Drop over frames
 
 ## Environment variables
 
 * `PAF_BROWSER_SETTING=chrome:90`: Sets the requested browser name and it's version.
 * `PAF_WINDOW_SIZE=1920x1080`: Sets the browsers default window size.
 * `PAF_SCREENSHOTS_DIR=screenshots`: Sets the screenshots' directory.
 * `PAF_SEQUENCE_WAIT_AFTER_FAIL=0.3`: Wait in seconds whenever a sequence action fails.
```

### Comparing `python-automation-framework-0.0.4/paf/assertion.py` & `python-automation-framework-0.0.5/paf/assertion.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.4/paf/common.py` & `python-automation-framework-0.0.5/paf/common.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.4/paf/component.py` & `python-automation-framework-0.0.5/paf/component.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.4/paf/control.py` & `python-automation-framework-0.0.5/paf/control.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.4/paf/javascript.py` & `python-automation-framework-0.0.5/paf/javascript.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.4/paf/locator.py` & `python-automation-framework-0.0.5/paf/locator.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.4/paf/manager.py` & `python-automation-framework-0.0.5/paf/manager.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.4/paf/page.py` & `python-automation-framework-0.0.5/paf/page.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.4/paf/request.py` & `python-automation-framework-0.0.5/paf/request.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.4/paf/uielement.py` & `python-automation-framework-0.0.5/paf/uielement.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import math
 from abc import abstractmethod, ABC
 from datetime import datetime
 from pathlib import Path
 from typing import Callable, Type, TypeVar, List, Generic, Iterable, Iterator
 
 import inject
+from selenium.webdriver import ActionChains
 from selenium.webdriver.common.by import By as SeleniumBy
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support.color import Color
 
 import paf.javascript as script
 from paf.assertion import StringAssertion, Format, BinaryAssertion, QuantityAssertion
@@ -22,14 +23,34 @@
 class UiElementActions:
 
     @abstractmethod
     def click(self):
         pass
 
     @abstractmethod
+    def hover(self):
+        pass
+
+    @abstractmethod
+    def context_click(self):
+        pass
+
+    @abstractmethod
+    def long_click(self):
+        pass
+
+    @abstractmethod
+    def double_click(self):
+        pass
+
+    @abstractmethod
+    def drag_and_drop_to(self, target_ui_element: "UiElement"):
+        pass
+
+    @abstractmethod
     def send_keys(self, value: str):
         pass
 
     @abstractmethod
     def type(self, value: str):
         pass
 
@@ -197,14 +218,51 @@
             web_element.clear()
             web_element.send_keys(value)
             assert web_element.get_attribute("value") == value
 
         self._action_sequence(_action)
         return self
 
+    def hover(self):
+        def _action(web_element: WebElement):
+            actions = ActionChains(self._webdriver)
+            actions.move_to_element(web_element).perform()
+
+        self._action_sequence(_action)
+
+    def context_click(self):
+        def _action(web_element: WebElement):
+            actions = ActionChains(self._webdriver)
+            actions.context_click(web_element).perform()
+
+        self._action_sequence(_action)
+
+    def long_click(self):
+        def _action(web_element: WebElement):
+            actions = ActionChains(self._webdriver)
+            actions.click_and_hold(web_element).perform()
+
+        self._action_sequence(_action)
+
+    def double_click(self):
+        def _action(web_element: WebElement):
+            actions = ActionChains(self._webdriver)
+            actions.double_click(web_element).perform()
+
+        self._action_sequence(_action)
+
+    def drag_and_drop_to(self, target_ui_element: "UiElement"):
+        def _action(source: WebElement):
+            def _target_found(target: WebElement):
+                actions = ActionChains(self._webdriver)
+                actions.drag_and_drop(source, target).perform()
+            target_ui_element.find_web_element(_target_found)
+
+        self._action_sequence(_action)
+
     @property
     def expect(self):
         return UiElementAssertion(self)
 
     @property
     def wait_for(self):
         return UiElementAssertion(self, raise_exception=False)
```

### Comparing `python-automation-framework-0.0.4/paf/xpath.py` & `python-automation-framework-0.0.5/paf/xpath.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.4/python_automation_framework.egg-info/PKG-INFO` & `python-automation-framework-0.0.5/python_automation_framework.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-automation-framework
-Version: 0.0.4
+Version: 0.0.5
 Summary: Automation framework for the WebDriver API
 Home-page: https://github.com/mreiche/python-automation-framework
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 
 # PAF - Python Automation Framework
 
@@ -62,16 +62,16 @@
 - [Components](doc/components.md)
 - [Managing WebDrivers](doc/webdriver.md)
 - [Execution controlling](doc/control.md)
 
 ### Missing features (todos)
 
 - Rect assertions
-- ContextClick/DoubleClick actions
 - Frames/ShadowRoot support
+- Drag & Drop over frames
 
 ## Environment variables
 
 * `PAF_BROWSER_SETTING=chrome:90`: Sets the requested browser name and it's version.
 * `PAF_WINDOW_SIZE=1920x1080`: Sets the browsers default window size.
 * `PAF_SCREENSHOTS_DIR=screenshots`: Sets the screenshots' directory.
 * `PAF_SEQUENCE_WAIT_AFTER_FAIL=0.3`: Wait in seconds whenever a sequence action fails.
```

### Comparing `python-automation-framework-0.0.4/python_automation_framework.egg-info/SOURCES.txt` & `python-automation-framework-0.0.5/python_automation_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.4/setup.py` & `python-automation-framework-0.0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="python-automation-framework",
     description="Automation framework for the WebDriver API",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.0.4",
+    version="0.0.5",
     url="https://github.com/mreiche/python-automation-framework",
     author="Mike Reiche",
     packages=["paf"],
     install_requires=["inject>=4.3.1", "selenium>=4.8.3", "is-empty>=1.0.1"],
 )
```

### Comparing `python-automation-framework-0.0.4/test/test_component.py` & `python-automation-framework-0.0.5/test/test_component.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.4/test/test_javascript.py` & `python-automation-framework-0.0.5/test/test_javascript.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.4/test/test_locator.py` & `python-automation-framework-0.0.5/test/test_locator.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.4/test/test_page.py` & `python-automation-framework-0.0.5/test/test_page.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.4/test/test_request.py` & `python-automation-framework-0.0.5/test/test_request.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.4/test/test_uielement.py` & `python-automation-framework-0.0.5/test/test_uielement.py`

 * *Files 17% similar despite different names*

```diff
@@ -68,24 +68,24 @@
 
     p = finder.find("#para1")
 
     assert p.wait_for.tag_name.be("p") is True
     assert p.wait_for.tag_name.be("b") is False
 
 
-def test_displayed():
-    finder = page_factory.create_page(FinderPage, create_webdriver())
-    finder.open("https://testpages.herokuapp.com/styled/alerts/fake-alert-test.html")
-
-    ok = finder.find("#dialog-ok")
-    btn = finder.find("#fakealert")
-
-    ok.expect.displayed.be(False)
-    btn.click()
-    ok.expect.displayed.be(True)
+# def test_displayed():
+#     finder = page_factory.create_page(FinderPage, create_webdriver())
+#     finder.open("https://testpages.herokuapp.com/styled/alerts/fake-alert-test.html")
+#
+#     ok = finder.find("#dialog-ok")
+#     btn = finder.find("#fakealert")
+#
+#     ok.expect.displayed.be(False)
+#     btn.click()
+#     ok.expect.displayed.be(True)
 
 
 def test_highlight():
     finder = page_factory.create_page(FinderPage, create_webdriver())
     finder.open("https://testpages.herokuapp.com/styled/basic-web-page-test.html")
 
     p = finder.find(By.id("para1"))
@@ -168,9 +168,49 @@
     clicks = finder.find(XPath.at("div").id("events").select("p"))
 
     control = inject.instance(Control)
     btn.click()
     control.retry(lambda: clicks.expect.count.be(3), lambda: btn.click(), wait_after_fail=0, count=3)
 
 
+def test_actions():
+    finder = page_factory.create_page(FinderPage, create_webdriver())
+    finder.open("https://testpages.herokuapp.com/styled/events/javascript-events.html")
+
+    click_btn = finder.find("#onclick")
+    click_status = finder.find("#onclickstatus")
+    click_status.expect.displayed.be(False)
+    click_btn.click()
+    click_status.expect.displayed.be(True)
+
+    hover_btn = finder.find("#onmouseover")
+    hover_status = finder.find("#onmouseoverstatus")
+    hover_status.expect.displayed.be(False)
+    hover_btn.hover()
+    hover_status.expect.displayed.be(True)
+
+    context_btn = finder.find("#oncontextmenu")
+    context_status = finder.find("#oncontextmenustatus")
+    context_status.expect.displayed.be(False)
+    context_btn.context_click()
+    context_status.expect.displayed.be(True)
+
+    double_click_btn = finder.find("#ondoubleclick")
+    double_click_status = finder.find("#ondoubleclickstatus")
+    double_click_status.expect.displayed.be(False)
+    double_click_btn.double_click()
+    double_click_status.expect.displayed.be(True)
+
+
+def test_drag_and_drop():
+    finder = page_factory.create_page(FinderPage, create_webdriver())
+    finder.open("https://testpages.herokuapp.com/styled/drag-drop-javascript.html")
+
+    drag = finder.find(".drag.left")
+    drop = finder.find("#droppable1")
+    drop.expect.text.be("Drop here")
+    drag.drag_and_drop_to(drop)
+    drop.expect.text.be("Dropped!")
+
+
 def teardown_module():
     inject.instance(WebDriverManager).shutdown_all()
```

### Comparing `python-automation-framework-0.0.4/test/test_webdriver.py` & `python-automation-framework-0.0.5/test/test_webdriver.py`

 * *Files identical despite different names*

