# Comparing `tmp/pywrapid-0.2.8.tar.gz` & `tmp/pywrapid-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywrapid-0.2.8.tar", last modified: Tue Apr 25 14:08:42 2023, max compression
+gzip compressed data, was "pywrapid-0.2.9.tar", last modified: Thu Apr 27 14:43:41 2023, max compression
```

## Comparing `pywrapid-0.2.8.tar` & `pywrapid-0.2.9.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.406487 pywrapid-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-25 14:08:31.000000 pywrapid-0.2.8/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.398487 pywrapid-0.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.402487 pywrapid-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-25 14:08:31.000000 pywrapid-0.2.8/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-25 14:08:31.000000 pywrapid-0.2.8/.github/workflows/dependency-review.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-25 14:08:31.000000 pywrapid-0.2.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-25 14:08:31.000000 pywrapid-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-25 14:08:31.000000 pywrapid-0.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-25 14:08:31.000000 pywrapid-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-04-25 14:08:42.406487 pywrapid-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-25 14:08:31.000000 pywrapid-0.2.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.398487 pywrapid-0.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.402487 pywrapid-0.2.8/docs/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-25 14:08:31.000000 pywrapid-0.2.8/docs/src/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-25 14:08:31.000000 pywrapid-0.2.8/docs/src/developer-guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.402487 pywrapid-0.2.8/docs/src/features/
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-25 14:08:31.000000 pywrapid-0.2.8/docs/src/features/config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-04-25 14:08:31.000000 pywrapid-0.2.8/docs/src/features/log.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-25 14:08:31.000000 pywrapid-0.2.8/docs/src/features/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-25 14:08:31.000000 pywrapid-0.2.8/docs/src/features/webclient.rst
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-25 14:08:31.000000 pywrapid-0.2.8/docs/src/features.rst
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-25 14:08:31.000000 pywrapid-0.2.8/docs/src/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-25 14:08:31.000000 pywrapid-0.2.8/docs/src/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-25 14:08:31.000000 pywrapid-0.2.8/docs/src/user-guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-25 14:08:31.000000 pywrapid-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 14:08:31.000000 pywrapid-0.2.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 14:08:31.000000 pywrapid-0.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:08:42.406487 pywrapid-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.398487 pywrapid-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.402487 pywrapid-0.2.8/src/pywrapid/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.402487 pywrapid-0.2.8/src/pywrapid/config/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10150 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/config/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/config/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.402487 pywrapid-0.2.8/src/pywrapid/log/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/log/application_log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.402487 pywrapid-0.2.8/src/pywrapid/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/utils/dict_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/utils/file_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.402487 pywrapid-0.2.8/src/pywrapid/webclient/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/webclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/webclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/webclient/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-04-25 14:08:31.000000 pywrapid-0.2.8/src/pywrapid/webclient/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.402487 pywrapid-0.2.8/src/pywrapid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-04-25 14:08:42.000000 pywrapid-0.2.8/src/pywrapid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-25 14:08:42.000000 pywrapid-0.2.8/src/pywrapid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:08:42.000000 pywrapid-0.2.8/src/pywrapid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-25 14:08:42.000000 pywrapid-0.2.8/src/pywrapid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 14:08:42.000000 pywrapid-0.2.8/src/pywrapid.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:42.402487 pywrapid-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-25 14:08:31.000000 pywrapid-0.2.8/tests/test_conf_ok.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-25 14:08:31.000000 pywrapid-0.2.8/tests/test_pywrapid_config_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-04-25 14:08:31.000000 pywrapid-0.2.8/tests/test_pywrapid_logging_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-04-25 14:08:31.000000 pywrapid-0.2.8/tests/test_pywrapid_utils_file_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-04-25 14:08:31.000000 pywrapid-0.2.8/tests/test_pywrapid_webclient_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-25 14:08:31.000000 pywrapid-0.2.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:43:41.033866 pywrapid-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-27 14:43:19.000000 pywrapid-0.2.9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:43:41.025866 pywrapid-0.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:43:41.029866 pywrapid-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-27 14:43:19.000000 pywrapid-0.2.9/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-27 14:43:19.000000 pywrapid-0.2.9/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-27 14:43:19.000000 pywrapid-0.2.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-27 14:43:19.000000 pywrapid-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-27 14:43:19.000000 pywrapid-0.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-27 14:43:19.000000 pywrapid-0.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 14:43:19.000000 pywrapid-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-04-27 14:43:41.033866 pywrapid-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-27 14:43:19.000000 pywrapid-0.2.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:43:41.025866 pywrapid-0.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:43:41.029866 pywrapid-0.2.9/docs/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-27 14:43:19.000000 pywrapid-0.2.9/docs/src/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-27 14:43:19.000000 pywrapid-0.2.9/docs/src/developer-guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:43:41.029866 pywrapid-0.2.9/docs/src/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-04-27 14:43:19.000000 pywrapid-0.2.9/docs/src/features/config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-04-27 14:43:19.000000 pywrapid-0.2.9/docs/src/features/log.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-27 14:43:19.000000 pywrapid-0.2.9/docs/src/features/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-27 14:43:19.000000 pywrapid-0.2.9/docs/src/features/webclient.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-27 14:43:19.000000 pywrapid-0.2.9/docs/src/features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-27 14:43:19.000000 pywrapid-0.2.9/docs/src/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-27 14:43:19.000000 pywrapid-0.2.9/docs/src/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-27 14:43:19.000000 pywrapid-0.2.9/docs/src/user-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-27 14:43:19.000000 pywrapid-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 14:43:19.000000 pywrapid-0.2.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 14:43:19.000000 pywrapid-0.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 14:43:41.033866 pywrapid-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:43:41.025866 pywrapid-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:43:41.029866 pywrapid-0.2.9/src/pywrapid/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-27 14:43:19.000000 pywrapid-0.2.9/src/pywrapid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:43:41.029866 pywrapid-0.2.9/src/pywrapid/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-27 14:43:19.000000 pywrapid-0.2.9/src/pywrapid/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-04-27 14:43:19.000000 pywrapid-0.2.9/src/pywrapid/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-27 14:43:19.000000 pywrapid-0.2.9/src/pywrapid/config/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 14:43:19.000000 pywrapid-0.2.9/src/pywrapid/config/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:43:41.029866 pywrapid-0.2.9/src/pywrapid/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-27 14:43:19.000000 pywrapid-0.2.9/src/pywrapid/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-27 14:43:19.000000 pywrapid-0.2.9/src/pywrapid/log/application_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:43:41.029866 pywrapid-0.2.9/src/pywrapid/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-27 14:43:19.000000 pywrapid-0.2.9/src/pywrapid/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-27 14:43:19.000000 pywrapid-0.2.9/src/pywrapid/utils/dict_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-04-27 14:43:19.000000 pywrapid-0.2.9/src/pywrapid/utils/filesystem_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:43:41.029866 pywrapid-0.2.9/src/pywrapid/webclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-27 14:43:19.000000 pywrapid-0.2.9/src/pywrapid/webclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-27 14:43:19.000000 pywrapid-0.2.9/src/pywrapid/webclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 14:43:19.000000 pywrapid-0.2.9/src/pywrapid/webclient/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13722 2023-04-27 14:43:19.000000 pywrapid-0.2.9/src/pywrapid/webclient/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:43:41.029866 pywrapid-0.2.9/src/pywrapid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-04-27 14:43:41.000000 pywrapid-0.2.9/src/pywrapid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-27 14:43:41.000000 pywrapid-0.2.9/src/pywrapid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 14:43:41.000000 pywrapid-0.2.9/src/pywrapid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-27 14:43:41.000000 pywrapid-0.2.9/src/pywrapid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 14:43:41.000000 pywrapid-0.2.9/src/pywrapid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:43:41.033866 pywrapid-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-27 14:43:19.000000 pywrapid-0.2.9/tests/test_conf_ok.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-27 14:43:19.000000 pywrapid-0.2.9/tests/test_pywrapid_config_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-04-27 14:43:19.000000 pywrapid-0.2.9/tests/test_pywrapid_logging_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-27 14:43:19.000000 pywrapid-0.2.9/tests/test_pywrapid_utils_dict_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12133 2023-04-27 14:43:19.000000 pywrapid-0.2.9/tests/test_pywrapid_utils_filesystem_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-04-27 14:43:19.000000 pywrapid-0.2.9/tests/test_pywrapid_webclient_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-27 14:43:19.000000 pywrapid-0.2.9/tox.ini
```

### Comparing `pywrapid-0.2.8/.github/workflows/codeql.yml` & `pywrapid-0.2.9/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.8/.github/workflows/dependency-review.yml` & `pywrapid-0.2.9/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.8/.github/workflows/python-publish.yml` & `pywrapid-0.2.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.8/.gitignore` & `pywrapid-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.8/CODE_OF_CONDUCT.md` & `pywrapid-0.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.8/LICENSE` & `pywrapid-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.8/PKG-INFO` & `pywrapid-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywrapid
-Version: 0.2.8
+Version: 0.2.9
 Summary: Collection of wrapper libraries for rapid development of python applications
 Author-email: Jonas Werme <jonas.werme@nsahq.se>, Marcus Wallgren <marcus.wallgren@nsahq.se>
 Maintainer-email: Jonas Werme <jonas.werme@nsahq.se>, Marcus Wallgren <marcus.wallgren@nsahq.se>
 License: MIT License
         
         Copyright (c) 2022 NSAHQ
