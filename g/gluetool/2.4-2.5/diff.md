# Comparing `tmp/gluetool-2.4.tar.gz` & `tmp/gluetool-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gluetool-2.4.tar", max compression
+gzip compressed data, was "gluetool-2.5.tar", max compression
```

## Comparing `gluetool-2.4.tar` & `gluetool-2.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1072 2023-03-14 16:49:21.402618 gluetool-2.4/README.rst
--rw-r--r--   0        0        0     4522 2023-03-14 16:49:21.402618 gluetool-2.4/assets/html-log/prism.css
--rw-r--r--   0        0        0    13651 2023-03-14 16:49:21.402618 gluetool-2.4/assets/html-log/prism.js
--rw-r--r--   0        0        0   628536 2023-03-14 16:49:21.404618 gluetool-2.4/assets/html-log/semantic.min.css
--rw-r--r--   0        0        0   275730 2023-03-14 16:49:21.405618 gluetool-2.4/assets/html-log/semantic.min.js
--rw-r--r--   0        0        0      351 2023-03-14 16:49:21.406618 gluetool-2.4/gluetool/__init__.py
--rw-r--r--   0        0        0    12916 2023-03-14 16:49:21.406618 gluetool-2.4/gluetool/action.py
--rw-r--r--   0        0        0     2167 2023-03-14 16:49:21.406618 gluetool-2.4/gluetool/color.py
--rw-r--r--   0        0        0      765 2023-03-14 16:49:21.406618 gluetool-2.4/gluetool/core.moduleinfo
--rw-r--r--   0        0        0    97437 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/glue.py
--rw-r--r--   0        0        0    19758 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/help.py
--rw-r--r--   0        0        0    14613 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/html_log.py
--rw-r--r--   0        0        0    47722 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/log.py
--rw-r--r--   0        0        0     3752 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/proxy.py
--rw-r--r--   0        0        0        0 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/py.typed
--rw-r--r--   0        0        0     4254 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/pylint/__init__.py
--rw-r--r--   0        0        0     5248 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/pylint/option_default.py
--rw-r--r--   0        0        0     4698 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/pylint/shared_defined.py
--rw-r--r--   0        0        0     3221 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/pylint/unknown_option.py
--rw-r--r--   0        0        0     6265 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/result.py
--rw-r--r--   0        0        0     9411 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/sentry.py
--rw-r--r--   0        0        0     2620 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/tests/__init__.py
--rw-r--r--   0        0        0      311 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/tests/assets/parse_config/configroot/config/data_config_root_a
--rw-r--r--   0        0        0      321 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/tests/assets/parse_config/configroot/config/data_config_root_b
--rw-r--r--   0        0        0       42 2023-03-14 16:49:21.407618 gluetool-2.4/gluetool/tests/assets/parse_config/configroot/config/data_not_unicode
--rw-r--r--   0        0        0      346 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/assets/parse_config/configroota/config/data_config_root_a
--rw-r--r--   0        0        0      321 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/assets/parse_config/configrootb/config/data_config_root_b
--rw-r--r--   0        0        0     1134 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/conftest.py
--rw-r--r--   0        0        0     5550 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_core.py
--rw-r--r--   0        0        0     4395 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_error.py
--rw-r--r--   0        0        0      930 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_eval_context.py
--rw-r--r--   0        0        0     1280 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_help.py
--rw-r--r--   0        0        0     1996 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_json.py
--rw-r--r--   0        0        0     3303 2023-04-21 12:14:52.374302 gluetool-2.4/gluetool/tests/test_load_yaml.py
--rw-r--r--   0        0        0     2342 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_log_exception.py
--rw-r--r--   0        0        0     1288 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_logging.py
--rw-r--r--   0        0        0     4470 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_module_discovery.py
--rw-r--r--   0        0        0      573 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_new_xml_element.py
--rw-r--r--   0        0        0     3296 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_normalize_option.py
--rw-r--r--   0        0        0     1132 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_option.py
--rw-r--r--   0        0        0     4021 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_parse_config.py
--rw-r--r--   0        0        0     1791 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_pipeline_step.py
--rw-r--r--   0        0        0      734 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_render_template.py
--rw-r--r--   0        0        0      665 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_requests.py
--rw-r--r--   0        0        0     2637 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_result.py
--rw-r--r--   0        0        0     8672 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_run_command.py
--rw-r--r--   0        0        0     8165 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_run_modules.py
--rw-r--r--   0        0        0     2517 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_tool.py
--rw-r--r--   0        0        0      754 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_treat_url.py
--rw-r--r--   0        0        0     2813 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_utils.py
--rw-r--r--   0        0        0     1987 2023-03-14 16:49:21.408618 gluetool-2.4/gluetool/tests/test_wait.py
--rw-r--r--   0        0        0    16475 2023-04-21 12:14:52.375302 gluetool-2.4/gluetool/tool.py
--rw-r--r--   0        0        0    58058 2023-04-21 12:14:52.375302 gluetool-2.4/gluetool/utils.py
--rw-r--r--   0        0        0      165 2023-03-14 16:49:21.409618 gluetool-2.4/gluetool/version.py
--rw-r--r--   0        0        0        0 2023-03-14 16:49:21.409618 gluetool-2.4/gluetool_modules/__init__.py
--rw-r--r--   0        0        0     4062 2023-03-14 16:49:21.409618 gluetool-2.4/gluetool_modules/bash_completion.py
--rw-r--r--   0        0        0    10863 2023-03-14 16:49:21.409618 gluetool-2.4/gluetool_modules/dep_list.py
--rw-r--r--   0        0        0     7490 2023-03-14 16:49:21.409618 gluetool-2.4/gluetool_modules/yaml_pipeline.py
--rw-r--r--   0        0        0     3412 2023-04-21 13:01:42.155351 gluetool-2.4/pyproject.toml
--rw-r--r--   0        0        0     2823 2023-04-21 13:02:05.329002 gluetool-2.4/setup.py
--rw-r--r--   0        0        0     2775 2023-04-21 13:02:05.329256 gluetool-2.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-14 16:49:21.402618 gluetool-2.5/README.rst
+-rw-r--r--   0        0        0     4522 2023-03-14 16:49:21.402618 gluetool-2.5/assets/html-log/prism.css
+-rw-r--r--   0        0        0    13651 2023-03-14 16:49:21.402618 gluetool-2.5/assets/html-log/prism.js
+-rw-r--r--   0        0        0   628536 2023-03-14 16:49:21.404618 gluetool-2.5/assets/html-log/semantic.min.css
+-rw-r--r--   0        0        0   275730 2023-03-14 16:49:21.405618 gluetool-2.5/assets/html-log/semantic.min.js
+-rw-r--r--   0        0        0      351 2023-03-14 16:49:21.406618 gluetool-2.5/gluetool/__init__.py
+-rw-r--r--   0        0        0    12916 2023-03-14 16:49:21.406618 gluetool-2.5/gluetool/action.py
+-rw-r--r--   0        0        0     2167 2023-03-14 16:49:21.406618 gluetool-2.5/gluetool/color.py
+-rw-r--r--   0        0        0      765 2023-03-14 16:49:21.406618 gluetool-2.5/gluetool/core.moduleinfo
+-rw-r--r--   0        0        0    97437 2023-03-14 16:49:21.407618 gluetool-2.5/gluetool/glue.py
+-rw-r--r--   0        0        0    19758 2023-03-14 16:49:21.407618 gluetool-2.5/gluetool/help.py
+-rw-r--r--   0        0        0    14613 2023-03-14 16:49:21.407618 gluetool-2.5/gluetool/html_log.py
+-rw-r--r--   0        0        0    47722 2023-03-14 16:49:21.407618 gluetool-2.5/gluetool/log.py
+-rw-r--r--   0        0        0     3752 2023-03-14 16:49:21.407618 gluetool-2.5/gluetool/proxy.py
+-rw-r--r--   0        0        0        0 2023-03-14 16:49:21.407618 gluetool-2.5/gluetool/py.typed
+-rw-r--r--   0        0        0     4254 2023-03-14 16:49:21.407618 gluetool-2.5/gluetool/pylint/__init__.py
+-rw-r--r--   0        0        0     5248 2023-03-14 16:49:21.407618 gluetool-2.5/gluetool/pylint/option_default.py
+-rw-r--r--   0        0        0     4698 2023-03-14 16:49:21.407618 gluetool-2.5/gluetool/pylint/shared_defined.py
+-rw-r--r--   0        0        0     3221 2023-03-14 16:49:21.407618 gluetool-2.5/gluetool/pylint/unknown_option.py
+-rw-r--r--   0        0        0     6265 2023-03-14 16:49:21.407618 gluetool-2.5/gluetool/result.py
+-rw-r--r--   0        0        0     9411 2023-03-14 16:49:21.407618 gluetool-2.5/gluetool/sentry.py
+-rw-r--r--   0        0        0     2620 2023-03-14 16:49:21.407618 gluetool-2.5/gluetool/tests/__init__.py
+-rw-r--r--   0        0        0      311 2023-03-14 16:49:21.407618 gluetool-2.5/gluetool/tests/assets/parse_config/configroot/config/data_config_root_a
+-rw-r--r--   0        0        0      321 2023-03-14 16:49:21.407618 gluetool-2.5/gluetool/tests/assets/parse_config/configroot/config/data_config_root_b
+-rw-r--r--   0        0        0       42 2023-03-14 16:49:21.407618 gluetool-2.5/gluetool/tests/assets/parse_config/configroot/config/data_not_unicode
+-rw-r--r--   0        0        0      346 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/assets/parse_config/configroota/config/data_config_root_a
+-rw-r--r--   0        0        0      321 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/assets/parse_config/configrootb/config/data_config_root_b
+-rw-r--r--   0        0        0     1134 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/conftest.py
+-rw-r--r--   0        0        0     5550 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/test_core.py
+-rw-r--r--   0        0        0     4395 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/test_error.py
+-rw-r--r--   0        0        0      930 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/test_eval_context.py
+-rw-r--r--   0        0        0     1280 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/test_help.py
+-rw-r--r--   0        0        0     1996 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/test_json.py
+-rw-r--r--   0        0        0     3303 2023-04-21 12:14:52.374302 gluetool-2.5/gluetool/tests/test_load_yaml.py
+-rw-r--r--   0        0        0     2342 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/test_log_exception.py
+-rw-r--r--   0        0        0     1288 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/test_logging.py
+-rw-r--r--   0        0        0     4470 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/test_module_discovery.py
+-rw-r--r--   0        0        0      573 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/test_new_xml_element.py
+-rw-r--r--   0        0        0     3296 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/test_normalize_option.py
+-rw-r--r--   0        0        0     1132 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/test_option.py
+-rw-r--r--   0        0        0     4021 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/test_parse_config.py
+-rw-r--r--   0        0        0     1791 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/test_pipeline_step.py
+-rw-r--r--   0        0        0      734 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/test_render_template.py
+-rw-r--r--   0        0        0      665 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/test_requests.py
+-rw-r--r--   0        0        0     2637 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/test_result.py
+-rw-r--r--   0        0        0     8672 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/test_run_command.py
+-rw-r--r--   0        0        0     8165 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/test_run_modules.py
+-rw-r--r--   0        0        0     3150 2023-04-27 11:08:47.032233 gluetool-2.5/gluetool/tests/test_tool.py
+-rw-r--r--   0        0        0      754 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/test_treat_url.py
+-rw-r--r--   0        0        0     2813 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/test_utils.py
+-rw-r--r--   0        0        0     1987 2023-03-14 16:49:21.408618 gluetool-2.5/gluetool/tests/test_wait.py
+-rw-r--r--   0        0        0    17149 2023-04-28 11:04:22.742148 gluetool-2.5/gluetool/tool.py
+-rw-r--r--   0        0        0    58058 2023-04-21 12:14:52.375302 gluetool-2.5/gluetool/utils.py
+-rw-r--r--   0        0        0      165 2023-03-14 16:49:21.409618 gluetool-2.5/gluetool/version.py
+-rw-r--r--   0        0        0        0 2023-03-14 16:49:21.409618 gluetool-2.5/gluetool_modules/__init__.py
+-rw-r--r--   0        0        0     4062 2023-03-14 16:49:21.409618 gluetool-2.5/gluetool_modules/bash_completion.py
+-rw-r--r--   0        0        0    10863 2023-03-14 16:49:21.409618 gluetool-2.5/gluetool_modules/dep_list.py
+-rw-r--r--   0        0        0     7490 2023-03-14 16:49:21.409618 gluetool-2.5/gluetool_modules/yaml_pipeline.py
+-rw-r--r--   0        0        0     3454 2023-04-28 11:15:40.673160 gluetool-2.5/pyproject.toml
+-rw-r--r--   0        0        0     2848 2023-04-28 11:59:38.767023 gluetool-2.5/setup.py
+-rw-r--r--   0        0        0     2814 2023-04-28 11:59:38.767290 gluetool-2.5/PKG-INFO
```

### Comparing `gluetool-2.4/README.rst` & `gluetool-2.5/README.rst`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/assets/html-log/prism.css` & `gluetool-2.5/assets/html-log/prism.css`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/assets/html-log/prism.js` & `gluetool-2.5/assets/html-log/prism.js`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/assets/html-log/semantic.min.css` & `gluetool-2.5/assets/html-log/semantic.min.css`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/assets/html-log/semantic.min.js` & `gluetool-2.5/assets/html-log/semantic.min.js`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/action.py` & `gluetool-2.5/gluetool/action.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/color.py` & `gluetool-2.5/gluetool/color.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/core.moduleinfo` & `gluetool-2.5/gluetool/core.moduleinfo`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/glue.py` & `gluetool-2.5/gluetool/glue.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/help.py` & `gluetool-2.5/gluetool/help.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/html_log.py` & `gluetool-2.5/gluetool/html_log.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/log.py` & `gluetool-2.5/gluetool/log.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/proxy.py` & `gluetool-2.5/gluetool/proxy.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/pylint/__init__.py` & `gluetool-2.5/gluetool/pylint/__init__.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/pylint/option_default.py` & `gluetool-2.5/gluetool/pylint/option_default.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/pylint/shared_defined.py` & `gluetool-2.5/gluetool/pylint/shared_defined.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/pylint/unknown_option.py` & `gluetool-2.5/gluetool/pylint/unknown_option.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/result.py` & `gluetool-2.5/gluetool/result.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/sentry.py` & `gluetool-2.5/gluetool/sentry.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/__init__.py` & `gluetool-2.5/gluetool/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/conftest.py` & `gluetool-2.5/gluetool/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/test_core.py` & `gluetool-2.5/gluetool/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/test_error.py` & `gluetool-2.5/gluetool/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/test_eval_context.py` & `gluetool-2.5/gluetool/tests/test_eval_context.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/test_help.py` & `gluetool-2.5/gluetool/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/test_json.py` & `gluetool-2.5/gluetool/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/test_load_yaml.py` & `gluetool-2.5/gluetool/tests/test_load_yaml.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/test_log_exception.py` & `gluetool-2.5/gluetool/tests/test_log_exception.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/test_logging.py` & `gluetool-2.5/gluetool/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/test_module_discovery.py` & `gluetool-2.5/gluetool/tests/test_module_discovery.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/test_new_xml_element.py` & `gluetool-2.5/gluetool/tests/test_new_xml_element.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/test_normalize_option.py` & `gluetool-2.5/gluetool/tests/test_normalize_option.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/test_option.py` & `gluetool-2.5/gluetool/tests/test_option.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/test_parse_config.py` & `gluetool-2.5/gluetool/tests/test_parse_config.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/test_pipeline_step.py` & `gluetool-2.5/gluetool/tests/test_pipeline_step.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/test_render_template.py` & `gluetool-2.5/gluetool/tests/test_render_template.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/test_requests.py` & `gluetool-2.5/gluetool/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/test_result.py` & `gluetool-2.5/gluetool/tests/test_result.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/test_run_command.py` & `gluetool-2.5/gluetool/tests/test_run_command.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/test_run_modules.py` & `gluetool-2.5/gluetool/tests/test_run_modules.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/test_tool.py` & `gluetool-2.5/gluetool/tests/test_tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 # pylint: disable=blacklisted-name
 
 import logging
 import os
 import signal
