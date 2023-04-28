# Comparing `tmp/capmonstercloudclient-1.2.2.tar.gz` & `tmp/capmonstercloudclient-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capmonstercloudclient-1.2.2.tar", last modified: Fri Apr 14 13:10:08 2023, max compression
+gzip compressed data, was "capmonstercloudclient-1.3.0.tar", last modified: Fri Apr 28 13:39:02 2023, max compression
```

## Comparing `capmonstercloudclient-1.2.2.tar` & `capmonstercloudclient-1.3.0.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:10:08.029091 capmonstercloudclient-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-14 13:10:08.029091 capmonstercloudclient-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:10:08.021090 capmonstercloudclient-1.2.2/capmonstercloud_client/
--rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/CapMonsterCloudClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/GetResultTimeouts.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/captchaResult.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/clientOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requestController.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:10:08.029091 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/ComplexImageTaskBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/FuncaptchaProxylessRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/FuncaptchaRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/FuncaptchaRequestBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/GeetestProxylessRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/GeetestRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/GeetestRequestBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/HcaptchaComplexImageTask.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/HcaptchaProxylessRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/HcaptchaRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/HcaptchaRequestBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/ImageToTextRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/RecaptchaComplexImageTask.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/RecaptchaV2EnterpiseRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/RecaptchaV2EnterpriseProxylessRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/RecaptchaV2EnterpriseRequestBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/RecaptchaV2ProxylessRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/RecaptchaV2Request.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/RecaptchaV2RequestBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/RecaptchaV3ProxylessRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/TurnstileProxylessRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/TurnstileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/TurnstileRequestBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/baseRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/requests/proxy_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/capmonstercloud_client/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:10:08.029091 capmonstercloudclient-1.2.2/capmonstercloudclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-14 13:10:08.000000 capmonstercloudclient-1.2.2/capmonstercloudclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-14 13:10:08.000000 capmonstercloudclient-1.2.2/capmonstercloudclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 13:10:08.000000 capmonstercloudclient-1.2.2/capmonstercloudclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-14 13:10:08.000000 capmonstercloudclient-1.2.2/capmonstercloudclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 13:10:08.000000 capmonstercloudclient-1.2.2/capmonstercloudclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 13:10:08.029091 capmonstercloudclient-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-14 13:09:58.000000 capmonstercloudclient-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:39:02.030903 capmonstercloudclient-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-28 13:39:02.030903 capmonstercloudclient-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:39:02.018903 capmonstercloudclient-1.3.0/capmonstercloud_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/CapMonsterCloudClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/GetResultTimeouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/captchaResult.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/clientOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requestController.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:39:02.030903 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/ComplexImageTaskBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/FuncaptchaComplexImageTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/FuncaptchaProxylessRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/FuncaptchaRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/FuncaptchaRequestBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/GeetestProxylessRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/GeetestRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/GeetestRequestBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/HcaptchaComplexImageTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/HcaptchaProxylessRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/HcaptchaRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/HcaptchaRequestBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/ImageToTextRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/RecaptchaComplexImageTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/RecaptchaV2EnterpiseRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/RecaptchaV2EnterpriseProxylessRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/RecaptchaV2EnterpriseRequestBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/RecaptchaV2ProxylessRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/RecaptchaV2Request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/RecaptchaV2RequestBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/RecaptchaV3ProxylessRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/TurnstileProxylessRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/TurnstileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/TurnstileRequestBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/baseRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/requests/proxy_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/capmonstercloud_client/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:39:02.030903 capmonstercloudclient-1.3.0/capmonstercloudclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-28 13:39:01.000000 capmonstercloudclient-1.3.0/capmonstercloudclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-28 13:39:02.000000 capmonstercloudclient-1.3.0/capmonstercloudclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:39:01.000000 capmonstercloudclient-1.3.0/capmonstercloudclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-28 13:39:01.000000 capmonstercloudclient-1.3.0/capmonstercloudclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 13:39:01.000000 capmonstercloudclient-1.3.0/capmonstercloudclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 13:39:02.030903 capmonstercloudclient-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-28 13:38:50.000000 capmonstercloudclient-1.3.0/setup.py
```

### Comparing `capmonstercloudclient-1.2.2/LICENSE` & `capmonstercloudclient-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/PKG-INFO` & `capmonstercloudclient-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capmonstercloudclient
-Version: 1.2.2
+Version: 1.3.0
 Summary: Official CapMonsterCloud Client: https://capmonster.cloud/
 Home-page: https://github.com/ZennoLab/capmonstercloud-client-python
 Author: Andrey Ilyin
 Author-email: andrey.ilyin@zennolab.com
 License: AGPL-3.0
 Keywords: captcha 
 				recaptcha
