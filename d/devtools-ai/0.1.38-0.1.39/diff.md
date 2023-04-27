# Comparing `tmp/devtools-ai-0.1.38.tar.gz` & `tmp/devtools-ai-0.1.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devtools-ai-0.1.38.tar", last modified: Thu Apr 27 22:30:14 2023, max compression
+gzip compressed data, was "devtools-ai-0.1.39.tar", last modified: Thu Apr 27 22:46:20 2023, max compression
```

## Comparing `devtools-ai-0.1.38.tar` & `devtools-ai-0.1.39.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-27 22:30:14.653283 devtools-ai-0.1.38/
--rw-r--r--   0 chris      (501) staff       (20)     9143 2022-06-18 16:37:36.000000 devtools-ai-0.1.38/LICENSE.md
--rw-r--r--   0 chris      (501) staff       (20)     2776 2023-04-27 22:30:14.652646 devtools-ai-0.1.38/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     1773 2023-03-02 18:30:06.000000 devtools-ai-0.1.38/README.md
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-27 22:30:14.644175 devtools-ai-0.1.38/devtools_ai/
--rw-r--r--   0 chris      (501) staff       (20)       21 2023-04-27 22:25:19.000000 devtools-ai-0.1.38/devtools_ai/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)    11829 2023-04-27 22:28:32.000000 devtools-ai-0.1.38/devtools_ai/appium.py
--rw-r--r--   0 chris      (501) staff       (20)    24563 2023-03-11 06:45:01.000000 devtools-ai-0.1.38/devtools_ai/selenium.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-27 22:30:14.651811 devtools-ai-0.1.38/devtools_ai/utils/
--rw-r--r--   0 chris      (501) staff       (20)        0 2022-06-18 16:37:36.000000 devtools-ai-0.1.38/devtools_ai/utils/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)    10713 2023-02-13 00:24:21.000000 devtools-ai-0.1.38/devtools_ai/utils/local_classify.py
--rw-r--r--   0 chris      (501) staff       (20)      342 2023-03-11 06:45:01.000000 devtools-ai-0.1.38/devtools_ai/utils/misc.py
--rw-r--r--   0 chris      (501) staff       (20)     2637 2023-02-13 00:24:21.000000 devtools-ai-0.1.38/devtools_ai/utils/network_utils.py
--rw-r--r--   0 chris      (501) staff       (20)    10521 2022-08-05 19:01:02.000000 devtools-ai-0.1.38/devtools_ai/utils/scanner.py
--rw-r--r--   0 chris      (501) staff       (20)    31695 2023-03-22 01:14:20.000000 devtools-ai-0.1.38/devtools_ai/utils/selenium_core.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-27 22:30:14.647668 devtools-ai-0.1.38/devtools_ai.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)     2776 2023-04-27 22:30:14.000000 devtools-ai-0.1.38/devtools_ai.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      479 2023-04-27 22:30:14.000000 devtools-ai-0.1.38/devtools_ai.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-04-27 22:30:14.000000 devtools-ai-0.1.38/devtools_ai.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)      103 2023-04-27 22:30:14.000000 devtools-ai-0.1.38/devtools_ai.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)       12 2023-04-27 22:30:14.000000 devtools-ai-0.1.38/devtools_ai.egg-info/top_level.txt
--rw-r--r--   0 chris      (501) staff       (20)      103 2022-06-18 16:37:36.000000 devtools-ai-0.1.38/pyproject.toml
--rw-r--r--   0 chris      (501) staff       (20)       38 2023-04-27 22:30:14.653486 devtools-ai-0.1.38/setup.cfg
--rw-r--r--   0 chris      (501) staff       (20)     1950 2023-02-13 00:24:21.000000 devtools-ai-0.1.38/setup.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-27 22:46:20.776709 devtools-ai-0.1.39/
+-rw-r--r--   0 chris      (501) staff       (20)     9143 2022-06-18 16:37:36.000000 devtools-ai-0.1.39/LICENSE.md
+-rw-r--r--   0 chris      (501) staff       (20)     2776 2023-04-27 22:46:20.776316 devtools-ai-0.1.39/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     1773 2023-03-02 18:30:06.000000 devtools-ai-0.1.39/README.md
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-27 22:46:20.770851 devtools-ai-0.1.39/devtools_ai/
+-rw-r--r--   0 chris      (501) staff       (20)       21 2023-04-27 22:46:13.000000 devtools-ai-0.1.39/devtools_ai/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)    11817 2023-04-27 22:46:03.000000 devtools-ai-0.1.39/devtools_ai/appium.py
+-rw-r--r--   0 chris      (501) staff       (20)    24563 2023-03-11 06:45:01.000000 devtools-ai-0.1.39/devtools_ai/selenium.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-27 22:46:20.775757 devtools-ai-0.1.39/devtools_ai/utils/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2022-06-18 16:37:36.000000 devtools-ai-0.1.39/devtools_ai/utils/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)    10713 2023-02-13 00:24:21.000000 devtools-ai-0.1.39/devtools_ai/utils/local_classify.py
+-rw-r--r--   0 chris      (501) staff       (20)      342 2023-03-11 06:45:01.000000 devtools-ai-0.1.39/devtools_ai/utils/misc.py
+-rw-r--r--   0 chris      (501) staff       (20)     2637 2023-02-13 00:24:21.000000 devtools-ai-0.1.39/devtools_ai/utils/network_utils.py
+-rw-r--r--   0 chris      (501) staff       (20)    10521 2022-08-05 19:01:02.000000 devtools-ai-0.1.39/devtools_ai/utils/scanner.py
+-rw-r--r--   0 chris      (501) staff       (20)    31695 2023-03-22 01:14:20.000000 devtools-ai-0.1.39/devtools_ai/utils/selenium_core.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-27 22:46:20.773134 devtools-ai-0.1.39/devtools_ai.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)     2776 2023-04-27 22:46:20.000000 devtools-ai-0.1.39/devtools_ai.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      479 2023-04-27 22:46:20.000000 devtools-ai-0.1.39/devtools_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-04-27 22:46:20.000000 devtools-ai-0.1.39/devtools_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)      103 2023-04-27 22:46:20.000000 devtools-ai-0.1.39/devtools_ai.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)       12 2023-04-27 22:46:20.000000 devtools-ai-0.1.39/devtools_ai.egg-info/top_level.txt
+-rw-r--r--   0 chris      (501) staff       (20)      103 2022-06-18 16:37:36.000000 devtools-ai-0.1.39/pyproject.toml
+-rw-r--r--   0 chris      (501) staff       (20)       38 2023-04-27 22:46:20.776825 devtools-ai-0.1.39/setup.cfg
+-rw-r--r--   0 chris      (501) staff       (20)     1950 2023-02-13 00:24:21.000000 devtools-ai-0.1.39/setup.py
```

### Comparing `devtools-ai-0.1.38/LICENSE.md` & `devtools-ai-0.1.39/LICENSE.md`

 * *Files identical despite different names*

### Comparing `devtools-ai-0.1.38/PKG-INFO` & `devtools-ai-0.1.39/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devtools-ai
-Version: 0.1.38
+Version: 0.1.39
 Summary: A package to bring ai to selenium scripts.
 Home-page: https://github.com/dev-tools-ai/python-sdk
 Author: Chris Navrides
 Author-email: chris@dev-tools.ai
 Project-URL: Bug Tracker, https://github.com/dev-tools-ai/python-sdk/issues
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `devtools-ai-0.1.38/README.md` & `devtools-ai-0.1.39/README.md`

 * *Files identical despite different names*

