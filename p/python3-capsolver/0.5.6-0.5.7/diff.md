# Comparing `tmp/python3-capsolver-0.5.6.tar.gz` & `tmp/python3-capsolver-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3-capsolver-0.5.6.tar", last modified: Fri Apr 28 17:37:17 2023, max compression
+gzip compressed data, was "python3-capsolver-0.5.7.tar", last modified: Fri Apr 28 18:41:37 2023, max compression
```

## Comparing `python3-capsolver-0.5.6.tar` & `python3-capsolver-0.5.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 17:37:17.133404 python3-capsolver-0.5.6/
--rw-r--r--   0 homea     (1000) homea     (1000)     4701 2023-04-28 17:37:17.133404 python3-capsolver-0.5.6/PKG-INFO
--rw-r--r--   0 homea     (1000) homea     (1000)      389 2022-11-19 01:26:43.000000 python3-capsolver-0.5.6/pyproject.toml
-drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 17:37:17.133404 python3-capsolver-0.5.6/python3_capsolver/
--rw-r--r--   0 homea     (1000) homea     (1000)        0 2022-10-28 01:40:08.000000 python3-capsolver-0.5.6/python3_capsolver/__init__.py
--rw-r--r--   0 homea     (1000) homea     (1000)       22 2023-04-28 17:37:13.000000 python3-capsolver-0.5.6/python3_capsolver/__version__.py
--rw-r--r--   0 homea     (1000) homea     (1000)     2491 2023-04-28 16:32:35.000000 python3-capsolver-0.5.6/python3_capsolver/control.py
-drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 17:37:17.133404 python3-capsolver-0.5.6/python3_capsolver/core/
--rw-r--r--   0 homea     (1000) homea     (1000)        0 2022-11-07 03:20:28.000000 python3-capsolver-0.5.6/python3_capsolver/core/__init__.py
--rw-r--r--   0 homea     (1000) homea     (1000)     8820 2023-04-28 17:33:16.000000 python3-capsolver-0.5.6/python3_capsolver/core/base.py
--rw-r--r--   0 homea     (1000) homea     (1000)     1008 2023-04-28 16:29:39.000000 python3-capsolver-0.5.6/python3_capsolver/core/config.py
--rw-r--r--   0 homea     (1000) homea     (1000)     3241 2023-04-28 17:03:22.000000 python3-capsolver-0.5.6/python3_capsolver/core/enum.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4259 2023-04-28 17:34:55.000000 python3-capsolver-0.5.6/python3_capsolver/core/serializer.py
--rw-r--r--   0 homea     (1000) homea     (1000)     6450 2023-04-28 16:32:35.000000 python3-capsolver-0.5.6/python3_capsolver/datadome_slider.py
--rw-r--r--   0 homea     (1000) homea     (1000)     8800 2023-04-28 17:34:04.000000 python3-capsolver-0.5.6/python3_capsolver/fun_captcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     7451 2023-04-28 16:32:35.000000 python3-capsolver-0.5.6/python3_capsolver/gee_test.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4855 2023-04-28 17:04:25.000000 python3-capsolver-0.5.6/python3_capsolver/hcaptcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     6472 2023-04-28 16:32:35.000000 python3-capsolver-0.5.6/python3_capsolver/image_to_text.py
--rw-r--r--   0 homea     (1000) homea     (1000)     7591 2023-04-28 16:32:35.000000 python3-capsolver-0.5.6/python3_capsolver/kasada.py
--rw-r--r--   0 homea     (1000) homea     (1000)     7182 2023-04-28 16:32:35.000000 python3-capsolver-0.5.6/python3_capsolver/mt_captcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     8162 2023-04-28 16:32:35.000000 python3-capsolver-0.5.6/python3_capsolver/recaptcha.py
-drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 17:37:17.133404 python3-capsolver-0.5.6/python3_capsolver.egg-info/
--rw-r--r--   0 homea     (1000) homea     (1000)     4701 2023-04-28 17:37:17.000000 python3-capsolver-0.5.6/python3_capsolver.egg-info/PKG-INFO
--rw-r--r--   0 homea     (1000) homea     (1000)      782 2023-04-28 17:37:17.000000 python3-capsolver-0.5.6/python3_capsolver.egg-info/SOURCES.txt
--rw-r--r--   0 homea     (1000) homea     (1000)        1 2023-04-28 17:37:17.000000 python3-capsolver-0.5.6/python3_capsolver.egg-info/dependency_links.txt
--rw-r--r--   0 homea     (1000) homea     (1000)        1 2023-04-28 17:37:17.000000 python3-capsolver-0.5.6/python3_capsolver.egg-info/not-zip-safe
--rw-r--r--   0 homea     (1000) homea     (1000)       60 2023-04-28 17:37:17.000000 python3-capsolver-0.5.6/python3_capsolver.egg-info/requires.txt
--rw-r--r--   0 homea     (1000) homea     (1000)       18 2023-04-28 17:37:17.000000 python3-capsolver-0.5.6/python3_capsolver.egg-info/top_level.txt
--rw-r--r--   0 homea     (1000) homea     (1000)       38 2023-04-28 17:37:17.133404 python3-capsolver-0.5.6/setup.cfg
--rw-r--r--   0 homea     (1000) homea     (1000)     4053 2023-04-28 17:36:49.000000 python3-capsolver-0.5.6/setup.py
+drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 18:41:37.612970 python3-capsolver-0.5.7/
+-rw-r--r--   0 homea     (1000) homea     (1000)     4701 2023-04-28 18:41:37.612970 python3-capsolver-0.5.7/PKG-INFO
+-rw-r--r--   0 homea     (1000) homea     (1000)      389 2022-11-19 01:26:43.000000 python3-capsolver-0.5.7/pyproject.toml
+drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 18:41:37.612970 python3-capsolver-0.5.7/python3_capsolver/
+-rw-r--r--   0 homea     (1000) homea     (1000)        0 2022-10-28 01:40:08.000000 python3-capsolver-0.5.7/python3_capsolver/__init__.py
+-rw-r--r--   0 homea     (1000) homea     (1000)       22 2023-04-28 18:41:27.000000 python3-capsolver-0.5.7/python3_capsolver/__version__.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     2477 2023-04-28 18:41:20.000000 python3-capsolver-0.5.7/python3_capsolver/control.py
+drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 18:41:37.612970 python3-capsolver-0.5.7/python3_capsolver/core/
+-rw-r--r--   0 homea     (1000) homea     (1000)        0 2022-11-07 03:20:28.000000 python3-capsolver-0.5.7/python3_capsolver/core/__init__.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     8850 2023-04-28 18:30:07.000000 python3-capsolver-0.5.7/python3_capsolver/core/base.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     1008 2023-04-28 16:29:39.000000 python3-capsolver-0.5.7/python3_capsolver/core/config.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     3489 2023-04-28 18:30:07.000000 python3-capsolver-0.5.7/python3_capsolver/core/enum.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4212 2023-04-28 18:30:07.000000 python3-capsolver-0.5.7/python3_capsolver/core/serializer.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     6374 2023-04-28 18:34:47.000000 python3-capsolver-0.5.7/python3_capsolver/datadome_slider.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     7880 2023-04-28 18:30:07.000000 python3-capsolver-0.5.7/python3_capsolver/fun_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4323 2023-04-28 18:30:07.000000 python3-capsolver-0.5.7/python3_capsolver/gee_test.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4831 2023-04-28 18:20:01.000000 python3-capsolver-0.5.7/python3_capsolver/hcaptcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     6350 2023-04-28 18:41:20.000000 python3-capsolver-0.5.7/python3_capsolver/image_to_text.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     7509 2023-04-28 18:41:20.000000 python3-capsolver-0.5.7/python3_capsolver/kasada.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     7072 2023-04-28 18:34:47.000000 python3-capsolver-0.5.7/python3_capsolver/mt_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4780 2023-04-28 18:41:20.000000 python3-capsolver-0.5.7/python3_capsolver/recaptcha.py
+drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 18:41:37.612970 python3-capsolver-0.5.7/python3_capsolver.egg-info/
+-rw-r--r--   0 homea     (1000) homea     (1000)     4701 2023-04-28 18:41:37.000000 python3-capsolver-0.5.7/python3_capsolver.egg-info/PKG-INFO
+-rw-r--r--   0 homea     (1000) homea     (1000)      782 2023-04-28 18:41:37.000000 python3-capsolver-0.5.7/python3_capsolver.egg-info/SOURCES.txt
+-rw-r--r--   0 homea     (1000) homea     (1000)        1 2023-04-28 18:41:37.000000 python3-capsolver-0.5.7/python3_capsolver.egg-info/dependency_links.txt
+-rw-r--r--   0 homea     (1000) homea     (1000)        1 2023-04-28 18:41:37.000000 python3-capsolver-0.5.7/python3_capsolver.egg-info/not-zip-safe
+-rw-r--r--   0 homea     (1000) homea     (1000)       60 2023-04-28 18:41:37.000000 python3-capsolver-0.5.7/python3_capsolver.egg-info/requires.txt
+-rw-r--r--   0 homea     (1000) homea     (1000)       18 2023-04-28 18:41:37.000000 python3-capsolver-0.5.7/python3_capsolver.egg-info/top_level.txt
+-rw-r--r--   0 homea     (1000) homea     (1000)       38 2023-04-28 18:41:37.612970 python3-capsolver-0.5.7/setup.cfg
+-rw-r--r--   0 homea     (1000) homea     (1000)     4053 2023-04-28 17:36:49.000000 python3-capsolver-0.5.7/setup.py
```

### Comparing `python3-capsolver-0.5.6/PKG-INFO` & `python3-capsolver-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-capsolver
-Version: 0.5.6
+Version: 0.5.7
 Summary: Python 3.7+ Capsolver library with AIO module.
 Home-page: https://andreidrang.github.io/python3-capsolver/
 Author: AndreiDrang
 Author-email: python-captcha@pm.me
 License: MIT
 Project-URL: Documentation, https://andreidrang.github.io/python3-capsolver/
 Project-URL: Source, https://github.com/AndreiDrang/python3-captchaai