+import subprocess
 
 import pkg_resources
 import pytest
 from mock import MagicMock
 
 import gluetool
 import gluetool.tool
@@ -35,15 +36,17 @@
 
 def test_init_environ(monkeypatch):
     os.environ['GLUETOOL_CONFIG_PATHS'] = 'path1,path2,path3'
 
     monkeypatch.setattr(gluetool.glue, 'Glue', NonLoadingGlue)
 
     tool = gluetool.tool.Gluetool()
-    tool.gluetool_config_paths == ['path1', 'path2', 'path3']
+    assert tool.gluetool_config_paths == [
+        os.path.join(os.getcwd(), path) for path in ('path1', 'path2', 'path3')
+    ]
 
 
 @pytest.mark.parametrize(
     'tested_signal,exception,excmsg,warnmsg',
     [
         (signal.SIGINT, KeyboardInterrupt, '', 'Interrupted by SIGINT (Ctrl+C?)'),
         (signal.SIGTERM, KeyboardInterrupt, '', 'Interrupted by SIGTERM'),
@@ -73,19 +76,30 @@
     orig_signal_handler = signal.getsignal(tested_signal)
 
     with pytest.raises(SystemExit, match='^0$'):
         tool.setup()
 
     signal_handler = signal.getsignal(tested_signal)
 
+    # run a background process which ignores SIGTERM to test the SIGUSR1 handling
+    gluetool.tool.DEFAULT_SIGTERM_TIMEOUT = 0
+
+    process = subprocess.Popen(
+        ['sleep', '30'],
+        preexec_fn=lambda: signal.signal(signal.SIGTERM, signal.SIG_IGN),
+        stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
+    )
+
     with pytest.raises(exception, match=excmsg):
         signal_handler(tested_signal, MagicMock)
 
     assert tool.Glue.pipeline_cancelled is True
 
-    assert log.records[-1].message == warnmsg
-    assert log.records[-2].message == 'Exiting with status 0'
-    assert log.records[-3].message == 'gluetool some-version'
+    assert log.records[-1].message == "Sending SIGKILL to child process 'sleep' (PID {})".format(process.pid)
+    assert log.records[-2].message == "Sending SIGTERM to child process 'sleep' (PID {})".format(process.pid)
+    assert log.records[-3].message == warnmsg
+    assert log.records[-4].message == 'Exiting with status 0'
+    assert log.records[-5].message == 'gluetool some-version'
 
     # restore original signal handler, so we start correctly
     # for the next test
     signal.signal(tested_signal, orig_signal_handler)
```

### Comparing `gluetool-2.4/gluetool/tests/test_treat_url.py` & `gluetool-2.5/gluetool/tests/test_treat_url.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/test_utils.py` & `gluetool-2.5/gluetool/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tests/test_wait.py` & `gluetool-2.5/gluetool/tests/test_wait.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool/tool.py` & `gluetool-2.5/gluetool/tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import re
 import signal
 import sys
 import traceback
 
 from six import ensure_str, iteritems, iterkeys
 
+import psutil
 import tabulate
 
 import gluetool
 import gluetool.action
 import gluetool.sentry
 
 from .glue import GlueError, GlueRetryError, Failure, PipelineStepModule
@@ -39,14 +40,16 @@
     '/etc/gluetool.d/gluetool',
     normalize_path('~/.gluetool.d/gluetool'),
     normalize_path('./.gluetool.d/gluetool')
 ]
 
 DEFAULT_HANDLED_SIGNALS = (signal.SIGUSR2,)
 
+DEFAULT_SIGTERM_TIMEOUT = 60
+
 
 def handle_exc(func: Callable[..., Any]) -> Callable[..., Any]:
 
     @functools.wraps(func)
     def wrapped(self: 'Gluetool', *args: Any, **kwargs: Any) -> Any:
 
         # pylint: disable=broad-except, protected-access
@@ -290,31 +293,47 @@
 
         # Python installs SIGINT handler that translates signal to
         # a KeyboardInterrupt exception. It's so good we want to use
         # it for SIGTERM as well, just wrap the handler with some logging.
         orig_sigint_handler = signal.getsignal(signal.SIGINT)
         sigmap = {getattr(signal, name): name for name in [name for name in dir(signal) if name.startswith('SIG')]}
 
+        def _terminate_or_kill(child: psutil.Process) -> None:
+            Glue.warn("Sending SIGTERM to child process '{}' (PID {})".format(child.name(), child.pid))
+            child.terminate()
+
+            try:
+                child.wait(timeout=DEFAULT_SIGTERM_TIMEOUT)
+
+            except psutil.TimeoutExpired:
+                Glue.warn("Sending SIGKILL to child process '{}' (PID {})".format(child.name(), child.pid))
+                child.kill()
+
+        def _terminate_children() -> None:
+            for child in psutil.Process().children():
+                _terminate_or_kill(child)
+
         def _signal_handler(signum: int,
                             frame: Optional[FrameType],
                             handler: Optional[Callable[[int, FrameType], None]] = None,
                             msg: Optional[str] = None) -> Any:
 
             msg = msg or 'Signal {} received'.format(sigmap[signum])
 
             Glue.warn(msg)
 
             # Provide a flag for modules to check if they should try to finish as early as possible
             Glue.pipeline_cancelled = True
 
+            _terminate_children()
+
             if handler is not None and frame is not None:
                 return handler(signum, frame)
 
         def _sigusr1_handler(signum: int, frame: FrameType) -> None:
-
             # pylint: disable=unused-argument
 
             raise GlueError('Pipeline timeout expired.')
 
         sigint_handler = functools.partial(_signal_handler,
                                            handler=orig_sigint_handler, msg='Interrupted by SIGINT (Ctrl+C?)')
         sigterm_handler = functools.partial(_signal_handler,
```

### Comparing `gluetool-2.4/gluetool/utils.py` & `gluetool-2.5/gluetool/utils.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool_modules/bash_completion.py` & `gluetool-2.5/gluetool_modules/bash_completion.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool_modules/dep_list.py` & `gluetool-2.5/gluetool_modules/dep_list.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/gluetool_modules/yaml_pipeline.py` & `gluetool-2.5/gluetool_modules/yaml_pipeline.py`

 * *Files identical despite different names*

### Comparing `gluetool-2.4/pyproject.toml` & `gluetool-2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gluetool"
-version = "2.4"
+version = "2.5"
 description = "Python framework for constructing command-line pipelines."
 authors = [
   "Milos Prchlik <mprchlik@redhat.com>",
   "Miroslav Vadkerti <mvadkert@redhat.com>",
   "Martin Kluson <mkluson@redhat.com>",
   "Ondrej Ptak <optak@redhat.com>",
   "Evgeny Fedin <efedin@redhat.com>",
@@ -67,14 +67,15 @@
 # depending on extended argument annotations.
 mypy-extensions = "*"
 zipp = "*"
 packaging = "*"
 MarkupSafe = "^2.0.0"
 attrs = "^22.2.0"
 cattrs = "^22.2.0"
+psutil = "^5.9.5"
 
 [tool.poetry.dev-dependencies]
 # flake8 5 introduced a bug https://github.com/tholo/pytest-flake8/issues/87
 flake8 = "<5.0.0"
 lazy-object_proxy = "*"
 hypothesis = "*"
 importlib-metadata = "*"
@@ -90,14 +91,15 @@
 types-mock = "*"
 types-requests = "*"
 
 # Using asterisk instead of specifying pytest-lint versions for each suported Python version seems to do the trick:
 # we limit the list of possible Pylint versions, and we limit the list of possible Pytest versions, and asterisk
 # apparently gives Poetry the enough space to find pytest-pylint to match both ends.
 pytest-pylint = "*"
+types-psutil = "^5.9.5"
 
 [tool.poetry.scripts]
 gluetool = "gluetool.tool:main"
 gluetool-html-log = "gluetool.html_log:main"
 
 [tool.poetry.plugins]
```

### Comparing `gluetool-2.4/setup.py` & `gluetool-2.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
  'colorama',
  'configparser',
  'docutils',
  'lxml',
  'mock',
  'mypy-extensions',
  'packaging',
+ 'psutil>=5.9.5,<6.0.0',
  'raven',
  'requests',
  'requests-toolbelt',
  'ruamel.yaml>=0.16.12,<0.17.0',
  'six',
  'tabulate',
  'urlnormalizer',
@@ -40,15 +41,15 @@
                       'gluetool_modules.bash_completion:BashCompletion',
                       '.dep_list = gluetool_modules.dep_list:DepList',
                       '.yaml_pipeline = '
                       'gluetool_modules.yaml_pipeline:YAMLPipeline']}
 
 setup_kwargs = {
     'name': 'gluetool',
-    'version': '2.4',
+    'version': '2.5',
     'description': 'Python framework for constructing command-line pipelines.',
     'long_description': 'gluetool - A tool for gluing together one-file python modules in a sequential command-line pipeline\n---------------------------------------------------------------------------------------------------\n\n``gluetool`` is a command line centric generic framework useable for glueing modules into pipeline\n\n\n.. image:: https://travis-ci.org/gluetool/gluetool.svg?branch=master\n    :target: https://travis-ci.org/gluetool/gluetool\n\n.. image:: https://codecov.io/gh/gluetool/gluetool/branch/master/graph/badge.svg\n     :target: https://codecov.io/gh/gluetool/gluetool\n     :alt: Code coverage\n\n.. image:: https://requires.io/github/gluetool/gluetool/requirements.svg?branch=master\n     :target: https://requires.io/github/gluetool/gluetool/requirements/?branch=master\n     :alt: Requirements Status\n\n.. image:: https://readthedocs.org/projects/gluetool/badge/?version=latest\n     :target: http://gluetool.readthedocs.io/en/latest/?badge=latest\n     :alt: Documentation Status\n\n\nDocumentation\n-------------\n\nFor more information see documentation:\n\nhttp://gluetool.readthedocs.io/\n',
     'author': 'Milos Prchlik',
     'author_email': 'mprchlik@redhat.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gluetool.readthedocs.org/',
```

### Comparing `gluetool-2.4/PKG-INFO` & `gluetool-2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gluetool
-Version: 2.4
+Version: 2.5
 Summary: Python framework for constructing command-line pipelines.
 Home-page: https://gluetool.readthedocs.org/
 License: BSD
 Author: Milos Prchlik
 Author-email: mprchlik@redhat.com
 Requires-Python: >=3.7.2,<3.10
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,14 +30,15 @@
 Requires-Dist: colorama
 Requires-Dist: configparser
 Requires-Dist: docutils
 Requires-Dist: lxml
 Requires-Dist: mock
 Requires-Dist: mypy-extensions
 Requires-Dist: packaging
+Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: raven
 Requires-Dist: requests
 Requires-Dist: requests-toolbelt
 Requires-Dist: ruamel.yaml (>=0.16.12,<0.17.0)
 Requires-Dist: six
 Requires-Dist: tabulate
 Requires-Dist: urlnormalizer
```