```

### Comparing `pywrapid-0.2.8/README.rst` & `pywrapid-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.8/docs/src/conf.py` & `pywrapid-0.2.9/docs/src/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,33 +13,34 @@
 import os
 import sys
 from datetime import datetime
 
 import sphinx_rtd_theme
 
 test_path = os.path.abspath("../")
-
 tp = os.path.abspath(os.path.join(test_path, "../", "src"))
 sys.path.insert(0, tp)
+sys.path.insert(0, os.path.abspath("../../"))
+sys.path.insert(0, os.path.abspath("../../src/pywrapid"))
 # pylint: disable=invalid-name
 
 # -- Project information -----------------------------------------------------
 
 project = "pywrapid"
 copyright = f"2022-{datetime.now().year}, NSAHQ"  # pylint: disable=redefined-builtin
 author = "Jonas Werme"
 
-version = "0.0.1"
-release = "0.0.1"
+version = "0.2.0"
+release = "0.2.0"
 
 # -- General configuration ---------------------------------------------------
 
 extensions = [
     "sphinx.ext.autodoc",
-    "sphinx_autodoc_typehints",
+#    "sphinx_autodoc_typehints",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
     "sphinx.ext.viewcode",
     "sphinx_rtd_theme",
 ]
```

### Comparing `pywrapid-0.2.8/docs/src/developer-guide.rst` & `pywrapid-0.2.9/docs/src/developer-guide.rst`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.8/docs/src/features/config.rst` & `pywrapid-0.2.9/docs/src/features/config.rst`

 * *Files 5% similar despite different names*