```

### Comparing `python3-capsolver-0.5.6/python3_capsolver/control.py` & `python3-capsolver-0.5.7/python3_capsolver/control.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from python3_capsolver.core.base import BaseCaptcha
-from python3_capsolver.core.enum import CaptchaTypeEnm, EndpointPostfixEnm
+from python3_capsolver.core.enum import EndpointPostfixEnm
 from python3_capsolver.core.config import REQUEST_URL
 from python3_capsolver.core.serializer import PostRequestSer, ControlResponseSer
 
 
 class BaseControl(BaseCaptcha):
     """
     Args:
@@ -18,15 +18,15 @@
         self,
         api_key: str,
         sleep_time: int = 10,
         request_url: str = REQUEST_URL,
     ):
 
         super().__init__(
-            api_key=api_key, sleep_time=sleep_time, request_url=request_url, captcha_type=CaptchaTypeEnm.Control
+            api_key=api_key, sleep_time=sleep_time, request_url=request_url, captcha_type="CaptchaTypeEnm.Control"
         )
 
 
 class Control(BaseControl):
     """
     The class is used to work with Capsolver control methods.
```

### Comparing `python3-capsolver-0.5.6/python3_capsolver/core/base.py` & `python3-capsolver-0.5.7/python3_capsolver/core/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,17 @@
 
     def _create_task(self, url_postfix: str = EndpointPostfixEnm.CREATE_TASK.value) -> dict:
         """
         Function send SYNC request to service and wait for result
         """
         try:
             print(self.task_payload.dict(exclude_none=True))
