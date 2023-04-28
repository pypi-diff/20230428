# Comparing `tmp/nautobot_data_validation_engine-2.0.0.tar.gz` & `tmp/nautobot_data_validation_engine-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_data_validation_engine-2.0.0.tar", max compression
+gzip compressed data, was "nautobot_data_validation_engine-2.0.1.tar", max compression
```

## Comparing `nautobot_data_validation_engine-2.0.0.tar` & `nautobot_data_validation_engine-2.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      591 2023-04-04 15:45:05.976216 nautobot_data_validation_engine-2.0.0/LICENSE
--rw-r--r--   0        0        0     4876 2023-04-04 15:45:05.976216 nautobot_data_validation_engine-2.0.0/README.md
--rw-r--r--   0        0        0     1026 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/__init__.py
--rw-r--r--   0        0        0       66 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/api/__init__.py
--rw-r--r--   0        0        0     2598 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/api/nested_serializers.py
--rw-r--r--   0        0        0     4258 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/api/serializers.py
--rw-r--r--   0        0        0      605 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/api/urls.py
--rw-r--r--   0        0        0     1727 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/api/views.py
--rw-r--r--   0        0        0     5509 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/custom_validators.py
--rw-r--r--   0        0        0     4261 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/filters.py
--rw-r--r--   0        0        0    11119 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/forms.py
--rw-r--r--   0        0        0     3452 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/migrations/0001_initial.py
--rw-r--r--   0        0        0     5786 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/migrations/0002_required_unique_types_regex_context.py
--rw-r--r--   0        0        0        0 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/migrations/__init__.py
--rw-r--r--   0        0        0    13313 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/models.py
--rw-r--r--   0        0        0     4248 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/navigation.py
--rw-r--r--   0        0        0     3392 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/tables.py
--rw-r--r--   0        0        0     1110 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/minmaxvalidationrule_retrieve.html
--rw-r--r--   0        0        0     1204 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/regularexpressionvalidationrule_retrieve.html
--rw-r--r--   0        0        0      907 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/requiredvalidationrule_retrieve.html
--rw-r--r--   0        0        0     1017 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/uniquevalidationrule_retrieve.html
--rw-r--r--   0        0        0       61 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/tests/__init__.py
--rw-r--r--   0        0        0     8124 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/tests/test_api.py
--rw-r--r--   0        0        0     1536 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/tests/test_basic.py
--rw-r--r--   0        0        0    13489 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/tests/test_custom_validators.py
--rw-r--r--   0        0        0     9131 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/tests/test_filters.py
--rw-r--r--   0        0        0    11014 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/tests/test_models.py
--rw-r--r--   0        0        0     8877 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/tests/test_views.py
--rw-r--r--   0        0        0     2246 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/urls.py
--rw-r--r--   0        0        0     2994 2023-04-04 15:45:05.980216 nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/views.py
--rw-r--r--   0        0        0     3700 2023-04-04 15:45:19.552399 nautobot_data_validation_engine-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     5911 1970-01-01 00:00:00.000000 nautobot_data_validation_engine-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      591 2023-04-28 17:25:51.701840 nautobot_data_validation_engine-2.0.1/LICENSE
+-rw-r--r--   0        0        0     4876 2023-04-28 17:25:51.701840 nautobot_data_validation_engine-2.0.1/README.md
+-rw-r--r--   0        0        0     1026 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/__init__.py
+-rw-r--r--   0        0        0       66 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/api/__init__.py
+-rw-r--r--   0        0        0     2598 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/api/nested_serializers.py
+-rw-r--r--   0        0        0     4258 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/api/serializers.py
+-rw-r--r--   0        0        0      605 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/api/urls.py
+-rw-r--r--   0        0        0     1727 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/api/views.py
+-rw-r--r--   0        0        0     5509 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/custom_validators.py
+-rw-r--r--   0        0        0     4261 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/filters.py
+-rw-r--r--   0        0        0    11119 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/forms.py
+-rw-r--r--   0        0        0     3452 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/migrations/0001_initial.py
+-rw-r--r--   0        0        0     5786 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/migrations/0002_required_unique_types_regex_context.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/migrations/__init__.py
+-rw-r--r--   0        0        0    13313 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/models.py
+-rw-r--r--   0        0        0     4248 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/navigation.py
+-rw-r--r--   0        0        0     3392 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tables.py
+-rw-r--r--   0        0        0     1110 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/minmaxvalidationrule_retrieve.html
+-rw-r--r--   0        0        0     1204 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/regularexpressionvalidationrule_retrieve.html
+-rw-r--r--   0        0        0      907 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/requiredvalidationrule_retrieve.html
+-rw-r--r--   0        0        0     1017 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/uniquevalidationrule_retrieve.html
+-rw-r--r--   0        0        0       61 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/__init__.py
+-rw-r--r--   0        0        0     8124 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/test_api.py
+-rw-r--r--   0        0        0     1536 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/test_basic.py
+-rw-r--r--   0        0        0    13489 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/test_custom_validators.py
+-rw-r--r--   0        0        0     9131 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/test_filters.py
+-rw-r--r--   0        0        0    11014 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/test_models.py
+-rw-r--r--   0        0        0     8877 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/test_views.py
+-rw-r--r--   0        0        0     2246 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/urls.py
+-rw-r--r--   0        0        0     2994 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/views.py
+-rw-r--r--   0        0        0     3700 2023-04-28 17:26:02.073921 nautobot_data_validation_engine-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5911 1970-01-01 00:00:00.000000 nautobot_data_validation_engine-2.0.1/PKG-INFO
```

### Comparing `nautobot_data_validation_engine-2.0.0/LICENSE` & `nautobot_data_validation_engine-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/README.md` & `nautobot_data_validation_engine-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/__init__.py` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/api/nested_serializers.py` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/api/serializers.py` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/api/serializers.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/api/urls.py` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/api/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/api/views.py` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/api/views.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/custom_validators.py` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/custom_validators.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/filters.py` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/forms.py` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/forms.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/migrations/0001_initial.py` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/migrations/0002_required_unique_types_regex_context.py` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/migrations/0002_required_unique_types_regex_context.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/models.py` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/models.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/navigation.py` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/navigation.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/tables.py` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tables.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/minmaxvalidationrule_retrieve.html` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/minmaxvalidationrule_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/regularexpressionvalidationrule_retrieve.html` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/regularexpressionvalidationrule_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/requiredvalidationrule_retrieve.html` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/requiredvalidationrule_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/uniquevalidationrule_retrieve.html` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/uniquevalidationrule_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/tests/test_api.py` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/tests/test_basic.py` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/tests/test_custom_validators.py` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/test_custom_validators.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/tests/test_filters.py` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/tests/test_models.py` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/tests/test_views.py` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/urls.py` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/nautobot_data_validation_engine/views.py` & `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/views.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.0/pyproject.toml` & `nautobot_data_validation_engine-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-data-validation-engine"
-version = "v2.0.0"
+version = "v2.0.1"
 description = "Provides UI to build custom data validation rules for data in Nautobot"
 authors = ["Network to Code, LLC <info@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-plugin-data-validation-engine"
 repository = "https://github.com/nautobot/nautobot-plugin-data-validation-engine"
 keywords = ["nautobot", "nautobot-plugin", "data", "validation", "django"]
```

### Comparing `nautobot_data_validation_engine-2.0.0/PKG-INFO` & `nautobot_data_validation_engine-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautobot-data-validation-engine
-Version: 2.0.0
+Version: 2.0.1
 Summary: Provides UI to build custom data validation rules for data in Nautobot
 Home-page: https://github.com/nautobot/nautobot-plugin-data-validation-engine
 License: Apache-2.0
 Keywords: nautobot,nautobot-plugin,data,validation,django
 Author: Network to Code, LLC
 Author-email: info@networktocode.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nautobot-data-validation-engine Version: 2.0.0
+Metadata-Version: 2.1 Name: nautobot-data-validation-engine Version: 2.0.1
 Summary: Provides UI to build custom data validation rules for data in Nautobot
 Home-page: https://github.com/nautobot/nautobot-plugin-data-validation-engine
 License: Apache-2.0 Keywords: nautobot,nautobot-plugin,data,validation,django
 Author: Network to Code, LLC Author-email: info@networktocode.com Requires-
 Python: >=3.7,<4.0 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