```diff
@@ -81,22 +81,20 @@
           level: 0
 
 Application Configuration
 -------------------------
 
 .. autoclass:: pywrapid.config.ApplicationConfig
    :members:
-   :undoc-members:
    :show-inheritance:
 
 Configuration Sub section
 -------------------------
 .. autoclass:: pywrapid.config.ConfigSubSection
    :members:
-   :undoc-members:
    :show-inheritance:
 
 Exceptions
 ----------
 .. autoexception:: pywrapid.config.ConfigurationException
    :show-inheritance:
```

### Comparing `pywrapid-0.2.8/docs/src/features/log.rst` & `pywrapid-0.2.9/docs/src/features/log.rst`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.8/docs/src/features/webclient.rst` & `pywrapid-0.2.9/docs/src/features/webclient.rst`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.8/docs/src/user-guide.rst` & `pywrapid-0.2.9/docs/src/user-guide.rst`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.8/pyproject.toml` & `pywrapid-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.8/src/pywrapid/config/config.py` & `pywrapid-0.2.9/src/pywrapid/config/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,15 @@
 import yaml
 
 from pywrapid.config.exceptions import (
     ConfigurationError,
     ConfigurationFileNotFoundError,
     ConfigurationValidationError,
 )
-from pywrapid.utils.dict_tools import dict_keys_exist
-from pywrapid.utils.file_tools import is_file_readable
+from pywrapid.utils import dict_keys_exist, is_file_readable
 
 log = logging.getLogger(__name__)
 
 
 class WrapidConfig:
     """Base configuration class"""