-            resp = self.__session.post(parse.urljoin(self.__request_url, url_postfix), json=self.task_payload.dict(exclude_none=True))
+            resp = self.__session.post(
+                parse.urljoin(self.__request_url, url_postfix), json=self.task_payload.dict(exclude_none=True)
+            )
             print(resp.status_code)
             print(resp.json())
             if resp.status_code in VALID_STATUS_CODES:
                 return resp.json()
             else:
                 raise ValueError(resp.raise_for_status())
         except Exception as error:
```

### Comparing `python3-capsolver-0.5.6/python3_capsolver/core/config.py` & `python3-capsolver-0.5.7/python3_capsolver/core/config.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.5.6/python3_capsolver/core/enum.py` & `python3-capsolver-0.5.7/python3_capsolver/core/enum.py`

 * *Files 13% similar despite different names*

```diff
@@ -40,36 +40,26 @@
     """
 
     GET_BALANCE = "getBalance"
     CREATE_TASK = "createTask"
     GET_TASK_RESULT = "getTaskResult"
 
 
-class CaptchaTypeEnm(str, MyEnum):
+class CaptchaTypeEnmXXX(str, MyEnum):
     """
     Enum with all available captcha types
 
     Notes:
         https://captchaai.atlassian.net/wiki/spaces/CAPTCHAAI/pages/393295
     """
 
     Control = "Control"  # custom captcha type
     ImageToTextTask = "ImageToTextTask"
-    # Recaptcha
-    ReCaptchaV2TaskProxyLess = "ReCaptchaV2TaskProxyLess"
-    ReCaptchaV2Task = "ReCaptchaV2Task"
-    ReCaptchaV2EnterpriseTask = "ReCaptchaV2EnterpriseTask"
-    ReCaptchaV2EnterpriseTaskProxyless = "ReCaptchaV2EnterpriseTaskProxyless"
-    ReCaptchaV3Task = "ReCaptchaV3Task"
-    ReCaptchaV3TaskProxyless = "ReCaptchaV3TaskProxyless"
     # HCaptcha
     HCaptchaClassification = "HCaptchaClassification"
-    # GeeTest
-    GeetestTask = "GeetestTask"
-    GeetestTaskProxyless = "GeetestTaskProxyless"
     # FunCaptcha
     FunCaptchaClassification = "FunCaptchaClassification"
     # Other types
     MtCaptchaTask = "MtCaptchaTask"
     DatadomeSliderTask = "DatadomeSliderTask"
     AntiKasadaTask = "AntiKasadaTask"
     AntiAkamaiBMPTask = "AntiAkamaiBMPTask"
@@ -79,18 +69,40 @@
     HCaptchaTask = "HCaptchaTask"
     HCaptchaTaskProxyless = "HCaptchaTaskProxyless"
     HCaptchaEnterpriseTask = "HCaptchaEnterpriseTask"
     HCaptchaEnterpriseTaskProxyLess = "HCaptchaEnterpriseTaskProxyLess"
     HCaptchaTurboTask = "HCaptchaTurboTask"
     HCaptchaTurboTaskProxyLess = "HCaptchaTurboTaskProxyLess"
 
+
 class FunCaptchaTypeEnm(str, MyEnum):
     FunCaptchaTask = "FunCaptchaTask"
     FunCaptchaTaskProxyLess = "FunCaptchaTaskProxyLess"
 
+
+class GeeTestCaptchaTypeEnm(str, MyEnum):
+    GeeTestTask = "GeeTestTask"
+    GeeTestTaskProxyLess = "GeeTestTaskProxyLess"
+
+
+class ReCaptchaV2TypeEnm(str, MyEnum):
+    # V2
+    ReCaptchaV2Task = "ReCaptchaV2Task"
+    ReCaptchaV2EnterpriseTask = "ReCaptchaV2EnterpriseTask"
+    ReCaptchaV2TaskProxyLess = "ReCaptchaV2TaskProxyLess"
+    ReCaptchaV2EnterpriseTaskProxyLess = "ReCaptchaV2EnterpriseTaskProxyLess"
+
+
+class ReCaptchaV3TypeEnm(str, MyEnum):
+    ReCaptchaV3Task = "ReCaptchaV3Task"
+    ReCaptchaV3EnterpriseTask = "ReCaptchaV3EnterpriseTask"
+    ReCaptchaV3TaskProxyLess = "ReCaptchaV3TaskProxyLess"
+    ReCaptchaV3EnterpriseTaskProxyLess = "ReCaptchaV3EnterpriseTaskProxyLess"
+
+
 class ResponseStatusEnm(str, MyEnum):
     """
     Enum store results `status` field variants
 
     Notes:
         https://captchaai.atlassian.net/wiki/spaces/CAPTCHAAI/pages/426124
     """
```

### Comparing `python3-capsolver-0.5.6/python3_capsolver/core/serializer.py` & `python3-capsolver-0.5.7/python3_capsolver/core/serializer.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,55 +69,48 @@
 
 
 class WebsiteDataOptionsSer(TaskSer):
     websiteURL: str = Field(..., description="Address of a webpage with Captcha")
     websiteKey: str = Field(..., description="Website key")
 
 
-class ReCaptchaV3ProxyLessOptionsSer(WebsiteDataOptionsSer):
+class ReCaptchaV3Ser(WebsiteDataOptionsSer):
     pageAction: str = Field(
         "verify",
         description="Widget action value."
         "Website owner defines what user is doing on the page through this parameter",
     )
 
 
-class ReCaptchaV3OptionsSer(ReCaptchaV3ProxyLessOptionsSer):
-    pass
-
-
-class HCaptchaOptionsSer(WebsiteDataOptionsSer):
-    pass
-
-
 class HCaptchaClassificationOptionsSer(BaseModel):
     queries: List[str] = Field(..., description="Base64-encoded images, do not include 'data:image/***;base64,'")
     question: str = Field(
         ..., description="Question ID. Support English and Chinese, other languages please convert yourself"
     )
 
 
-class GeeTestProxyLessOptionsSer(BaseModel):
+class GeeTestSer(TaskSer):
     websiteURL: str = Field(..., description="Address of a webpage with Geetest")
     gt: str = Field(..., description="The domain public key, rarely updated")
-
-
-class GeeTestOptionsSer(GeeTestProxyLessOptionsSer):
-    pass
+    challenge: Optional[str] = Field(
+        "",
+        description="If you need to solve Geetest V3 you must use this parameter, don't need if you need to solve GeetestV4",
+    )
 
 
 class FunCaptchaSer(TaskSer):
     websiteURL: str = Field(..., description="Address of a webpage with Funcaptcha")
     websitePublicKey: str = Field(..., description="Funcaptcha website key.")
     funcaptchaApiJSSubdomain: Optional[str] = Field(
         None,
         description="A special subdomain of funcaptcha.com, from which the JS captcha widget should be loaded."
         "Most FunCaptcha installations work from shared domains.",
     )
 
+
 class DatadomeSliderOptionsSer(BaseModel):
     websiteURL: str = Field(..., description="Address of a webpage with DatadomeSlider")
     captchaUrl: str = Field(..., description="Captcha Url where is the captcha")
 
 
 class MtCaptchaOptionsSer(WebsiteDataOptionsSer):
     proxy: str = Field(..., description="String with proxy connection params, example: `198.22.3.1:10001:user:pwd`")
```

### Comparing `python3-capsolver-0.5.6/python3_capsolver/datadome_slider.py` & `python3-capsolver-0.5.7/python3_capsolver/datadome_slider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Union, Optional
 
 from python3_capsolver.core.base import BaseCaptcha
-from python3_capsolver.core.enum import ProxyType, CaptchaTypeEnm
+from python3_capsolver.core.enum import ProxyType
 from python3_capsolver.core.config import REQUEST_URL
 from python3_capsolver.core.serializer import CaptchaResponseSer, RequestCreateTaskSer, DatadomeSliderOptionsSer
 
 
 class BaseDatadomeSlider(BaseCaptcha):
     """
     The class is used to work with Capsolver DatadomeSlider method.