```

### Comparing `capmonstercloudclient-1.2.2/README.md` & `capmonstercloudclient-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/CapMonsterCloudClient.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/CapMonsterCloudClient.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     ((RecaptchaV2EnterpriseProxylessRequest, RecaptchaV2EnterpriseRequest), getRecaptchaV2EnterpriseTimeouts),
     ((RecaptchaV3ProxylessRequest), getRecaptchaV3Timeouts),
     ((ImageToTextRequest), getImage2TextTimeouts),
     ((FuncaptchaProxylessRequest, FuncaptchaRequest), getFuncaptchaTimeouts),
     ((HcaptchaProxylessRequest, HcaptchaRequest), getHcaptchaTimeouts),
     ((GeetestProxylessRequest, GeetestRequest), getGeetestTimeouts),
     ((TurnstileProxylessRequest, TurnstileRequest), getTurnstileTimeouts),
-    ((RecaptchaComplexImageTaskRequest, HcaptchaComplexImageTaskRequest), getImage2TextTimeouts),
+    ((RecaptchaComplexImageTaskRequest, HcaptchaComplexImageTaskRequest, 
+      FunCaptchaComplexImageTaskRequest), getImage2TextTimeouts),
 )
 
 
 class CapMonsterClient:
     def __init__(self, 
                  options: ClientOptions) -> None:
         self.options = options
@@ -64,15 +65,16 @@
                                                  HcaptchaRequest, 
                                                  HcaptchaProxylessRequest,
                                                  GeetestProxylessRequest, 
                                                  GeetestRequest,
                                                  TurnstileProxylessRequest, 
                                                  TurnstileRequest,
                                                  HcaptchaComplexImageTaskRequest, 
-                                                 RecaptchaComplexImageTaskRequest],
+                                                 RecaptchaComplexImageTaskRequest,
+                                                 FunCaptchaComplexImageTaskRequest],
                             ) -> Dict[str, str]:
         '''
         Non-blocking method for captcha solving. 
 
         Args:
             request : This object must be an instance of "requests", otherwise an exception will be thrown
         '''
@@ -94,15 +96,16 @@
                                           HcaptchaRequest, 
                                           HcaptchaProxylessRequest,
                                           GeetestProxylessRequest, 
                                           GeetestRequest,
                                           TurnstileProxylessRequest, 
                                           TurnstileRequest,
                                           HcaptchaComplexImageTaskRequest, 
-                                          RecaptchaComplexImageTaskRequest],
+                                          RecaptchaComplexImageTaskRequest,
+                                          FunCaptchaComplexImageTaskRequest],
                            timeouts: GetResultTimeouts,
                            ) -> Dict[str, str]:
 
         getTaskResponse = await self._createTask(request)
         if getTaskResponse.get('errorId') != 0:
             raise GetTaskError(f'[{getTaskResponse.get("errorCode")}] ' \
                                f'{getTaskResponse.get("errorDescription")}.')