```

### Comparing `pywrapid-0.2.8/src/pywrapid/config/exceptions.py` & `pywrapid-0.2.9/src/pywrapid/config/exceptions.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.8/src/pywrapid/log/application_log.py` & `pywrapid-0.2.9/src/pywrapid/log/application_log.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.8/src/pywrapid/utils/dict_tools.py` & `pywrapid-0.2.9/src/pywrapid/utils/dict_tools.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,19 +5,25 @@
 from copy import deepcopy
 from typing import Optional
 
 
 def dict_merge(
     base: dict, data: dict, path: Optional[list] = None, raise_on_conflict: bool = False
 ) -> dict:
-    """Recursive merge of dict objects
+    """Recursive merge of dict objects into new dict
+
+    The merge will make a deep copy of the base dict and merge the data dict into it.
+    It will not modify the base dict being passed in.
+
+    If the same key exists in base and data, the value from data will be used unless
+    raise_on_conflict is True, in which case a ValueError will be raised.
 
     Args:
-        base (dict): _description_
-        data (dict): _description_
+        base (dict): The base dict to merge into
+        data (dict): The data dict to merge into base
         path (list, optional): _description_. Defaults to None.
         raise_on_conflict (bool): Raise on conflict instead of overwriting base
 
     Raises:
         ValueError: Raised on leaf conflict when raise_on_conflict is True
 
     Returns: Merged dict
@@ -33,15 +39,15 @@
                     data[key],
                     path=path + [str(key)],
                     raise_on_conflict=raise_on_conflict,
                 )
             elif data[key] is None:
                 continue
             elif copy[key] == data[key]:
-                continue  # same leaf value
+                continue  # same leaf value, skip traversal if children are the same
             else:
                 if raise_on_conflict:
                     raise ValueError(f"Conflict at {'.'.join(path + [str(key)])}")
                 copy[key] = data[key]
         else:
             copy[key] = data[key]
 
@@ -69,16 +75,16 @@
         bool: True when validation is passed.
     """
     if not expected_keys:
         if raise_on_fail:
             raise ValueError("No expected values supplied")
         return False
 
+    missed = []
     for key in expected_keys:
-        missed = []
         if key not in data:
             missed.append(key)
         elif data[key] in ["", (), [], {}, None] and allow_empty is False:
             if raise_on_fail:
                 raise ValueError(f"Empty value in: {key}")
             return False
```

### Comparing `pywrapid-0.2.8/src/pywrapid/utils/file_tools.py` & `pywrapid-0.2.9/src/pywrapid/utils/filesystem_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,17 +141,17 @@
     if os.path.islink(path):
         metadata["type"] = "symlink"
         metadata["symlink"] = os.path.realpath(path)
 
     return metadata
 
 
-def find_directory_content(  # pylint: disable=R0912,R0914
+def find_directory_content(
     path: str, depth: int = 0, **options: Any
-) -> list[dict]:
+) -> list[dict]:  # pylint: disable=R0912,R0914
     """Get directory content and allow os walk.
     Includes sub levels of user defined depth with metadata and item names as list of dict return.
 
     Args:
         path (str): Path to configuration file.
         depth (int, optional): Depth to walk. Defaults to 0/unlimited.