@@ -71,15 +71,14 @@
         proxyPort: int,
         sleep_time: Optional[int] = 5,
         request_url: Optional[str] = REQUEST_URL,
     ):
 
         super().__init__(
             api_key=api_key,
-            captcha_type=CaptchaTypeEnm.DatadomeSliderTask,
             sleep_time=sleep_time,
             request_url=request_url,
         )
 
         self.task_params = DatadomeSliderOptionsSer(**locals()).dict()
 
 
@@ -114,15 +113,15 @@
                                solution={'gRecaptchaResponse': '44795sds...'}
                               )
 
         Returns:
             CaptchaResponseSer model with full service response
 
         Notes:
-            Check class docstirng for more info
+            Check class docstring for more info
         """
         return self._processing_captcha(serializer=RequestCreateTaskSer, type=self.captcha_type, **additional_params)
 
     async def aio_captcha_handler(
         self,
         **additional_params,
     ) -> CaptchaResponseSer:
@@ -150,12 +149,12 @@
                                solution={'gRecaptchaResponse': '44795sds...'}
                               )
 
         Returns:
             CaptchaResponseSer model with full service response
 
         Notes:
-            Check class docstirng for more info
+            Check class docstring for more info
         """
         return await self._aio_processing_captcha(
             serializer=RequestCreateTaskSer, type=self.captcha_type, **additional_params
         )
```

### Comparing `python3-capsolver-0.5.6/python3_capsolver/fun_captcha.py` & `python3-capsolver-0.5.7/python3_capsolver/fun_captcha.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,23 @@
-from typing import Union, Optional
+from typing import Union
 
 from python3_capsolver.core.base import BaseCaptcha
 from python3_capsolver.core.enum import FunCaptchaTypeEnm
-from python3_capsolver.core.serializer import (
-    CaptchaResponseSer,
-    FunCaptchaSer,
-    RequestCreateTaskSer,
-)
+from python3_capsolver.core.serializer import FunCaptchaSer, CaptchaResponseSer
 
 
 class FunCaptcha(BaseCaptcha):
     """
     The class is used to work with Capsolver FuncaptchaTask methods.
 
     Args:
         api_key: Capsolver API key
-        captcha_type: Captcha type name, like ``GeetestTaskProxyless`` and etc.
+        captcha_type: Captcha type name, like ``FuncaptchaTaskProxyless`` and etc.
         websiteURL: Address of a webpage with Geetest.
         websitePublicKey: Funcaptcha website key.
-        funcaptchaApiJSSubdomain: A special subdomain of funcaptcha.com,from which the JS captcha should be loaded.
-                                    Most FunCaptcha installations work from shared domains.
-        proxyType: Type of the proxy
-        proxyAddress: Proxy IP address IPv4/IPv6. Not allowed to use:
-                        host names instead of IPs,
-                        transparent proxies (where client IP is visible),
-                        proxies from local networks (192.., 10.., 127...)
-        proxyPort: Proxy port.
-        sleep_time: The waiting time between requests to get the result of the Captcha
-        request_url: API address for sending requests
 
     Examples:
         >>> with FunCaptcha(api_key="CAI-1324...",
         ...             captcha_type="FuncaptchaTaskProxyless",
         ...             websiteURL="https://api.funcaptcha.com/fc/api/nojs/",
         ...             websitePublicKey="69A21A01-CC7B-B9C6-0F9A-E7FA06677FFC",
         ...             funcaptchaApiJSSubdomain="https://api.funcaptcha.com/"
@@ -60,17 +46,15 @@
                            solution={'token': '44795sds...'}
                           )
 
     Returns:
         CaptchaResponseSer model with full server response
 
     Notes:
-        https://captchaai.atlassian.net/wiki/spaces/CAPTCHAAI/pages/426302
-        https://captchaai.atlassian.net/wiki/spaces/CAPTCHAAI/pages/394062
-        https://captchaai.atlassian.net/wiki/spaces/CAPTCHAAI/pages/426373
+        https://docs.capsolver.com/guide/captcha/FunCaptcha.html
     """
 
     def __init__(
         self, captcha_type: Union[FunCaptchaSer, str], websiteURL: str, websitePublicKey: str, *args, **kwargs
     ):
         super().__init__(*args, **kwargs)
 