```

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/GetResultTimeouts.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/GetResultTimeouts.py`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/clientOptions.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/clientOptions.py`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/exceptions.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/requests/ComplexImageTaskBase.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/requests/ComplexImageTaskBase.py`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/requests/FuncaptchaProxylessRequest.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/requests/FuncaptchaProxylessRequest.py`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/requests/FuncaptchaRequest.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/requests/FuncaptchaRequest.py`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/requests/GeetestProxylessRequest.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/requests/GeetestProxylessRequest.py`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/requests/GeetestRequest.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/requests/GeetestRequest.py`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/requests/HcaptchaComplexImageTask.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/requests/HcaptchaComplexImageTask.py`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/requests/HcaptchaProxylessRequest.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/requests/HcaptchaProxylessRequest.py`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/requests/HcaptchaRequest.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/requests/HcaptchaRequest.py`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/requests/ImageToTextRequest.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/requests/ImageToTextRequest.py`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/requests/RecaptchaComplexImageTask.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/requests/RecaptchaComplexImageTask.py`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/requests/RecaptchaV2EnterpiseRequest.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/requests/RecaptchaV2EnterpiseRequest.py`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/requests/RecaptchaV2EnterpriseProxylessRequest.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/requests/RecaptchaV2EnterpriseProxylessRequest.py`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/requests/RecaptchaV2ProxylessRequest.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/requests/RecaptchaV2ProxylessRequest.py`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/requests/RecaptchaV2Request.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/requests/RecaptchaV2Request.py`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/requests/RecaptchaV3ProxylessRequest.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/requests/RecaptchaV3ProxylessRequest.py`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/requests/TurnstileProxylessRequest.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/requests/TurnstileProxylessRequest.py`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/requests/TurnstileRequest.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/requests/TurnstileRequest.py`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/requests/__init__.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/requests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .RecaptchaV2EnterpriseProxylessRequest import RecaptchaV2EnterpriseProxylessRequest
 from .RecaptchaV2EnterpiseRequest import RecaptchaV2EnterpriseRequest
 from .RecaptchaV3ProxylessRequest import RecaptchaV3ProxylessRequest
 from .HcaptchaProxylessRequest import HcaptchaProxylessRequest
 from .HcaptchaRequest import HcaptchaRequest
 from .FuncaptchaProxylessRequest import FuncaptchaProxylessRequest
 from .FuncaptchaRequest import FuncaptchaRequest
+from .FuncaptchaComplexImageTask import FunCaptchaComplexImageTaskRequest
 from .GeetestProxylessRequest import GeetestProxylessRequest
 from .GeetestRequest import GeetestRequest
 from .TurnstileProxylessRequest import TurnstileProxylessRequest
 from .TurnstileRequest import TurnstileRequest
 from .HcaptchaComplexImageTask import HcaptchaComplexImageTaskRequest
 from .RecaptchaComplexImageTask import RecaptchaComplexImageTaskRequest
 from .baseRequest import BaseRequest
```

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/requests/enums.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/requests/enums.py`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/requests/proxy_info.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/requests/proxy_info.py`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloud_client/utils.py` & `capmonstercloudclient-1.3.0/capmonstercloud_client/utils.py`

 * *Files identical despite different names*

### Comparing `capmonstercloudclient-1.2.2/capmonstercloudclient.egg-info/PKG-INFO` & `capmonstercloudclient-1.3.0/capmonstercloudclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capmonstercloudclient
-Version: 1.2.2
+Version: 1.3.0
 Summary: Official CapMonsterCloud Client: https://capmonster.cloud/
 Home-page: https://github.com/ZennoLab/capmonstercloud-client-python
 Author: Andrey Ilyin
 Author-email: andrey.ilyin@zennolab.com
 License: AGPL-3.0
 Keywords: captcha 
 				recaptcha
```

### Comparing `capmonstercloudclient-1.2.2/capmonstercloudclient.egg-info/SOURCES.txt` & `capmonstercloudclient-1.3.0/capmonstercloudclient.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 capmonstercloud_client/captchaResult.py
 capmonstercloud_client/clientOptions.py
 capmonstercloud_client/exceptions.py
 capmonstercloud_client/requestController.py
 capmonstercloud_client/utils.py
 capmonstercloud_client/version.txt
 capmonstercloud_client/requests/ComplexImageTaskBase.py
+capmonstercloud_client/requests/FuncaptchaComplexImageTask.py
 capmonstercloud_client/requests/FuncaptchaProxylessRequest.py
 capmonstercloud_client/requests/FuncaptchaRequest.py
 capmonstercloud_client/requests/FuncaptchaRequestBase.py
 capmonstercloud_client/requests/GeetestProxylessRequest.py
 capmonstercloud_client/requests/GeetestRequest.py
 capmonstercloud_client/requests/GeetestRequestBase.py
 capmonstercloud_client/requests/HcaptchaComplexImageTask.py
```

### Comparing `capmonstercloudclient-1.2.2/setup.py` & `capmonstercloudclient-1.3.0/setup.py`

 * *Files identical despite different names*