```

### Comparing `pywrapid-0.2.8/src/pywrapid/webclient/__init__.py` & `pywrapid-0.2.9/src/pywrapid/webclient/__init__.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.8/src/pywrapid/webclient/exceptions.py` & `pywrapid-0.2.9/src/pywrapid/webclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.8/src/pywrapid/webclient/web.py` & `pywrapid-0.2.9/src/pywrapid/webclient/web.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 from time import time
 from typing import Any, Optional, Type, Union
 from urllib.parse import urlparse
 
 import jwt
 from requests import HTTPError, RequestException, Response, Timeout, TooManyRedirects, request
 
-from pywrapid.config.config import WrapidConfig
-from pywrapid.utils.file_tools import is_file_readable
+from pywrapid.config import WrapidConfig
+from pywrapid.utils import is_file_readable
 
 from .exceptions import (
     ClientAuthenticationError,
     ClientAuthorizationError,
     ClientConnectionError,
     ClientError,
     ClientHTTPError,
```

### Comparing `pywrapid-0.2.8/src/pywrapid.egg-info/PKG-INFO` & `pywrapid-0.2.9/src/pywrapid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywrapid
-Version: 0.2.8
+Version: 0.2.9
 Summary: Collection of wrapper libraries for rapid development of python applications
 Author-email: Jonas Werme <jonas.werme@nsahq.se>, Marcus Wallgren <marcus.wallgren@nsahq.se>
 Maintainer-email: Jonas Werme <jonas.werme@nsahq.se>, Marcus Wallgren <marcus.wallgren@nsahq.se>
 License: MIT License
         
         Copyright (c) 2022 NSAHQ
```

### Comparing `pywrapid-0.2.8/src/pywrapid.egg-info/SOURCES.txt` & `pywrapid-0.2.9/src/pywrapid.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .flake8
 .gitignore
+.readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 tox.ini
@@ -30,17 +31,18 @@
 src/pywrapid/config/config.py
 src/pywrapid/config/exceptions.py
 src/pywrapid/config/requirements.txt
 src/pywrapid/log/__init__.py
 src/pywrapid/log/application_log.py
 src/pywrapid/utils/__init__.py
 src/pywrapid/utils/dict_tools.py
-src/pywrapid/utils/file_tools.py
+src/pywrapid/utils/filesystem_tools.py
 src/pywrapid/webclient/__init__.py
 src/pywrapid/webclient/exceptions.py
 src/pywrapid/webclient/requirements.txt
 src/pywrapid/webclient/web.py
 tests/test_conf_ok.yml
 tests/test_pywrapid_config_config.py
 tests/test_pywrapid_logging_logging.py
-tests/test_pywrapid_utils_file_tools.py
+tests/test_pywrapid_utils_dict_tools.py
+tests/test_pywrapid_utils_filesystem_tools.py
 tests/test_pywrapid_webclient_web.py
```

### Comparing `pywrapid-0.2.8/tests/test_pywrapid_config_config.py` & `pywrapid-0.2.9/tests/test_pywrapid_config_config.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.8/tests/test_pywrapid_logging_logging.py` & `pywrapid-0.2.9/tests/test_pywrapid_logging_logging.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.8/tests/test_pywrapid_utils_file_tools.py` & `pywrapid-0.2.9/tests/test_pywrapid_utils_filesystem_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
-"""Pywrapid config tests"""
+"""Pywrapid filesystem tools tests"""
 
 import os
 
 import pytest
 
-import pywrapid.utils.file_tools as module_0
+import pywrapid.utils as module_0
 
 # pylint: disable=redefined-outer-name, protected-access
 
 
 @pytest.fixture()
 def filesystem_fixture_0(tmp_path) -> str:
     """Fixture for producing file and directory structure"""
```

### Comparing `pywrapid-0.2.8/tests/test_pywrapid_webclient_web.py` & `pywrapid-0.2.9/tests/test_pywrapid_webclient_web.py`

 * *Files identical despite different names*

### Comparing `pywrapid-0.2.8/tox.ini` & `pywrapid-0.2.9/tox.ini`

 * *Files identical despite different names*