@@ -80,17 +64,15 @@
             raise ValueError(
                 f"""Invalid `captcha_type` parameter set for `{self.__class__.__name__}`,
                 available - {FunCaptchaTypeEnm.list()}"""
             )
         for key in kwargs:
             self.task_params.update({key: kwargs[key]})
 
-    def captcha_handler(
-        self
-    ) -> CaptchaResponseSer:
+    def captcha_handler(self) -> CaptchaResponseSer:
         """
         Sync solving method
 
         Examples:
             >>> FunCaptcha(api_key="CAI-BA9XXXXXXXXXXXXX2702E010",
             ...         captcha_type="FuncaptchaTaskProxyless",
             ...         websiteURL="https://api.funcaptcha.com/fc/api/nojs/",
@@ -122,21 +104,19 @@
                                solution={'token': '44795sds...'}
                               )
 
         Returns:
             CaptchaResponseSer model with full service response
 
         Notes:
-            Check class docstirng for more info
+            Check class docstring for more info
         """
         return self._processing_captcha(create_params=self.task_params)
 
-    async def aio_captcha_handler(
-        self
-    ) -> CaptchaResponseSer:
+    async def aio_captcha_handler(self) -> CaptchaResponseSer:
         """
         Async method for captcha solving
 
         Examples:
             >>> await FunCaptcha(api_key="CAI-1324...",
             ...         captcha_type="FuncaptchaTaskProxyless",
             ...         websiteURL="https://api.funcaptcha.com/fc/api/nojs/",
@@ -184,10 +164,10 @@
                                solution={'token': '44795sds...'}
                               )
 
         Returns:
             CaptchaResponseSer model with full service response
 
         Notes:
-            Check class docstirng for more info
+            Check class docstring for more info
         """
         return await self._aio_processing_captcha(create_params=self.task_params)
```

### Comparing `python3-capsolver-0.5.6/python3_capsolver/gee_test.py` & `python3-capsolver-0.5.7/python3_capsolver/kasada.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,173 +1,176 @@
 from typing import Union, Optional
 
 from python3_capsolver.core.base import BaseCaptcha
-from python3_capsolver.core.enum import ProxyType, CaptchaTypeEnm
+from python3_capsolver.core.enum import ProxyType
 from python3_capsolver.core.config import REQUEST_URL
-from python3_capsolver.core.serializer import (
-    GeeTestOptionsSer,
-    CaptchaResponseSer,
-    RequestCreateTaskSer,
-    GeeTestProxyLessOptionsSer,
-)
+from python3_capsolver.core.serializer import KasadaOptionsSer, CaptchaResponseSer, RequestCreateTaskSer
 
 
-class BaseGeeTest(BaseCaptcha):
+class BaseKasada(BaseCaptcha):
     """
-    The class is used to work with Capsolver GeetestTask methods.
+    The class is used to work with Capsolver AntiKasadaTask methods.
 
     Args:
         api_key: Capsolver API key
-        captcha_type: Captcha type name, like ``GeetestTaskProxyless`` and etc.
-        websiteURL: Address of a webpage with Geetest
-        gt: The domain public key, rarely updated
+        pageURL: Address of a webpage with Kasada
         proxyType: Type of the proxy
         proxyAddress: Proxy IP address IPv4/IPv6. Not allowed to use:
                         host names instead of IPs,
                         transparent proxies (where client IP is visible),
                         proxies from local networks (192.., 10.., 127...)
         proxyPort: Proxy port.
+        proxyLogin: Login for proxy which requires authorizaiton (basic).
+                        This isn’t required if you are using proxies authenticated by IP
+        proxyPassword: This isn’t required if you are using proxies authenticated by IP
         sleep_time: The waiting time between requests to get the result of the Captcha
         request_url: API address for sending requests
 
     Examples:
-        >>> GeeTest(api_key="CAI-1324...",
-        ...         captcha_type="GeetestTaskProxyless",
-        ...         websiteURL="https://www.geetest.com/en/demo",
-        ...         gt="022397c99c9f646f6477822485f30404",
-        ...        ).captcha_handler(
-        ...                    challenge="a66f31a53a404af8d1f271eec5138aa1",
-        ...                    geetestApiServerSubdomain="api.geetest.com"
-        ...                )
+        >>> Kasada(api_key="CAI-1324...",
+        ...         pageURL="http://mywebsite.com/kasada",
+        ...         proxyType="http",
+        ...         proxyAddress="0.0.0.0",
+        ...         proxyPort=9090,
+        ...         proxyLogin="some_login",
+        ...         proxyPassword="some_password",
+        ...        ).captcha_handler()
         CaptchaResponseSer(errorId=False,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
-                           solution={'gRecaptchaResponse': '44795sds...'}
+                           solution={
+                               "x-kpsdk-ct": "",
+                                "x-kpsdk-cd": "",
+                                "user-agent": "Mozilla/5.0 (Windows NT 10...."
+                            }
+                          )
+
+        >>> Kasada(api_key="CAI-1324...",
+        ...         pageURL="http://mywebsite.com/kasada",
+        ...         proxyType="http",
+        ...         proxyAddress="0.0.0.0",
+        ...         proxyPort=9090,
+        ...         proxyLogin="some_login",
+        ...         proxyPassword="some_password",
+        ...        ).captcha_handler(userAgent="Mozilla/5.0 (pl.....")
+        CaptchaResponseSer(errorId=False,
+                           errorCode=None,
+                           errorDescription=None,
+                           taskId='73bdcd28-6c77-4414-8....',
+                           status=<ResponseStatusEnm.Ready: 'ready'>,
+                           solution={
+                               "x-kpsdk-ct": "",
+                                "x-kpsdk-cd": "",
+                                "user-agent": "Mozilla/5.0 (Windows NT 10...."
+                            }
                           )
 
     Returns:
         CaptchaResponseSer model with full server response
 
     Notes:
-        https://captchaai.atlassian.net/wiki/spaces/CAPTCHAAI/pages/394048
-        https://captchaai.atlassian.net/wiki/spaces/CAPTCHAAI/pages/426338
+        https://captchaai.atlassian.net/wiki/spaces/CAPTCHAAI/pages/426407
     """
 
     def __init__(
         self,
         api_key: str,
-        captcha_type: Union[CaptchaTypeEnm, str],
-        websiteURL: str,
-        gt: str,
-        proxyType: Optional[Union[ProxyType, str]] = None,
-        proxyAddress: Optional[str] = None,
-        proxyPort: Optional[int] = None,
+        pageURL: str,
+        proxyType: Union[ProxyType, str],
+        proxyAddress: str,
+        proxyPort: int,
+        proxyLogin: str,
+        proxyPassword: str,
         sleep_time: Optional[int] = 5,
         request_url: Optional[str] = REQUEST_URL,
     ):