### Comparing `devtools-ai-0.1.38/devtools_ai/appium.py` & `devtools-ai-0.1.39/devtools_ai/appium.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     def _classify(self, element_name, is_backup=False, custom_ai_threshold=None):
         msg = ''
         if self.test_case_creation_mode:
             self._test_case_upload_screenshot(element_name)
             element_box, needs_reload, has_training_data = self._test_case_get_box(element_name)
             if element_box:
                 if self.use_ai_elem:
-                    root_elem = self.driver.find_elements(by='xpath', value='//*')[0]._id
+                    root_elem = self.driver.find_elements(by='xpath', value='//*')[0]
                     element = ai_elem(None, root_elem._id, element_box, self.driver,
                                       self.multiplier, smart_driver=self, base_elem=root_elem)
                 else:
                     element = self._match_bounding_box_to_web_element(element_box, multiplier=self.multiplier, use_first=self.use_ai_elem)
 
                 return element, self.last_test_case_screenshot_uuid, msg
             else:
@@ -70,15 +70,15 @@
                 log.info('Waiting for bounding box of element {} to be drawn in the UI: \n\t{}'.format(element_name,
                                                                                                        label_url))
                 webbrowser.open(label_url)
                 while True:
                     element_box, needs_reload, has_training_data = self._test_case_get_box(element_name, event_id=event_id)
                     if element_box is not None:
                         if self.use_ai_elem:
-                            root_elem = self.driver.find_elements(by='xpath', value='//*')[0]._id
+                            root_elem = self.driver.find_elements(by='xpath', value='//*')[0]
                             element = ai_elem(None, root_elem._id, element_box, self.driver,
                                           self.multiplier, smart_driver=self, base_elem=root_elem)
                         else:
                             element = self._match_bounding_box_to_web_element(element_box, multiplier=self.multiplier, use_first=self.use_ai_elem)
 
                         return element, self.last_test_case_screenshot_uuid, msg
 
@@ -94,15 +94,15 @@
             screenshotBase64 = self._get_screenshot()
             key = self.get_screenshot_hash(screenshotBase64)
             resp_data = self._check_screenshot_exists(key, element_name)
             if resp_data['success'] and 'box' in resp_data:
                 if self.debug:
                     print(f'Found cached box in action info for {element_name} using that')
                 if self.use_ai_elem:
-                    root_elem = self.driver.find_elements(by='xpath', value='//*')[0]._id
+                    root_elem = self.driver.find_elements(by='xpath', value='//*')[0]
                     element = ai_elem(None, root_elem.id, resp_data['box'], self.driver,
                                     self.multiplier)
                 else:
                     element = self._match_bounding_box_to_web_element(resp_data['box'], multiplier=self.multiplier, use_first=self.use_ai_elem)
 
                 return element, key, msg
```

### Comparing `devtools-ai-0.1.38/devtools_ai/selenium.py` & `devtools-ai-0.1.39/devtools_ai/selenium.py`

 * *Files identical despite different names*

### Comparing `devtools-ai-0.1.38/devtools_ai/utils/local_classify.py` & `devtools-ai-0.1.39/devtools_ai/utils/local_classify.py`

 * *Files identical despite different names*

### Comparing `devtools-ai-0.1.38/devtools_ai/utils/network_utils.py` & `devtools-ai-0.1.39/devtools_ai/utils/network_utils.py`

 * *Files identical despite different names*

### Comparing `devtools-ai-0.1.38/devtools_ai/utils/scanner.py` & `devtools-ai-0.1.39/devtools_ai/utils/scanner.py`

 * *Files identical despite different names*

### Comparing `devtools-ai-0.1.38/devtools_ai/utils/selenium_core.py` & `devtools-ai-0.1.39/devtools_ai/utils/selenium_core.py`

 * *Files identical despite different names*

### Comparing `devtools-ai-0.1.38/devtools_ai.egg-info/PKG-INFO` & `devtools-ai-0.1.39/devtools_ai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devtools-ai
-Version: 0.1.38
+Version: 0.1.39
 Summary: A package to bring ai to selenium scripts.
 Home-page: https://github.com/dev-tools-ai/python-sdk
 Author: Chris Navrides
 Author-email: chris@dev-tools.ai
 Project-URL: Bug Tracker, https://github.com/dev-tools-ai/python-sdk/issues
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `devtools-ai-0.1.38/setup.py` & `devtools-ai-0.1.39/setup.py`

 * *Files identical despite different names*

