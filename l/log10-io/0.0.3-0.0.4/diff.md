# Comparing `tmp/log10_io-0.0.3.tar.gz` & `tmp/log10_io-0.0.4.tar.gz`

## Comparing `log10_io-0.0.3.tar` & `log10_io-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,20 @@
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 log10_io-0.0.3/setup.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 log10_io-0.0.3/.github/workflows/release.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 log10_io-0.0.3/log10/        __init__.py
--rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 log10_io-0.0.3/log10/load.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 log10_io-0.0.3/tests/test_chatcompletion.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 log10_io-0.0.3/tests/test_completion.py
--rw-r--r--   0        0        0    10777 2020-02-02 00:00:00.000000 log10_io-0.0.3/tests/test_langchain_babyagi.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 log10_io-0.0.3/tests/test_langchain_multiple_tools.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 log10_io-0.0.3/tests/test_langchain_simple_sequential.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 log10_io-0.0.3/tests/test_langchain_sqlagent.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 log10_io-0.0.3/tests/test_multiple_sessions.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 log10_io-0.0.3/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 log10_io-0.0.3/LICENSE
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 log10_io-0.0.3/README.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 log10_io-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 log10_io-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 log10_io-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 log10_io-0.0.4/setup.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 log10_io-0.0.4/.github/workflows/release.yml
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 log10_io-0.0.4/examples/chatcompletion.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 log10_io-0.0.4/examples/chatcompletion_async_vs_sync.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 log10_io-0.0.4/examples/completion.py
+-rw-r--r--   0        0        0    10777 2020-02-02 00:00:00.000000 log10_io-0.0.4/examples/langchain_babyagi.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 log10_io-0.0.4/examples/langchain_multiple_tools.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 log10_io-0.0.4/examples/langchain_simple_sequential.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 log10_io-0.0.4/examples/langchain_sqlagent.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 log10_io-0.0.4/examples/multiple_sessions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 log10_io-0.0.4/log10/        __init__.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 log10_io-0.0.4/log10/bigquery.py
+-rw-r--r--   0        0        0     9672 2020-02-02 00:00:00.000000 log10_io-0.0.4/log10/load.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 log10_io-0.0.4/log10/schemas/bigquery.json
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 log10_io-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 log10_io-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 log10_io-0.0.4/README.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 log10_io-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 log10_io-0.0.4/PKG-INFO
```

### Comparing `log10_io-0.0.3/.github/workflows/release.yml` & `log10_io-0.0.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.3/tests/test_langchain_babyagi.py` & `log10_io-0.0.4/examples/langchain_babyagi.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.3/tests/test_langchain_multiple_tools.py` & `log10_io-0.0.4/examples/langchain_multiple_tools.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.3/tests/test_langchain_simple_sequential.py` & `log10_io-0.0.4/examples/langchain_simple_sequential.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.3/tests/test_langchain_sqlagent.py` & `log10_io-0.0.4/examples/langchain_sqlagent.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.3/tests/test_multiple_sessions.py` & `log10_io-0.0.4/examples/multiple_sessions.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.3/LICENSE` & `log10_io-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.3/pyproject.toml` & `log10_io-0.0.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "log10-io"
-version = "0.0.3"
+version = "0.0.4"
 authors = []
 license = "MIT"
 description = "Unified LLM data management"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `log10_io-0.0.3/PKG-INFO` & `log10_io-0.0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,14 @@
-Metadata-Version: 2.1
-Name: log10-io
-Version: 0.0.3
-Summary: Unified LLM data management
-Project-URL: Homepage, https://github.com/log10-io/log10
-Project-URL: Bug Tracker, https://github.com/log10-io/log10/issues
-License-Expression: MIT
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # log10
 
 ⚡ Unified LLM data management ⚡
 
+[![pypi](https://github.com/log10-io/log10/actions/workflows/release.yml/badge.svg)](https://github.com/log10-io/log10/actions/workflows/release.yml)
+[![](https://dcbadge.vercel.app/api/server/CZQvnuRV94?compact=true&style=flat)](https://discord.gg/CZQvnuRV94)
+
 ## Quick Install
 
 `pip install log10-io`
 
 ## 🤔 What is this?
 
 A one-line Python integration to manage your LLM data.
@@ -41,22 +30,42 @@
 
 Prompt chains such as those in [Langchain](https://github.com/hwchase17/langchain) can be difficult to debug. Log10 provides prompt provenance, session tracking and call stack functionality to help debug chains.
 
 **📝📊 Logging**
 
 Log all your OpenAI calls to compare and find the best prompts, store feedback, collect latency and usage metrics, and perform analytics and compliance monitoring of LLM powered features.
 
+**💿🧩 Flexible data store**
+
+log10 provides a managed data store, but if you'd prefer to manage data in your own environment, you can use data stores like google big query.
+
+Install the big query client library with:
+
+`pip install log10-io[bigquery]`
+
+And provide the following configuration in either a `.env` file, or as environment variables:
+
+| Name | Description |
+|------|-------------|
+| `LOG10_DATA_STORE`  |  Either `log10` or `bigquery` |
+| `LOG10_BQ_PROJECT_ID`   | Your google cloud project id      |
+| `LOG10_BQ_DATASET_ID`  |  The big query dataset id  |
+| `LOG10_BQ_COMPLETIONS_TABLE_ID` | The name of the table to store completions in |
+
+**Note** that your environment should have been setup with google cloud credentials. Read more [here](https://cloud.google.com/sdk/gcloud/reference/auth/login) about authenticating.
+
 **🧠🔁 Readiness for RLHF & self hosting**
 
 Use your data and feedback from users to fine-tune custom models with RLHF with the option of building and deploying more reliable, accurate and efficient self-hosted models. 
 
 **👥🤝 Collaboration**
 
 Create flexible groups to share and collaborate over all of the above features
 
 ## ⚙️ Setup
 
 Create a free account at [log10.io](https://log10.io) to get a `LOG10_TOKEN` and a `LOG10_ORG_ID`. Please add these to your environment along with `LOG10_URL=https://log10.io`. 
 
+
 ## 💬 Community
 
-We welcome community participation and feedback. Please leave an issue, submit a PR or join our [Discord](https://discord.gg/CGW6xNbC).
+We welcome community participation and feedback. Please leave an issue, submit a PR or join our [Discord](https://discord.gg/CZQvnuRV94).
```