+        self.task_postfix = "/kasada/invoke"
 
-        super().__init__(api_key=api_key, captcha_type=captcha_type, sleep_time=sleep_time, request_url=request_url)
+        super().__init__(api_key=api_key, sleep_time=sleep_time, request_url=request_url)
 
-        # validation of the received parameters for GeetestTaskProxyless
-        if self.captcha_type == CaptchaTypeEnm.GeetestTaskProxyless:
-            self.task_params = GeeTestProxyLessOptionsSer(**locals()).dict()
-        # validation of the received parameters for GeetestTask
-        elif self.captcha_type == CaptchaTypeEnm.GeetestTask:
-            self.task_params = GeeTestOptionsSer(**locals()).dict()
-        else:
-            raise ValueError(
-                f"""Invalid `captcha_type` parameter set for `{self.__class__.__name__}`,
-                available - {CaptchaTypeEnm.GeetestTaskProxyless.value,
-                             CaptchaTypeEnm.GeetestTask.value}"""
-            )
+        self.task_params = KasadaOptionsSer(**locals()).dict()
 
 
-class GeeTest(BaseGeeTest):
-    __doc__ = BaseGeeTest.__doc__
+class Kasada(BaseKasada):
+    __doc__ = BaseKasada.__doc__
 
-    def captcha_handler(
-        self,
-        challenge: str,
-        **additional_params,
-    ) -> CaptchaResponseSer:
+    def captcha_handler(self, **additional_params) -> CaptchaResponseSer:
         """
         Synchronous method for captcha solving
 
         Args:
-            challenge: Changing token key.
-                        Make sure you grab a fresh one for each captcha;
-                        otherwise, you'll be charged for an error task.
             additional_params: Some additional parameters that will be used in creating the task
                                 and will be passed to the payload under ``task`` key.
-                                Like ``coordinate``, ``enterprisePayload`` and etc. - more info in service docs
+                                Like ``onlyCD``, ``userAgent`` and etc. - more info in service docs
 
         Examples:
-            >>> GeeTest(api_key="CAI-1324...",
-            ...         captcha_type="GeetestTaskProxyless",
-            ...         websiteURL="https://www.geetest.com/en/demo",
-            ...         gt="022397c99c9f646f6477822485f30404",
-            ...        ).captcha_handler(
-            ...                    challenge="a66f31a53a404af8d1f271eec5138aa1",
-            ...                    geetestApiServerSubdomain="api.geetest.com"
-            ...                )
+            >>> Kasada(api_key="CAI-1324...",
+            ...         pageURL="http://mywebsite.com/kasada",
+            ...         proxyType="http",
+            ...         proxyAddress="0.0.0.0",
+            ...         proxyPort=9090,
+            ...         proxyLogin="some_login",
+            ...         proxyPassword="some_password",
+            ...        ).captcha_handler()
             CaptchaResponseSer(errorId=False,
                                errorCode=None,
                                errorDescription=None,
                                taskId='73bdcd28-6c77-4414-8....',
                                status=<ResponseStatusEnm.Ready: 'ready'>,
-                               solution={'gRecaptchaResponse': '44795sds...'}
+                               solution={
+                                   "x-kpsdk-ct": "",
+                                    "x-kpsdk-cd": "",
+                                    "user-agent": "Mozilla/5.0 (Windows NT 10...."
+                                }
                               )
 
         Returns:
             CaptchaResponseSer model with full service response
 
         Notes:
-            Check class docstirng for more info
+            Check class docstring for more info
         """
-        self.task_params.update({**additional_params, "challenge": challenge})
-        return self._processing_captcha(serializer=RequestCreateTaskSer, type=self.captcha_type, **self.task_params)
+        self.task_params.update({**additional_params})
+        self._prepare_create_task_payload(serializer=RequestCreateTaskSer, create_params=self.task_params)
+        return CaptchaResponseSer(**self._create_task(url_postfix=self.task_postfix))
 
