# Comparing `tmp/david-test-datadog-sma-0.0.3.tar.gz` & `tmp/david-test-datadog-sma-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "david-test-datadog-sma-0.0.3.tar", last modified: Mon Apr 24 19:33:29 2023, max compression
+gzip compressed data, was "david-test-datadog-sma-0.0.4.tar", last modified: Fri Apr 28 02:57:03 2023, max compression
```

## Comparing `david-test-datadog-sma-0.0.3.tar` & `david-test-datadog-sma-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-04-24 19:33:29.007841 david-test-datadog-sma-0.0.3/
--rw-r--r--   0 david.lee   (503) staff       (20)       66 2023-04-24 19:33:29.007684 david-test-datadog-sma-0.0.3/PKG-INFO
--rw-r--r--   0 david.lee   (503) staff       (20)      107 2023-04-24 19:33:24.000000 david-test-datadog-sma-0.0.3/pyproject.toml
--rw-r--r--   0 david.lee   (503) staff       (20)       38 2023-04-24 19:33:29.007889 david-test-datadog-sma-0.0.3/setup.cfg
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-04-24 19:33:28.999946 david-test-datadog-sma-0.0.3/src/
--rw-r--r--   0 david.lee   (503) staff       (20)        0 2023-04-18 15:20:38.000000 david-test-datadog-sma-0.0.3/src/__init__.py
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-04-24 19:33:29.000068 david-test-datadog-sma-0.0.3/src/datadog-serverless-agent-linux-amd64/
--rw-r--r--   0 david.lee   (503) staff       (20)  3135520 2023-04-24 19:33:24.000000 david-test-datadog-sma-0.0.3/src/datadog-serverless-agent-linux-amd64/datadog-serverless-trace-mini-agent
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-04-24 19:33:29.002020 david-test-datadog-sma-0.0.3/src/datadog-serverless-agent-windows-amd64/
--rw-r--r--   0 david.lee   (503) staff       (20)   824832 2023-04-24 16:56:16.000000 david-test-datadog-sma-0.0.3/src/datadog-serverless-agent-windows-amd64/datadog-serverless-trace-mini-agent.exe
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-04-24 19:33:29.007440 david-test-datadog-sma-0.0.3/src/david_test_datadog_sma.egg-info/
--rw-r--r--   0 david.lee   (503) staff       (20)       66 2023-04-24 19:33:28.000000 david-test-datadog-sma-0.0.3/src/david_test_datadog_sma.egg-info/PKG-INFO
--rw-r--r--   0 david.lee   (503) staff       (20)      390 2023-04-24 19:33:28.000000 david-test-datadog-sma-0.0.3/src/david_test_datadog_sma.egg-info/SOURCES.txt
--rw-r--r--   0 david.lee   (503) staff       (20)        1 2023-04-24 19:33:28.000000 david-test-datadog-sma-0.0.3/src/david_test_datadog_sma.egg-info/dependency_links.txt
--rw-r--r--   0 david.lee   (503) staff       (20)       85 2023-04-24 19:33:28.000000 david-test-datadog-sma-0.0.3/src/david_test_datadog_sma.egg-info/top_level.txt
+drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-04-28 02:57:03.436971 david-test-datadog-sma-0.0.4/
+-rw-r--r--   0 david.lee   (503) staff       (20)       66 2023-04-28 02:57:03.436811 david-test-datadog-sma-0.0.4/PKG-INFO
+-rw-r--r--   0 david.lee   (503) staff       (20)      107 2023-04-28 02:56:58.000000 david-test-datadog-sma-0.0.4/pyproject.toml
+-rw-r--r--   0 david.lee   (503) staff       (20)       38 2023-04-28 02:57:03.437023 david-test-datadog-sma-0.0.4/setup.cfg
+drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-04-28 02:57:03.433973 david-test-datadog-sma-0.0.4/src/
+-rw-r--r--   0 david.lee   (503) staff       (20)        0 2023-04-18 15:20:38.000000 david-test-datadog-sma-0.0.4/src/__init__.py
+drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-04-28 02:57:03.434146 david-test-datadog-sma-0.0.4/src/datadog-serverless-agent-linux-amd64/
+-rwxr-xr-x   0 david.lee   (503) staff       (20)  3135520 2023-04-24 19:33:24.000000 david-test-datadog-sma-0.0.4/src/datadog-serverless-agent-linux-amd64/datadog-serverless-trace-mini-agent
+drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-04-28 02:57:03.436584 david-test-datadog-sma-0.0.4/src/david_test_datadog_sma.egg-info/
+-rw-r--r--   0 david.lee   (503) staff       (20)       66 2023-04-28 02:57:03.000000 david-test-datadog-sma-0.0.4/src/david_test_datadog_sma.egg-info/PKG-INFO
+-rw-r--r--   0 david.lee   (503) staff       (20)      307 2023-04-28 02:57:03.000000 david-test-datadog-sma-0.0.4/src/david_test_datadog_sma.egg-info/SOURCES.txt
+-rw-r--r--   0 david.lee   (503) staff       (20)        1 2023-04-28 02:57:03.000000 david-test-datadog-sma-0.0.4/src/david_test_datadog_sma.egg-info/dependency_links.txt
+-rw-r--r--   0 david.lee   (503) staff       (20)       46 2023-04-28 02:57:03.000000 david-test-datadog-sma-0.0.4/src/david_test_datadog_sma.egg-info/top_level.txt
```

### Comparing `david-test-datadog-sma-0.0.3/src/datadog-serverless-agent-linux-amd64/datadog-serverless-trace-mini-agent` & `david-test-datadog-sma-0.0.4/src/datadog-serverless-agent-linux-amd64/datadog-serverless-trace-mini-agent`

 * *Files identical despite different names*

