# Comparing `tmp/db_contrib_tool-0.6.1.tar.gz` & `tmp/db_contrib_tool-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db_contrib_tool-0.6.1.tar", max compression
+gzip compressed data, was "db_contrib_tool-0.6.2.tar", max compression
```

## Comparing `db_contrib_tool-0.6.1.tar` & `db_contrib_tool-0.6.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     5222 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/README.md
--rw-r--r--   0        0        0     2139 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/pyproject.toml
--rw-r--r--   0        0        0       13 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/__init__.py
--rw-r--r--   0        0        0      883 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/cli.py
--rw-r--r--   0        0        0        0 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/clients/__init__.py
--rw-r--r--   0        0        0     7147 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/clients/download_client.py
--rw-r--r--   0        0        0     1329 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/clients/file_service.py
--rw-r--r--   0        0        0     2636 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/clients/git_client.py
--rw-r--r--   0        0        0      305 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/clients/io_client.py
--rw-r--r--   0        0        0      984 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/clients/platform_details.py
--rw-r--r--   0        0        0     2524 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/clients/resmoke_proxy.py
--rw-r--r--   0        0        0     6667 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/config/setup_repro_env_config.yml
--rw-r--r--   0        0        0     5999 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/config.py
--rw-r--r--   0        0        0     8844 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/evg_aware_bisect/__init__.py
--rw-r--r--   0        0        0     4639 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/evg_aware_bisect/cli.py
--rw-r--r--   0        0        0      110 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/evg_aware_bisect/run_user_script.sh
--rw-r--r--   0        0        0      418 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/evg_aware_bisect/setup_test_env.sh
--rw-r--r--   0        0        0       52 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/evg_aware_bisect/teardown_test_env.sh
--rw-r--r--   0        0        0        0 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/services/__init__.py
--rw-r--r--   0        0        0     9131 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/services/evergreen_service.py
--rw-r--r--   0        0        0     2404 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/services/git_service.py
--rw-r--r--   0        0        0     2027 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/services/platform_service.py
--rw-r--r--   0        0        0    13919 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/README.md
--rw-r--r--   0        0        0       13 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/__init__.py
--rw-r--r--   0        0        0    17392 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py
--rw-r--r--   0        0        0     8912 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/cli.py
--rw-r--r--   0        0        0     8290 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/download_service.py
--rw-r--r--   0        0        0     4513 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/release_discovery_service.py
--rw-r--r--   0        0        0     5586 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/release_models.py
--rw-r--r--   0        0        0     3155 2023-04-21 14:16:26.506060 db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/request_models.py
--rw-r--r--   0        0        0    11018 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/setup_repro_env.py
--rw-r--r--   0        0        0      614 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/symbolizer/README.md
--rw-r--r--   0        0        0        0 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/symbolizer/__init__.py
--rw-r--r--   0        0        0     4190 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/symbolizer/cli.py
--rw-r--r--   0        0        0     4798 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py
--rw-r--r--   0        0        0    26368 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/symbolizer/mongosymb.py
--rw-r--r--   0        0        0     2269 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/usage_analytics.py
--rw-r--r--   0        0        0      235 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/utils/__init__.py
--rw-r--r--   0        0        0     1855 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/utils/build_system_options.py
--rw-r--r--   0        0        0     2160 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/utils/evergreen_conn.py
--rw-r--r--   0        0        0     1085 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/utils/filesystem.py
--rw-r--r--   0        0        0    10608 2023-04-21 14:16:26.510060 db_contrib_tool-0.6.1/src/db_contrib_tool/utils/oauth.py
--rw-r--r--   0        0        0     6795 1970-01-01 00:00:00.000000 db_contrib_tool-0.6.1/setup.py
--rw-r--r--   0        0        0     6436 1970-01-01 00:00:00.000000 db_contrib_tool-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     5222 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/README.md
+-rw-r--r--   0        0        0     2139 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/__init__.py
+-rw-r--r--   0        0        0      883 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/cli.py
+-rw-r--r--   0        0        0        0 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/clients/__init__.py
+-rw-r--r--   0        0        0     7147 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/clients/download_client.py
+-rw-r--r--   0        0        0     1329 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/clients/file_service.py
+-rw-r--r--   0        0        0     2636 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/clients/git_client.py
+-rw-r--r--   0        0        0      305 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/clients/io_client.py
+-rw-r--r--   0        0        0      984 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/clients/platform_details.py
+-rw-r--r--   0        0        0     2524 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/clients/resmoke_proxy.py
+-rw-r--r--   0        0        0     6667 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/config/setup_repro_env_config.yml
+-rw-r--r--   0        0        0     5999 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/config.py
+-rw-r--r--   0        0        0     8844 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/evg_aware_bisect/__init__.py
+-rw-r--r--   0        0        0     4639 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/evg_aware_bisect/cli.py
+-rw-r--r--   0        0        0      110 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/evg_aware_bisect/run_user_script.sh
+-rw-r--r--   0        0        0      418 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/evg_aware_bisect/setup_test_env.sh
+-rw-r--r--   0        0        0       52 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/evg_aware_bisect/teardown_test_env.sh
+-rw-r--r--   0        0        0        0 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/services/__init__.py
+-rw-r--r--   0        0        0     9131 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/services/evergreen_service.py
+-rw-r--r--   0        0        0     2404 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/services/git_service.py
+-rw-r--r--   0        0        0     2027 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/services/platform_service.py
+-rw-r--r--   0        0        0    13919 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/README.md
+-rw-r--r--   0        0        0       13 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/__init__.py
+-rw-r--r--   0        0        0    17392 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py
+-rw-r--r--   0        0        0     8912 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/cli.py
+-rw-r--r--   0        0        0     8290 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/download_service.py
+-rw-r--r--   0        0        0     4513 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/release_discovery_service.py
+-rw-r--r--   0        0        0     5586 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/release_models.py
+-rw-r--r--   0        0        0     3155 2023-04-28 09:19:45.146205 db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/request_models.py
+-rw-r--r--   0        0        0    11018 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/setup_repro_env.py
+-rw-r--r--   0        0        0      614 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/symbolizer/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/symbolizer/__init__.py
+-rw-r--r--   0        0        0     4190 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/symbolizer/cli.py
+-rw-r--r--   0        0        0     4798 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py
+-rw-r--r--   0        0        0    24229 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/symbolizer/mongosymb.py
+-rw-r--r--   0        0        0     2269 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/usage_analytics.py
+-rw-r--r--   0        0        0      235 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/utils/__init__.py
+-rw-r--r--   0        0        0     1855 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/utils/build_system_options.py
+-rw-r--r--   0        0        0     2160 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/utils/evergreen_conn.py
+-rw-r--r--   0        0        0     1085 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/utils/filesystem.py
+-rw-r--r--   0        0        0    10608 2023-04-28 09:19:45.150205 db_contrib_tool-0.6.2/src/db_contrib_tool/utils/oauth.py
+-rw-r--r--   0        0        0     6795 1970-01-01 00:00:00.000000 db_contrib_tool-0.6.2/setup.py
+-rw-r--r--   0        0        0     6436 1970-01-01 00:00:00.000000 db_contrib_tool-0.6.2/PKG-INFO
```

### Comparing `db_contrib_tool-0.6.1/README.md` & `db_contrib_tool-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/pyproject.toml` & `db_contrib_tool-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "db-contrib-tool"
-version = "0.6.1"
+version = "0.6.2"
 description = "The `db-contrib-tool` - MongoDB's tool for contributors."
 authors = ["DAG team <dev-prod-dag@mongodb.com>"]
 readme = "README.md"
 repository = "https://github.com/10gen/db-contrib-tool"
 include = [
     "src/db_contrib_tool/bisect/*.sh",
     "src/db_contrib_tool/config/*.yml",
```

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/cli.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/clients/download_client.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/clients/download_client.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/clients/file_service.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/clients/file_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/clients/git_client.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/clients/git_client.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/clients/platform_details.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/clients/platform_details.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/clients/resmoke_proxy.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/clients/resmoke_proxy.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/config/setup_repro_env_config.yml` & `db_contrib_tool-0.6.2/src/db_contrib_tool/config/setup_repro_env_config.yml`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/config.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/config.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/evg_aware_bisect/__init__.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/evg_aware_bisect/__init__.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/evg_aware_bisect/cli.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/evg_aware_bisect/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/services/evergreen_service.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/services/evergreen_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/services/git_service.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/services/git_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/services/platform_service.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/services/platform_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/README.md` & `db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/README.md`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/cli.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/download_service.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/download_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/release_discovery_service.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/release_discovery_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/release_models.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/release_models.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/request_models.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/request_models.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/setup_repro_env/setup_repro_env.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/setup_repro_env/setup_repro_env.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/symbolizer/README.md` & `db_contrib_tool-0.6.2/src/db_contrib_tool/symbolizer/README.md`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/symbolizer/cli.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/symbolizer/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/symbolizer/mongosymb.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/symbolizer/mongosymb.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Script for symbolizing MongoDB stack traces."""
+from __future__ import annotations
 
 import json
 import os
 import signal
 import subprocess
 import sys
 import time
-from collections import OrderedDict
 from enum import Enum
 from typing import IO, Any, AnyStr, Dict, List, NamedTuple, Optional, TextIO, Tuple
 
 import inject
 import requests
 from tenacity import Retrying, retry_if_result, stop_after_delay, wait_fixed
 
@@ -29,69 +29,46 @@
     get_oauth_credentials,
 )
 
 SYMBOLIZER_PATH_ENV = "MONGOSYMB_SYMBOLIZER_PATH"
 DEFAULT_SYMBOLIZER_PATH = "/opt/mongodbtoolchain/v4/bin/llvm-symbolizer"
 
 
-class CachedResults(object):
-    """
-    Used to manage / store results in a cache form (using dict as an underlying data structure).
-
-    Idea is to allow only N items to be present in cache at a time and eliminate extra items on the go.
-    """
+class BuildData(NamedTuple):
+    """Model for data returned by symbolizer service."""
 
-    def __init__(self, max_cache_size: int, initial_cache: Optional[Dict[str, str]] = None):
-        """
-        Initialize instance.
+    url: Optional[str] = None
+    debug_symbols_url: Optional[str] = None
+    file_name: Optional[str] = None
 
-        :param max_cache_size: max number of items that can be added to cache
-        :param initial_cache: initial items as dict
+    @classmethod
+    def from_response_data(cls, data: Dict[str, Any]) -> BuildData:
         """
-        self._max_cache_size = max_cache_size
-        self._cached_results = OrderedDict(initial_cache or {})
+        Make build data from symbolizer service response data.
 
-    def insert(self, key: str, value: str) -> Optional[Dict[str, str]]:
+        :param data: Symbolizer service response data
+        :return: Build data.
         """
-        Insert new data into cache.
+        return cls(
+            url=data.get("url"),
+            debug_symbols_url=data.get("debug_symbols_url"),
+            file_name=data.get("file_name"),
+        )
 
-        :param key: Key string.
-        :param value: Value string.
-        :return: Inserted data as dict or None (if not possible to insert).
+    def is_san_build(self) -> bool:
         """
-        if self._max_cache_size <= 0:
-            # we can't insert into 0-length dict
-            return None
-
-        if len(self._cached_results) >= self._max_cache_size:
-            # remove items causing the size overflow of cache
-            # we use FIFO order when removing objects from cache,
-            # so that we delete olds and keep track of only the recent ones
-            keys_iterator = iter(self._cached_results.keys())
-            while len(self._cached_results) >= self._max_cache_size:
-                # pop the first (the oldest) item in dict
-                self._cached_results.pop(next(keys_iterator))
+        Check whether this is a sanitizer build.
 
-        if key not in self._cached_results:
-            # actual insert operation
-            self._cached_results[key] = value
+        Sanitizer build binary files has debug symbols, so
+        if URL to binaries and URL to debug symbols is the same,
+        this is a sanitizer build.
 
-        return dict(build_id=value)
-
-    def get(self, key: str) -> Optional[str]:
-        """
-        Try to get object by key.
-
-        :param key: Key string.
-        :return: Value for key.
+        :return: True if sanitizer build.
         """
-        if self._max_cache_size <= 0:
-            return None
-
-        return self._cached_results.get(key)
+        return self.url == self.debug_symbols_url
 
 
 class PathResolver(object):
     """
     Class to find path for given buildId.
 
     We'll be sending request each time to another server to get path.
@@ -108,41 +85,37 @@
     default_creds_file_path = os.path.join(os.getcwd(), ".symbolizer_credentials.json")
     default_client_credentials_scope = "servertig-symbolizer-fullaccess"
     default_client_credentials_user_name = "client-user"
 
     def __init__(
         self,
         host: Optional[str] = None,
-        cache_size: int = 0,
         cache_dir: Optional[str] = None,
         client_credentials_scope: Optional[str] = None,
         client_credentials_user_name: Optional[str] = None,
         client_id: Optional[str] = None,
         client_secret: Optional[str] = None,
         redirect_port: Optional[int] = None,
         scope: Optional[str] = None,
         auth_domain: Optional[str] = None,
     ):
         """
         Initialize instance.
 
         :param host: URL of web service running the API to get debug symbol URL.
-        :param cache_size: Size of cache. We try to cache recent results and use them instead of asking from server.
-            Use 0 (by default) to disable caching.
         :param cache_dir: Full path to a directory to store cache/files.
         :param client_credentials_scope: Client credentials scope.
         :param client_credentials_user_name: Client credentials username.
         :param client_id: Client id for Okta Oauth.
         :param client_secret: Secret key for Okta Oauth.
         :param redirect_port: Redirect port.
         :param scope: Auth scope.
         :param auth_domain: Auth domain.
         """
         self.host = host or self.default_host
-        self._cached_results = CachedResults(max_cache_size=cache_size)
         self.cache_dir = cache_dir or self.default_cache_dir
         self.client_credentials_scope = (
             client_credentials_scope or self.default_client_credentials_scope
         )
         self.client_credentials_user_name = (
             client_credentials_user_name or self.default_client_credentials_user_name
         )
@@ -210,33 +183,14 @@
         If we need to do extra checks on path, we'll do all of them here.
 
         :param path: Path string.
         :return: Bool indicating the validation status.
         """
         return os.path.exists(path)
 
-    def get_from_cache(self, key: str) -> Optional[str]:
-        """
-        Try to get value from cache.
-
-        :param key: Key string.
-        :return: Value or None (if doesn't exist).
-        """
-        return self._cached_results.get(key)
-
-    def add_to_cache(self, key: str, value: str) -> Optional[Dict[str, str]]:
-        """
-        Add new value to cache.
-
-        :param key: Key string.
-        :param value: Value string.
-        :return: Added data as dict.
-        """
-        return self._cached_results.insert(key, value)
-
     @staticmethod
     def url_to_filename(url: str) -> str:
         """
         Convert URL to local filename.
 
         :param url: Download URL.
         :return: Full name for local file.
@@ -287,63 +241,57 @@
         To get path for given buildId.
 
         :param soinfo: Information about process that printed backtrace.
         :return: Path as string or None (if path not found).
         """
         build_id = soinfo.build_id.lower() if soinfo.build_id is not None else ""
         version = soinfo.mongodb_version
-        binary_name = "mongo"
-        # search from cached results
-        path = self.get_from_cache(build_id)
-        if not path:
-            # path does not exist in cache, so we send request to server
-            try:
-                search_parameters = {"build_id": build_id}
-                if version:
-                    search_parameters["version"] = version
-                print(f"Getting data from service... Search parameters: {search_parameters}")
-                response = self.http_client.get(f"{self.host}/find_by_id", params=search_parameters)
-                if response.status_code != 200:
-                    sys.stderr.write(
-                        f"Server returned unsuccessful status: {response.status_code}, "
-                        f"response body: {response.text}\n"
-                    )
-                    return None
-                else:
-                    data = response.json().get("data", {})
-                    path, binary_name = data.get("debug_symbols_url"), data.get("file_name")
-            except Exception as err:  # noqa
+        try:
+            search_parameters = {"build_id": build_id}
+            if version:
+                search_parameters["version"] = version
+            print(f"Getting data from service... Search parameters: {search_parameters}")
+            response = self.http_client.get(f"{self.host}/find_by_id", params=search_parameters)
+            if response.status_code != 200:
                 sys.stderr.write(
-                    f"Error occurred while trying to get response from server "
-                    f"for buildId({build_id}): {err}\n"
+                    f"Server returned unsuccessful status: {response.status_code}, "
+                    f"response body: {response.text}\n"
                 )
                 return None
+            else:
+                data = response.json().get("data", {})
+                build_data = BuildData.from_response_data(data)
+        except Exception as err:  # noqa
+            sys.stderr.write(
+                f"Error occurred while trying to get response from server "
+                f"for buildId({build_id}): {err}\n"
+            )
+            return None
 
-            # update cached results
-            if path:
-                self.add_to_cache(build_id, path)
-
-        if not path:
+        if build_data.debug_symbols_url is None:
             return None
 
-        # download & unpack debug symbols file and assign `path` to unpacked file's local path
         try:
-            dl_path, exists_locally = self.download(path)
+            dl_path, exists_locally = self.download(build_data.debug_symbols_url)
             if exists_locally:
                 path = dl_path.replace(".tgz", "", 1)
             else:
                 sys.stdout.write("Downloaded, now unpacking...\n")
                 path = self.unpack(dl_path)
         except Exception as err:  # noqa
             sys.stderr.write(f"Failed to download & unpack file: {err}\n")
-        # we may have '<name>.debug', '<name>.so' or just executable binary file which may not have file 'extension'.
-        # if file has extension, it is good. if not, we should append .debug, because those without extension are
-        # from release builds, and their debug symbol files contain .debug extension.
-        # we need to map those 2 different file names ('<name>' becomes '<name>.debug').
-        if not binary_name.endswith(".debug"):
+            return None
+
+        binary_name = build_data.file_name or "mongo"
+        # Regular builds have separate file with debug symbols and for linux builds it has "<binary-name>.debug" name.
+        # Sanitizer builds have debug symbols in the same binary file.
+        # Symbolizer service returns us the name of the file the build id was extracted from.
+        # If it is a regular build and the binary file name is returned
+        # we need to append ".debug" to it to get the debug symbols file name.
+        if not build_data.is_san_build() and not binary_name.endswith(".debug"):
             binary_name = f"{binary_name}.debug"
 
         inner_folder_name = self.path_options.get_binary_folder_name(binary_name)
 
         return os.path.join(path, inner_folder_name, binary_name)
```

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/usage_analytics.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/usage_analytics.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/utils/build_system_options.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/utils/build_system_options.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/utils/evergreen_conn.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/utils/evergreen_conn.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/utils/filesystem.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/src/db_contrib_tool/utils/oauth.py` & `db_contrib_tool-0.6.2/src/db_contrib_tool/utils/oauth.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.1/setup.py` & `db_contrib_tool-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
  'tenacity>=8.0.1,<9.0.0']
 
 entry_points = \
 {'console_scripts': ['db-contrib-tool = db_contrib_tool.cli:cli']}
 
 setup_kwargs = {
     'name': 'db-contrib-tool',
-    'version': '0.6.1',
+    'version': '0.6.2',
     'description': "The `db-contrib-tool` - MongoDB's tool for contributors.",
     'long_description': '# db-contrib-tool\n\nThe `db-contrib-tool` - MongoDB\'s tools for contributors.\n\n## Table of contents\n\n- [db-contrib-tool](#db-contrib-tool)\n  - [Table of contents](#table-of-contents)\n  - [Description](#description)\n  - [Dependencies](#dependencies)\n  - [Installation](#installation)\n  - [Usage](#usage)\n  - [Contributor\'s Guide (local development)](#contributors-guide-local-development)\n    - [Install project dependencies](#install-project-dependencies)\n    - [Run command line tool (local development)](#run-command-line-tool-local-development)\n    - [Run linters](#run-linters)\n    - [Run tests](#run-tests)\n    - [Pre-commit](#pre-commit)\n    - [Testing changes in mongo](#testing-changes-in-mongo)\n    - [Test pipx package](#test-pipx-package)\n    - [Versioning](#versioning)\n    - [Code Review](#code-review)\n    - [Deployment](#deployment)\n\n## Description\n\nThe command line tool with various subcommands:\n- `bisect` - performs an evergreen-aware git-bisect to find the \'last passing version\' and \'first failing version\' of mongo\n- `setup-repro-env`\n  - [README.md](https://github.com/10gen/db-contrib-tool/blob/main/src/db_contrib_tool/setup_repro_env/README.md)\n  - downloads and installs:\n    - particular MongoDB versions\n    - debug symbols\n    - artifacts (including resmoke, python scripts etc)\n    - python venv for resmoke, python scripts etc\n- `symbolize`\n  - [README.md](https://github.com/10gen/db-contrib-tool/blob/main/src/db_contrib_tool/symbolizer/README.md)\n  - Symbolizes stacktraces from recent `mongod` and `mongos` binaries compiled in Evergreen, including patch builds, mainline builds, and release/production builds.\n  - Requires authenticating to an internal MongoDB symbol mapping service.\n\n## Dependencies\n\n- Python 3.9 or later (python3 from the [MongoDB Toolchain](https://github.com/10gen/toolchain-builder/blob/master/INSTALL.md) is highly recommended)\n\n## Installation\n\nMake sure [dependencies](#dependencies) are installed.\nUse [pipx](https://pypa.github.io/pipx/) to install db-contrib-tool that will be available globally on your machine:\n```bash\n$ python3 -m pip install pipx\n$ python3 -m pipx ensurepath\n```\n\nInstalling db-contrib-tool:\n```bash\n$ python3 -m pipx install db-contrib-tool\n```\n\nUpgrading db-contrib-tool:\n```bash\n$ python3 -m pipx upgrade db-contrib-tool\n```\n\n## Usage\n\nPrint out help message:\n```bash\n$ db-contrib-tool -h\n```\nMore information on the usage of `setup-repro-env` can be found [here](https://github.com/10gen/db-contrib-tool/blob/main/src/db_contrib_tool/setup_repro_env/README.md).\n\n## Contributor\'s Guide (local development)\n\n### Install project dependencies\n\nThis project uses [poetry](https://python-poetry.org/) for dependency management.\n```bash\n$ poetry install\n```\n\n### Run command line tool (local development)\n\n```bash\n$ ENV=DEV poetry run db-contrib-tool -h\n```\n\n### Run linters\n\n```bash\n$ poetry run isort src tests\n$ poetry run black src tests\n```\n\n### Run tests\n\n```bash\n$ poetry run pytest\n```\n\n### Pre-commit\n\nThis project has [pre-commit](https://pre-commit.com/) configured. Pre-commit will run\nconfigured checks at git commit time.<br>\nTo enable pre-commit on your local repository run:\n```bash\n$ poetry run pre-commit install\n```\n\nTo run pre-commit manually:\n```bash\n$ poetry run pre-commit run\n```\n\n### Testing changes in mongo\n\nThis tool is used to help run tests in the mongodb/mongo repository. On occasion, it may be\ndesirable to run a mongodb-mongo-* patch build with in-flight changes to this repository. The\nfollowing steps can be take to accomplish that.\n\n- Create a branch with the changes you wish to test.\n- Push the branch to the origin repository: `git push -u origin <branch_name>`.\n- In the "mongo" repository, edit the [evergreen/prelude_db_contrib_tool.sh](https://github.com/10gen/mongo/blob/b1a3a357af735a53981737d91fd49e5e3ae67b95/evergreen/prelude_db_contrib_tool.sh#L10)\n  to install from the git repository instead of from pypi:\n\n  ```bash\n  pipx install "git+ssh://git@github.com/<user_name>/db-contrib-tool.git@<branch_name>" || exit 1\n  ```\n\n- Create a patch build.\n\nThe patch build should now pull down the changes from your branch instead of using the published\ndb-contrib-tool.\n\n**Note**: Since the db-contrib-tool is pulled from your branch, if you need to make additional\nchanges to the tool, you can just push to the branch and then restart the desired tasks. There is\nno need to create an additional patch build unless you also need to make updates to the mongo\nrepository.\n\n### Test pipx package\n\nPipx installation recommendations can be found in [installation](#installation) section.<br>\nThe tool can be installed via pipx from your local repo:\n```bash\n$ python3 -m pipx install /path/to/db-contrib-tool\n```\n\n### Versioning\n\nThis project uses [semver](https://semver.org/) for versioning.\nPlease include a description what is added for each new version in `CHANGELOG.md`.\n\n### Code Review\n\nPlease open a Github Pull Request for code review.\nThis project uses the [Evergreen Commit Queue](https://github.com/evergreen-ci/evergreen/wiki/Commit-Queue#pr).\nAdd a PR comment with `evergreen merge` to trigger a merge.\n\n### Deployment\n\nDeployment to pypi is automatically triggered on merges to main.\n',
     'author': 'DAG team',
     'author_email': 'dev-prod-dag@mongodb.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/10gen/db-contrib-tool',
```

### Comparing `db_contrib_tool-0.6.1/PKG-INFO` & `db_contrib_tool-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db-contrib-tool
-Version: 0.6.1
+Version: 0.6.2
 Summary: The `db-contrib-tool` - MongoDB's tool for contributors.
 Home-page: https://github.com/10gen/db-contrib-tool
 Author: DAG team
 Author-email: dev-prod-dag@mongodb.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