-    async def aio_captcha_handler(
-        self,
-        challenge: str,
-        **additional_params,
-    ) -> CaptchaResponseSer:
+    async def aio_captcha_handler(self, **additional_params) -> CaptchaResponseSer:
         """
         Asynchronous method for captcha solving
 
         Args:
-            challenge: Changing token key.
-                        Make sure you grab a fresh one for each captcha;
-                        otherwise, you'll be charged for an error task.
             additional_params: Some additional parameters that will be used in creating the task
                                 and will be passed to the payload under ``task`` key.
-                                Like ``coordinate``, ``enterprisePayload`` and etc. - more info in service docs
+                                Like ``onlyCD``, ``userAgent`` and etc. - more info in service docs
 
         Examples:
-            >>> await GeeTest(api_key="CAI-1324...",
-            ...                 captcha_type="GeetestTaskProxyless",
-            ...                 websiteURL="https://www.geetest.com/en/demo",
-            ...                 gt="022397c99c9f646f6477822485f30404",
-            ...             ).aio_captcha_handler(
-            ...                    challenge="a66f31a53a404af8d1f271eec5138aa1",
-            ...                    geetestApiServerSubdomain="api.geetest.com"
-            ...                )
+            >>> await Kasada(api_key="CAI-1324...",
+            ...         pageURL="http://mywebsite.com/kasada",
+            ...         proxyType="http",
+            ...         proxyAddress="0.0.0.0",
+            ...         proxyPort=9090,
+            ...         proxyLogin="some_login",
+            ...         proxyPassword="some_password",
+            ...        ).aio_captcha_handler()
             CaptchaResponseSer(errorId=False,
                                errorCode=None,
                                errorDescription=None,
                                taskId='73bdcd28-6c77-4414-8....',
                                status=<ResponseStatusEnm.Ready: 'ready'>,
-                               solution={'gRecaptchaResponse': '44795sds...'}
+                               solution={
+                                   "x-kpsdk-ct": "",
+                                    "x-kpsdk-cd": "",
+                                    "user-agent": "Mozilla/5.0 (Windows NT 10...."
+                                }
                               )
 
         Returns:
             CaptchaResponseSer model with full service response
 
         Notes:
-            Check class docstirng for more info
+            Check class docstring for more info
         """
-        self.task_params.update({**additional_params, "challenge": challenge})
-        return await self._aio_processing_captcha(
-            serializer=RequestCreateTaskSer, type=self.captcha_type, **self.task_params
-        )
+        self.task_params.update({**additional_params})
+        self._prepare_create_task_payload(serializer=RequestCreateTaskSer, create_params=self.task_params)
+        return CaptchaResponseSer(**await self._aio_create_task(url_postfix=self.task_postfix))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python3-capsolver-0.5.6/python3_capsolver/hcaptcha.py` & `python3-capsolver-0.5.7/python3_capsolver/hcaptcha.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,25 +10,14 @@
     The class is used to work with Capsolver HCaptcha methods.
 
     Args:
         api_key: Capsolver API key
         captcha_type: Captcha type name, like ``HCaptchaTaskProxyless`` and etc.
         websiteURL: Address of a webpage with hCaptcha
         websiteKey: hCaptcha website key
-        queries: Base64-encoded images, do not include "data : image / *** ; base64,".
-                    Format to send: [“base64”,”base64”,”base64”,…..]
-        question: Question ID. Support English and Chinese, other languages please convert yourself
-        proxyType: Type of the proxy
-        proxyAddress: Proxy IP address IPv4/IPv6. Not allowed to use:
-                        host names instead of IPs,
-                        transparent proxies (where client IP is visible),
-                        proxies from local networks (192.., 10.., 127...)
-        proxyPort: Proxy port.
-        sleep_time: The waiting time between requests to get the result of the Captcha
-        request_url: API address for sending requests
 
     Examples:
         >>> HCaptcha(api_key="CAI-BA9XXXXXXXXXXXXX2702E010",
         ...          captcha_type='HCaptchaTaskProxyless',
         ...          websiteURL="https://accounts.hcaptcha.com/demo",
         ...          websiteKey="a5f74b19-9e45-40e0-b45d-47ff91b7a6c2",
         ...         ).captcha_handler()
@@ -37,30 +26,43 @@
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
                            solution={'gRecaptchaResponse': '44795sds...'}
                           )
 
         >>> HCaptcha(api_key="CAI-BA9XXXXXXXXXXXXX2702E010",
-        ...          captcha_type='HCaptchaTask',
+        ...          captcha_type=HCaptchaTypeEnm.HCaptchaEnterpriseTaskProxyLess,
+        ...          websiteURL="https://accounts.hcaptcha.com/demo",
+        ...          websiteKey="a5f74b19-9e45-40e0-b45d-47ff91b7a6c2",
+        ...         ).captcha_handler()
+        CaptchaResponseSer(errorId=False,
+                           errorCode=None,
+                           errorDescription=None,
+                           taskId='73bdcd28-6c77-4414-8....',
+                           status=<ResponseStatusEnm.Ready: 'ready'>,
+                           solution={'gRecaptchaResponse': '44795sds...'}
+                          )
+
+        >>> HCaptcha(api_key="CAI-BA9XXXXXXXXXXXXX2702E010",
+        ...          captcha_type=HCaptchaTypeEnm.HCaptchaTask,
         ...          websiteURL="https://accounts.hcaptcha.com/demo",
         ...          websiteKey="a5f74b19-9e45-40e0-b45d-47ff91b7a6c2",
         ...          proxy="socks5:192.191.100.10:4780:user:pwd"
         ...          isInvisible=True
         ...         ).captcha_handler()
         CaptchaResponseSer(errorId=False,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
                            solution={'gRecaptchaResponse': '44795sds...'}
                           )
 
         >>> await HCaptcha(api_key="CAI-BA9650D2B9C2786B21120D512702E010",
-        ...          captcha_type='HCaptchaTaskProxyless',
+        ...          captcha_type=HCaptchaTypeEnm.HCaptchaTaskProxyless,
         ...          websiteURL="https://accounts.hcaptcha.com/demo",
         ...          websiteKey="a5f74b19-9e45-40e0-b45d-47ff91b7a6c2",
         ...         ).aio_captcha_handler()
         CaptchaResponseSer(errorId=False,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `python3-capsolver-0.5.6/python3_capsolver/image_to_text.py` & `python3-capsolver-0.5.7/python3_capsolver/image_to_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from python3_capsolver.core.base import BaseCaptcha
-from python3_capsolver.core.enum import CaptchaTypeEnm
 from python3_capsolver.core.config import REQUEST_URL
 from python3_capsolver.core.serializer import CaptchaResponseSer, RequestCreateTaskSer
 
 
 class BaseImageToText(BaseCaptcha):
     """
     The class is used to work with Capsolver Image captcha solving methods.
@@ -74,17 +73,15 @@
     def __init__(
         self,
         api_key: str,
         sleep_time: int = 10,
         request_url: str = REQUEST_URL,
     ):
 
-        super().__init__(
-            api_key=api_key, sleep_time=sleep_time, request_url=request_url, captcha_type=CaptchaTypeEnm.ImageToTextTask
-        )
+        super().__init__(api_key=api_key, sleep_time=sleep_time, request_url=request_url)
 
 
 class ImageToText(BaseImageToText):
     __doc__ = BaseImageToText.__doc__
 
     def captcha_handler(self, body: str, **additional_params) -> CaptchaResponseSer:
         """
@@ -108,15 +105,15 @@
                                solution={'gRecaptchaResponse': '44795sds...'}
                               )
 
         Returns:
             CaptchaResponseSer model with full server response
 
         Notes:
-            Check class docstirng for more info
+            Check class docstring for more info
         """
         return self._processing_captcha(
             serializer=RequestCreateTaskSer, type=self.captcha_type, body=body, **additional_params
         )
 
     async def aio_captcha_handler(self, body: str, **additional_params) -> CaptchaResponseSer:
         """
@@ -140,12 +137,12 @@
                                solution={'gRecaptchaResponse': '44795sds...'}
                               )
 
         Returns:
             CaptchaResponseSer model with full server response
 
         Notes:
-            Check class docstirng for more info
+            Check class docstring for more info
         """
         return await self._aio_processing_captcha(
             serializer=RequestCreateTaskSer, type=self.captcha_type, body=body, **additional_params
         )
```

### Comparing `python3-capsolver-0.5.6/python3_capsolver/mt_captcha.py` & `python3-capsolver-0.5.7/python3_capsolver/mt_captcha.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Optional
 
 from python3_capsolver.core.base import BaseCaptcha
-from python3_capsolver.core.enum import CaptchaTypeEnm
 from python3_capsolver.core.config import REQUEST_URL
 from python3_capsolver.core.serializer import CaptchaResponseSer, MtCaptchaOptionsSer, RequestCreateTaskSer
 
 
 class BaseMtCaptcha(BaseCaptcha):
     """
     The class is used to work with Capsolver MtCaptcha method.
@@ -86,15 +85,14 @@
         proxy: str,
         sleep_time: Optional[int] = 5,
         request_url: Optional[str] = REQUEST_URL,
     ):
 
         super().__init__(
             api_key=api_key,
-            captcha_type=CaptchaTypeEnm.MtCaptchaTask,
             sleep_time=sleep_time,
             request_url=request_url,
         )
 
         self.task_params = MtCaptchaOptionsSer(**locals()).dict()
 
 
@@ -127,15 +125,15 @@
                                solution={'token': 'v1(03,79a,MTPublic-tqNCRE0GS,c9...'}
                               )
 
         Returns:
             CaptchaResponseSer model with full service response
 
         Notes:
-            Check class docstirng for more info
+            Check class docstring for more info
         """
         return self._processing_captcha(serializer=RequestCreateTaskSer, type=self.captcha_type, **additional_params)
 
     async def aio_captcha_handler(
         self,
         **additional_params,
     ) -> CaptchaResponseSer:
@@ -161,12 +159,12 @@
                                solution={'token': 'v1(03,79a,MTPublic-tqNCRE0GS,c9...'}
                               )
 
         Returns:
             CaptchaResponseSer model with full service response
 
         Notes:
-            Check class docstirng for more info
+            Check class docstring for more info
         """
         return await self._aio_processing_captcha(
             serializer=RequestCreateTaskSer, type=self.captcha_type, **additional_params
         )
```

### Comparing `python3-capsolver-0.5.6/python3_capsolver.egg-info/PKG-INFO` & `python3-capsolver-0.5.7/python3_capsolver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-capsolver
-Version: 0.5.6
+Version: 0.5.7
 Summary: Python 3.7+ Capsolver library with AIO module.
 Home-page: https://andreidrang.github.io/python3-capsolver/
 Author: AndreiDrang
 Author-email: python-captcha@pm.me
 License: MIT
 Project-URL: Documentation, https://andreidrang.github.io/python3-capsolver/
 Project-URL: Source, https://github.com/AndreiDrang/python3-captchaai
```

### Comparing `python3-capsolver-0.5.6/python3_capsolver.egg-info/SOURCES.txt` & `python3-capsolver-0.5.7/python3_capsolver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.5.6/setup.py` & `python3-capsolver-0.5.7/setup.py`

 * *Files identical despite different names*

