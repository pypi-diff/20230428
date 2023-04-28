# Comparing `tmp/orquestra-sdk-0.46.0.tar.gz` & `tmp/orquestra-sdk-0.47.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orquestra-sdk-0.46.0.tar", last modified: Fri Apr 14 11:54:27 2023, max compression
+gzip compressed data, was "orquestra-sdk-0.47.0.tar", last modified: Fri Apr 28 13:27:42 2023, max compression
```

## Comparing `orquestra-sdk-0.46.0.tar` & `orquestra-sdk-0.47.0.tar`

### file list

```diff
@@ -1,414 +1,759 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.239473 orquestra-sdk-0.46.0/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.927627 orquestra-sdk-0.46.0/.github/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.928884 orquestra-sdk-0.46.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 alex       (501) staff       (20)      605 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 alex       (501) staff       (20)      600 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 alex       (501) staff       (20)      678 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/.github/pull_request_template.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.933721 orquestra-sdk-0.46.0/.github/workflows/
--rw-r--r--   0 alex       (501) staff       (20)     1734 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/.github/workflows/coverage.yml
--rw-r--r--   0 alex       (501) staff       (20)      939 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/.github/workflows/performance.yml
--rw-r--r--   0 alex       (501) staff       (20)     2814 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/.github/workflows/publish_release.yml
--rw-r--r--   0 alex       (501) staff       (20)     1212 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/.github/workflows/style.yml
--rw-r--r--   0 alex       (501) staff       (20)      776 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/.github/workflows/typing.yml
--rw-r--r--   0 alex       (501) staff       (20)     1836 2023-01-11 16:41:33.000000 orquestra-sdk-0.46.0/.gitignore
--rw-r--r--   0 alex       (501) staff       (20)    11446 2023-04-14 11:54:11.000000 orquestra-sdk-0.46.0/CHANGELOG.md
--rw-r--r--   0 alex       (501) staff       (20)      241 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/CODEOWNERS
--rw-r--r--   0 alex       (501) staff       (20)     3839 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/CONTRIBUTING.md
--rw-r--r--   0 alex       (501) staff       (20)    11358 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)        9 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/MANIFEST.in
--rw-r--r--   0 alex       (501) staff       (20)     3661 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/Makefile
--rw-r--r--   0 alex       (501) staff       (20)     1654 2023-04-14 11:54:27.239769 orquestra-sdk-0.46.0/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     1009 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.934947 orquestra-sdk-0.46.0/docs/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.939656 orquestra-sdk-0.46.0/docs/examples/
--rw-r--r--   0 alex       (501) staff       (20)      204 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/docs/examples/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      835 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/docs/examples/config_management.py
--rw-r--r--   0 alex       (501) staff       (20)     1170 2023-04-03 14:17:03.000000 orquestra-sdk-0.46.0/docs/examples/quickstart.py
--rw-r--r--   0 alex       (501) staff       (20)      488 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/docs/examples/remote_workflow.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.948347 orquestra-sdk-0.46.0/docs/examples/tests/
--rw-r--r--   0 alex       (501) staff       (20)      260 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/docs/examples/tests/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      836 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/docs/examples/tests/conftest.py
--rw-r--r--   0 alex       (501) staff       (20)      989 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/docs/examples/tests/parsers.py
--rw-r--r--   0 alex       (501) staff       (20)     3710 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/docs/examples/tests/test_local_ray.py
--rw-r--r--   0 alex       (501) staff       (20)     1966 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/docs/examples/tests/test_logging.py
--rw-r--r--   0 alex       (501) staff       (20)     5077 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/docs/examples/tests/test_parametrized_workflows.py
--rw-r--r--   0 alex       (501) staff       (20)     6395 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/docs/examples/tests/test_remote.py
--rw-r--r--   0 alex       (501) staff       (20)     5509 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/docs/examples/tests/test_secrets.py
--rw-r--r--   0 alex       (501) staff       (20)    13856 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/docs/examples/tests/test_workflow_syntax.py
--rw-r--r--   0 alex       (501) staff       (20)      505 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/docs/examples/workflow_defs.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.954737 orquestra-sdk-0.46.0/docs/guides/
--rw-r--r--   0 alex       (501) staff       (20)     9090 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/docs/guides/dependency-installation.rst
--rw-r--r--   0 alex       (501) staff       (20)      181 2023-04-14 11:50:54.000000 orquestra-sdk-0.46.0/docs/guides/index.rst
--rw-r--r--   0 alex       (501) staff       (20)     1305 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/docs/guides/logging.rst
--rw-r--r--   0 alex       (501) staff       (20)     6731 2023-04-14 11:50:54.000000 orquestra-sdk-0.46.0/docs/guides/resource-management.rst
--rw-r--r--   0 alex       (501) staff       (20)     2066 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/docs/guides/runtime-configuration.rst
--rw-r--r--   0 alex       (501) staff       (20)     5060 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/docs/guides/workflow-runs.rst
--rw-r--r--   0 alex       (501) staff       (20)     5901 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/docs/guides/workflow-syntax.rst
--rw-r--r--   0 alex       (501) staff       (20)      834 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/docs/index.rst
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.956857 orquestra-sdk-0.46.0/docs/quickref/
--rw-r--r--   0 alex       (501) staff       (20)      247 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/docs/quickref/cli-reference.rst
--rw-r--r--   0 alex       (501) staff       (20)       89 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/docs/quickref/index.rst
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.966151 orquestra-sdk-0.46.0/docs/tutorials/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.971477 orquestra-sdk-0.46.0/docs/tutorials/images/
--rw-r--r--   0 alex       (501) staff       (20)   235665 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/docs/tutorials/images/orq-login-copy-token.png
--rw-r--r--   0 alex       (501) staff       (20)   104197 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/docs/tutorials/images/orq-login-grant-access.png
--rw-r--r--   0 alex       (501) staff       (20)   110685 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/docs/tutorials/images/orq-login-landing-page.png
--rw-r--r--   0 alex       (501) staff       (20)     5286 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/docs/tutorials/images/win-redist-picture.png
--rw-r--r--   0 alex       (501) staff       (20)      400 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/docs/tutorials/index.rst
--rw-r--r--   0 alex       (501) staff       (20)     2743 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/docs/tutorials/installing-macos-linux.rst
--rw-r--r--   0 alex       (501) staff       (20)     3947 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/docs/tutorials/installing-windows.rst
--rw-r--r--   0 alex       (501) staff       (20)     5224 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/docs/tutorials/jupyter-sdk.rst
--rw-r--r--   0 alex       (501) staff       (20)     2385 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/docs/tutorials/parametrized-workflows.rst
--rw-r--r--   0 alex       (501) staff       (20)     1476 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/docs/tutorials/quickstart.rst
--rw-r--r--   0 alex       (501) staff       (20)     1760 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/docs/tutorials/ray.rst
--rw-r--r--   0 alex       (501) staff       (20)     3232 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/docs/tutorials/remote.rst
--rw-r--r--   0 alex       (501) staff       (20)     2438 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/docs/tutorials/secrets.rst
--rw-r--r--   0 alex       (501) staff       (20)     1978 2023-04-03 14:17:03.000000 orquestra-sdk-0.46.0/pyproject.toml
--rw-r--r--   0 alex       (501) staff       (20)      193 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/pytest.ini
--rw-r--r--   0 alex       (501) staff       (20)     1473 2023-04-14 11:54:27.241054 orquestra-sdk-0.46.0/setup.cfg
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.900500 orquestra-sdk-0.46.0/src/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.891892 orquestra-sdk-0.46.0/src/orquestra/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.974947 orquestra-sdk-0.46.0/src/orquestra/sdk/
--rw-r--r--   0 alex       (501) staff       (20)     1270 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.993875 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/
--rw-r--r--   0 alex       (501) staff       (20)      204 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.997760 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_api/
--rw-r--r--   0 alex       (501) staff       (20)      624 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_api/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    24662 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_api/_config.py
--rw-r--r--   0 alex       (501) staff       (20)     9923 2023-04-03 14:17:03.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_api/_task_run.py
--rw-r--r--   0 alex       (501) staff       (20)    21216 2023-04-14 11:54:11.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_api/_wf_run.py
--rw-r--r--   0 alex       (501) staff       (20)     8563 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_ast.py
--rw-r--r--   0 alex       (501) staff       (20)    23338 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_config.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.002238 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_conversions/
--rw-r--r--   0 alex       (501) staff       (20)      204 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_conversions/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     3509 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_conversions/_ids.py
--rw-r--r--   0 alex       (501) staff       (20)     7074 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_conversions/_imports.py
--rw-r--r--   0 alex       (501) staff       (20)    12578 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_conversions/_invocations.py
--rw-r--r--   0 alex       (501) staff       (20)     3905 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_conversions/_yaml_exporter.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.005052 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_db/
--rw-r--r--   0 alex       (501) staff       (20)      288 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_db/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     5107 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_db/_db.py
--rw-r--r--   0 alex       (501) staff       (20)      894 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_db/_migration.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.009560 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_driver/
--rw-r--r--   0 alex       (501) staff       (20)      204 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_driver/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    16995 2023-04-14 11:54:11.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_driver/_ce_runtime.py
--rw-r--r--   0 alex       (501) staff       (20)    22013 2023-04-14 11:54:11.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_driver/_client.py
--rw-r--r--   0 alex       (501) staff       (20)     4563 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_driver/_exceptions.py
--rw-r--r--   0 alex       (501) staff       (20)     7799 2023-04-14 11:54:11.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_driver/_models.py
--rw-r--r--   0 alex       (501) staff       (20)    39676 2023-04-14 11:50:54.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_dsl.py
--rw-r--r--   0 alex       (501) staff       (20)     1999 2023-04-14 11:50:54.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_env.py
--rw-r--r--   0 alex       (501) staff       (20)     2338 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_exec_ctx.py
--rw-r--r--   0 alex       (501) staff       (20)     1776 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_factory.py
--rw-r--r--   0 alex       (501) staff       (20)     3433 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_git_url_utils.py
--rw-r--r--   0 alex       (501) staff       (20)     3021 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_graphs.py
--rw-r--r--   0 alex       (501) staff       (20)    10014 2023-04-14 11:54:11.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_in_process_runtime.py
--rw-r--r--   0 alex       (501) staff       (20)     6460 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_log_adapter.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.011939 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_qe/
--rw-r--r--   0 alex       (501) staff       (20)      204 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_qe/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     7213 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_qe/_client.py
--rw-r--r--   0 alex       (501) staff       (20)    30607 2023-04-14 11:54:11.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_qe/_qe_runtime.py
--rw-r--r--   0 alex       (501) staff       (20)     4331 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_services.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.016108 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_testing/
--rw-r--r--   0 alex       (501) staff       (20)      204 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_testing/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     3979 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_testing/_connections.py
--rw-r--r--   0 alex       (501) staff       (20)     6942 2023-04-03 14:17:03.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_testing/_example_wfs.py
--rw-r--r--   0 alex       (501) staff       (20)      261 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_testing/_long_import.py
--rw-r--r--   0 alex       (501) staff       (20)    25529 2023-04-14 11:50:54.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_traversal.py
--rw-r--r--   0 alex       (501) staff       (20)     4347 2023-01-11 15:05:44.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_viz.py
--rw-r--r--   0 alex       (501) staff       (20)    25625 2023-04-14 11:54:11.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_workflow.py
--rw-r--r--   0 alex       (501) staff       (20)     7639 2023-04-14 11:54:11.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/abc.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.895412 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.021095 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/
--rw-r--r--   0 alex       (501) staff       (20)    12294 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_arg_resolvers.py
--rw-r--r--   0 alex       (501) staff       (20)      698 2023-04-14 11:50:54.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_cli_logs.py
--rw-r--r--   0 alex       (501) staff       (20)     3032 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_dumpers.py
--rw-r--r--   0 alex       (501) staff       (20)     9871 2023-04-14 11:50:54.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_entry.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.022924 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_login/
--rw-r--r--   0 alex       (501) staff       (20)     3043 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_login/_login.py
--rw-r--r--   0 alex       (501) staff       (20)     1489 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_login/_login_server.py
--rw-r--r--   0 alex       (501) staff       (20)    20331 2023-04-03 14:17:03.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_repos.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.025614 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_services/
--rw-r--r--   0 alex       (501) staff       (20)     1621 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_services/_down.py
--rw-r--r--   0 alex       (501) staff       (20)     1327 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_services/_status.py
--rw-r--r--   0 alex       (501) staff       (20)     2135 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_services/_up.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.027938 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_task/
--rw-r--r--   0 alex       (501) staff       (20)     3106 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_task/_logs.py
--rw-r--r--   0 alex       (501) staff       (20)     3627 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_task/_results.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.032693 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_ui/
--rw-r--r--   0 alex       (501) staff       (20)      367 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_ui/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.034704 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_corq_format/
--rw-r--r--   0 alex       (501) staff       (20)      624 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_corq_format/color.py
--rw-r--r--   0 alex       (501) staff       (20)     7794 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_corq_format/per_command.py
--rw-r--r--   0 alex       (501) staff       (20)     4107 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_errors.py
--rw-r--r--   0 alex       (501) staff       (20)     1648 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_models.py
--rw-r--r--   0 alex       (501) staff       (20)    10300 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_presenters.py
--rw-r--r--   0 alex       (501) staff       (20)     8309 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_prompts.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.040126 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/
--rw-r--r--   0 alex       (501) staff       (20)     3486 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_list.py
--rw-r--r--   0 alex       (501) staff       (20)     2739 2023-01-24 09:35:29.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_logs.py
--rw-r--r--   0 alex       (501) staff       (20)     3140 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_results.py
--rw-r--r--   0 alex       (501) staff       (20)     2507 2023-01-24 09:35:29.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_stop.py
--rw-r--r--   0 alex       (501) staff       (20)     3993 2023-01-24 09:35:29.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_submit.py
--rw-r--r--   0 alex       (501) staff       (20)     2138 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_view.py
--rw-r--r--   0 alex       (501) staff       (20)    11810 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/dispatch.py
--rw-r--r--   0 alex       (501) staff       (20)     6001 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/loader.py
--rw-r--r--   0 alex       (501) staff       (20)     5953 2023-04-03 14:17:03.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_base/serde.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.044941 orquestra-sdk-0.46.0/src/orquestra/sdk/_ray/
--rw-r--r--   0 alex       (501) staff       (20)      204 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_ray/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     6498 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_ray/_client.py
--rw-r--r--   0 alex       (501) staff       (20)    37302 2023-04-14 11:54:11.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_ray/_dag.py
--rw-r--r--   0 alex       (501) staff       (20)      867 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_ray/_id_gen.py
--rw-r--r--   0 alex       (501) staff       (20)     4389 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/_ray/_ray_logs.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.047826 orquestra-sdk-0.46.0/src/orquestra/sdk/examples/
--rw-r--r--   0 alex       (501) staff       (20)      204 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/examples/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1558 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/examples/exportable_wf.py
--rw-r--r--   0 alex       (501) staff       (20)     1116 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/examples/workflow_defs.py
--rw-r--r--   0 alex       (501) staff       (20)     3511 2023-04-14 11:54:11.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/exceptions.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.049792 orquestra-sdk-0.46.0/src/orquestra/sdk/kubernetes/
--rw-r--r--   0 alex       (501) staff       (20)      113 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/kubernetes/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2420 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/kubernetes/quantity.py
--rw-r--r--   0 alex       (501) staff       (20)     3090 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/packaging.py
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/py.typed
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.056461 orquestra-sdk-0.46.0/src/orquestra/sdk/schema/
--rw-r--r--   0 alex       (501) staff       (20)      204 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/schema/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1474 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/schema/configs.py
--rw-r--r--   0 alex       (501) staff       (20)    12189 2023-04-03 14:17:04.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/schema/ir.py
--rw-r--r--   0 alex       (501) staff       (20)      832 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/schema/local_database.py
--rw-r--r--   0 alex       (501) staff       (20)     4572 2023-03-31 15:43:09.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/schema/responses.py
--rw-r--r--   0 alex       (501) staff       (20)     1444 2023-04-14 11:54:11.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/schema/workflow_run.py
--rw-r--r--   0 alex       (501) staff       (20)     4114 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/schema/yaml_model.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.062547 orquestra-sdk-0.46.0/src/orquestra/sdk/secrets/
--rw-r--r--   0 alex       (501) staff       (20)     1104 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/secrets/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     5356 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/secrets/_api.py
--rw-r--r--   0 alex       (501) staff       (20)     2090 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/secrets/_auth.py
--rw-r--r--   0 alex       (501) staff       (20)     5243 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/secrets/_client.py
--rw-r--r--   0 alex       (501) staff       (20)     1222 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/secrets/_exceptions.py
--rw-r--r--   0 alex       (501) staff       (20)     1319 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/secrets/_models.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.063632 orquestra-sdk-0.46.0/src/orquestra/sdk/v2/
--rw-r--r--   0 alex       (501) staff       (20)     1072 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/src/orquestra/sdk/v2/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.072913 orquestra-sdk-0.46.0/src/orquestra_sdk.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     1654 2023-04-14 11:54:26.000000 orquestra-sdk-0.46.0/src/orquestra_sdk.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)    13008 2023-04-14 11:54:26.000000 orquestra-sdk-0.46.0/src/orquestra_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-04-14 11:54:26.000000 orquestra-sdk-0.46.0/src/orquestra_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       66 2023-04-14 11:54:26.000000 orquestra-sdk-0.46.0/src/orquestra_sdk.egg-info/entry_points.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-01-11 16:28:07.000000 orquestra-sdk-0.46.0/src/orquestra_sdk.egg-info/not-zip-safe
--rw-r--r--   0 alex       (501) staff       (20)      539 2023-04-14 11:54:26.000000 orquestra-sdk-0.46.0/src/orquestra_sdk.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       10 2023-04-14 11:54:26.000000 orquestra-sdk-0.46.0/src/orquestra_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.901429 orquestra-sdk-0.46.0/subtrees/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.082655 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/
--rw-r--r--   0 alex       (501) staff       (20)        9 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/MANIFEST.in
--rw-r--r--   0 alex       (501) staff       (20)     4535 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/Makefile
--rw-r--r--   0 alex       (501) staff       (20)     5600 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/README.rst
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.902822 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/actions/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.084224 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/actions/publish-release/
--rw-r--r--   0 alex       (501) staff       (20)     3132 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/actions/publish-release/action.yml
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.085412 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/actions/ssh_setup/
--rw-r--r--   0 alex       (501) staff       (20)      458 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/actions/ssh_setup/action.yml
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.086266 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/actions/style/
--rw-r--r--   0 alex       (501) staff       (20)      467 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/actions/style/action.yml
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.087216 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/bin/
--rwxr-xr-x   0 alex       (501) staff       (20)     2756 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/bin/get_next_version.py
--rw-r--r--   0 alex       (501) staff       (20)     1548 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/pyproject.toml
--rw-r--r--   0 alex       (501) staff       (20)       24 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/pytest.ini
--rw-r--r--   0 alex       (501) staff       (20)     1535 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/sample_setup.py
--rw-r--r--   0 alex       (501) staff       (20)      585 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/setup_extras.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.088256 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/tests/
--rw-r--r--   0 alex       (501) staff       (20)     1131 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/tests/test_get_next_version.py
--rw-r--r--   0 alex       (501) staff       (20)       19 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/variables.mk
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.091222 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/workflow-templates/
--rw-r--r--   0 alex       (501) staff       (20)     1781 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml
--rw-r--r--   0 alex       (501) staff       (20)      696 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/workflow-templates/publish_release.yml
--rw-r--r--   0 alex       (501) staff       (20)     1248 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/subtrees/z_quantum_actions/workflow-templates/style.yml
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.095114 orquestra-sdk-0.46.0/tests/
--rw-r--r--   0 alex       (501) staff       (20)      347 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.096611 orquestra-sdk-0.46.0/tests/cli/
--rw-r--r--   0 alex       (501) staff       (20)      204 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/cli/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.105806 orquestra-sdk-0.46.0/tests/cli/dorq/
--rw-r--r--   0 alex       (501) staff       (20)      204 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/cli/dorq/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.107169 orquestra-sdk-0.46.0/tests/cli/dorq/data/
--rw-r--r--   0 alex       (501) staff       (20)      427 2023-04-14 11:50:54.000000 orquestra-sdk-0.46.0/tests/cli/dorq/data/simulate_cli_logging_stuff.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.109275 orquestra-sdk-0.46.0/tests/cli/dorq/task/
--rw-r--r--   0 alex       (501) staff       (20)     6560 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/tests/cli/dorq/task/test_task_logs.py
--rw-r--r--   0 alex       (501) staff       (20)     8070 2023-04-03 14:17:03.000000 orquestra-sdk-0.46.0/tests/cli/dorq/task/test_task_results.py
--rw-r--r--   0 alex       (501) staff       (20)    32755 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/tests/cli/dorq/test_arg_resolvers.py
--rw-r--r--   0 alex       (501) staff       (20)     2263 2023-04-14 11:50:54.000000 orquestra-sdk-0.46.0/tests/cli/dorq/test_cli_logs.py
--rw-r--r--   0 alex       (501) staff       (20)     5747 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/tests/cli/dorq/test_dumpers.py
--rw-r--r--   0 alex       (501) staff       (20)     6149 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/tests/cli/dorq/test_entrypoint.py
--rw-r--r--   0 alex       (501) staff       (20)     6778 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/tests/cli/dorq/test_login.py
--rw-r--r--   0 alex       (501) staff       (20)     1879 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/tests/cli/dorq/test_login_server.py
--rw-r--r--   0 alex       (501) staff       (20)    48346 2023-04-03 14:17:03.000000 orquestra-sdk-0.46.0/tests/cli/dorq/test_repos.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.111083 orquestra-sdk-0.46.0/tests/cli/dorq/ui/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.905877 orquestra-sdk-0.46.0/tests/cli/dorq/ui/data/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.112728 orquestra-sdk-0.46.0/tests/cli/dorq/ui/data/wf_runs/
--rw-r--r--   0 alex       (501) staff       (20)      648 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/tests/cli/dorq/ui/data/wf_runs/running.txt
--rw-r--r--   0 alex       (501) staff       (20)      427 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/tests/cli/dorq/ui/data/wf_runs/waiting.txt
--rw-r--r--   0 alex       (501) staff       (20)     3845 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/tests/cli/dorq/ui/test_errors.py
--rw-r--r--   0 alex       (501) staff       (20)    14087 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/tests/cli/dorq/ui/test_presenters.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.118570 orquestra-sdk-0.46.0/tests/cli/dorq/workflow/
--rw-r--r--   0 alex       (501) staff       (20)     4138 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/tests/cli/dorq/workflow/test_list.py
--rw-r--r--   0 alex       (501) staff       (20)     5383 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/tests/cli/dorq/workflow/test_logs.py
--rw-r--r--   0 alex       (501) staff       (20)     6106 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/tests/cli/dorq/workflow/test_results.py
--rw-r--r--   0 alex       (501) staff       (20)     2793 2023-01-24 09:35:29.000000 orquestra-sdk-0.46.0/tests/cli/dorq/workflow/test_stop.py
--rw-r--r--   0 alex       (501) staff       (20)    12873 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/cli/dorq/workflow/test_submit.py
--rw-r--r--   0 alex       (501) staff       (20)     2417 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/tests/cli/dorq/workflow/test_view.py
--rw-r--r--   0 alex       (501) staff       (20)     2527 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/conftest.py
--rw-r--r--   0 alex       (501) staff       (20)      952 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/reloaders.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.123733 orquestra-sdk-0.46.0/tests/runtime/
--rw-r--r--   0 alex       (501) staff       (20)      261 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/runtime/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.126659 orquestra-sdk-0.46.0/tests/runtime/api/
--rw-r--r--   0 alex       (501) staff       (20)      393 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/runtime/api/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     9586 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/tests/runtime/api/test_api_with_qe.py
--rw-r--r--   0 alex       (501) staff       (20)     3766 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/tests/runtime/api/test_api_with_ray.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.128733 orquestra-sdk-0.46.0/tests/runtime/corq/
--rw-r--r--   0 alex       (501) staff       (20)      261 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/runtime/corq/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.908379 orquestra-sdk-0.46.0/tests/runtime/corq/data/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.129648 orquestra-sdk-0.46.0/tests/runtime/corq/data/cli_outputs/
--rw-r--r--   0 alex       (501) staff       (20)      958 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/runtime/corq/data/cli_outputs/failed_wf_run.txt
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.130618 orquestra-sdk-0.46.0/tests/runtime/corq/data/responses/
--rw-r--r--   0 alex       (501) staff       (20)     9676 2023-04-03 14:17:03.000000 orquestra-sdk-0.46.0/tests/runtime/corq/data/responses/failed_wf_run.json
--rw-r--r--   0 alex       (501) staff       (20)     6028 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/tests/runtime/corq/test_format.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.132837 orquestra-sdk-0.46.0/tests/runtime/db/
--rw-r--r--   0 alex       (501) staff       (20)     1599 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/tests/runtime/db/test_db.py
--rw-r--r--   0 alex       (501) staff       (20)     2865 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/tests/runtime/db/test_migration.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.135852 orquestra-sdk-0.46.0/tests/runtime/performance/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/runtime/performance/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1110 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/runtime/performance/conftest.py
--rw-r--r--   0 alex       (501) staff       (20)     3766 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/tests/runtime/performance/test_cli_perf.py
--rw-r--r--   0 alex       (501) staff       (20)      688 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/runtime/project_state.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.139365 orquestra-sdk-0.46.0/tests/runtime/qe/
--rw-r--r--   0 alex       (501) staff       (20)     2731 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/runtime/qe/test_qe_date_conversion.py
--rw-r--r--   0 alex       (501) staff       (20)    53913 2023-04-14 11:54:11.000000 orquestra-sdk-0.46.0/tests/runtime/qe/test_qe_runtime.py
--rw-r--r--   0 alex       (501) staff       (20)     1158 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/runtime/qe/test_response_parsers.py
--rw-r--r--   0 alex       (501) staff       (20)     4513 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/runtime/qe/test_tar_extraction.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.147049 orquestra-sdk-0.46.0/tests/runtime/ray/
--rw-r--r--   0 alex       (501) staff       (20)      261 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/runtime/ray/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      844 2023-01-24 09:35:29.000000 orquestra-sdk-0.46.0/tests/runtime/ray/conftest.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.911807 orquestra-sdk-0.46.0/tests/runtime/ray/data/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.148162 orquestra-sdk-0.46.0/tests/runtime/ray/data/ml_demo/
--rw-r--r--   0 alex       (501) staff       (20)      975 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/runtime/ray/data/ml_demo/workflow_defs.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.149204 orquestra-sdk-0.46.0/tests/runtime/ray/data/module_level_function/
--rw-r--r--   0 alex       (501) staff       (20)      602 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/runtime/ray/data/module_level_function/workflow_defs.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.150027 orquestra-sdk-0.46.0/tests/runtime/ray/data/passing_closures/
--rw-r--r--   0 alex       (501) staff       (20)     1286 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/runtime/ray/data/passing_closures/workflow_defs.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.151830 orquestra-sdk-0.46.0/tests/runtime/ray/data/python_package/
--rw-r--r--   0 alex       (501) staff       (20)      350 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/tests/runtime/ray/data/python_package/original_workflow.py
--rw-r--r--   0 alex       (501) staff       (20)     3974 2023-04-03 14:17:03.000000 orquestra-sdk-0.46.0/tests/runtime/ray/data/python_package/python_package_dependent_workflow.json
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.152917 orquestra-sdk-0.46.0/tests/runtime/ray/ray_logs/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.912554 orquestra-sdk-0.46.0/tests/runtime/ray/ray_logs/data/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.912810 orquestra-sdk-0.46.0/tests/runtime/ray/ray_logs/data/ray_temp/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:26.913127 orquestra-sdk-0.46.0/tests/runtime/ray/ray_logs/data/ray_temp/session_2023-02-09_12-23-55_156174_25782/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.158343 orquestra-sdk-0.46.0/tests/runtime/ray/ray_logs/data/ray_temp/session_2023-02-09_12-23-55_156174_25782/logs/
--rw-r--r--   0 alex       (501) staff       (20)     1770 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/tests/runtime/ray/ray_logs/data/ray_temp/session_2023-02-09_12-23-55_156174_25782/logs/worker1.err
--rw-r--r--   0 alex       (501) staff       (20)       36 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/tests/runtime/ray/ray_logs/data/ray_temp/session_2023-02-09_12-23-55_156174_25782/logs/worker1.out
--rw-r--r--   0 alex       (501) staff       (20)       20 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/tests/runtime/ray/ray_logs/data/ray_temp/session_2023-02-09_12-23-55_156174_25782/logs/worker2.err
--rw-r--r--   0 alex       (501) staff       (20)       20 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/tests/runtime/ray/ray_logs/data/ray_temp/session_2023-02-09_12-23-55_156174_25782/logs/worker2.out
--rw-r--r--   0 alex       (501) staff       (20)     4932 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/tests/runtime/ray/ray_logs/data/ray_temp/session_2023-02-09_12-23-55_156174_25782/logs/worker3.err
--rw-r--r--   0 alex       (501) staff       (20)       73 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/tests/runtime/ray/ray_logs/data/ray_temp/session_2023-02-09_12-23-55_156174_25782/logs/worker3.out
--rw-r--r--   0 alex       (501) staff       (20)    16259 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/tests/runtime/ray/ray_logs/test_ray_logs.py
--rw-r--r--   0 alex       (501) staff       (20)     2155 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/tests/runtime/ray/test_client.py
--rw-r--r--   0 alex       (501) staff       (20)    22378 2023-04-14 11:54:11.000000 orquestra-sdk-0.46.0/tests/runtime/ray/test_dag.py
--rw-r--r--   0 alex       (501) staff       (20)      466 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/runtime/ray/test_id_gen.py
--rw-r--r--   0 alex       (501) staff       (20)    30008 2023-04-14 11:54:11.000000 orquestra-sdk-0.46.0/tests/runtime/ray/test_integration.py
--rw-r--r--   0 alex       (501) staff       (20)     1515 2023-04-14 11:50:54.000000 orquestra-sdk-0.46.0/tests/runtime/ray/test_logger.py
--rw-r--r--   0 alex       (501) staff       (20)     2935 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/runtime/test_config.py
--rw-r--r--   0 alex       (501) staff       (20)     4759 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/tests/runtime/test_log_adapter.py
--rw-r--r--   0 alex       (501) staff       (20)     7645 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/tests/runtime/test_services.py
--rw-r--r--   0 alex       (501) staff       (20)      879 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/tests/runtime/test_services_integration.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.159192 orquestra-sdk-0.46.0/tests/sdk/
--rw-r--r--   0 alex       (501) staff       (20)      347 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.181011 orquestra-sdk-0.46.0/tests/sdk/v2/
--rw-r--r--   0 alex       (501) staff       (20)      347 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.184584 orquestra-sdk-0.46.0/tests/sdk/v2/api/
--rw-r--r--   0 alex       (501) staff       (20)      253 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/tests/sdk/v2/api/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    27632 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/tests/sdk/v2/api/test_config.py
--rw-r--r--   0 alex       (501) staff       (20)    17581 2023-04-03 14:17:03.000000 orquestra-sdk-0.46.0/tests/sdk/v2/api/test_task_run.py
--rw-r--r--   0 alex       (501) staff       (20)    25007 2023-04-14 11:54:11.000000 orquestra-sdk-0.46.0/tests/sdk/v2/api/test_wf_run.py
--rw-r--r--   0 alex       (501) staff       (20)     1341 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/tests/sdk/v2/conftest.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.188496 orquestra-sdk-0.46.0/tests/sdk/v2/conversions/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.202426 orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/
--rw-r--r--   0 alex       (501) staff       (20)     2796 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/additional-metrics.yml
--rw-r--r--   0 alex       (501) staff       (20)     1370 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/basics.yml
--rw-r--r--   0 alex       (501) staff       (20)     1370 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/basics_file_ref.yml
--rw-r--r--   0 alex       (501) staff       (20)     1506 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/basics_with_data_aggregation.yml
--rw-r--r--   0 alex       (501) staff       (20)     1394 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/basics_with_gpu.yml
--rw-r--r--   0 alex       (501) staff       (20)     1408 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/custom_json.yml
--rw-r--r--   0 alex       (501) staff       (20)     2636 2023-04-03 14:17:03.000000 orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/exportable_wf.yml
--rw-r--r--   0 alex       (501) staff       (20)     3075 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/inline_function.yml
--rw-r--r--   0 alex       (501) staff       (20)     1339 2023-04-03 14:17:03.000000 orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/main_test.json
--rw-r--r--   0 alex       (501) staff       (20)     1223 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/main_test.yml
--rw-r--r--   0 alex       (501) staff       (20)     2325 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/multi_task_outputs.yml
--rw-r--r--   0 alex       (501) staff       (20)     2651 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/multi_task_outputs_as_inputs.yml
--rw-r--r--   0 alex       (501) staff       (20)     1393 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/positional.yml
--rw-r--r--   0 alex       (501) staff       (20)     2474 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/positional_artifact.yml
--rw-r--r--   0 alex       (501) staff       (20)     1526 2023-02-14 13:55:21.000000 orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/python_import.yml
--rw-r--r--   0 alex       (501) staff       (20)     2876 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/conversions/test_ids.py
--rw-r--r--   0 alex       (501) staff       (20)     4858 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/tests/sdk/v2/conversions/test_imports.py
--rw-r--r--   0 alex       (501) staff       (20)    37666 2023-04-03 14:17:03.000000 orquestra-sdk-0.46.0/tests/sdk/v2/conversions/test_yaml_exporter.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.207490 orquestra-sdk-0.46.0/tests/sdk/v2/data/
--rw-r--r--   0 alex       (501) staff       (20)       42 2023-01-24 09:35:29.000000 orquestra-sdk-0.46.0/tests/sdk/v2/data/bad_requirements.txt
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.208699 orquestra-sdk-0.46.0/tests/sdk/v2/data/complex_serialization/
--rw-r--r--   0 alex       (501) staff       (20)     4055 2023-04-03 14:17:03.000000 orquestra-sdk-0.46.0/tests/sdk/v2/data/complex_serialization/workflow_defs.py
--rw-r--r--   0 alex       (501) staff       (20)     1415 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/tests/sdk/v2/data/configs.py
--rw-r--r--   0 alex       (501) staff       (20)       28 2023-01-24 09:35:29.000000 orquestra-sdk-0.46.0/tests/sdk/v2/data/requirements.txt
--rw-r--r--   0 alex       (501) staff       (20)       70 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/data/requirements_with_extras.txt
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.212078 orquestra-sdk-0.46.0/tests/sdk/v2/data/sample_project/
--rw-r--r--   0 alex       (501) staff       (20)      351 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/data/sample_project/helpers.py
--rw-r--r--   0 alex       (501) staff       (20)      487 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/data/sample_project/workflow_defs.py
--rw-r--r--   0 alex       (501) staff       (20)      531 2023-04-14 11:50:54.000000 orquestra-sdk-0.46.0/tests/sdk/v2/data/sample_project/workflow_defs_no_raise.py
--rw-r--r--   0 alex       (501) staff       (20)     1473 2023-04-03 14:17:03.000000 orquestra-sdk-0.46.0/tests/sdk/v2/data/task_run_workflow_defs.py
--rw-r--r--   0 alex       (501) staff       (20)      581 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/dirs.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.216368 orquestra-sdk-0.46.0/tests/sdk/v2/driver/
--rw-r--r--   0 alex       (501) staff       (20)      204 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/driver/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    12592 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/tests/sdk/v2/driver/resp_mocks.py
--rw-r--r--   0 alex       (501) staff       (20)    36588 2023-04-14 11:54:11.000000 orquestra-sdk-0.46.0/tests/sdk/v2/driver/test_ce_runtime.py
--rw-r--r--   0 alex       (501) staff       (20)    81008 2023-04-14 11:54:11.000000 orquestra-sdk-0.46.0/tests/sdk/v2/driver/test_client.py
--rw-r--r--   0 alex       (501) staff       (20)      806 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/tests/sdk/v2/project_state.py
--rw-r--r--   0 alex       (501) staff       (20)      712 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/sample_wfs.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.221891 orquestra-sdk-0.46.0/tests/sdk/v2/secrets/
--rw-r--r--   0 alex       (501) staff       (20)      204 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/secrets/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1632 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/secrets/resp_mocks.py
--rw-r--r--   0 alex       (501) staff       (20)     4394 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/tests/sdk/v2/secrets/test_api.py
--rw-r--r--   0 alex       (501) staff       (20)     4940 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/tests/sdk/v2/secrets/test_auth.py
--rw-r--r--   0 alex       (501) staff       (20)    13976 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/secrets/test_client.py
--rw-r--r--   0 alex       (501) staff       (20)     1528 2023-03-31 10:01:21.000000 orquestra-sdk-0.46.0/tests/sdk/v2/secrets/test_importing.py
--rw-r--r--   0 alex       (501) staff       (20)     4490 2023-04-03 14:17:03.000000 orquestra-sdk-0.46.0/tests/sdk/v2/test_api_tutorial_scripts.py
--rw-r--r--   0 alex       (501) staff       (20)    12819 2023-04-03 14:17:04.000000 orquestra-sdk-0.46.0/tests/sdk/v2/test_artifact_future_methods.py
--rw-r--r--   0 alex       (501) staff       (20)     7130 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/tests/sdk/v2/test_ast.py
--rw-r--r--   0 alex       (501) staff       (20)    16553 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/tests/sdk/v2/test_config.py
--rw-r--r--   0 alex       (501) staff       (20)      775 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/test_constant_nodes_serialization.py
--rw-r--r--   0 alex       (501) staff       (20)    20866 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/tests/sdk/v2/test_dispatch.py
--rw-r--r--   0 alex       (501) staff       (20)     6413 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/tests/sdk/v2/test_dispatch_integration.py
--rw-r--r--   0 alex       (501) staff       (20)    22084 2023-04-14 11:50:54.000000 orquestra-sdk-0.46.0/tests/sdk/v2/test_dsl.py
--rw-r--r--   0 alex       (501) staff       (20)     1135 2023-04-14 11:50:54.000000 orquestra-sdk-0.46.0/tests/sdk/v2/test_env.py
--rw-r--r--   0 alex       (501) staff       (20)     6590 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/tests/sdk/v2/test_git_url_utils.py
--rw-r--r--   0 alex       (501) staff       (20)     1635 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/test_graphs.py
--rw-r--r--   0 alex       (501) staff       (20)     7032 2023-04-14 11:54:11.000000 orquestra-sdk-0.46.0/tests/sdk/v2/test_in_process_runtime.py
--rw-r--r--   0 alex       (501) staff       (20)     3815 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/test_loader.py
--rw-r--r--   0 alex       (501) staff       (20)     4949 2023-04-14 11:50:54.000000 orquestra-sdk-0.46.0/tests/sdk/v2/test_packaging.py
--rw-r--r--   0 alex       (501) staff       (20)     4359 2023-03-09 14:40:28.000000 orquestra-sdk-0.46.0/tests/sdk/v2/test_serde.py
--rw-r--r--   0 alex       (501) staff       (20)     9718 2023-04-03 14:17:04.000000 orquestra-sdk-0.46.0/tests/sdk/v2/test_task_ast_parsing.py
--rw-r--r--   0 alex       (501) staff       (20)    35378 2023-04-03 14:17:04.000000 orquestra-sdk-0.46.0/tests/sdk/v2/test_traversal.py
--rw-r--r--   0 alex       (501) staff       (20)     2607 2023-04-03 14:17:03.000000 orquestra-sdk-0.46.0/tests/sdk/v2/test_viz.py
--rw-r--r--   0 alex       (501) staff       (20)    10858 2023-04-14 11:50:54.000000 orquestra-sdk-0.46.0/tests/sdk/v2/test_workflow.py
--rw-r--r--   0 alex       (501) staff       (20)     1632 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/test_workflow_ast_parsing.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.224297 orquestra-sdk-0.46.0/tests/sdk/v2/typing/
--rw-r--r--   0 alex       (501) staff       (20)     1272 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/typing/full_example.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.231869 orquestra-sdk-0.46.0/tests/sdk/v2/typing/task/
--rw-r--r--   0 alex       (501) staff       (20)      252 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/typing/task/assign_n_outputs.py
--rw-r--r--   0 alex       (501) staff       (20)      248 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/typing/task/has_n_outputs.py
--rw-r--r--   0 alex       (501) staff       (20)      241 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/typing/task/passed_correct_arg_type.py
--rw-r--r--   0 alex       (501) staff       (20)      247 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/typing/task/passed_keyword_as_positional.py
--rw-r--r--   0 alex       (501) staff       (20)      240 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/typing/task/passed_too_few_args.py
--rw-r--r--   0 alex       (501) staff       (20)      247 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/typing/task/passed_too_many_args.py
--rw-r--r--   0 alex       (501) staff       (20)      243 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/typing/task/passed_wrong_arg_type.py
--rw-r--r--   0 alex       (501) staff       (20)      338 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/typing/task/task_base.py
--rw-r--r--   0 alex       (501) staff       (20)     3659 2023-04-03 14:17:04.000000 orquestra-sdk-0.46.0/tests/sdk/v2/typing/test_typing.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.236966 orquestra-sdk-0.46.0/tests/sdk/v2/typing/workflow/
--rw-r--r--   0 alex       (501) staff       (20)      592 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/typing/workflow/assign_model.py
--rw-r--r--   0 alex       (501) staff       (20)      249 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/typing/workflow/does_not_have_validate.py
--rw-r--r--   0 alex       (501) staff       (20)      252 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/typing/workflow/has_local_run.py
--rw-r--r--   0 alex       (501) staff       (20)      244 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/typing/workflow/has_model.py
--rw-r--r--   0 alex       (501) staff       (20)      272 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/sdk/v2/typing/workflow/workflow_base.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 11:54:27.238618 orquestra-sdk-0.46.0/tests/workflow/
--rw-r--r--   0 alex       (501) staff       (20)      994 2023-01-11 15:05:45.000000 orquestra-sdk-0.46.0/tests/workflow/test_generating_schema.py
--rw-r--r--   0 alex       (501) staff       (20)     2274 2023-04-03 14:17:03.000000 orquestra-sdk-0.46.0/tests/workflow/test_serde.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.759167 orquestra-sdk-0.47.0/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.667468 orquestra-sdk-0.47.0/.github/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.667851 orquestra-sdk-0.47.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 james      (501) wheel        (0)      605 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 james      (501) wheel        (0)      600 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 james      (501) wheel        (0)      766 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/.github/pull_request_template.md
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.668666 orquestra-sdk-0.47.0/.github/workflows/
+-rw-r--r--   0 james      (501) wheel        (0)     1734 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/.github/workflows/coverage.yml
+-rw-r--r--   0 james      (501) wheel        (0)      939 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/.github/workflows/performance.yml
+-rw-r--r--   0 james      (501) wheel        (0)     2814 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/.github/workflows/publish_release.yml
+-rw-r--r--   0 james      (501) wheel        (0)     1212 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/.github/workflows/style.yml
+-rw-r--r--   0 james      (501) wheel        (0)      776 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/.github/workflows/typing.yml
+-rw-r--r--   0 james      (501) wheel        (0)     1836 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/.gitignore
+-rw-r--r--   0 james      (501) wheel        (0)    13396 2023-04-28 13:26:39.000000 orquestra-sdk-0.47.0/CHANGELOG.md
+-rw-r--r--   0 james      (501) wheel        (0)      241 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/CODEOWNERS
+-rw-r--r--   0 james      (501) wheel        (0)     3839 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/CONTRIBUTING.md
+-rw-r--r--   0 james      (501) wheel        (0)    11358 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/LICENSE
+-rw-r--r--   0 james      (501) wheel        (0)        9 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/MANIFEST.in
+-rw-r--r--   0 james      (501) wheel        (0)     3661 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/Makefile
+-rw-r--r--   0 james      (501) wheel        (0)     1654 2023-04-28 13:27:42.759297 orquestra-sdk-0.47.0/PKG-INFO
+-rw-r--r--   0 james      (501) wheel        (0)     1009 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/README.md
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.668889 orquestra-sdk-0.47.0/docs/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.669667 orquestra-sdk-0.47.0/docs/examples/
+-rw-r--r--   0 james      (501) wheel        (0)      204 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/examples/__init__.py
+-rw-r--r--   0 james      (501) wheel        (0)      835 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/examples/config_management.py
+-rw-r--r--   0 james      (501) wheel        (0)     1174 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/examples/quickstart.py
+-rw-r--r--   0 james      (501) wheel        (0)      488 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/examples/remote_workflow.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.670953 orquestra-sdk-0.47.0/docs/examples/tests/
+-rw-r--r--   0 james      (501) wheel        (0)      260 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/examples/tests/__init__.py
+-rw-r--r--   0 james      (501) wheel        (0)      836 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/examples/tests/conftest.py
+-rw-r--r--   0 james      (501) wheel        (0)      989 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/examples/tests/parsers.py
+-rw-r--r--   0 james      (501) wheel        (0)     3710 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/examples/tests/test_local_ray.py
+-rw-r--r--   0 james      (501) wheel        (0)     1966 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/examples/tests/test_logging.py
+-rw-r--r--   0 james      (501) wheel        (0)     5077 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/examples/tests/test_parametrized_workflows.py
+-rw-r--r--   0 james      (501) wheel        (0)     6395 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/examples/tests/test_remote.py
+-rw-r--r--   0 james      (501) wheel        (0)     5509 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/examples/tests/test_secrets.py
+-rw-r--r--   0 james      (501) wheel        (0)    13856 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/examples/tests/test_workflow_syntax.py
+-rw-r--r--   0 james      (501) wheel        (0)      505 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/examples/workflow_defs.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.672074 orquestra-sdk-0.47.0/docs/guides/
+-rw-r--r--   0 james      (501) wheel        (0)     9090 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/guides/dependency-installation.rst
+-rw-r--r--   0 james      (501) wheel        (0)      207 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/guides/index.rst
+-rw-r--r--   0 james      (501) wheel        (0)     1305 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/guides/logging.rst
+-rw-r--r--   0 james      (501) wheel        (0)     6713 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/guides/resource-management.rst
+-rw-r--r--   0 james      (501) wheel        (0)     2066 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/guides/runtime-configuration.rst
+-rw-r--r--   0 james      (501) wheel        (0)     2909 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/guides/version-compatibility.rst
+-rw-r--r--   0 james      (501) wheel        (0)     5060 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/guides/workflow-runs.rst
+-rw-r--r--   0 james      (501) wheel        (0)     5901 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/guides/workflow-syntax.rst
+-rw-r--r--   0 james      (501) wheel        (0)      834 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/index.rst
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.672360 orquestra-sdk-0.47.0/docs/quickref/
+-rw-r--r--   0 james      (501) wheel        (0)      247 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/quickref/cli-reference.rst
+-rw-r--r--   0 james      (501) wheel        (0)       89 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/quickref/index.rst
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.673637 orquestra-sdk-0.47.0/docs/tutorials/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.674457 orquestra-sdk-0.47.0/docs/tutorials/images/
+-rw-r--r--   0 james      (501) wheel        (0)   235665 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/tutorials/images/orq-login-copy-token.png
+-rw-r--r--   0 james      (501) wheel        (0)   104197 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/tutorials/images/orq-login-grant-access.png
+-rw-r--r--   0 james      (501) wheel        (0)   110685 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/tutorials/images/orq-login-landing-page.png
+-rw-r--r--   0 james      (501) wheel        (0)     5286 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/tutorials/images/win-redist-picture.png
+-rw-r--r--   0 james      (501) wheel        (0)      400 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/tutorials/index.rst
+-rw-r--r--   0 james      (501) wheel        (0)     2743 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/tutorials/installing-macos-linux.rst
+-rw-r--r--   0 james      (501) wheel        (0)     3947 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/tutorials/installing-windows.rst
+-rw-r--r--   0 james      (501) wheel        (0)     5224 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/tutorials/jupyter-sdk.rst
+-rw-r--r--   0 james      (501) wheel        (0)     2385 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/tutorials/parametrized-workflows.rst
+-rw-r--r--   0 james      (501) wheel        (0)     1476 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/tutorials/quickstart.rst
+-rw-r--r--   0 james      (501) wheel        (0)     1760 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/tutorials/ray.rst
+-rw-r--r--   0 james      (501) wheel        (0)     3232 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/tutorials/remote.rst
+-rw-r--r--   0 james      (501) wheel        (0)     2438 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/docs/tutorials/secrets.rst
+-rw-r--r--   0 james      (501) wheel        (0)     1996 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/pyproject.toml
+-rw-r--r--   0 james      (501) wheel        (0)      193 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/pytest.ini
+-rw-r--r--   0 james      (501) wheel        (0)     1475 2023-04-28 13:27:42.759721 orquestra-sdk-0.47.0/setup.cfg
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.656872 orquestra-sdk-0.47.0/src/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.655169 orquestra-sdk-0.47.0/src/orquestra/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.674881 orquestra-sdk-0.47.0/src/orquestra/sdk/
+-rw-r--r--   0 james      (501) wheel        (0)     1270 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/__init__.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.678262 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/
+-rw-r--r--   0 james      (501) wheel        (0)      204 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/__init__.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.678935 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_api/
+-rw-r--r--   0 james      (501) wheel        (0)      624 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_api/__init__.py
+-rw-r--r--   0 james      (501) wheel        (0)    24790 2023-04-28 13:26:39.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_api/_config.py
+-rw-r--r--   0 james      (501) wheel        (0)     9505 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_api/_task_run.py
+-rw-r--r--   0 james      (501) wheel        (0)    21600 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_api/_wf_run.py
+-rw-r--r--   0 james      (501) wheel        (0)     8563 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_ast.py
+-rw-r--r--   0 james      (501) wheel        (0)    24930 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_config.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.679758 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_conversions/
+-rw-r--r--   0 james      (501) wheel        (0)      204 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_conversions/__init__.py
+-rw-r--r--   0 james      (501) wheel        (0)     3509 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_conversions/_ids.py
+-rw-r--r--   0 james      (501) wheel        (0)     7074 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_conversions/_imports.py
+-rw-r--r--   0 james      (501) wheel        (0)    12944 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_conversions/_invocations.py
+-rw-r--r--   0 james      (501) wheel        (0)     3905 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_conversions/_yaml_exporter.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.680200 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_db/
+-rw-r--r--   0 james      (501) wheel        (0)      288 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_db/__init__.py
+-rw-r--r--   0 james      (501) wheel        (0)     5107 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_db/_db.py
+-rw-r--r--   0 james      (501) wheel        (0)      894 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_db/_migration.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.680999 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_driver/
+-rw-r--r--   0 james      (501) wheel        (0)      204 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_driver/__init__.py
+-rw-r--r--   0 james      (501) wheel        (0)    18368 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_driver/_ce_runtime.py
+-rw-r--r--   0 james      (501) wheel        (0)    23277 2023-04-28 13:26:39.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_driver/_client.py
+-rw-r--r--   0 james      (501) wheel        (0)     4563 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_driver/_exceptions.py
+-rw-r--r--   0 james      (501) wheel        (0)     8104 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_driver/_models.py
+-rw-r--r--   0 james      (501) wheel        (0)    36433 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_dsl.py
+-rw-r--r--   0 james      (501) wheel        (0)     1999 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_env.py
+-rw-r--r--   0 james      (501) wheel        (0)     2338 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_exec_ctx.py
+-rw-r--r--   0 james      (501) wheel        (0)     1776 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_factory.py
+-rw-r--r--   0 james      (501) wheel        (0)     3433 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_git_url_utils.py
+-rw-r--r--   0 james      (501) wheel        (0)     3021 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_graphs.py
+-rw-r--r--   0 james      (501) wheel        (0)    11245 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_in_process_runtime.py
+-rw-r--r--   0 james      (501) wheel        (0)     6460 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_log_adapter.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.681412 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_qe/
+-rw-r--r--   0 james      (501) wheel        (0)      204 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_qe/__init__.py
+-rw-r--r--   0 james      (501) wheel        (0)     7213 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_qe/_client.py
+-rw-r--r--   0 james      (501) wheel        (0)    34072 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_qe/_qe_runtime.py
+-rw-r--r--   0 james      (501) wheel        (0)     1407 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_retry.py
+-rw-r--r--   0 james      (501) wheel        (0)     4331 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_services.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.681990 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_testing/
+-rw-r--r--   0 james      (501) wheel        (0)      204 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_testing/__init__.py
+-rw-r--r--   0 james      (501) wheel        (0)     4031 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_testing/_connections.py
+-rw-r--r--   0 james      (501) wheel        (0)     7009 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_testing/_example_wfs.py
+-rw-r--r--   0 james      (501) wheel        (0)      261 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_testing/_long_import.py
+-rw-r--r--   0 james      (501) wheel        (0)    32145 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_traversal.py
+-rw-r--r--   0 james      (501) wheel        (0)     4629 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_viz.py
+-rw-r--r--   0 james      (501) wheel        (0)    26694 2023-04-28 13:26:39.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_workflow.py
+-rw-r--r--   0 james      (501) wheel        (0)     8381 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/abc.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.655830 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.682696 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/
+-rw-r--r--   0 james      (501) wheel        (0)    12294 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_arg_resolvers.py
+-rw-r--r--   0 james      (501) wheel        (0)      698 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_cli_logs.py
+-rw-r--r--   0 james      (501) wheel        (0)     3032 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_dumpers.py
+-rw-r--r--   0 james      (501) wheel        (0)     9871 2023-04-28 13:26:39.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_entry.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.683091 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_login/
+-rw-r--r--   0 james      (501) wheel        (0)     3043 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_login/_login.py
+-rw-r--r--   0 james      (501) wheel        (0)     1489 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_login/_login_server.py
+-rw-r--r--   0 james      (501) wheel        (0)    21340 2023-04-28 13:26:39.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_repos.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.683615 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_services/
+-rw-r--r--   0 james      (501) wheel        (0)     1621 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_services/_down.py
+-rw-r--r--   0 james      (501) wheel        (0)     1327 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_services/_status.py
+-rw-r--r--   0 james      (501) wheel        (0)     2135 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_services/_up.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.683923 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_task/
+-rw-r--r--   0 james      (501) wheel        (0)     3106 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_task/_logs.py
+-rw-r--r--   0 james      (501) wheel        (0)     3627 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_task/_results.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.684655 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_ui/
+-rw-r--r--   0 james      (501) wheel        (0)      367 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_ui/__init__.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.684950 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_corq_format/
+-rw-r--r--   0 james      (501) wheel        (0)      624 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_corq_format/color.py
+-rw-r--r--   0 james      (501) wheel        (0)     7794 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_corq_format/per_command.py
+-rw-r--r--   0 james      (501) wheel        (0)     4107 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_errors.py
+-rw-r--r--   0 james      (501) wheel        (0)     1648 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_models.py
+-rw-r--r--   0 james      (501) wheel        (0)    10300 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_presenters.py
+-rw-r--r--   0 james      (501) wheel        (0)     8309 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_prompts.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.685843 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/
+-rw-r--r--   0 james      (501) wheel        (0)     3486 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_list.py
+-rw-r--r--   0 james      (501) wheel        (0)     2739 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_logs.py
+-rw-r--r--   0 james      (501) wheel        (0)     3140 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_results.py
+-rw-r--r--   0 james      (501) wheel        (0)     2507 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_stop.py
+-rw-r--r--   0 james      (501) wheel        (0)     3993 2023-04-28 13:26:39.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_submit.py
+-rw-r--r--   0 james      (501) wheel        (0)     2138 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_view.py
+-rw-r--r--   0 james      (501) wheel        (0)    11810 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/dispatch.py
+-rw-r--r--   0 james      (501) wheel        (0)     6001 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/loader.py
+-rw-r--r--   0 james      (501) wheel        (0)     7004 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_base/serde.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.687013 orquestra-sdk-0.47.0/src/orquestra/sdk/_ray/
+-rw-r--r--   0 james      (501) wheel        (0)      204 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_ray/__init__.py
+-rw-r--r--   0 james      (501) wheel        (0)    15792 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_ray/_build_workflow.py
+-rw-r--r--   0 james      (501) wheel        (0)     6498 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_ray/_client.py
+-rw-r--r--   0 james      (501) wheel        (0)    20523 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_ray/_dag.py
+-rw-r--r--   0 james      (501) wheel        (0)      867 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_ray/_id_gen.py
+-rw-r--r--   0 james      (501) wheel        (0)     4389 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_ray/_ray_logs.py
+-rw-r--r--   0 james      (501) wheel        (0)     1278 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/_ray/_wf_metadata.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.687480 orquestra-sdk-0.47.0/src/orquestra/sdk/examples/
+-rw-r--r--   0 james      (501) wheel        (0)      204 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/examples/__init__.py
+-rw-r--r--   0 james      (501) wheel        (0)     1558 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/examples/exportable_wf.py
+-rw-r--r--   0 james      (501) wheel        (0)     1116 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/examples/workflow_defs.py
+-rw-r--r--   0 james      (501) wheel        (0)     3982 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/exceptions.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.687773 orquestra-sdk-0.47.0/src/orquestra/sdk/kubernetes/
+-rw-r--r--   0 james      (501) wheel        (0)      113 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/kubernetes/__init__.py
+-rw-r--r--   0 james      (501) wheel        (0)     2420 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/kubernetes/quantity.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.688045 orquestra-sdk-0.47.0/src/orquestra/sdk/packaging/
+-rw-r--r--   0 james      (501) wheel        (0)      427 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/packaging/__init__.py
+-rw-r--r--   0 james      (501) wheel        (0)     4084 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/packaging/_versions.py
+-rw-r--r--   0 james      (501) wheel        (0)        0 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/py.typed
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.689260 orquestra-sdk-0.47.0/src/orquestra/sdk/schema/
+-rw-r--r--   0 james      (501) wheel        (0)      204 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/schema/__init__.py
+-rw-r--r--   0 james      (501) wheel        (0)     1874 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/schema/_compat.py
+-rw-r--r--   0 james      (501) wheel        (0)     1474 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/schema/configs.py
+-rw-r--r--   0 james      (501) wheel        (0)    14980 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/schema/ir.py
+-rw-r--r--   0 james      (501) wheel        (0)      832 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/schema/local_database.py
+-rw-r--r--   0 james      (501) wheel        (0)     4745 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/schema/responses.py
+-rw-r--r--   0 james      (501) wheel        (0)     1565 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/schema/workflow_run.py
+-rw-r--r--   0 james      (501) wheel        (0)     4114 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/schema/yaml_model.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.690238 orquestra-sdk-0.47.0/src/orquestra/sdk/secrets/
+-rw-r--r--   0 james      (501) wheel        (0)     1104 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/secrets/__init__.py
+-rw-r--r--   0 james      (501) wheel        (0)     5356 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/secrets/_api.py
+-rw-r--r--   0 james      (501) wheel        (0)     2090 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/secrets/_auth.py
+-rw-r--r--   0 james      (501) wheel        (0)     5243 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/secrets/_client.py
+-rw-r--r--   0 james      (501) wheel        (0)     1222 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/secrets/_exceptions.py
+-rw-r--r--   0 james      (501) wheel        (0)     1319 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/secrets/_models.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.690413 orquestra-sdk-0.47.0/src/orquestra/sdk/v2/
+-rw-r--r--   0 james      (501) wheel        (0)     1072 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/src/orquestra/sdk/v2/__init__.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.691329 orquestra-sdk-0.47.0/src/orquestra_sdk.egg-info/
+-rw-r--r--   0 james      (501) wheel        (0)     1654 2023-04-28 13:27:42.000000 orquestra-sdk-0.47.0/src/orquestra_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) wheel        (0)    50318 2023-04-28 13:27:42.000000 orquestra-sdk-0.47.0/src/orquestra_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:27:42.000000 orquestra-sdk-0.47.0/src/orquestra_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) wheel        (0)       66 2023-04-28 13:27:42.000000 orquestra-sdk-0.47.0/src/orquestra_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:27:42.000000 orquestra-sdk-0.47.0/src/orquestra_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 james      (501) wheel        (0)      541 2023-04-28 13:27:42.000000 orquestra-sdk-0.47.0/src/orquestra_sdk.egg-info/requires.txt
+-rw-r--r--   0 james      (501) wheel        (0)       10 2023-04-28 13:27:42.000000 orquestra-sdk-0.47.0/src/orquestra_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.656994 orquestra-sdk-0.47.0/subtrees/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.692325 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/
+-rw-r--r--   0 james      (501) wheel        (0)        9 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/MANIFEST.in
+-rw-r--r--   0 james      (501) wheel        (0)     4535 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/Makefile
+-rw-r--r--   0 james      (501) wheel        (0)     5600 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/README.rst
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.657257 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/actions/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.692467 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/actions/publish-release/
+-rw-r--r--   0 james      (501) wheel        (0)     3132 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/actions/publish-release/action.yml
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.692604 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/actions/ssh_setup/
+-rw-r--r--   0 james      (501) wheel        (0)      458 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/actions/ssh_setup/action.yml
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.692730 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/actions/style/
+-rw-r--r--   0 james      (501) wheel        (0)      467 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/actions/style/action.yml
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.692876 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/bin/
+-rwxr-xr-x   0 james      (501) wheel        (0)     2756 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/bin/get_next_version.py
+-rw-r--r--   0 james      (501) wheel        (0)     1548 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/pyproject.toml
+-rw-r--r--   0 james      (501) wheel        (0)       24 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/pytest.ini
+-rw-r--r--   0 james      (501) wheel        (0)     1535 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/sample_setup.py
+-rw-r--r--   0 james      (501) wheel        (0)      585 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/setup_extras.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.693045 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/tests/
+-rw-r--r--   0 james      (501) wheel        (0)     1131 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/tests/test_get_next_version.py
+-rw-r--r--   0 james      (501) wheel        (0)       19 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/variables.mk
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.693436 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/workflow-templates/
+-rw-r--r--   0 james      (501) wheel        (0)     1781 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml
+-rw-r--r--   0 james      (501) wheel        (0)      696 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/workflow-templates/publish_release.yml
+-rw-r--r--   0 james      (501) wheel        (0)     1248 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/subtrees/z_quantum_actions/workflow-templates/style.yml
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.693811 orquestra-sdk-0.47.0/tests/
+-rw-r--r--   0 james      (501) wheel        (0)      347 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/__init__.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.693931 orquestra-sdk-0.47.0/tests/cli/
+-rw-r--r--   0 james      (501) wheel        (0)      204 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/cli/__init__.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.694938 orquestra-sdk-0.47.0/tests/cli/dorq/
+-rw-r--r--   0 james      (501) wheel        (0)      204 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/cli/dorq/__init__.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.695100 orquestra-sdk-0.47.0/tests/cli/dorq/data/
+-rw-r--r--   0 james      (501) wheel        (0)      427 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/cli/dorq/data/simulate_cli_logging_stuff.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.695360 orquestra-sdk-0.47.0/tests/cli/dorq/task/
+-rw-r--r--   0 james      (501) wheel        (0)     6560 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/cli/dorq/task/test_task_logs.py
+-rw-r--r--   0 james      (501) wheel        (0)     8086 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/cli/dorq/task/test_task_results.py
+-rw-r--r--   0 james      (501) wheel        (0)    32755 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/cli/dorq/test_arg_resolvers.py
+-rw-r--r--   0 james      (501) wheel        (0)     2263 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/cli/dorq/test_cli_logs.py
+-rw-r--r--   0 james      (501) wheel        (0)     5747 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/cli/dorq/test_dumpers.py
+-rw-r--r--   0 james      (501) wheel        (0)     6149 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/cli/dorq/test_entrypoint.py
+-rw-r--r--   0 james      (501) wheel        (0)     6778 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/cli/dorq/test_login.py
+-rw-r--r--   0 james      (501) wheel        (0)     1879 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/cli/dorq/test_login_server.py
+-rw-r--r--   0 james      (501) wheel        (0)    51591 2023-04-28 13:26:39.000000 orquestra-sdk-0.47.0/tests/cli/dorq/test_repos.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.695607 orquestra-sdk-0.47.0/tests/cli/dorq/ui/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.658255 orquestra-sdk-0.47.0/tests/cli/dorq/ui/data/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.695865 orquestra-sdk-0.47.0/tests/cli/dorq/ui/data/wf_runs/
+-rw-r--r--   0 james      (501) wheel        (0)      648 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/cli/dorq/ui/data/wf_runs/running.txt
+-rw-r--r--   0 james      (501) wheel        (0)      427 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/cli/dorq/ui/data/wf_runs/waiting.txt
+-rw-r--r--   0 james      (501) wheel        (0)     3845 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/cli/dorq/ui/test_errors.py
+-rw-r--r--   0 james      (501) wheel        (0)    14087 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/cli/dorq/ui/test_presenters.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.696605 orquestra-sdk-0.47.0/tests/cli/dorq/workflow/
+-rw-r--r--   0 james      (501) wheel        (0)     4138 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/cli/dorq/workflow/test_list.py
+-rw-r--r--   0 james      (501) wheel        (0)     5383 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/cli/dorq/workflow/test_logs.py
+-rw-r--r--   0 james      (501) wheel        (0)     6106 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/cli/dorq/workflow/test_results.py
+-rw-r--r--   0 james      (501) wheel        (0)     2793 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/cli/dorq/workflow/test_stop.py
+-rw-r--r--   0 james      (501) wheel        (0)    12873 2023-04-28 13:26:39.000000 orquestra-sdk-0.47.0/tests/cli/dorq/workflow/test_submit.py
+-rw-r--r--   0 james      (501) wheel        (0)     2417 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/cli/dorq/workflow/test_view.py
+-rw-r--r--   0 james      (501) wheel        (0)     2527 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/conftest.py
+-rw-r--r--   0 james      (501) wheel        (0)      952 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/reloaders.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.697354 orquestra-sdk-0.47.0/tests/runtime/
+-rw-r--r--   0 james      (501) wheel        (0)      261 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/__init__.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.697786 orquestra-sdk-0.47.0/tests/runtime/api/
+-rw-r--r--   0 james      (501) wheel        (0)      393 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/api/__init__.py
+-rw-r--r--   0 james      (501) wheel        (0)     9586 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/api/test_api_with_qe.py
+-rw-r--r--   0 james      (501) wheel        (0)     3766 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/api/test_api_with_ray.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.698048 orquestra-sdk-0.47.0/tests/runtime/corq/
+-rw-r--r--   0 james      (501) wheel        (0)      261 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/corq/__init__.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.658740 orquestra-sdk-0.47.0/tests/runtime/corq/data/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.698174 orquestra-sdk-0.47.0/tests/runtime/corq/data/cli_outputs/
+-rw-r--r--   0 james      (501) wheel        (0)      958 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/corq/data/cli_outputs/failed_wf_run.txt
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.698302 orquestra-sdk-0.47.0/tests/runtime/corq/data/responses/
+-rw-r--r--   0 james      (501) wheel        (0)    10015 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/corq/data/responses/failed_wf_run.json
+-rw-r--r--   0 james      (501) wheel        (0)     6116 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/corq/test_format.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.698583 orquestra-sdk-0.47.0/tests/runtime/db/
+-rw-r--r--   0 james      (501) wheel        (0)     1599 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/db/test_db.py
+-rw-r--r--   0 james      (501) wheel        (0)     2865 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/db/test_migration.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.698958 orquestra-sdk-0.47.0/tests/runtime/performance/
+-rw-r--r--   0 james      (501) wheel        (0)        0 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/performance/__init__.py
+-rw-r--r--   0 james      (501) wheel        (0)     1110 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/performance/conftest.py
+-rw-r--r--   0 james      (501) wheel        (0)     3766 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/performance/test_cli_perf.py
+-rw-r--r--   0 james      (501) wheel        (0)      688 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/project_state.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.699522 orquestra-sdk-0.47.0/tests/runtime/qe/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.699649 orquestra-sdk-0.47.0/tests/runtime/qe/regression/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.699779 orquestra-sdk-0.47.0/tests/runtime/qe/regression/data/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.700051 orquestra-sdk-0.47.0/tests/runtime/qe/regression/data/0.46.0/
+-rw-r--r--   0 james      (501) wheel        (0)     1309 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/qe/regression/data/0.46.0/get_artifact_responses.json
+-rw-r--r--   0 james      (501) wheel        (0)    10917 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/qe/regression/data/0.46.0/workflow_def.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.700353 orquestra-sdk-0.47.0/tests/runtime/qe/regression/data/0.47.0/
+-rw-r--r--   0 james      (501) wheel        (0)     1321 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/qe/regression/data/0.47.0/get_artifact_responses.json
+-rw-r--r--   0 james      (501) wheel        (0)    10592 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/qe/regression/data/0.47.0/workflow_def.json
+-rw-r--r--   0 james      (501) wheel        (0)      479 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/qe/regression/data/workflow.py
+-rw-r--r--   0 james      (501) wheel        (0)     3662 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/qe/regression/test_regression.py
+-rw-r--r--   0 james      (501) wheel        (0)     2731 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/qe/test_qe_date_conversion.py
+-rw-r--r--   0 james      (501) wheel        (0)    55208 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/qe/test_qe_runtime.py
+-rw-r--r--   0 james      (501) wheel        (0)     1158 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/qe/test_response_parsers.py
+-rw-r--r--   0 james      (501) wheel        (0)     4513 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/qe/test_tar_extraction.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.701443 orquestra-sdk-0.47.0/tests/runtime/ray/
+-rw-r--r--   0 james      (501) wheel        (0)      261 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/__init__.py
+-rw-r--r--   0 james      (501) wheel        (0)      844 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/conftest.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.659675 orquestra-sdk-0.47.0/tests/runtime/ray/data/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.701573 orquestra-sdk-0.47.0/tests/runtime/ray/data/ml_demo/
+-rw-r--r--   0 james      (501) wheel        (0)      975 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/data/ml_demo/workflow_defs.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.701717 orquestra-sdk-0.47.0/tests/runtime/ray/data/module_level_function/
+-rw-r--r--   0 james      (501) wheel        (0)      602 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/data/module_level_function/workflow_defs.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.701846 orquestra-sdk-0.47.0/tests/runtime/ray/data/passing_closures/
+-rw-r--r--   0 james      (501) wheel        (0)     1286 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/data/passing_closures/workflow_defs.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.702113 orquestra-sdk-0.47.0/tests/runtime/ray/data/python_package/
+-rw-r--r--   0 james      (501) wheel        (0)      358 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/data/python_package/original_workflow.py
+-rw-r--r--   0 james      (501) wheel        (0)     4314 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/data/python_package/python_package_dependent_workflow.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.702261 orquestra-sdk-0.47.0/tests/runtime/ray/ray_logs/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.659870 orquestra-sdk-0.47.0/tests/runtime/ray/ray_logs/data/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.659958 orquestra-sdk-0.47.0/tests/runtime/ray/ray_logs/data/ray_temp/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.660010 orquestra-sdk-0.47.0/tests/runtime/ray/ray_logs/data/ray_temp/session_2023-02-09_12-23-55_156174_25782/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.703135 orquestra-sdk-0.47.0/tests/runtime/ray/ray_logs/data/ray_temp/session_2023-02-09_12-23-55_156174_25782/logs/
+-rw-r--r--   0 james      (501) wheel        (0)     1770 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/ray_logs/data/ray_temp/session_2023-02-09_12-23-55_156174_25782/logs/worker1.err
+-rw-r--r--   0 james      (501) wheel        (0)       36 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/ray_logs/data/ray_temp/session_2023-02-09_12-23-55_156174_25782/logs/worker1.out
+-rw-r--r--   0 james      (501) wheel        (0)       20 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/ray_logs/data/ray_temp/session_2023-02-09_12-23-55_156174_25782/logs/worker2.err
+-rw-r--r--   0 james      (501) wheel        (0)       20 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/ray_logs/data/ray_temp/session_2023-02-09_12-23-55_156174_25782/logs/worker2.out
+-rw-r--r--   0 james      (501) wheel        (0)     4932 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/ray_logs/data/ray_temp/session_2023-02-09_12-23-55_156174_25782/logs/worker3.err
+-rw-r--r--   0 james      (501) wheel        (0)       73 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/ray_logs/data/ray_temp/session_2023-02-09_12-23-55_156174_25782/logs/worker3.out
+-rw-r--r--   0 james      (501) wheel        (0)    16259 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/ray_logs/test_ray_logs.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.703293 orquestra-sdk-0.47.0/tests/runtime/ray/regression/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.703704 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.703840 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/
+-rw-r--r--   0 james      (501) wheel        (0)        0 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/_valid
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.661929 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.660416 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/__status__/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.704489 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/__status__/SUCCESSFUL/
+-rw-r--r--   0 james      (501) wheel        (0)        0 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/__status__/SUCCESSFUL/wf.multi_json_wf.0000001
+-rw-r--r--   0 james      (501) wheel        (0)        0 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/__status__/SUCCESSFUL/wf.multi_pickle_wf.0000002
+-rw-r--r--   0 james      (501) wheel        (0)        0 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/__status__/SUCCESSFUL/wf.single_json_wf.0000003
+-rw-r--r--   0 james      (501) wheel        (0)        0 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/__status__/SUCCESSFUL/wf.single_pickle_wf.0000004
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.705137 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.705627 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/duplicate_name_counter/
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/duplicate_name_counter/invocation-0-task-multi-json
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/duplicate_name_counter/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/duplicate_name_counter/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote
+-rw-r--r--   0 james      (501) wheel        (0)       32 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/post_run_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       34 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/pre_run_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.705778 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.706858 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/invocation-0-task-multi-json/
+-rw-r--r--   0 james      (501) wheel        (0)        5 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/invocation-0-task-multi-json/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     3627 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/invocation-0-task-multi-json/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      645 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/invocation-0-task-multi-json/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)       24 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/invocation-0-task-multi-json/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       31 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/invocation-0-task-multi-json/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       34 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/invocation-0-task-multi-json/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)      133 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/invocation-0-task-multi-json/user_task_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.707924 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/
+-rw-r--r--   0 james      (501) wheel        (0)      102 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     1220 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      348 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)       24 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       31 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       33 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)        2 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/user_task_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.709040 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/
+-rw-r--r--   0 james      (501) wheel        (0)      120 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     2202 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      423 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)       27 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       31 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       34 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)        4 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/user_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       96 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/tasks/outputs.json
+-rw-r--r--   0 james      (501) wheel        (0)     2929 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/user_run_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       24 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_json_wf.0000001/workflow_meta.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.709724 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.710306 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/duplicate_name_counter/
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/duplicate_name_counter/invocation-0-task-multi-pickle
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/duplicate_name_counter/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/duplicate_name_counter/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote
+-rw-r--r--   0 james      (501) wheel        (0)       30 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/post_run_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       33 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/pre_run_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.710497 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.711768 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/invocation-0-task-multi-pickle/
+-rw-r--r--   0 james      (501) wheel        (0)        5 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/invocation-0-task-multi-pickle/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     3633 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/invocation-0-task-multi-pickle/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      661 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/invocation-0-task-multi-pickle/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)       18 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/invocation-0-task-multi-pickle/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       30 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/invocation-0-task-multi-pickle/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       32 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/invocation-0-task-multi-pickle/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)      139 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/invocation-0-task-multi-pickle/user_task_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.713130 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/
+-rw-r--r--   0 james      (501) wheel        (0)      102 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     1220 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      348 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)       18 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       30 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       32 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)        2 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/user_task_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.714485 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/
+-rw-r--r--   0 james      (501) wheel        (0)      120 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     2202 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      425 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)       21 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       30 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       32 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)        4 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/user_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       96 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/tasks/outputs.json
+-rw-r--r--   0 james      (501) wheel        (0)     2965 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/user_run_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       24 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.multi_pickle_wf.0000002/workflow_meta.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.715088 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.715574 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/duplicate_name_counter/
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/duplicate_name_counter/invocation-0-task-single-json
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/duplicate_name_counter/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/duplicate_name_counter/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote
+-rw-r--r--   0 james      (501) wheel        (0)       30 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/post_run_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       33 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/pre_run_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.715721 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.716762 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/invocation-0-task-single-json/
+-rw-r--r--   0 james      (501) wheel        (0)        5 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/invocation-0-task-single-json/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     3615 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/invocation-0-task-single-json/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      653 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/invocation-0-task-single-json/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)        5 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/invocation-0-task-single-json/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       30 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/invocation-0-task-single-json/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       32 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/invocation-0-task-single-json/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)      136 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/invocation-0-task-single-json/user_task_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.717891 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/
+-rw-r--r--   0 james      (501) wheel        (0)      102 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     1220 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      348 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)       16 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       30 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       32 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)        2 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/user_task_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.719095 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/
+-rw-r--r--   0 james      (501) wheel        (0)      102 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     2118 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      424 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)       19 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       30 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       31 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)        4 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/user_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       96 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/tasks/outputs.json
+-rw-r--r--   0 james      (501) wheel        (0)     2748 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/user_run_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       24 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_json_wf.0000003/workflow_meta.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.719663 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.720114 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/duplicate_name_counter/
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/duplicate_name_counter/invocation-0-task-single-pickle
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/duplicate_name_counter/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/duplicate_name_counter/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote
+-rw-r--r--   0 james      (501) wheel        (0)       31 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/post_run_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       32 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/pre_run_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.720255 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.721276 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/invocation-0-task-single-pickle/
+-rw-r--r--   0 james      (501) wheel        (0)        5 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/invocation-0-task-single-pickle/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     3630 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/invocation-0-task-single-pickle/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      669 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/invocation-0-task-single-pickle/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)        5 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/invocation-0-task-single-pickle/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       30 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/invocation-0-task-single-pickle/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       32 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/invocation-0-task-single-pickle/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)      142 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/invocation-0-task-single-pickle/user_task_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.722350 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/
+-rw-r--r--   0 james      (501) wheel        (0)      102 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     1220 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      348 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)       16 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       30 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       32 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)        2 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._dag._make_ray_dag.locals.handle_data_aggregation_error/user_task_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.723547 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/
+-rw-r--r--   0 james      (501) wheel        (0)      102 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     2118 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      426 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)       19 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       30 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       32 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)        4 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._dag._make_ray_dag_node.locals._ray_remote/user_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       96 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/tasks/outputs.json
+-rw-r--r--   0 james      (501) wheel        (0)     2786 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/user_run_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       24 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.46.0/workflows/wf.single_pickle_wf.0000004/workflow_meta.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.723728 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/
+-rw-r--r--   0 james      (501) wheel        (0)        0 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/_valid
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.664099 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.662596 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/__status__/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.724261 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/__status__/SUCCESSFUL/
+-rw-r--r--   0 james      (501) wheel        (0)        0 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/__status__/SUCCESSFUL/wf.multi_json_wf.0000001
+-rw-r--r--   0 james      (501) wheel        (0)        0 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/__status__/SUCCESSFUL/wf.multi_pickle_wf.0000002
+-rw-r--r--   0 james      (501) wheel        (0)        0 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/__status__/SUCCESSFUL/wf.single_json_wf.0000003
+-rw-r--r--   0 james      (501) wheel        (0)        0 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/__status__/SUCCESSFUL/wf.single_pickle_wf.0000004
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.724835 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.725316 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/duplicate_name_counter/
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/duplicate_name_counter/invocation-0-task-multi-json
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/duplicate_name_counter/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/duplicate_name_counter/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error
+-rw-r--r--   0 james      (501) wheel        (0)       31 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/post_run_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       31 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/pre_run_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.725483 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.726594 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/invocation-0-task-multi-json/
+-rw-r--r--   0 james      (501) wheel        (0)        5 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/invocation-0-task-multi-json/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     3760 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/invocation-0-task-multi-json/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      644 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/invocation-0-task-multi-json/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)      416 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/invocation-0-task-multi-json/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       29 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/invocation-0-task-multi-json/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       33 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/invocation-0-task-multi-json/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)      132 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/invocation-0-task-multi-json/user_task_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.727798 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/
+-rw-r--r--   0 james      (501) wheel        (0)      120 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     2467 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      434 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)      368 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       30 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       32 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)        4 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/user_task_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.728948 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/
+-rw-r--r--   0 james      (501) wheel        (0)      102 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     1337 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      369 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)      365 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       30 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       31 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)        2 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/user_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)      106 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/tasks/outputs.json
+-rw-r--r--   0 james      (501) wheel        (0)     3307 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/user_run_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       24 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_json_wf.0000001/workflow_meta.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.729545 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.729996 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/duplicate_name_counter/
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/duplicate_name_counter/invocation-0-task-multi-pickle
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/duplicate_name_counter/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/duplicate_name_counter/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error
+-rw-r--r--   0 james      (501) wheel        (0)       31 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/post_run_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       32 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/pre_run_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.730142 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.731181 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/invocation-0-task-multi-pickle/
+-rw-r--r--   0 james      (501) wheel        (0)        5 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/invocation-0-task-multi-pickle/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     3941 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/invocation-0-task-multi-pickle/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      660 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/invocation-0-task-multi-pickle/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)      426 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/invocation-0-task-multi-pickle/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       31 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/invocation-0-task-multi-pickle/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       32 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/invocation-0-task-multi-pickle/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)      138 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/invocation-0-task-multi-pickle/user_task_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.732314 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/
+-rw-r--r--   0 james      (501) wheel        (0)      120 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     2471 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      436 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)      398 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       31 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       32 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)        4 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/user_task_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.733424 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/
+-rw-r--r--   0 james      (501) wheel        (0)      102 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     1337 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      369 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)      395 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       30 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       33 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)        2 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/user_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)      106 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/tasks/outputs.json
+-rw-r--r--   0 james      (501) wheel        (0)     3527 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/user_run_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       24 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.multi_pickle_wf.0000002/workflow_meta.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.734060 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.734616 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/duplicate_name_counter/
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/duplicate_name_counter/invocation-0-task-single-json
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/duplicate_name_counter/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/duplicate_name_counter/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error
+-rw-r--r--   0 james      (501) wheel        (0)       30 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/post_run_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       32 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/pre_run_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.734800 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.736082 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/invocation-0-task-single-json/
+-rw-r--r--   0 james      (501) wheel        (0)        5 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/invocation-0-task-single-json/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     3919 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/invocation-0-task-single-json/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      652 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/invocation-0-task-single-json/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)      290 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/invocation-0-task-single-json/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       31 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/invocation-0-task-single-json/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       33 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/invocation-0-task-single-json/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)      135 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/invocation-0-task-single-json/user_task_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.737383 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/
+-rw-r--r--   0 james      (501) wheel        (0)      102 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     2393 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      435 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)      293 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       31 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       32 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)        4 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/user_task_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.738825 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/
+-rw-r--r--   0 james      (501) wheel        (0)      102 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     1337 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      369 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)      290 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       30 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       33 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)        2 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/user_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)      106 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/tasks/outputs.json
+-rw-r--r--   0 james      (501) wheel        (0)     3141 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/user_run_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       24 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_json_wf.0000003/workflow_meta.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.739503 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.739983 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/duplicate_name_counter/
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/duplicate_name_counter/invocation-0-task-single-pickle
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/duplicate_name_counter/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote
+-rw-r--r--   0 james      (501) wheel        (0)        1 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/duplicate_name_counter/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error
+-rw-r--r--   0 james      (501) wheel        (0)       30 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/post_run_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       31 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/pre_run_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.740135 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.741212 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/invocation-0-task-single-pickle/
+-rw-r--r--   0 james      (501) wheel        (0)        5 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/invocation-0-task-single-pickle/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     3934 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/invocation-0-task-single-pickle/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      668 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/invocation-0-task-single-pickle/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)      314 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/invocation-0-task-single-pickle/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       30 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/invocation-0-task-single-pickle/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       32 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/invocation-0-task-single-pickle/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)      141 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/invocation-0-task-single-pickle/user_task_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.742371 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/
+-rw-r--r--   0 james      (501) wheel        (0)      102 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     2395 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      437 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)      317 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       30 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       33 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)        4 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._build_workflow._make_ray_dag_node.locals._ray_remote/user_task_metadata.json
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.743488 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/
+-rw-r--r--   0 james      (501) wheel        (0)      102 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/args.pkl
+-rw-r--r--   0 james      (501) wheel        (0)     1337 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/func_body.pkl
+-rw-r--r--   0 james      (501) wheel        (0)      369 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/inputs.json
+-rw-r--r--   0 james      (501) wheel        (0)      314 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/output.pkl
+-rw-r--r--   0 james      (501) wheel        (0)       30 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/post_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       33 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/pre_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)        2 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/orquestra.sdk._ray._build_workflow.make_ray_dag.locals.handle_data_aggregation_error/user_task_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)      106 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/tasks/outputs.json
+-rw-r--r--   0 james      (501) wheel        (0)     3179 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/user_run_metadata.json
+-rw-r--r--   0 james      (501) wheel        (0)       24 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/0.47.0/workflows/wf.single_pickle_wf.0000004/workflow_meta.json
+-rw-r--r--   0 james      (501) wheel        (0)      953 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/README.md
+-rw-r--r--   0 james      (501) wheel        (0)      843 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/rename_workflows.sh
+-rw-r--r--   0 james      (501) wheel        (0)      883 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/data/workflows.py
+-rw-r--r--   0 james      (501) wheel        (0)     3602 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/regression/test_workflow_outputs.py
+-rw-r--r--   0 james      (501) wheel        (0)    11102 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/test_build_workflow.py
+-rw-r--r--   0 james      (501) wheel        (0)     2155 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/test_client.py
+-rw-r--r--   0 james      (501) wheel        (0)    13903 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/test_dag.py
+-rw-r--r--   0 james      (501) wheel        (0)      466 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/test_id_gen.py
+-rw-r--r--   0 james      (501) wheel        (0)    32514 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/test_integration.py
+-rw-r--r--   0 james      (501) wheel        (0)     1515 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/ray/test_logger.py
+-rw-r--r--   0 james      (501) wheel        (0)     2935 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/test_config.py
+-rw-r--r--   0 james      (501) wheel        (0)     4759 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/test_log_adapter.py
+-rw-r--r--   0 james      (501) wheel        (0)     7645 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/test_services.py
+-rw-r--r--   0 james      (501) wheel        (0)      879 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/runtime/test_services_integration.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.743636 orquestra-sdk-0.47.0/tests/sdk/
+-rw-r--r--   0 james      (501) wheel        (0)      347 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/__init__.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.746875 orquestra-sdk-0.47.0/tests/sdk/v2/
+-rw-r--r--   0 james      (501) wheel        (0)      347 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/__init__.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.747435 orquestra-sdk-0.47.0/tests/sdk/v2/api/
+-rw-r--r--   0 james      (501) wheel        (0)      253 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/api/__init__.py
+-rw-r--r--   0 james      (501) wheel        (0)    28995 2023-04-28 13:26:39.000000 orquestra-sdk-0.47.0/tests/sdk/v2/api/test_config.py
+-rw-r--r--   0 james      (501) wheel        (0)    18330 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/api/test_task_run.py
+-rw-r--r--   0 james      (501) wheel        (0)    26444 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/api/test_wf_run.py
+-rw-r--r--   0 james      (501) wheel        (0)     1341 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/conftest.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.747929 orquestra-sdk-0.47.0/tests/sdk/v2/conversions/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.750088 orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/
+-rw-r--r--   0 james      (501) wheel        (0)     2916 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/additional-metrics.yml
+-rw-r--r--   0 james      (501) wheel        (0)     1430 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/basics.yml
+-rw-r--r--   0 james      (501) wheel        (0)     1430 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/basics_file_ref.yml
+-rw-r--r--   0 james      (501) wheel        (0)     1565 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/basics_with_data_aggregation.yml
+-rw-r--r--   0 james      (501) wheel        (0)     1453 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/basics_with_gpu.yml
+-rw-r--r--   0 james      (501) wheel        (0)     1468 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/custom_json.yml
+-rw-r--r--   0 james      (501) wheel        (0)     3147 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/exportable_wf.yml
+-rw-r--r--   0 james      (501) wheel        (0)     3135 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/inline_function.yml
+-rw-r--r--   0 james      (501) wheel        (0)     1405 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/main_test.json
+-rw-r--r--   0 james      (501) wheel        (0)     1283 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/main_test.yml
+-rw-r--r--   0 james      (501) wheel        (0)     2445 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/multi_task_outputs.yml
+-rw-r--r--   0 james      (501) wheel        (0)     2771 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/multi_task_outputs_as_inputs.yml
+-rw-r--r--   0 james      (501) wheel        (0)     1453 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/positional.yml
+-rw-r--r--   0 james      (501) wheel        (0)     2594 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/positional_artifact.yml
+-rw-r--r--   0 james      (501) wheel        (0)     1526 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/python_import.yml
+-rw-r--r--   0 james      (501) wheel        (0)     2876 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/conversions/test_ids.py
+-rw-r--r--   0 james      (501) wheel        (0)     4858 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/conversions/test_imports.py
+-rw-r--r--   0 james      (501) wheel        (0)    44614 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/conversions/test_yaml_exporter.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.750856 orquestra-sdk-0.47.0/tests/sdk/v2/data/
+-rw-r--r--   0 james      (501) wheel        (0)       42 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/data/bad_requirements.txt
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.751034 orquestra-sdk-0.47.0/tests/sdk/v2/data/complex_serialization/
+-rw-r--r--   0 james      (501) wheel        (0)     4128 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/data/complex_serialization/workflow_defs.py
+-rw-r--r--   0 james      (501) wheel        (0)     1415 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/data/configs.py
+-rw-r--r--   0 james      (501) wheel        (0)       28 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/data/requirements.txt
+-rw-r--r--   0 james      (501) wheel        (0)       70 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/data/requirements_with_extras.txt
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.751541 orquestra-sdk-0.47.0/tests/sdk/v2/data/sample_project/
+-rw-r--r--   0 james      (501) wheel        (0)      351 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/data/sample_project/helpers.py
+-rw-r--r--   0 james      (501) wheel        (0)      487 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/data/sample_project/workflow_defs.py
+-rw-r--r--   0 james      (501) wheel        (0)      531 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/data/sample_project/workflow_defs_no_raise.py
+-rw-r--r--   0 james      (501) wheel        (0)     1579 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/data/task_run_workflow_defs.py
+-rw-r--r--   0 james      (501) wheel        (0)      581 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/dirs.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.752411 orquestra-sdk-0.47.0/tests/sdk/v2/driver/
+-rw-r--r--   0 james      (501) wheel        (0)      204 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/driver/__init__.py
+-rw-r--r--   0 james      (501) wheel        (0)     1437 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/driver/conftest.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.752635 orquestra-sdk-0.47.0/tests/sdk/v2/driver/regression/
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.754681 orquestra-sdk-0.47.0/tests/sdk/v2/driver/regression/data/
+-rw-r--r--   0 james      (501) wheel        (0)       51 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/driver/regression/data/v0.46.0_json-single.json
+-rw-r--r--   0 james      (501) wheel        (0)       50 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/driver/regression/data/v0.46.0_json-single_ids.json
+-rw-r--r--   0 james      (501) wheel        (0)       68 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/driver/regression/data/v0.46.0_json.json
+-rw-r--r--   0 james      (501) wheel        (0)       50 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/driver/regression/data/v0.46.0_json_ids.json
+-rw-r--r--   0 james      (501) wheel        (0)      105 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/driver/regression/data/v0.46.0_pickle-single.json
+-rw-r--r--   0 james      (501) wheel        (0)       50 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/driver/regression/data/v0.46.0_pickle-single_ids.json
+-rw-r--r--   0 james      (501) wheel        (0)      105 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/driver/regression/data/v0.46.0_pickle.json
+-rw-r--r--   0 james      (501) wheel        (0)       50 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/driver/regression/data/v0.46.0_pickle_ids.json
+-rw-r--r--   0 james      (501) wheel        (0)      205 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/driver/regression/data/v0.47.0_mixed.json
+-rw-r--r--   0 james      (501) wheel        (0)       50 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/driver/regression/data/v0.47.0_mixed_ids.json
+-rw-r--r--   0 james      (501) wheel        (0)      155 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/driver/regression/data/v0.47.0_single.json
+-rw-r--r--   0 james      (501) wheel        (0)       50 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/driver/regression/data/v0.47.0_single_ids.json
+-rw-r--r--   0 james      (501) wheel        (0)     2529 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/driver/regression/test_compat_results.py
+-rw-r--r--   0 james      (501) wheel        (0)    13071 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/driver/resp_mocks.py
+-rw-r--r--   0 james      (501) wheel        (0)    38586 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/driver/test_ce_runtime.py
+-rw-r--r--   0 james      (501) wheel        (0)    80999 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/driver/test_client.py
+-rw-r--r--   0 james      (501) wheel        (0)      806 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/project_state.py
+-rw-r--r--   0 james      (501) wheel        (0)      716 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/sample_wfs.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.755102 orquestra-sdk-0.47.0/tests/sdk/v2/schema/
+-rw-r--r--   0 james      (501) wheel        (0)      238 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/schema/__init__.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.755630 orquestra-sdk-0.47.0/tests/sdk/v2/schema/data/
+-rw-r--r--   0 james      (501) wheel        (0)     1261 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/schema/data/unpacking.py
+-rw-r--r--   0 james      (501) wheel        (0)     7007 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/schema/data/unpacking_wf_0.44.0.json
+-rw-r--r--   0 james      (501) wheel        (0)     7089 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/schema/data/unpacking_wf_0.45.1.json
+-rw-r--r--   0 james      (501) wheel        (0)     6865 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/schema/test_compat.py
+-rw-r--r--   0 james      (501) wheel        (0)     1728 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/schema/test_ir.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.756610 orquestra-sdk-0.47.0/tests/sdk/v2/secrets/
+-rw-r--r--   0 james      (501) wheel        (0)      204 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/secrets/__init__.py
+-rw-r--r--   0 james      (501) wheel        (0)     1632 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/secrets/resp_mocks.py
+-rw-r--r--   0 james      (501) wheel        (0)     4394 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/secrets/test_api.py
+-rw-r--r--   0 james      (501) wheel        (0)     4940 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/secrets/test_auth.py
+-rw-r--r--   0 james      (501) wheel        (0)    13976 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/secrets/test_client.py
+-rw-r--r--   0 james      (501) wheel        (0)     1528 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/secrets/test_importing.py
+-rw-r--r--   0 james      (501) wheel        (0)     4495 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/test_api_tutorial_scripts.py
+-rw-r--r--   0 james      (501) wheel        (0)    12777 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/test_artifact_future_methods.py
+-rw-r--r--   0 james      (501) wheel        (0)     7130 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/test_ast.py
+-rw-r--r--   0 james      (501) wheel        (0)    16553 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/test_config.py
+-rw-r--r--   0 james      (501) wheel        (0)      775 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/test_constant_nodes_serialization.py
+-rw-r--r--   0 james      (501) wheel        (0)    20866 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/test_dispatch.py
+-rw-r--r--   0 james      (501) wheel        (0)     6413 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/test_dispatch_integration.py
+-rw-r--r--   0 james      (501) wheel        (0)    20997 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/test_dsl.py
+-rw-r--r--   0 james      (501) wheel        (0)     1135 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/test_env.py
+-rw-r--r--   0 james      (501) wheel        (0)     6590 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/test_git_url_utils.py
+-rw-r--r--   0 james      (501) wheel        (0)     1635 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/test_graphs.py
+-rw-r--r--   0 james      (501) wheel        (0)     7690 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/test_in_process_runtime.py
+-rw-r--r--   0 james      (501) wheel        (0)     3815 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/test_loader.py
+-rw-r--r--   0 james      (501) wheel        (0)     5017 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/test_packaging.py
+-rw-r--r--   0 james      (501) wheel        (0)     4905 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/test_serde.py
+-rw-r--r--   0 james      (501) wheel        (0)     9718 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/test_task_ast_parsing.py
+-rw-r--r--   0 james      (501) wheel        (0)    39911 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/test_traversal.py
+-rw-r--r--   0 james      (501) wheel        (0)     2983 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/test_viz.py
+-rw-r--r--   0 james      (501) wheel        (0)    10858 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/test_workflow.py
+-rw-r--r--   0 james      (501) wheel        (0)     1632 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/test_workflow_ast_parsing.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.756935 orquestra-sdk-0.47.0/tests/sdk/v2/typing/
+-rw-r--r--   0 james      (501) wheel        (0)     1272 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/typing/full_example.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.758234 orquestra-sdk-0.47.0/tests/sdk/v2/typing/task/
+-rw-r--r--   0 james      (501) wheel        (0)      252 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/typing/task/assign_n_outputs.py
+-rw-r--r--   0 james      (501) wheel        (0)      248 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/typing/task/has_n_outputs.py
+-rw-r--r--   0 james      (501) wheel        (0)      241 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/typing/task/passed_correct_arg_type.py
+-rw-r--r--   0 james      (501) wheel        (0)      247 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/typing/task/passed_keyword_as_positional.py
+-rw-r--r--   0 james      (501) wheel        (0)      240 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/typing/task/passed_too_few_args.py
+-rw-r--r--   0 james      (501) wheel        (0)      247 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/typing/task/passed_too_many_args.py
+-rw-r--r--   0 james      (501) wheel        (0)      243 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/typing/task/passed_wrong_arg_type.py
+-rw-r--r--   0 james      (501) wheel        (0)      338 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/typing/task/task_base.py
+-rw-r--r--   0 james      (501) wheel        (0)     3659 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/typing/test_typing.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.758902 orquestra-sdk-0.47.0/tests/sdk/v2/typing/workflow/
+-rw-r--r--   0 james      (501) wheel        (0)      592 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/typing/workflow/assign_model.py
+-rw-r--r--   0 james      (501) wheel        (0)      249 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/typing/workflow/does_not_have_validate.py
+-rw-r--r--   0 james      (501) wheel        (0)      252 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/typing/workflow/has_local_run.py
+-rw-r--r--   0 james      (501) wheel        (0)      244 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/typing/workflow/has_model.py
+-rw-r--r--   0 james      (501) wheel        (0)      272 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/sdk/v2/typing/workflow/workflow_base.py
+drwxr-xr-x   0 james      (501) wheel        (0)        0 2023-04-28 13:27:42.759029 orquestra-sdk-0.47.0/tests/workflow/
+-rw-r--r--   0 james      (501) wheel        (0)      994 2023-04-28 13:26:29.000000 orquestra-sdk-0.47.0/tests/workflow/test_generating_schema.py
```

### Comparing `orquestra-sdk-0.46.0/.github/ISSUE_TEMPLATE/bug_report.md` & `orquestra-sdk-0.47.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/.github/ISSUE_TEMPLATE/feature_request.md` & `orquestra-sdk-0.47.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/.github/workflows/coverage.yml` & `orquestra-sdk-0.47.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/.github/workflows/performance.yml` & `orquestra-sdk-0.47.0/.github/workflows/performance.yml`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/.github/workflows/publish_release.yml` & `orquestra-sdk-0.47.0/.github/workflows/publish_release.yml`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/.github/workflows/style.yml` & `orquestra-sdk-0.47.0/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/.github/workflows/typing.yml` & `orquestra-sdk-0.47.0/.github/workflows/typing.yml`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/.gitignore` & `orquestra-sdk-0.47.0/.gitignore`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/CHANGELOG.md` & `orquestra-sdk-0.47.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,81 @@
 # Changelog
 
 ## Unreleased
 
 🚨 *Breaking Changes*
-
-- Workflow definitions now require at least one task in order to be submitted. This check is performed during traversal, and raises a WorkflowSyntaxError if no tasks are required to be executed.
-- Remove TaskDef.model and TaskDef.import_models interfaces
-- Public API classes `sdk.GitImport`, `sdk.GithubImport`, `sdk.LocalImport`, `sdk.InlineImport` now use `dataclasses.dataclass` instead of `typing.NamedTuple`.
-- Local Ray will now always pass resources to underlying ray.remote functions. 
+* Task results on QE have changed shape. This may cause some oddness when downloading older task artifacts.
 
 🔥 *Features*
-- Sort WF runs by start date in `list wf` command. Show start date as one of the columns
-- Sort WF runs by start date in all workflow commands in prompt selection. Show start date with WF id
-- Set resources for workflows on CE via `resources` keyword argument in the `@workflow` decorator or with `.with_resources()` on a `WorkflowDef`.
-- New parameters for `@workflow` decorator - `default_source_import` and `default_dependency_imports`.
-These parameters let you set the default imports for all tasks in given workflow.
-If a task defines its own imports (either source, dependencies, or both) - it will overwrite workflow defaults.
-- Allow single imports as `dependency_imports` in `@task` decorators.
-- Listing workflow runs from Compute Engine now allows an upper limit to the number of runs to be listed to be set via the `limit` keyword.
-- Print HTTP requests and other debug information from `orq` CLI if `ORQ_VERBOSE` env flag is set.
+* New built-in config name - "auto" - used to submit workflows to a remote cluster when used inside Orquestra Studio.
+* "auto" built-in config name becomes alias to "local" if not in a Studio environment
 
 👩‍🔬 *Experimental*
-
+* Setting workflow_id and project_id is now available on workflow Python API start() and prepare() functions
 
 🐛 *Bug Fixes*
-* Stopping a QE workflow after it has already stopped will no longer raise an exception.
-* Attempting to use the "in-process" runtime on the CLI will no longer raise an exception. Instead, a message teeling you to use the Python API or Ray will be printed.
-* Fix dependency issues causing CE workflows to fail if WF constant was library-dependent object.
-
+* Retry getting results from CE if the results were not ready but the workflow succeeded.
+* Using secrets inside the workflow function will now work correctly on Ray
+* Fix WorkflowDef.graph - honour kwargs of tasks and add aggregate_output to show outputs
+* Fixed returning intermediate workflow values (e.g. with `orq task results`) when the task has multiple outputs and only some of them were used in the rest of the workflow function. The following should work now as expected:
+```python
+@sdk.workflow
+def my_wf():
+    _, b = two_output_task()
+    all_outputs = two_output_task()
+    out1, out2 = all_outputs
+    return b, all_outputs, out1, out2
+```
+* Pickled workflow/task results should no longer cause workflows to fail inside the SDK machinery. Note: when passing a Python object between your tasks, you **must** ensure the Python dependencies are installed.
 
 💅 *Improvements*
+* `VersionMismatch` warning will be presented if we detect accessing a workflow def IR generated with another SDK version.
 
+🥷 *Internal*
+* `TaskOutputMetadata` model was added to the workflow def IR schema.
+* Workflows from CE return a new shape for workflow results and task results.
+* Workflows from Ray return a new shape for workflow and task results.
+* Workflows from QE return a new shape for task results.
+* Custom images will default to `None`, unless using Quantum Engine where the defaults stay the same.
+
+📃 *Docs*
+* _Resource Management_ guide should render properly now.
+
+## v0.46.0
+
+🚨 *Breaking Changes*
+* Workflow definitions now require at least one task in order to be submitted. This check is performed during traversal, and raises a `WorkflowSyntaxError` if no tasks are required to be executed.
+* Remove `TaskDef.model` and `TaskDef.import_models` interfaces
+* Public API classes `sdk.GitImport`, `sdk.GithubImport`, `sdk.LocalImport`, `sdk.InlineImport` now use `dataclasses.dataclass` instead of `typing.NamedTuple`.
+* Local Ray will now always pass resources to underlying ray.remote functions. 
+
+🔥 *Features*
+* Sort WF runs by start date in `list wf` command. Show start date as one of the columns
+* Sort WF runs by start date in all workflow commands in prompt selection. Show start date with WF id
+* Set resources for workflows on CE via `resources` keyword argument in the `@workflow` decorator or with `.with_resources()` on a `WorkflowDef`.
+* New parameters for `@workflow` decorator - `default_source_import` and `default_dependency_imports`.
+These parameters let you set the default imports for all tasks in given workflow.
+If a task defines its own imports (either source, dependencies, or both) - it will overwrite workflow defaults.
+* Allow single imports as `dependency_imports` in `@task` decorators.
+* Listing workflow runs from Compute Engine now allows an upper limit to the number of runs to be listed to be set via the `limit` keyword.
+* Print HTTP requests and other debug information from `orq` CLI if `ORQ_VERBOSE` env flag is set.
+* CE runtime now supports getting logs from remote Ray runtimes.
+
+🐛 *Bug Fixes*
+* Stopping a QE workflow after it has already stopped will no longer raise an exception.
+* Fix dependency issues causing CE workflows to fail if WF constant was library-dependent object.
+* Attempting to use the "in-process" runtime on the CLI will no longer raise an exception. Instead, a message telling you to use the Python API or Ray will be printed.
 
 🥷 *Internal*
 * During YAML conversion, Workflow SDK repo matched on host and path, not full URL.
 * On QE, Github URLs will be converted to SSH URLs.
 * Removed `corq` code.
 * Old `RuntimeInterface` methods have been removed.
 
-
 📃 *Docs*
-
 * Guide: CE Resource Management
 
 ## v0.45.1
 
 🐛 *Bug Fixes*
 * Ensure `int`-like resource values are passed to Ray correctly
 
@@ -52,15 +83,14 @@
 
 🚨 *Breaking Changes*
 * Pickling library switched to `cloudpickle` instead of `dill`. While no breakages are expected, this change may result in objects raising an error during pickling, even if they were previously able to be pickled. Please report any instances of these as bugs.
 
 
 🔥 *Features*
 * Use the requested resources from a workflow's tasks when submitting to CE
-* CE runtime now supports getting logs from remote Ray runtimes.
 
 
 🥷 *Internal*
 * RayRuntime can now be configured to pass resources to underlying remote functions
 * Added version metadata to the workflow IR
 
 ## v0.44.0
```

### Comparing `orquestra-sdk-0.46.0/CONTRIBUTING.md` & `orquestra-sdk-0.47.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/LICENSE` & `orquestra-sdk-0.47.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/Makefile` & `orquestra-sdk-0.47.0/Makefile`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/PKG-INFO` & `orquestra-sdk-0.47.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orquestra-sdk
-Version: 0.46.0
+Version: 0.47.0
 Summary: "Compose Orquestra workflows using a Python DSL"
 Home-page: https://github.com/zapatacomputing/orquestra-workflow-sdk
 Author: Zapata Computing Inc.
 Author-email: info@zapatacomputing.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `orquestra-sdk-0.46.0/README.md` & `orquestra-sdk-0.47.0/README.md`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/examples/config_management.py` & `orquestra-sdk-0.47.0/docs/examples/config_management.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/examples/quickstart.py` & `orquestra-sdk-0.47.0/docs/examples/quickstart.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,10 +29,10 @@
 wf_run_2 = wf.run("in_process")
 
 # >> end run workflow with stored config - short version
 
 results_1 = wf_run_1.get_results()
 results_2 = wf_run_2.get_results()
 assert results_1 == results_2, f"Expected {results_1} to look like {results_2}"
-assert (
-    results_1 == "Hello Orquestra!"
-), f"Expected {results_1} to look like 'Hello Orquestra!'"
+assert results_1 == (
+    "Hello Orquestra!",
+), f"Expected {results_1} to look like ('Hello Orquestra!',)"
```

### Comparing `orquestra-sdk-0.46.0/docs/examples/tests/conftest.py` & `orquestra-sdk-0.47.0/docs/examples/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/examples/tests/parsers.py` & `orquestra-sdk-0.47.0/docs/examples/tests/parsers.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/examples/tests/test_local_ray.py` & `orquestra-sdk-0.47.0/docs/examples/tests/test_local_ray.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/examples/tests/test_logging.py` & `orquestra-sdk-0.47.0/docs/examples/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/examples/tests/test_parametrized_workflows.py` & `orquestra-sdk-0.47.0/docs/examples/tests/test_parametrized_workflows.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/examples/tests/test_remote.py` & `orquestra-sdk-0.47.0/docs/examples/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/examples/tests/test_secrets.py` & `orquestra-sdk-0.47.0/docs/examples/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/examples/tests/test_workflow_syntax.py` & `orquestra-sdk-0.47.0/docs/examples/tests/test_workflow_syntax.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/guides/dependency-installation.rst` & `orquestra-sdk-0.47.0/docs/guides/dependency-installation.rst`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/guides/logging.rst` & `orquestra-sdk-0.47.0/docs/guides/logging.rst`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/guides/resource-management.rst` & `orquestra-sdk-0.47.0/docs/guides/resource-management.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Resource Management
-=======================
+===================
 
 Workflows submitted to run on Compute Engine and Local Ray can specify the computational resources they require, enabling precise management of resources and costs.
 
 .. note::
+
     Resource management is supported only when executing on Compute Engine and Local Ray runtimes. Tasks and workflows defined with these parameters may still be executed on other runtimes, however the resource specification will be ignored.
 
 Setting Task Resources
 ----------------------
 
 Required hardware resources are configured on a per-task basis by setting the ``resources`` field of the task decorator:
 
 .. code-block::
-   :caption: task resource request example
+    :caption: Task resource request example
 
     @sdk.task(
         resources=sdk.Resources(cpu="100m", memory="1Gi", disk="10Gi", gpu="1")
     )
     def my_task():
         ...
 
 ``resources`` expects a ``sdk.Resources()`` object that specifies some or all of:
 * ``cpu``: number of cores.
 * ``memory``: amount of RAM (bytes).
 * ``disk``: disk space (bytes).
 * ``gpu``: whether access to a gpu unit is required (``1`` if a GPU is required, ``0`` otherwise).
 
-Amounts of cpu and memory resources are specified by a string comprising a floating point value, and, optionally, a modifier to the base unit ('byte' in the case of ``memory`` and ``disk`` requests, 'cores' in the case of ``cpu`` requests). The modifier can be a SI (metric), or IEC (binary) multiplier as detailed in the table below. So ``disk="10k"`` will be interpreted as '10 kilobytes', while ``cpu="10k"`` would request 10^7 cores.
+Amounts of CPU and memory resources are specified by a string comprising a floating point value, and, optionally, a modifier to the base unit ('byte' in the case of ``memory`` and ``disk`` requests, 'cores' in the case of ``cpu`` requests). The modifier can be a SI (metric), or IEC (binary) multiplier as detailed in the table below. So ``disk="10k"`` will be interpreted as '10 kilobytes', while ``cpu="10k"`` would request 10^7 cores.
 
-.. table:: unit multipliers
+.. table:: Unit multipliers
     :widths: auto
 
     +---------+-------+--------+-------+
     |         | Name  | String | Value |
     +=========+=======+========+=======+
     | Binary  | kibi  | Ki     | 2^10  |
     |         | mibi  | Mi     | 2^20  |
@@ -48,40 +49,42 @@
     |         | mega  | M      | 10^6  |
     |         | giga  | G      | 10^9  |
     |         | tera  | T      | 10^12 |
     |         | peta  | P      | 10^15 |
     |         | exa   | E      | 10^18 |
     +---------+-------+--------+-------+
 
-Convention is to use binary prefixes for memory resource requests (``disk`` and ``memory``), and decimal prefixes to specify the number of cores. The task resource request example above specifies a task that requires 100 milicores (or 0.1 cores), 1 gibibyte of RAM (2^30 bytes), 10 gibibytes of disk space(1.25*2^33 bytes), and access to a GPU.
+Convention is to use binary prefixes for memory resource requests (``disk`` and ``memory``), and decimal prefixes to specify the number of cores. The task resource request example above specifies a task that requires 100 millicores (or 0.1 cores), 1 gibibyte of RAM (2^30 bytes), 10 gibibytes of disk space(1.25*2^33 bytes), and access to a GPU.
+
+.. note::
 
-.. note:: mixing unit prefixes
     Binary and decimal units can be used interchangeably, however this can occasionally cause confusion, and care must be taken when specifying these parameters. For example, a memory request of ``100m`` specifies not 100 megabytes, but 100 millibytes, or 0.1 bytes.
 
 Setting Workflow Resources
 --------------------------
 
 Resources can also be configured at the workflow definition level using the same syntax as with tasks, with one difference - the ``sdk.Resources()`` object my additionally specify a number of nodes to be requested for the workflow. The full parameter list is therefore:
 * ``cpu``: number of cores.
 * ``memory``: amount of RAM (bytes).
 * ``disk``: disk space (bytes).
 * ``gpu``: whether access to a gpu unit is required (``1`` if a GPU is required, ``0`` otherwise).
 * ``nodes``: the number of nodes requested.
 
 .. code-block::
-    :caption: workflow resource request example
+    :caption: Workflow resource request example
 
     @sdk.workflow(
         resources=sdk.Resources(cpu="100m", memory="1Gi", disk="10Gi", gpu="1", nodes=5)
     )
     def my_workflow():
         ...
 
 
-.. note:: nodes
+.. note::
+
     Note that unlike the other parameters, ``nodes`` must be an integer rather than a string.
 
 Currently, the workflow resource request is only utilised by Compute Engine.
 If resources are not provided, Compute Engine will infer the overall resource requirements from the aggregated requirements of individual tasks.
 Tweaking the resource request may be required when your tasks spawn additional actors or remote functions to avoid deadlock, see below.
 
 
@@ -92,20 +95,21 @@
 ^^^^^^^^^^^^^^^^^^^
 
 Due to the way Ray's RLLib works, a deadlock can be created on Compute Engine if a task attempts to spawn additional actors or remote functions via the DNQ ``rollouts`` facility. Resources requested in a task definition are bound to the task process, so additional actors can rapidly exhaust the provisioned resources.
 
 In these cases, additional resources should be specified in the workflow decorator.
 
 .. code-block::
-    :caption: Example: override workflow resources.
-    @sdk.task(resources=...)                    # task resources requested.
+    :caption: Example: override workflow resources
+
+    @sdk.task(resources=...)                    # Task resources requested.
     def task():
         config = DQNConfig()
         ...
-        config.rollouts(num_rollout_workers=2)  # additional actors do not have
+        config.rollouts(num_rollout_workers=2)  # Additional actors do not have
         ...                                     # access to task resources.
         return results
 
     @sdk.workflow(resources=...)                # Override the aggregated task
     def wf():                                   # resources to provision additional
         results = []                            # resources for the additional
         for _ in range(5):                      # actors.
@@ -114,32 +118,34 @@
 My Local Tasks Aren't Running
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 Task resources are used to schedule tasks both locally and on remote runtimes.
 This might lead to issues when running tasks locally if they require resources that are unavailable.
 
 For example, you have a task that requires:
 
-1. a GPU but during development you run the workflow on your laptop without a GPU.
-2. 32GB of memory, but your Studio notebook only has 8GB available.
+1. A GPU but during development you run the workflow on your laptop without a GPU.
+2. 32 GB of memory, but your Studio notebook only has 8 GB available.
 3. 16 CPU cores but your desktop only has 8 available.
 
 In these examples, those tasks will not be scheduled by a local Ray instance due to the lack of resources.
-To workaround this problem, you should reduce the resources to match what is available. This can be done in the decorator:
+To work around this problem, you should reduce the resources to match what is available. This can be done in the decorator:
+
+.. code-block::
 
-.. code-block:
     @sdk.task(resources=sdk.Resources(gpu="0"))
     def my_task():
         ...
 
 or when the task is invoked, with the ``.with_resources()`` method:
 
-.. code-block:
+.. code-block::
+
     # Usual request
     @sdk.task(resources=sdk.Resources(gpu="1"))
     def my_task():
         ...
 
     @sdk.workflow
     def my_workflow():
         # The resources are overridden for this one invocation
         result = my_task().with_resources(gpu="0")
-        return result
+        return result
```

### Comparing `orquestra-sdk-0.46.0/docs/guides/runtime-configuration.rst` & `orquestra-sdk-0.47.0/docs/guides/runtime-configuration.rst`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/guides/workflow-runs.rst` & `orquestra-sdk-0.47.0/docs/guides/workflow-runs.rst`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/guides/workflow-syntax.rst` & `orquestra-sdk-0.47.0/docs/guides/workflow-syntax.rst`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/index.rst` & `orquestra-sdk-0.47.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/tutorials/images/orq-login-copy-token.png` & `orquestra-sdk-0.47.0/docs/tutorials/images/orq-login-copy-token.png`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/tutorials/images/orq-login-grant-access.png` & `orquestra-sdk-0.47.0/docs/tutorials/images/orq-login-grant-access.png`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/tutorials/images/orq-login-landing-page.png` & `orquestra-sdk-0.47.0/docs/tutorials/images/orq-login-landing-page.png`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/tutorials/images/win-redist-picture.png` & `orquestra-sdk-0.47.0/docs/tutorials/images/win-redist-picture.png`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/tutorials/installing-macos-linux.rst` & `orquestra-sdk-0.47.0/docs/tutorials/installing-macos-linux.rst`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/tutorials/installing-windows.rst` & `orquestra-sdk-0.47.0/docs/tutorials/installing-windows.rst`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/tutorials/jupyter-sdk.rst` & `orquestra-sdk-0.47.0/docs/tutorials/jupyter-sdk.rst`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/tutorials/parametrized-workflows.rst` & `orquestra-sdk-0.47.0/docs/tutorials/parametrized-workflows.rst`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/tutorials/quickstart.rst` & `orquestra-sdk-0.47.0/docs/tutorials/quickstart.rst`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/tutorials/ray.rst` & `orquestra-sdk-0.47.0/docs/tutorials/ray.rst`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/tutorials/remote.rst` & `orquestra-sdk-0.47.0/docs/tutorials/remote.rst`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/docs/tutorials/secrets.rst` & `orquestra-sdk-0.47.0/docs/tutorials/secrets.rst`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/pyproject.toml` & `orquestra-sdk-0.47.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -49,11 +49,12 @@
 exclude_lines = [
   "pragma: no cover",
   "def __repr__",
   "def __str__",
   "raise AssertionError",
   "raise NotImplementedError",
   "if __name__ == .__main__.:",
+  "assert_never",
 ]
 
 [tool.pytest.ini_options]
 log_level="INFO"
```

### Comparing `orquestra-sdk-0.46.0/setup.cfg` & `orquestra-sdk-0.47.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 	dill==0.3.6
 	wrapt
 	filelock>=3.3.2
 	packaging>=21
 	GitPython
 	pip-api==0.0.30
 	importlib_metadata~=4.0
-	typing-extensions~=4.0
+	typing-extensions>=4.1.0
 	pyyaml
 	requests~=2.28
 	graphviz
 	argcomplete
 	click~=8.0
 	cloup~=2.0
 	inquirer~=3.0
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/__init__.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_api/__init__.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_api/_config.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_api/_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,15 +319,18 @@
         Args:
             config_save_file: The path to the config file from which to read. If
                 omitted, the default config file will be used.
 
         Returns:
             list: list of configurations within the save file.
         """
-        return _config.read_config_names() + list(_config.UNIQUE_CONFIGS)
+        configs = _config.read_config_names() + list(_config.UNIQUE_CONFIGS)
+        if _config.is_passport_file_available():
+            configs.append(_config.AUTO_CONFIG_NAME)
+        return configs
 
     @classmethod
     def load(
         cls,
         config_name: str,
     ):
         """Load an existing configuration from a file.
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_api/_task_run.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_api/_task_run.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 # © Copyright 2022-2023 Zapata Computing Inc.
 ################################################################################
 
 import typing as t
 from collections import namedtuple
 from itertools import chain
 
+from orquestra.sdk._base import serde
 from orquestra.sdk.schema import ir
+from orquestra.sdk.schema.responses import WorkflowResult
 from orquestra.sdk.schema.workflow_run import State, TaskInvocationId
 from orquestra.sdk.schema.workflow_run import TaskRun as TaskRunModel
 from orquestra.sdk.schema.workflow_run import TaskRunId, WorkflowRunId
 
 from ...exceptions import TaskRunNotFound
 from ..abc import ArtifactValue, RuntimeInterface
 from ..serde import deserialize_constant
@@ -106,38 +108,34 @@
             wf_run_id=self.workflow_run_id, task_inv_id=self.task_invocation_id
         )
 
     def get_outputs(self) -> t.Any:
         """
         Get values calculated by this task run.
 
+        Returns whatever the task function returned, regardless of
+        ``@task(n_outputs=...)``.
+
         Raises:
             TaskRunNotFound: if the task wasn't completed yet, or the ID is invalid.
         """
         # NOTE: this is a possible place for improvement. If future runtime APIs support
         # getting a subset of artifacts, we should use them here.
         workflow_artifacts = self._runtime.get_available_outputs(self.workflow_run_id)
 
         try:
-            filtered_artifacts = {
-                self.task_invocation_id: workflow_artifacts[self.task_invocation_id]
-            }
+            task_outputs = workflow_artifacts[self.task_invocation_id]
         except KeyError as e:
             raise TaskRunNotFound(
                 f"Output for task `{self.task_invocation_id}` in "
                 f"`{self.workflow_run_id}` wasn't found. "
                 "It may have failed or not be completed yet."
             ) from e
 
-        # The runtime always returns tuples, even of the task has n_outputs = 1. We
-        # need to unwrap it for user's convenience.
-        return unwrap_task_retvals(
-            artifacts=filtered_artifacts,
-            task_invocations=self._wf_def.task_invocations,
-        )[self.task_invocation_id]
+        return serde.deserialize(task_outputs)
 
     def _find_invocation_by_output_id(self, output: ir.ArgumentId) -> ir.TaskInvocation:
         """
         Helper method that locates the invocation object responsible for returning
         output with given ID
         It is based on the assumption that output IDs are unique, and one output
         is returned by a single task invocation (but one invocation can produce
@@ -148,45 +146,52 @@
             for inv in self._wf_def.task_invocations.values()
             if output in inv.output_ids
         )
 
     def _find_value_by_id(
         self,
         arg_id: ir.ArgumentId,
-        available_outputs: t.Mapping[TaskInvocationId, t.Tuple[ArtifactValue, ...]],
+        available_outputs: t.Mapping[TaskInvocationId, WorkflowResult],
     ) -> ArtifactValue:
         """
         Helper method that finds and deserializes input artifact value based on the
         artifact/argument ID. Uses values from available_outputs, or deserializes the
         constant embedded in the workflow def.
         """
         if arg_id in self._wf_def.constant_nodes:
             value = deserialize_constant(self._wf_def.constant_nodes[arg_id])
             return value
+        elif arg_id in self._wf_def.secret_nodes:
+            return self._wf_def.secret_nodes[arg_id]
 
         producer_inv = self._find_invocation_by_output_id(arg_id)
-        output_index = producer_inv.output_ids.index(arg_id)
+        output_index = self._wf_def.artifact_nodes[arg_id].artifact_index
         try:
-            parent_output_vals = available_outputs[producer_inv.id]
+            artifact_node = available_outputs[producer_inv.id]
         except KeyError:
             # Parent invocation ID not in available outputs => parent invocation
             # wasn't completed yet.
             return self.INPUT_UNAVAILABLE
 
+        parent_output_vals = serde.deserialize(artifact_node)
+
         # A task function can return multiple values. We're only interested in one
         # of them.
         #
         # Assumption 1: RuntimeInterface.get_available_outputs() returns tuples even
         # for tasks with single output.
         #
         # Assumption 2: either a task wasn't completed yet and we don't have any
         # outputs (handled above) or we have access to all outputs of this task.
         # There shouldn't be a situation where we have access to a subset of a given
         # task's outputs.
-        return parent_output_vals[output_index]
+        if output_index is None:
+            return parent_output_vals
+        else:
+            return parent_output_vals[output_index]
 
     def get_inputs(self) -> Inputs:
         """
         Get values of inputs (parameters) of a task run
 
         Returns:  Input namedTuple with Input.args and .kwargs parameters.
         """
@@ -248,23 +253,7 @@
                 runtime=self._runtime,
                 wf_def=self._wf_def,
             )
             for model in parent_run_models
         ]
 
         return set(parents)
-
-
-def unwrap_task_retvals(
-    artifacts: t.Mapping[ir.TaskInvocationId, ArtifactValue],
-    task_invocations: t.Mapping[TaskInvocationId, ir.TaskInvocation],
-) -> t.Mapping[ir.TaskInvocationId, t.Union[ArtifactValue, t.Tuple[ArtifactValue]]]:
-    unwrapped_dict = {}
-    for inv_id, outputs in artifacts.items():
-        inv = task_invocations[inv_id]
-        if len(inv.output_ids) == 1:
-            unwrapped = outputs[0]
-        else:
-            unwrapped = outputs
-
-        unwrapped_dict[inv_id] = unwrapped
-    return unwrapped_dict
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_api/_wf_run.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_api/_wf_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,21 @@
     WorkflowRunNotFoundError,
     WorkflowRunNotStarted,
     WorkflowRunNotSucceeded,
 )
 from ...schema import ir
 from ...schema.configs import ConfigName
 from ...schema.local_database import StoredWorkflowRun
-from ...schema.workflow_run import State, TaskInvocationId
+from ...schema.workflow_run import ProjectRef, State, TaskInvocationId
 from ...schema.workflow_run import WorkflowRun as WorkflowRunModel
 from ...schema.workflow_run import WorkflowRunId
+from .. import serde
 from ..abc import RuntimeInterface
 from ._config import RuntimeConfig
-from ._task_run import TaskRun, unwrap_task_retvals
+from ._task_run import TaskRun
 
 COMPLETED_STATES = [State.FAILED, State.TERMINATED, State.SUCCEEDED]
 
 
 class WorkflowRun:
     """
     Represents a single "execution" of a workflow. Used to get the workflow results.
@@ -125,14 +126,15 @@
 
     def __init__(
         self,
         run_id: t.Optional[WorkflowRunId],
         wf_def: ir.WorkflowDef,
         runtime: RuntimeInterface,
         config: t.Optional["RuntimeConfig"] = None,
+        project: t.Optional[ProjectRef] = None,
     ):
         """
         Users aren't expected to use __init__() directly. Please use
         `WorkflowRun.by_id`, `WorkflowDef.prepare()`, or `WorkflowDef.run()`.
 
         Args:
             wf_def: the workflow being run. Workflow definition in the model
@@ -142,14 +144,15 @@
                 Ray or Quantum Engine have corresponding classes.
         """
 
         self._run_id = run_id
         self._wf_def = wf_def
         self._runtime = runtime
         self._config = config
+        self._project = project
 
     def __str__(self) -> str:
         outstr: str = ""
         if self._run_id is None:
             outstr += "Unstarted WorkflowRun with parameters:"
         else:
             outstr += f"WorkflowRun '{self._run_id}' with parameters:"
@@ -195,15 +198,15 @@
             raise WorkflowRunNotStarted(workflow_not_started_message)
         return self._run_id
 
     def start(self):
         """
         Schedule workflow for execution.
         """
-        run_id = self._runtime.create_workflow_run(self._wf_def)
+        run_id = self._runtime.create_workflow_run(self._wf_def, self._project)
         self._run_id = run_id
 
     def wait_until_finished(self, frequency: float = 0.25, verbose=True) -> State:
         """Block until the workflow run finishes.
 
         This method draws no distinctions between whether the workflow run completes
         successfully, fails, or is terminated for any other reason.
@@ -347,23 +350,29 @@
         if (state := self.get_status()) not in COMPLETED_STATES:
             raise WorkflowRunNotFinished(
                 f"Workflow run with id {run_id} has not finished. "
                 f"Current state: {state}",
                 state,
             )
         try:
-            return self._runtime.get_workflow_run_outputs_non_blocking(run_id)
+            return (
+                *(
+                    serde.deserialize(o)
+                    for o in self._runtime.get_workflow_run_outputs_non_blocking(run_id)
+                ),
+            )
         except WorkflowRunNotSucceeded:
             raise
 
     def get_artifacts(self) -> t.Mapping[ir.TaskInvocationId, t.Any]:
         """
         Unstable: this API will change.
 
-        Returns all values returned by this workflow's tasks.
+        Returns values calculated by this workflow's tasks. If a given task hasn't
+        succeeded yet, the mapping won't contain the corresponding entry.
 
         Raises:
             WorkflowRunNotStarted: when the workflow has not started
 
         Returns:
             A dictionary with an entry for each task run in the workflow. The key is the
                 task's invocation ID. The value is whatever the task returned. If the
@@ -379,21 +388,23 @@
                 "You will need to call the `.start()` method prior to calling this "
                 "method."
             )
             raise WorkflowRunNotStarted(message) from e
 
         # NOTE: this is a possible place for improvement. If future runtime APIs support
         # getting a subset of artifacts, we should use them here.
-        workflow_artifacts = self._runtime.get_available_outputs(run_id)
+        inv_outputs = self._runtime.get_available_outputs(run_id)
 
-        # The runtime always returns tuples, even of the task has n_outputs = 1. We
-        # need to unwrap it for user's convenience.
-        return unwrap_task_retvals(
-            artifacts=workflow_artifacts, task_invocations=self._wf_def.task_invocations
-        )
+        # The output shape differs across runtimes when the workflow functions returns a
+        # single, packed future. See more in:
+        # https://zapatacomputing.atlassian.net/browse/ORQSDK-801
+        return {
+            inv_id: serde.deserialize(inv_output)
+            for inv_id, inv_output in inv_outputs.items()
+        }
 
     def get_logs(self) -> t.Mapping[TaskInvocationId, t.List[str]]:
         """
         Unstable: this API will change.
 
         Returns logs produced by all task runs in this workflow. If you're interested in
         only subset of tasks, consider using ``WorkflowRun.get_tasks()`` and
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_ast.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_ast.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_config.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # © Copyright 2022-2023 Zapata Computing Inc.
 ################################################################################
 """
 This is the internal module for saving and loading runtime configurations.
 See docs/runtime_configurations.rst for more information.
 """
 import os
+import pathlib
 from pathlib import Path
 from typing import Any, List, Mapping, Optional, Tuple, Union
 from urllib.parse import urlparse
 
 import filelock
 from pydantic.error_wrappers import ValidationError
 
@@ -18,27 +19,28 @@
     CONFIG_FILE_CURRENT_VERSION,
     ConfigName,
     RuntimeConfiguration,
     RuntimeConfigurationFile,
     RuntimeName,
 )
 
-from ._env import CONFIG_PATH_ENV
+from ._env import CONFIG_PATH_ENV, PASSPORT_FILE_ENV
 
 # Why JSON?
 #  The Python TOML package is unmaintained as of 2022-02-18.
 #  It is not compatible with the 1.0 version of the TOML spec:
 #    https://github.com/uiri/toml/issues/267#issuecomment-886139340
 #  YAML is not accepted by Pydantic's parse_file and is unlikely to ever be supported:
 #    https://github.com/samuelcolvin/pydantic/issues/136
 CONFIG_FILE_NAME = "config.json"
 LOCK_FILE_NAME = "config.json.lock"
 BUILT_IN_CONFIG_NAME = "local"
 RAY_CONFIG_NAME_ALIAS = "ray"
 IN_PROCESS_CONFIG_NAME = "in_process"
+AUTO_CONFIG_NAME = "auto"
 
 LOCAL_RUNTIME_CONFIGURATION = RuntimeConfiguration(
     config_name=BUILT_IN_CONFIG_NAME,
     runtime_name=RuntimeName.RAY_LOCAL,
     runtime_options={
         "address": "auto",
         "log_to_driver": False,
@@ -48,19 +50,30 @@
     },
 )
 IN_PROCESS_RUNTIME_CONFIGURATION = RuntimeConfiguration(
     config_name=IN_PROCESS_CONFIG_NAME,
     runtime_name=RuntimeName.IN_PROCESS,
     runtime_options={},
 )
+# this runtime config is not ready-to-be-used without runtime options
+SAME_CLUSTER_RUNTIME_CONFIGURATION = RuntimeConfiguration(
+    config_name=AUTO_CONFIG_NAME,
+    runtime_name=RuntimeName.CE_REMOTE,
+    runtime_options={},
+)
+# We assume that we can access the workflow API under a well-known URI if the passport
+# auth is being used. This relies on the DNS configuration on the remote cluster.
+# Works from CE and jupiter-notebook inside Studio
+SAME_CLUSTER_URL = "http://workflow-driver.workflow-driver"
 
 SPECIAL_CONFIG_NAME_DICT = {
     IN_PROCESS_CONFIG_NAME: IN_PROCESS_RUNTIME_CONFIGURATION,
     BUILT_IN_CONFIG_NAME: LOCAL_RUNTIME_CONFIGURATION,
     RAY_CONFIG_NAME_ALIAS: LOCAL_RUNTIME_CONFIGURATION,
+    AUTO_CONFIG_NAME: SAME_CLUSTER_RUNTIME_CONFIGURATION,
 }
 # Unique config list to prompt to the users. Separate from SPECIAL_CONFIG_NAME_DICT
 # as SPECIAL_CONFIG_NAME_DICT might have duplicate names which could be confusing for
 # the user
 UNIQUE_CONFIGS = {RAY_CONFIG_NAME_ALIAS, IN_PROCESS_CONFIG_NAME}
 CLI_IGNORED_CONFIGS = {IN_PROCESS_CONFIG_NAME}
 
@@ -107,14 +120,18 @@
         _config_file_path = Path(config_file_path).resolve()
     else:
         _config_file_path = Path.home() / ".orquestra" / CONFIG_FILE_NAME
     _ensure_directory(_config_file_path.parent)
     return _config_file_path
 
 
+def is_passport_file_available() -> bool:
+    return PASSPORT_FILE_ENV in os.environ
+
+
 def _get_config_directory() -> Path:
     """
     Get the path to the directory that contains the configuration file.
 
     Returns:
         Path: path to the parent directory.
     """
@@ -178,19 +195,44 @@
             version=CONFIG_FILE_CURRENT_VERSION,
             configs={},
         )
     new_config_file.configs[resolved_config_name] = new_config_entry
     return new_config_file
 
 
+def _resolve_auto_config(config_name) -> RuntimeConfiguration:
+    # if not in the Studio environment, return local Ray as auto configuration
+    if PASSPORT_FILE_ENV not in os.environ:
+        return LOCAL_RUNTIME_CONFIGURATION
+    passport_file = pathlib.Path(os.environ[PASSPORT_FILE_ENV])
+
+    try:
+        passport_token = Path(passport_file).read_text()
+    except FileNotFoundError as e:
+        raise FileNotFoundError(
+            f"Environmental variable {PASSPORT_FILE_ENV} was set, but no file was found"
+            "under its value"
+        ) from e
+
+    runtime_config = SPECIAL_CONFIG_NAME_DICT[config_name]
+    runtime_config.runtime_options = {
+        "uri": SAME_CLUSTER_URL,
+        "token": passport_token,
+    }
+    return runtime_config
+
+
 def _handle_config_name_special_cases(config_name: str) -> RuntimeConfiguration:
     # special cases: the built-in config ('local') and in process config have
     # hardcoded runtime options.
     if config_name in SPECIAL_CONFIG_NAME_DICT:
-        return SPECIAL_CONFIG_NAME_DICT[config_name]
+        if config_name == AUTO_CONFIG_NAME:
+            return _resolve_auto_config(config_name)
+        else:
+            return SPECIAL_CONFIG_NAME_DICT[config_name]
     else:
         raise NotImplementedError(
             f"Config name '{config_name}' is reserved, but we don't have a config "
             "to return for it. Please report this as a bug."
         )
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_conversions/_ids.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_conversions/_ids.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_conversions/_imports.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_conversions/_imports.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_conversions/_invocations.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_conversions/_invocations.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from orquestra.sdk.schema import ir, responses, yaml_model
 
 # TODO: it would be nice to have a single document where the user could look up a "type"
 # from the workflow yaml and see what it's about.
 RESULT_DICT_TYPE_NAME = "workflow-result-dict"
 SECRET_DICT_TYPE_NAME = "workflow-secret-dict"
 SDK_METADATA_TYPE_NAME = "sdk-metadata"
+QE_DEFAULT_IMAGE = "zapatacomputing/orquestra-default:v0.0.0"
+QE_GPU_IMAGE = "zapatacomputing/orquestra-nvidia:v0.0.0"
 
 
 def _json_dict_from_pydantic(model):
     return json.loads(model.json())
 
 
 class InvocationTranslator:
@@ -95,14 +97,22 @@
             step_resources = yaml_model.Resources(
                 cpu=task_resources.cpu,
                 memory=task_resources.memory,
                 disk=task_resources.disk,
                 gpu=task_resources.gpu,
             )
 
+        custom_image = inv.custom_image or task.custom_image
+
+        if custom_image is None:
+            if step_resources is not None and step_resources.gpu:
+                custom_image = QE_GPU_IMAGE
+            else:
+                custom_image = QE_DEFAULT_IMAGE
+
         dependency_ids = task.dependency_import_ids or []
 
         ir_import_ids = [task.source_import_id, *dependency_ids]
         step_import_names = [
             self._ir_yaml_import_map[ir_id]
             for ir_id in ir_import_ids
             if not isinstance(self._ir_imports[ir_id], ir.InlineImport)
@@ -113,15 +123,15 @@
                 step_import_names.insert(0, name)
 
         return yaml_model.Step(
             name=inv.id,
             config=yaml_model.StepConfig(
                 runtime=yaml_model.Runtime(
                     language=yaml_model.RuntimeLanguage.PYTHON3,
-                    customImage=inv.custom_image or task.custom_image,
+                    customImage=custom_image,
                     imports=step_import_names,
                     parameters=yaml_model.RuntimeParameters(
                         # Hardcoded reference of the single entrypoint "dispatcher" in
                         # the SDK.
                         file=_make_fn_file_path(
                             self._sdk_import_name,
                             "src/orquestra/sdk/_base/dispatch.py",
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_conversions/_yaml_exporter.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_conversions/_yaml_exporter.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_db/_db.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_db/_db.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_db/_migration.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_db/_migration.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_driver/_ce_runtime.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_driver/_ce_runtime.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 ################################################################################
 # © Copyright 2022-2023 Zapata Computing Inc.
 ################################################################################
 import warnings
 from datetime import timedelta
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Dict, List, Optional, Sequence, Union
 
 from orquestra.sdk import exceptions
-from orquestra.sdk._base import serde
+from orquestra.sdk._base import _retry, serde
 from orquestra.sdk._base._db import WorkflowDB
-from orquestra.sdk._base.abc import ArtifactValue, RuntimeInterface
+from orquestra.sdk._base.abc import RuntimeInterface
 from orquestra.sdk.kubernetes.quantity import parse_quantity
 from orquestra.sdk.schema.configs import RuntimeConfiguration
-from orquestra.sdk.schema.ir import TaskInvocationId, WorkflowDef
+from orquestra.sdk.schema.ir import ArtifactFormat, TaskInvocationId, WorkflowDef
 from orquestra.sdk.schema.local_database import StoredWorkflowRun
+from orquestra.sdk.schema.responses import ComputeEngineWorkflowResult, WorkflowResult
 from orquestra.sdk.schema.workflow_run import (
+    ProjectRef,
     State,
     TaskRunId,
     WorkflowRun,
     WorkflowRunId,
     WorkflowRunMinimal,
 )
 
@@ -84,23 +86,23 @@
     def from_runtime_configuration(
         cls, project_dir: Path, config: RuntimeConfiguration, verbose: bool
     ) -> "RuntimeInterface":
         """Returns an initilaised version of the class from a runtime configuration"""
         return cls(config, verbose)
 
     def create_workflow_run(
-        self,
-        workflow_def: WorkflowDef,
+        self, workflow_def: WorkflowDef, project: Optional[ProjectRef]
     ) -> WorkflowRunId:
         """
         Schedules a workflow definition for execution
 
         Args:
             workflow_def: the IR of the workflow to run
-
+            project: Project dir (workspace and project ID) on which the workflow
+            will be run
         Raises:
             WorkflowSyntaxError: when the workflow definition was rejected by the remote
                 cluster
             WorkflowRunNotStarted: for all other errors that prevented the workflow run
                 from being scheduled
             UnauthorizedError: if the current token was rejected by the remote cluster
 
@@ -115,15 +117,16 @@
                 gpu=workflow_def.resources.gpu,
                 nodes=workflow_def.resources.nodes,
             )
         else:
             resources = _get_max_resources(workflow_def)
 
         try:
-            workflow_def_id = self._client.create_workflow_def(workflow_def)
+            workflow_def_id = self._client.create_workflow_def(workflow_def, project)
+
             workflow_run_id = self._client.create_workflow_run(
                 workflow_def_id, resources
             )
         except _exceptions.InvalidWorkflowDef as e:
             raise exceptions.WorkflowSyntaxError(
                 "Unable to start the workflow run "
                 "- there are errors in the workflow definition."
@@ -171,17 +174,22 @@
         except (_exceptions.InvalidTokenError, _exceptions.ForbiddenError) as e:
             raise exceptions.UnauthorizedError(
                 "Could not get the workflow status for run with id "
                 f"`{workflow_run_id}` "
                 "- the authorization token was rejected by the remote cluster."
             ) from e
 
+    @_retry.retry(
+        attempts=5,
+        delay=0.2,
+        allowed_exceptions=(exceptions.WorkflowResultsNotReadyError,),
+    )
     def get_workflow_run_outputs_non_blocking(
         self, workflow_run_id: WorkflowRunId
-    ) -> Sequence[Any]:
+    ) -> Sequence[WorkflowResult]:
         """Non-blocking version of get_workflow_run_outputs.
 
         This method raises exceptions if the workflow output artifacts are not available
 
         Args:
             workflow_run_id: the ID of a workflow run
 
@@ -189,49 +197,77 @@
             WorkflowRunNotFound: if the workflow run cannot be found
             WorkflowRunNotSucceeded: if the workflow has not yet succeeded
             UnauthorizedError: if the remote cluster rejects the token
 
         Returns:
             the outputs associated with the workflow run
         """
+
         try:
             result_ids = self._client.get_workflow_run_results(workflow_run_id)
-        except (_exceptions.InvalidWorkflowRunID, _exceptions.WorkflowRunNotFound) as e:
+        except (
+            _exceptions.InvalidWorkflowRunID,
+            _exceptions.WorkflowRunNotFound,
+        ) as e:
             raise exceptions.WorkflowRunNotFoundError(
                 f"Workflow run with id `{workflow_run_id}` not found"
             ) from e
         except (_exceptions.InvalidTokenError, _exceptions.ForbiddenError) as e:
             raise exceptions.UnauthorizedError(
                 "Could not get the outputs for workflow run with id "
                 f"`{workflow_run_id}` "
                 "- the authorization token was rejected by the remote cluster."
             ) from e
 
         if len(result_ids) == 0:
             wf_run = self.get_workflow_run_status(workflow_run_id)
-            raise exceptions.WorkflowRunNotSucceeded(
-                f"Workflow run `{workflow_run_id}` is in state {wf_run.status.state}",
-                wf_run.status.state,
-            )
+            if wf_run.status.state == State.SUCCEEDED:
+                raise exceptions.WorkflowResultsNotReadyError(
+                    f"Workflow run `{workflow_run_id}` has succeded, but the results "
+                    "are not ready yet.\n"
+                    "After a workflow completes, there may be a short delay before the "
+                    "results are ready to download. Please try again!"
+                )
+            else:
+                raise exceptions.WorkflowRunNotSucceeded(
+                    f"Workflow run `{workflow_run_id}` is in state "
+                    f"{wf_run.status.state}",
+                    wf_run.status.state,
+                )
 
-        assert len(result_ids) == 1, "We're currently expecting a single result."
+        assert len(result_ids) == 1, "Assuming a single output"
 
         try:
-            wf_result = self._client.get_workflow_run_result(result_ids[0])
-            return tuple(serde.deserialize(wf_result))
+            result = self._client.get_workflow_run_result(result_ids[0])
         except (_exceptions.InvalidTokenError, _exceptions.ForbiddenError) as e:
             raise exceptions.UnauthorizedError(
                 "Could not get the outputs for workflow run with id "
                 f"`{workflow_run_id}` "
                 "- the authorization token was rejected by the remote cluster."
             ) from e
 
+        if not isinstance(result, ComputeEngineWorkflowResult):
+            # It's a WorkflowResult.
+            # We need to match the old way of storing results into the new way
+            # this is done by unpacking the deserialised values and re-serialising.
+            # This is unfortunate, but should only happen for <0.47.0 workflow runs.
+            # Example:
+            #   We get JSONResult([100, "json_string"]) from the API
+            #   We need (JSONResult(100), JSONResult("json_string"))
+            deserialised_results = serde.deserialize(result)
+            return tuple(
+                serde.result_from_artifact(unpacked, ArtifactFormat.AUTO)
+                for unpacked in deserialised_results
+            )
+        else:
+            return result.results
+
     def get_available_outputs(
         self, workflow_run_id: WorkflowRunId
-    ) -> Dict[TaskInvocationId, Union[ArtifactValue, Tuple[ArtifactValue, ...]]]:
+    ) -> Dict[TaskInvocationId, WorkflowResult]:
         """Returns all available outputs for a workflow
 
         This method returns all available artifacts. When the workflow fails
         it returns artifacts only for the steps that did success.
         Might raise an exception if runtime doesn't support getting artifacts from
         in-progress workflow
 
@@ -259,34 +295,28 @@
         except (_exceptions.InvalidTokenError, _exceptions.ForbiddenError) as e:
             raise exceptions.UnauthorizedError(
                 "Could not get the outputs for workflow run with id "
                 f"`{workflow_run_id}` "
                 "- the authorization token was rejected by the remote cluster."
             ) from e
 
-        artifact_vals: Dict[
-            TaskInvocationId, Union[ArtifactValue, Tuple[ArtifactValue]]
-        ] = {}
+        artifact_vals: Dict[TaskInvocationId, WorkflowResult] = {}
 
         for task_run_id, artifact_ids in artifact_map.items():
             inv_id = self._invocation_id_by_task_run_id(workflow_run_id, task_run_id)
-            outputs = []
-            for artifact_id in artifact_ids:
-                try:
-                    output = serde.deserialize(
-                        self._client.get_workflow_run_artifact(artifact_id)
-                    )
-                except Exception:
-                    # If we fail for any reason, this artifact wasn't available yet
-                    continue
-                outputs.append(output)
-
-            if len(outputs) > 0:
-                # We don't want to litter the dictionary with empty containers.
-                artifact_vals[inv_id] = tuple(outputs)
+            assert (
+                len(artifact_ids) == 1
+            ), "Expecting a single artifact containing the packed values from the task"
+            try:
+                artifact_vals[inv_id] = self._client.get_workflow_run_artifact(
+                    artifact_ids[0]
+                )
+            except Exception:
+                # If we fail for any reason, this artifact wasn't available yet
+                continue
 
         return artifact_vals
 
     def _invocation_id_by_task_run_id(
         self, wf_run_id: WorkflowRunId, task_run_id: TaskRunId
     ) -> TaskInvocationId:
         # We shouldn't expect any particular format of the task run ID.
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_driver/_client.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_driver/_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,25 +8,29 @@
     https://github.com/zapatacomputing/workflow-driver/tree/2b3534/openapi
 """
 
 import io
 import json
 import zlib
 from tarfile import TarFile
-from typing import Generic, List, Mapping, Optional, TypeVar
+from typing import Generic, List, Mapping, Optional, Tuple, TypeVar, Union
 from urllib.parse import urljoin
 
 import pydantic
 import requests
 from requests import codes
 
 from orquestra.sdk._ray._ray_logs import WFLog
 from orquestra.sdk.schema.ir import WorkflowDef
-from orquestra.sdk.schema.responses import WorkflowResult
-from orquestra.sdk.schema.workflow_run import WorkflowRun, WorkflowRunMinimal
+from orquestra.sdk.schema.responses import ComputeEngineWorkflowResult, WorkflowResult
+from orquestra.sdk.schema.workflow_run import (
+    ProjectRef,
+    WorkflowRun,
+    WorkflowRunMinimal,
+)
 
 from . import _exceptions, _models
 
 API_ACTIONS = {
     # Workflow Definitions
     "create_workflow_def": "/api/workflow-definitions",
     "list_workflow_defs": "/api/workflow-definitions",
@@ -139,48 +143,67 @@
             urljoin(self._base_uri, endpoint),
             params=query_params,
             allow_redirects=allow_redirects,
         )
 
         return response
 
-    def _post(self, endpoint: str, body_params: Optional[Mapping]) -> requests.Response:
+    def _post(
+        self,
+        endpoint: str,
+        body_params: Optional[Mapping],
+        query_params: Optional[Mapping] = None,
+    ) -> requests.Response:
         """Helper method for POST requests"""
         response = self._session.post(
             urljoin(self._base_uri, endpoint),
             json=body_params,
+            params=query_params,
         )
         return response
 
     def _delete(self, endpoint: str) -> requests.Response:
         """Helper method for DELETE requests"""
         response = self._session.delete(urljoin(self._base_uri, endpoint))
 
         return response
 
     # --- queries ---
 
     # ---- Worklow Defs ----
 
-    def create_workflow_def(self, workflow_def: WorkflowDef) -> _models.WorkflowDefID:
+    def create_workflow_def(
+        self,
+        workflow_def: WorkflowDef,
+        project: Optional[ProjectRef],
+    ) -> _models.WorkflowDefID:
         """
         Stores a workflow definition for future submission
 
         Raises:
             InvalidWorkflowDef: see the exception's docstring
             InvalidTokenError: see the exception's docstring
             ForbiddenError: see the exception's docstring
             UnknownHTTPError: see the exception's docstring
 
         Returns:
             the WorkflowDefID associated with the stored definition
         """
+        query_params = (
+            _models.CreateWorkflowDefsRequest(
+                workspaceId=project.workspace_id,
+                projectId=project.project_id,
+            ).dict()
+            if project
+            else None
+        )
         resp = self._post(
             API_ACTIONS["create_workflow_def"],
             body_params=workflow_def.dict(),
+            query_params=query_params,
         )
 
         if resp.status_code == codes.BAD_REQUEST:
             error = _models.Error.parse_obj(resp.json())
             raise _exceptions.InvalidWorkflowDef(
                 message=error.message, detail=error.detail
             )
@@ -530,15 +553,15 @@
             _models.GetWorkflowRunResultsResponse, _models.MetaEmpty
         ].parse_obj(resp.json())
 
         return parsed_response.data
 
     def get_workflow_run_result(
         self, result_id: _models.WorkflowRunResultID
-    ) -> WorkflowResult:
+    ) -> Union[WorkflowResult, ComputeEngineWorkflowResult]:
         """
         Gets workflow run results from the workflow driver
 
         Raises:
             InvalidWorkflowRunResultID: see the exception's docstring
             WorkflowRunResultNotFound: see the exception's docstring
             InvalidTokenError: see the exception's docstring
@@ -553,19 +576,36 @@
         if resp.status_code == codes.NOT_FOUND:
             raise _exceptions.WorkflowRunResultNotFound(result_id)
         elif resp.status_code == codes.BAD_REQUEST:
             raise _exceptions.InvalidWorkflowRunResultID(result_id)
 
         _handle_common_errors(resp)
 
-        # Bug with mypy and Pydantic:
-        #   Unions cannot be passed to parse_obj_as: pydantic/pydantic#1847
-        return pydantic.parse_obj_as(
-            WorkflowResult, resp.json()  # type: ignore[arg-type]
-        )
+        # To ensure the correct ordering of results, we serialize the results on CE as:
+        # {
+        #   "results": [
+        #       (JSONResult | PickleResult).json(),
+        #       (JSONResult | PickleResult).json(),
+        #       ...
+        #   ]
+        # } aka a ComputeEngineWorkflowResult.json()
+        # For older workflows, we respond with:
+        # (JSONResult | PickleResult).json()
+
+        json_response = resp.json()
+        try:
+            # Try an older response
+            # Bug with mypy and Pydantic:
+            #   Unions cannot be passed to parse_obj_as: pydantic/pydantic#1847
+            return pydantic.parse_obj_as(
+                WorkflowResult, json_response  # type: ignore[arg-type]
+            )
+        except pydantic.ValidationError:
+            # If we fail, try parsing each part of a list separately
+            return ComputeEngineWorkflowResult.parse_obj(json_response)
 
     # --- Workflow Logs ---
 
     def get_workflow_run_logs(self, wf_run_id: _models.WorkflowRunID) -> List[str]:
         """
         Gets the logs of a workflow run from the workflow driver
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_driver/_exceptions.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_driver/_exceptions.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_driver/_models.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_driver/_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,24 @@
         https://github.com/zapatacomputing/workflow-driver/blob/cdb667ef6d1053876250daff27e19fb50374c0d4/openapi/src/resources/workflow-definitions.yaml#L8
     """
 
     pageSize: Optional[int]
     pageToken: Optional[str]
 
 
+class CreateWorkflowDefsRequest(pydantic.BaseModel):
+    """
+    Implements:
+        https://github.com/zapatacomputing/workflow-driver/blob/dc8a2a37d92324f099afefc048f6486a5061850f/openapi/src/resources/workflow-definitions.yaml#L39
+    """
+
+    workspaceId: Optional[str]
+    projectId: Optional[str]
+
+
 ListWorkflowDefsResponse = List[GetWorkflowDefResponse]
 
 # --- Workflow Runs ---
 
 
 class StateResponse(str, Enum):
     """
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_dsl.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_dsl.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,17 +42,14 @@
 import wrapt  # type: ignore
 
 from ..exceptions import DirtyGitRepo, InvalidTaskDefinitionError, WorkflowSyntaxError
 from . import _ast
 
 DIRECT_EXECUTION = False
 
-DEFAULT_IMAGE = "zapatacomputing/orquestra-default:v0.0.0"
-GPU_IMAGE = "zapatacomputing/orquestra-nvidia:v0.0.0"
-
 
 # ----- SDK exceptions  -----
 
 
 class NoRemoteRepo(Exception):
     pass
 
@@ -67,15 +64,19 @@
 
 class UnknownPlaceholderInCustomNameWarning(Warning):
     pass
 
 
 # ----- data structures -----
 
+# Type alias used to mark variables expected to hold raw constant values.
 Constant = Any
+# Type alias used to mark variables that can be used as task arguments. These are the
+# graph nodes that can represent data (contrary to task invocations that represent
+# function calls).
 Argument = Union[Constant, "ArtifactFuture", "Secret"]
 
 
 class Secret(NamedTuple):
     name: str
     # Config name is only used for the local runtimes where we can't infer the location
     # where we get a secret's value from.
@@ -457,20 +458,14 @@
         self._use_default_dependency_imports = dependency_imports is None
         self._source_import = source_import
         self._use_default_source_import = source_import is None
 
         # task itself is not part of any workflow yet. Don't pass wf defaults
         self._resolve_task_source_data()
 
-        if self._custom_image is None:
-            if resources.gpu:
-                self._custom_image = GPU_IMAGE
-            else:
-                self._custom_image = DEFAULT_IMAGE
-
     @property
     def n_outputs(self):
         warnings.warn(
             '"n_outputs" is deprecated. Please use "output_metadata".',
             DeprecationWarning,
         )
         return self._output_metadata.n_outputs
@@ -642,20 +637,23 @@
     #
     # Add more cases here when we allow users to specify artifact format explicitly.
     # This has to be accompanied by corresponding implementation in orquestra.sdk._base.
     AUTO = "AUTO"
 
 
 class ArtifactFuture:
+    DEFAULT_CUSTOM_NAME = None
+    DEFAULT_SERIALIZATION_FORMAT = ArtifactFormat.AUTO
+
     def __init__(
         self,
         invocation: TaskInvocation,
         output_index: Optional[int] = None,
-        custom_name: Optional[str] = None,
-        serialization_format: ArtifactFormat = ArtifactFormat.AUTO,
+        custom_name: Optional[str] = DEFAULT_CUSTOM_NAME,
+        serialization_format: ArtifactFormat = DEFAULT_SERIALIZATION_FORMAT,
     ):
         self.invocation = invocation
         # if the invocation returns multiple values, this the index in the output
         # sequence
         self.output_index = output_index
         # metadata below
         self.custom_name = custom_name
@@ -1054,106 +1052,7 @@
 
         return task_def
 
     if fn is None:
         return _inner
     else:
         return _inner(fn)
-
-
-# ----- utilities -----
-
-
-# NOTE: we have both `external_file_task` and `external_module_task` because they
-# refer to functions in different ways.
-#
-# - `external_file_task` - uses `FileFunctionRef`, exists for backwards compatibility
-#     with Orquestra v1. For details how Python functions are called there, see:
-#     https://github.com/zapatacomputing/python3-runtime/blob/af4cd913ba1f35db792c939f578bbb968364ede1/run#L319
-#
-# - `external_module_task` - uses `ModuleFunctionRef`, allows referring to functions by
-#     the "fully qualified name", like `numpy.testing.assert_array_equal`. It's more
-#     general than `FileFunctionRef`, as it allows to call a function that's a part of
-#     any module in a given Python process. It would be nice to encourage using this
-#     in the future (vs `FileFunctionRef`).
-
-
-def external_file_task(
-    file_path: str,
-    function: str,
-    repo_url: str,
-    git_ref: Optional[str] = None,
-    resources: Resources = Resources(),
-    n_outputs: Optional[int] = None,
-):
-    def _proxy(*args, **kwargs):
-        raise ValueError(
-            f"Attempted to execute a task that's only a proxy. Call "
-            f"{file_path}:{function} instead."
-        )
-
-    _proxy.__name__ = function
-
-    git_ref = git_ref or "main"
-
-    if n_outputs is None:
-        warnings.warn(
-            "External tasks cannot be inspected and default to 1 (one) output. "
-            "Explicitly pass the number of outputs to hide this warning."
-        )
-        output_metadata = TaskOutputMetadata(is_subscriptable=False, n_outputs=1)
-    else:
-        # Assume if a user has specified the number of outputs, then this output is
-        # subscriptable
-        output_metadata = TaskOutputMetadata(is_subscriptable=True, n_outputs=n_outputs)
-
-    return TaskDef(
-        fn=_proxy,
-        fn_ref=FileFunctionRef(
-            file_path=file_path,
-            function_name=function,
-        ),
-        source_import=GitImport(repo_url=repo_url, git_ref=git_ref),
-        resources=resources,
-        output_metadata=output_metadata,
-    )
-
-
-def external_module_task(
-    module: str,
-    function: str,
-    repo_url: str,
-    git_ref: Optional[str] = None,
-    resources: Resources = Resources(),
-    n_outputs: Optional[int] = None,
-):
-    def _proxy(*args, **kwargs):
-        raise ValueError(
-            f"Attempted to execute a task that's only a proxy. Call "
-            f"{module}.{function} instead."
-        )
-
-    _proxy.__name__ = function
-
-    git_ref = git_ref or "main"
-
-    if n_outputs is None:
-        warnings.warn(
-            "External tasks cannot be inspected and default to 1 (one) output. "
-            "Explicitly pass the number of outputs to hide this warning."
-        )
-        output_metadata = TaskOutputMetadata(is_subscriptable=False, n_outputs=1)
-    else:
-        # Assume if a user has specified the number of outputs, then this output is
-        # subscriptable
-        output_metadata = TaskOutputMetadata(is_subscriptable=True, n_outputs=n_outputs)
-
-    return TaskDef(
-        fn=_proxy,
-        fn_ref=ModuleFunctionRef(
-            module=module,
-            function_name=function,
-        ),
-        source_import=GitImport(repo_url=repo_url, git_ref=git_ref),
-        resources=resources,
-        output_metadata=output_metadata,
-    )
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_env.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_env.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_exec_ctx.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_exec_ctx.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_factory.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_factory.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_git_url_utils.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_git_url_utils.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_graphs.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_graphs.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_in_process_runtime.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_in_process_runtime.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 ################################################################################
 # © Copyright 2022-2023 Zapata Computing Inc.
 ################################################################################
 import typing as t
+import warnings
 from datetime import datetime, timedelta, timezone
 
+from orquestra.sdk import exceptions
 from orquestra.sdk._base import abc
 from orquestra.sdk.schema import ir
+from orquestra.sdk.schema.responses import WorkflowResult
 from orquestra.sdk.schema.workflow_run import (
+    ProjectRef,
     RunStatus,
     State,
     TaskRun,
     TaskRunId,
     WorkflowRun,
     WorkflowRunId,
 )
 
 from .. import secrets
 from ..exceptions import WorkflowRunNotFoundError
+from . import serde
 from ._graphs import iter_invocations_topologically
 from .dispatch import locate_fn_ref
-from .serde import deserialize_constant
 
 WfRunId = str
 ArtifactValue = t.Any
 TaskOutputs = t.Tuple[ArtifactValue, ...]
 
 
 def _make_completed_task_run(workflow_run_id, start_time, end_time, task_inv):
@@ -82,22 +86,32 @@
         self._workflow_def_store: t.Dict[WfRunId, ir.WorkflowDef] = {}
         self._start_time_store: t.Dict[WfRunId, datetime] = {}
         self._end_time_store: t.Dict[WfRunId, datetime] = {}
 
     def _gen_next_run_id(self, wf_def: ir.WorkflowDef):
         return f"{wf_def.name}-{len(self._output_store) + 1}"
 
-    def create_workflow_run(self, workflow_def: ir.WorkflowDef) -> WfRunId:
+    def create_workflow_run(
+        self, workflow_def: ir.WorkflowDef, project: t.Optional[ProjectRef]
+    ) -> WfRunId:
+
+        if project:
+            warnings.warn(
+                "in_process runtime doesn't support project-scoped workflows. "
+                "Project and workspace IDs will be ignored.",
+                category=exceptions.UnsupportedRuntimeFeature,
+            )
+
         run_id = self._gen_next_run_id(workflow_def)
 
         self._start_time_store[run_id] = datetime.now(timezone.utc)
 
         # We deserialize the constants in one go, instead of as needed
         consts: t.Dict[ir.ConstantNodeId, t.Any] = {
-            id: deserialize_constant(node)
+            id: serde.deserialize(node)
             for id, node in workflow_def.constant_nodes.items()
         }
         for id, secret in workflow_def.secret_nodes.items():
             consts[id] = secrets.get(
                 secret.secret_name, config_name=secret.secret_config
             )
         # We'll store artifacts for this run here.
@@ -130,46 +144,60 @@
                         artifact.artifact_index
                     ]
 
         # Ordinary functions return `obj` or `tuple(obj, obj)`
         outputs = tuple(
             _get_args(consts, self._artifact_store[run_id], workflow_def.output_ids)
         )
-        self._output_store[run_id] = outputs[0] if len(outputs) == 1 else outputs
+        self._output_store[run_id] = outputs
 
         self._end_time_store[run_id] = datetime.now(timezone.utc)
         self._workflow_def_store[run_id] = workflow_def
         return run_id
 
     def get_workflow_run_outputs_non_blocking(
         self, workflow_run_id: WfRunId
-    ) -> t.Sequence[t.Any]:
-        return self._output_store[workflow_run_id]
+    ) -> t.Tuple[WorkflowResult, ...]:
+        return (
+            *(
+                serde.result_from_artifact(output, ir.ArtifactFormat.AUTO)
+                for output in self._output_store[workflow_run_id]
+            ),
+        )
 
     def get_available_outputs(
         self, workflow_run_id: WfRunId
-    ) -> t.Dict[ir.TaskInvocationId, TaskOutputs]:
+    ) -> t.Dict[ir.TaskInvocationId, WorkflowResult]:
         wf_def = self._workflow_def_store[workflow_run_id]
 
-        inv_outputs: t.Dict[ir.TaskInvocationId, TaskOutputs] = {}
+        inv_outputs: t.Dict[ir.TaskInvocationId, WorkflowResult] = {}
         for inv in wf_def.task_invocations.values():
-            output_vals = tuple(
-                [
-                    self._artifact_store[workflow_run_id][art_id]
-                    for art_id in inv.output_ids
-                ]
-            )
+            # Assumption there's always a non-unpacked artifact. We want to return
+            # whatever shape was returned from the task function so we can use the
+            # "packed" artifact. For more info on artifact unpacking, see
+            # "orquestra.sdk._base._traversal".
+
+            artifact_nodes = [wf_def.artifact_nodes[id] for id in inv.output_ids]
+            packed_nodes = [n for n in artifact_nodes if n.artifact_index is None]
+            assert (
+                len(packed_nodes) == 1
+            ), f"Task invocation should have exactly 1 packed output. {inv.id} has {len(packed_nodes)}: {packed_nodes}"  # noqa: E501
+            packed_artifact = packed_nodes[0]
+
+            task_result = self._artifact_store[workflow_run_id][packed_artifact.id]
 
-            inv_outputs[inv.id] = output_vals
+            inv_outputs[inv.id] = serde.result_from_artifact(
+                task_result, ir.ArtifactFormat.AUTO
+            )
 
         return inv_outputs
 
     def get_workflow_run_status(self, workflow_run_id: WfRunId) -> WorkflowRun:
         if workflow_run_id not in self._output_store:
-            raise WorkflowRunNotFoundError(
+            raise exceptions.WorkflowRunNotFoundError(
                 f"Workflow with id {workflow_run_id} not found"
             )
         workflow_def = self._workflow_def_store[workflow_run_id]
         start_time = self._start_time_store[workflow_run_id]
         end_time = self._end_time_store[workflow_run_id]
         return WorkflowRun(
             id=workflow_run_id,
@@ -193,15 +221,15 @@
             # stopped, by definition of the InProcessRuntime. If the user is running
             # the workflow using the InProcessRuntime the only way to call this method
             # would be after the workflow has finished, or in a different process.
             # We don't do IPC for this runtime class.
             pass
         else:
             # We didn't see this workflow run.
-            raise WorkflowRunNotFoundError(
+            raise exceptions.WorkflowRunNotFoundError(
                 f"Workflow with id {workflow_run_id} not found"
             )
 
     def list_workflow_runs(
         self,
         *,
         limit: t.Optional[int] = None,
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_log_adapter.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_log_adapter.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_qe/_client.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_qe/_client.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_qe/_qe_runtime.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_qe/_qe_runtime.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,33 +5,43 @@
 import gzip
 import io
 import json
 import re
 import sqlite3
 import sys
 import tarfile
+import warnings
 from contextlib import contextmanager
 from datetime import datetime, timedelta, timezone
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
+import pydantic
 import requests
 
 from orquestra.sdk import exceptions
 from orquestra.sdk._base import serde
 from orquestra.sdk._base._conversions._yaml_exporter import (
     pydantic_to_yaml,
     workflow_to_yaml,
 )
 from orquestra.sdk._base._db import WorkflowDB
 from orquestra.sdk._base.abc import RuntimeInterface
 from orquestra.sdk.schema.configs import RuntimeConfiguration
-from orquestra.sdk.schema.ir import TaskInvocation, TaskInvocationId, WorkflowDef
+from orquestra.sdk.schema.ir import (
+    ArtifactFormat,
+    ArtifactNodeId,
+    TaskInvocation,
+    TaskInvocationId,
+    WorkflowDef,
+)
 from orquestra.sdk.schema.local_database import StoredWorkflowRun
+from orquestra.sdk.schema.responses import WorkflowResult
 from orquestra.sdk.schema.workflow_run import (
+    ProjectRef,
     RunStatus,
     State,
     TaskRun,
     TaskRunId,
     WorkflowRun,
     WorkflowRunId,
 )
@@ -197,37 +207,55 @@
     """
     return {
         task_invocation_id: task_invocation
         for task_invocation_id, task_invocation in wf_def.task_invocations.items()
     }
 
 
-def _parse_workflow_result(result_bytes: bytes) -> Dict[str, Dict]:
-    """Parse a workflow run result
+def _extract_results(result_bytes: bytes) -> Dict[str, Any]:
+    """
+    Extract the raw bytes we get from QE
 
     Args:
-        result_bytes: bytes received from QE from '/v2/workflows/{id}/result'
+        result_bytes: bytes received from QE, either a result or an artifact
 
     Returns:
-        A nested dictionary. Level 1 keys are QE step IDs. The level 2 keys
-            are QE artifact names as well as:
-            - 'inputs'
-            - 'stepID'
-            - 'stepName'
-            - 'workflowId'
+        A dictionary loaded by the JSON we extract.
+        This JSON is context dependent.
+
     Raises:
-        IndexError: when the `result_bytes` is not a archive we expect.
+        NotFoundError: when the `result_bytes` is not a archive we expect.
     """
-
     try:
         return extract_result_json(result_bytes)
     except IndexError as e:
         raise exceptions.NotFoundError("Invalid archive") from e
 
 
+def _parse_workflow_result(result_bytes: bytes) -> WorkflowResult:
+    """
+    Parse bytes to a WorkflowResult
+
+    Args:
+        result_bytes: bytes received from QE
+
+    Returns:
+        A parsed WorkflowResult
+
+    Raises:
+        NotFoundError: when the `result_bytes` is not a archive we expect.
+            From _extract_results
+    """
+
+    result_json = _extract_results(result_bytes)
+    # Bug with mypy and Pydantic:
+    #   Unions cannot be passed to parse_obj_as: pydantic/pydantic#1847
+    return pydantic.parse_obj_as(WorkflowResult, result_json)  # type: ignore[arg-type] # noqa: E501
+
+
 def extract_result_json(tgz_bytes: bytes) -> Dict:
     # Treat the response as a tgz file and extract the workflow result JSON
     fileobj = io.BytesIO(tgz_bytes)
     with tarfile.open(mode="r:gz", fileobj=fileobj) as tar:
         # TODO: Assuming result is the only file in the tgz
         file_to_extract = tar.getmembers()[0]
         file_buf = tar.extractfile(file_to_extract)
@@ -338,14 +366,31 @@
                 "Try reducing the size of your workflow either by using fewer tasks or "
                 "contact Zapata support for more assistance."
             ) from e
         else:
             raise e
 
 
+def _find_packed_artifact_id(
+    wf_def: WorkflowDef, inv_id: TaskInvocationId
+) -> Optional[ArtifactNodeId]:
+    output_ids = wf_def.task_invocations[inv_id].output_ids
+    artifact_nodes = (wf_def.artifact_nodes[id] for id in output_ids)
+    packed_nodes = [n for n in artifact_nodes if n.artifact_index is None]
+
+    if (n_packed := len(packed_nodes)) == 0:
+        return None
+
+    assert (
+        n_packed == 1
+    ), f"Task invocation should have no more than 1 packed output. {inv_id} has {n_packed}: {packed_nodes}"  # noqa: E501
+
+    return packed_nodes[0].id
+
+
 class QERuntime(RuntimeInterface):
     def __init__(
         self,
         config: RuntimeConfiguration,
         project_dir: Path,
         verbose: bool = False,
     ):
@@ -461,29 +506,64 @@
                 "- consist only of lowercase alphanumeric characters, '-', '_', "
                 "or '.'\n"
                 "- start and end with an alphanumeric character\n"
                 "Potential workflow names can be checked here: "
                 "https://regex101.com/r/CxEZKW/1"
             )
 
-    def create_workflow_run(self, workflow_def: WorkflowDef) -> WorkflowRunId:
+    def _handle_legacy_qe_result(
+        self, workflow_run_id: WorkflowRunId, task_invocation: TaskInvocation
+    ) -> WorkflowResult:
+        task_results = []
+        for artifact_id in task_invocation.output_ids:
+            # Let http errors bubble up to caller
+            result = self._client.get_artifact(
+                workflow_run_id, task_invocation.id, artifact_id
+            )
+            # QERuntime.get_available_outputs is expected to return a WorkflowResult
+            # We need to deserialize the unpacked values, pack them, then serialize
+            parsed_output = serde.deserialize(_parse_workflow_result(result))
+            # This is where we pack the deserialized values
+            task_results.append(parsed_output)
+        # Finally, we serialize the packed values, mimicking how Python functions work
+        if len(task_results) == 0:
+            # No outputs mean we return `None`
+            return serde.result_from_artifact(None, ArtifactFormat.AUTO)
+        elif len(task_results) == 1:
+            # A single output means we return the value
+            return serde.result_from_artifact(task_results[0], ArtifactFormat.AUTO)
+        else:
+            # Multiple outputs mean we return a tuple
+            return serde.result_from_artifact(tuple(task_results), ArtifactFormat.AUTO)
+
+    def create_workflow_run(
+        self, workflow_def: WorkflowDef, project: Optional[ProjectRef]
+    ) -> WorkflowRunId:
         """
         Submits a workflow to the Quantum Engine
 
         Args:
             workflow_def: The workflow definition to submit
+            project: Unused on QE runtime
 
         Returns:
             A workflow run id, created by QE
 
         Raises:
             orquestra.sdk.exceptions.UnauthorizedError if QE returns 401
             orquestra.sdk.exceptions.InvalidWorkflowDefinitionError if the
                 workflow definition name does not conform to QE requirements.
         """
+        if project:
+            warnings.warn(
+                "QE runtime doesn't support project-scoped workflows. "
+                "Project and workspace IDs will be ignored.",
+                category=exceptions.UnsupportedRuntimeFeature,
+            )
+
         if self._verbose:
             print_yaml_of_workflow(workflow_def)
 
         self._check_workflow_name(workflow_def.name)
 
         try:
             qe_workflow = workflow_to_yaml(workflow_def)
@@ -581,29 +661,30 @@
             raise exceptions.WorkflowRunNotSucceeded(
                 f"Workflow Run {workflow_run_id} is {workflow_status.status.state}",
                 workflow_status.status.state,
             )
 
         with _http_error_handling():
             result_bytes = self._client.get_workflow_result(workflow_run_id)
-        result_dict = _parse_workflow_result(result_bytes)
+        result_dict = _extract_results(result_bytes)
         task_invocations = _get_task_invocations(wf_def)
         artifacts = _get_artifacts(task_invocations, result_dict)
 
         # 1. Find the output IDs from the workflow def
         # 2, Find the artifact from the artifact dict
-        # 3. Deserialise the artifact
-        # 4. Append the artifact to the outputs list
-        # 5. ???
-        # 6. Profit
+        # 3. Append the artifact to the outputs tuple
+        # 4. ???
+        # 5. Profit
         output_ids = wf_def.output_ids
 
+        # Bug with mypy and Pydantic:
+        #   Unions cannot be passed to parse_obj_as: pydantic/pydantic#1847
         return (
             *(
-                serde.value_from_result_dict(artifacts[output_id])
+                pydantic.parse_obj_as(WorkflowResult, artifacts[output_id])  # type: ignore[arg-type] # noqa: E501
                 for output_id in output_ids
             ),
         )
 
     def get_available_outputs(self, workflow_run_id: WorkflowRunId):
         """Returns all available output artifacts of a workflow
         run even if workflow failed
@@ -622,41 +703,45 @@
              a dictionary of:
                  task invocation IDs: value returned from each invocation
         """
         with WorkflowDB.open_project_db(self._project_dir) as db:
             wf_run = db.get_workflow_run(workflow_run_id)
         wf_def = wf_run.workflow_def
         # Return dict contains return values for task invocation
-        return_dict = {}
+        return_dict: Dict[str, WorkflowResult] = {}
         with _http_error_handling():
-            # retrieve each artifact for each step
-            for step in wf_def.task_invocations:
-                step_artifacts = []
-                for artifact in wf_def.task_invocations[step].output_ids:
-                    try:
-                        result = self._client.get_artifact(
-                            workflow_run_id, step, artifact
+            # Assumption: task invocations produce "packed" and "unpacked" artifacts.
+            # We want to fetch whatever object was returned from the task function, so
+            # we only need the "packed" artifact. For more info on artifact unpacking,
+            # see "orquestra.sdk._base._traversal".
+            # If we don't have a packed artifact, then this is an older QE result that
+            # was unpacked. In this case, we'll just return what we have.
+            for inv in wf_def.task_invocations.values():
+                packed_id = _find_packed_artifact_id(wf_def, inv.id)
+                try:
+                    if packed_id is None:
+                        artifact_value = self._handle_legacy_qe_result(
+                            workflow_run_id, inv
+                        )
+                    else:
+                        artifact_bytes = self._client.get_artifact(
+                            workflow_id=workflow_run_id,
+                            step_name=inv.id,
+                            artifact_name=packed_id,
                         )
-                    except requests.exceptions.HTTPError as e:
-                        # 404 error happens when task is not finished yet.
-                        # 500 error is thrown by QE in case of failed task
-                        if (
-                            e.response.status_code == 404
-                            or e.response.status_code == 500
-                        ):
-                            continue
-                        else:
-                            raise e
-                    parsed_output = serde.value_from_result_dict(
-                        _parse_workflow_result(result)
-                    )
-
-                    step_artifacts.append(parsed_output)
-                if step_artifacts:
-                    return_dict[step] = tuple(step_artifacts)
+                        artifact_value = _parse_workflow_result(artifact_bytes)
+                except requests.exceptions.HTTPError as e:
+                    # 404 error happens when task is not finished yet.
+                    # 500 error is thrown by QE in case of failed task.
+                    if e.response.status_code == 404 or e.response.status_code == 500:
+                        continue
+                    else:
+                        raise e
+
+                return_dict[inv.id] = artifact_value
 
         return return_dict
 
     def get_task_logs(
         self, wf_run_id: WorkflowRunId, task_inv_id: TaskInvocationId
     ) -> List[str]:
         """
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_services.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_services.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_testing/_connections.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_testing/_connections.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             # that a PermissionError might happen at the time of removal of ray temp
             # dir. It should be fine to ignore it, as temporary directories should be
             # pruned by the OS anyway.
             pass
 
 
 @contextmanager
-def make_ray_conn() -> t.Iterator[_dag.RayParams]:
+def make_ray_conn(storage_path: t.Optional[str] = None) -> t.Iterator[_dag.RayParams]:
     """
     Initializes ray connection. By default, starts a linked cluster on its
     own.
     Can be changed to run against a background cluster that needs to
     be started separately ('ray start --head'). To do that, set the
     'RAY_CLUSTER_URL' env variable. `RAY_CLUSTER_URL="auto"` tells Ray to
     discover a running cluster.
@@ -81,21 +81,21 @@
             ray_temp_dir = None
         else:
             # No env var value? => Starting a linked cluster.
             # - Use the Ray's magic constant value for starting the cluster.
             # - Need to pass storage path (workflow data)
             # - Need to pass temp dir (Ray log files location).
             address = "local"
-            storage_path = tmp_path / "ray" / "storage"
-            ray_temp_dir = tmp_path / "ray" / "tmp"
+            storage_path = storage_path or str(tmp_path / "ray" / "storage")
+            ray_temp_dir = str(tmp_path / "ray" / "tmp")
         params = _dag.RayParams(
             address=address,
             log_to_driver=False,
-            storage=str(storage_path),
-            _temp_dir=str(ray_temp_dir),
+            storage=storage_path,
+            _temp_dir=ray_temp_dir,
         )
 
         # Ray plugs in its own breakpoint entrypoint during 'ray.init()', but
         # unfortunately it wrecks the PDB in pytest. To workaround this we can
         # bring back the old handler after initializing Ray connection.
         breakpoint_handler = os.environ.get("PYTHONBREAKPOINT", "")
         _dag.RayRuntime.startup(params)
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_testing/_example_wfs.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_testing/_example_wfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,16 +118,18 @@
     return [full_name, company_cap]
 
 
 @sdk.workflow
 def multioutput_task_wf():
     a, b = multioutput_task()
     _, c = multioutput_task()
-    d = multioutput_task()
-    return a, b, c, d
+    d, _ = multioutput_task()
+    packed = multioutput_task()
+    f, g = packed
+    return a, b, c, d, packed, f, g
 
 
 @sdk.workflow
 def my_workflow():
     first_name = "alex"
     last_name = "zapata"
     _, there = multi_output_test()
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_traversal.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_traversal.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,30 +6,26 @@
 The main highlight is `flatten_graph()`.
 """
 
 import collections.abc
 import hashlib
 import inspect
 import re
-import sys
 import typing as t
 import warnings
-from collections import OrderedDict, defaultdict
+from collections import OrderedDict
 from functools import singledispatch
 
-from packaging.version import parse as parse_version
 from pip_api import Requirement
 
-import orquestra.sdk.schema.ir as model
-from orquestra.sdk.exceptions import NodesInTaskResourcesWarning
-from orquestra.sdk.schema import responses
+from orquestra.sdk.schema import ir, responses
 
 from .. import exceptions
-from ..packaging import get_installed_version
-from . import _dsl, _git_url_utils, _workflow, serde
+from ..packaging._versions import get_current_python_version, get_current_sdk_version
+from . import _dsl, _exec_ctx, _git_url_utils, _workflow, serde
 
 N_BYTES_IN_HASH = 8
 
 
 def _make_key(obj: t.Any):
     """Returns a hashable key for all types
 
@@ -70,92 +66,265 @@
 
 def _gen_id_hash(*args):
     bytes = b"".join(map(_hash_or_repr_bytes, args))
     shake = hashlib.shake_256(bytes)
     return shake.hexdigest(5)
 
 
-def _make_artifact_id(source_task: _dsl.TaskDef, future_index: int):
-    return _qe_compliant_name(f"artifact-{future_index}-{source_task._fn_name}")
+def _make_artifact_id(source_task: _dsl.TaskDef, wf_scoped_artifact_index: int):
+    return _qe_compliant_name(
+        f"artifact-{wf_scoped_artifact_index}-{source_task._fn_name}"
+    )
 
 
-GraphNode = t.Union[_dsl.ArtifactFuture, _dsl.Constant, _dsl.Secret]
+# DSL object that represents a data node in the workflow graph. Data nodes are
+# constants, secrets, artifact futures, but not task invocations.
+DSLDataNode = _dsl.Argument
 
 
 class GraphTraversal:
     def __init__(self):
-        self._artifacts = {}
-        self._invocations = {}
-        self._secrets = {}
-        self._constants = {}
+        self._secrets: t.MutableMapping[t.Hashable, ir.SecretNode] = {}
+        self._constants: t.MutableMapping[t.Hashable, ir.ConstantNode] = {}
+
+        # Running a task invocation results in values. The values are stored in
+        # artifacts. Some of the values can be subscripted. Some of the values
+        # can be left unused.
+        #
+        # If the task output is substritable, an invocation of an n-output task produces
+        # n+1 artifacts: one for each subscripted output and one for non-subscripted
+        # output.
+        #
+        # If the task output is not substriptable, an invocation produces one artifact.
+        #
+        # Use case example:
+        # foo = task()
+        # bar, baz, _ = foo
+        # qux = task2(bar)
+        # bla = task2(bar)
+        #
+        # In the example above, there are:
+        # - 3 task invocations ("task()", "task2(bar)", and "task2(bar)")
+        # - 5 futures ("foo", "bar", "baz", "qux", "bla")
+        # - 6 artifacts:
+        #     - 3 unpacked outputs "bar", "baz", "_"
+        #     - 3 non-unpacked outputs "foo", "qux", "bla"
+
+        # Each future points to an artifact. This field to powers "self.get_node_id()".
+        self._future_artifacts: t.MutableMapping[
+            _dsl.ArtifactFuture, ir.ArtifactNode
+        ] = {}
+
+        # Artifacts for "bar" and "baz" in the example above. This field powers
+        # "self.artifacts". We need it in addition to "self._future_artifacts" because
+        # some artifact nodes can be not referenced in the workflow function ("_" in
+        # the example above).
+        self._invocation_unpacked_artifacts: t.MutableMapping[
+            _dsl.TaskInvocation, t.MutableSequence[ir.ArtifactNode]
+        ] = {}
+
+        # Artifacts for "foo" in the example above. This field powers "self.artifacts".
+        # We need it in addition to "self._invocation_unpacked_artifacts" because of
+        # "foo" in the example above.
+        self._invocation_non_unpacked_artifacts: t.MutableMapping[
+            _dsl.TaskInvocation, ir.ArtifactNode
+        ] = {}
+
+        # Needed to generate workflow-def-scoped artifact IDs.
+        self._wf_artifact_counter = 0
+
+    def _point_future_to_artifact(self, future: _dsl.ArtifactFuture):
+        """
+        Helper subroutine used in ``traverse()``. Mutates ``self._future_artifacts`` to
+        point ``future`` to an already generated artifact node.
+        """
+        if future.output_index is not None:
+            # This future is a result of unpacking another future ("bar"
+            # and "baz" in the example above).
+            self._future_artifacts[future] = self._invocation_unpacked_artifacts[
+                future.invocation
+            ][future.output_index]
+        else:
+            # This future is non-unpacked output ("foo" in the example
+            # above).
+            self._future_artifacts[future] = self._invocation_non_unpacked_artifacts[
+                future.invocation
+            ]
+
+    def _gen_artifact(
+        self,
+        task_def: _dsl.TaskDef,
+        custom_name: t.Optional[str],
+        format: ir.ArtifactFormat,
+        invocation_output_index: t.Optional[int],
+    ) -> ir.ArtifactNode:
+        """
+        Creates artifact node models with workflow-def-scoped IDs.
+        """
+        artifact = ir.ArtifactNode(
+            id=_make_artifact_id(
+                source_task=task_def,
+                wf_scoped_artifact_index=self._wf_artifact_counter,
+            ),
+            custom_name=custom_name,
+            serialization_format=format,
+            artifact_index=invocation_output_index,
+        )
+        self._wf_artifact_counter += 1
+
+        return artifact
 
-    def traverse(self, root_futures: t.Sequence[GraphNode]):
+    def traverse(self, output_nodes: t.Sequence[DSLDataNode]):
         """
-        Traverse the workflow graph.
+        Traverse the DSL workflow graph and collect the IR models.
 
         We iterate over the futures returned from the workflow find the artifacts,
         constants, and secrets.
         """
-        artifact_counter = 0
         secret_counter = 0
         constant_counter = 0
-        for n in _iter_nodes(root_futures):
+
+        seen_futures: t.MutableSet[_dsl.ArtifactFuture] = set()
+        seen_invocations: t.MutableSet[_dsl.TaskInvocation] = set()
+
+        for n in _iter_nodes(output_nodes):
             if isinstance(n, _dsl.ArtifactFuture):
-                self._artifacts[_make_key(n)] = _make_artifact_node(artifact_counter, n)
-                artifact_counter += 1
-                # Map the invocation to the future.
-                # Note: Each unique future has one invocation, but each invocation
-                #       can have many Futures.
-                #       We're mapping `invocation: set(futures from invocation)`
-                self._invocations.setdefault(n.invocation, set()).add(n)
+                # The main point of handling artifact futures is to populate:
+                # - self._future_artifacts
+                # - self._invocation_unpacked_artifacts
+                # - self._invocation_non_unpacked_artifacts
+
+                # A single future can be used in multiple places in the workflow. We
+                # only want to handle it once.
+                if n in seen_futures:
+                    continue
+
+                out_meta = n.invocation.task._output_metadata
+
+                # There can be many futures requiring to run the same task invocation.
+                if n.invocation in seen_invocations:
+                    # We've already handled the invocation, but not this future. We're
+                    # supposed to have artifact nodes already generated for it. We just
+                    # need to point "self._future_artifacts" to it.
+
+                    if out_meta.is_subscriptable:
+                        assert n.invocation in self._invocation_unpacked_artifacts
+
+                    assert n.invocation in self._invocation_non_unpacked_artifacts
+
+                    self._point_future_to_artifact(n)
+                else:
+                    # We haven't seen the invocation and haven't seen the future. We'll
+                    # have to generate artifact nodes before we can point
+                    # "self._future_artifacts" to it.
+
+                    if out_meta.is_subscriptable:
+                        # Generate artifact nodes for unpacking ("bar" and "baz" in the
+                        # example above).
+                        unpacked_artifacts = []
+                        for output_i in range(out_meta.n_outputs):
+                            default_format = ir.ArtifactFormat(
+                                _dsl.ArtifactFuture.DEFAULT_SERIALIZATION_FORMAT.value
+                            )
+                            artifact = self._gen_artifact(
+                                task_def=n.invocation.task,
+                                custom_name=_dsl.ArtifactFuture.DEFAULT_CUSTOM_NAME,
+                                format=default_format,
+                                invocation_output_index=output_i,
+                            )
+                            unpacked_artifacts.append(artifact)
+                        self._invocation_unpacked_artifacts[
+                            n.invocation
+                        ] = unpacked_artifacts
+
+                    # Generate artifact node for non-unpacked use ("foo", "qux", "bla"
+                    # in the example above).
+                    artifact = self._gen_artifact(
+                        task_def=n.invocation.task,
+                        custom_name=n.custom_name,
+                        format=ir.ArtifactFormat(n.serialization_format.value),
+                        invocation_output_index=None,
+                    )
+
+                    self._invocation_non_unpacked_artifacts[n.invocation] = artifact
+
+                    self._point_future_to_artifact(n)
+
+                # due dilligence
+                seen_futures.add(n)
+                seen_invocations.add(n.invocation)
+
             elif isinstance(n, _dsl.Secret):
-                self._secrets[_make_key(n)] = model.SecretNode(
+                self._secrets[_make_key(n)] = ir.SecretNode(
                     id=f"secret-{secret_counter}",
                     secret_name=n.name,
                     secret_config=n.config_name,
                 )
                 secret_counter += 1
             else:
                 self._constants[_make_key(n)] = _make_constant_node(constant_counter, n)
                 constant_counter += 1
 
     @property
-    def artifacts(self):
-        return self._artifacts
+    def artifacts(self) -> t.Iterable[ir.ArtifactNode]:
+        # Collect unpacked artifacts
+        unpacked = (
+            artifact
+            for artifacts in self._invocation_unpacked_artifacts.values()
+            for artifact in artifacts
+        )
+        # Collect non-unpacked artifacts
+        non_unpacked = self._invocation_non_unpacked_artifacts.values()
 
-    @property
-    def constants(self):
-        return self._constants
+        return (*unpacked, *non_unpacked)
 
     @property
-    def invocations(self):
-        return self._invocations
+    def constants(self) -> t.Iterable[ir.ConstantNode]:
+        return self._constants.values()
 
     @property
-    def secrets(self):
-        return self._secrets
+    def invocations(self) -> t.Iterable[_dsl.TaskInvocation]:
+        # Every seen invocation has a non-unpacked artifact so we can use this field.
+        return self._invocation_non_unpacked_artifacts.keys()
+
+    def output_ids_for_invocation(
+        self, invocation: _dsl.TaskInvocation
+    ) -> t.Sequence[ir.ArtifactNodeId]:
+        # Collect unpacked artifacts (a sequence)
+        unpacked: t.Iterable[ir.ArtifactNode]
+        if invocation.task._output_metadata.is_subscriptable:
+            unpacked = (
+                artifact for artifact in self._invocation_unpacked_artifacts[invocation]
+            )
+        else:
+            unpacked = []
+
+        # Get the non-unpacked artifact (a single one)
+        non_unpacked = self._invocation_non_unpacked_artifacts[invocation]
 
-    def get_argument_id(self, node: GraphNode):
-        return self[node].id
+        return [artifact.id for artifact in (*unpacked, non_unpacked)]
 
-    def __getitem__(self, node: GraphNode):
+    @property
+    def secrets(self) -> t.Iterable[ir.SecretNode]:
+        return self._secrets.values()
+
+    def get_node_id(self, node: DSLDataNode) -> ir.ArgumentId:
         key = _make_key(node)
-        if key in self._artifacts:
-            return self._artifacts[key]
-        elif key in self._secrets:
-            return self._secrets[key]
-        elif key in self._constants:
-            return self._constants[key]
+
+        if isinstance(node, _dsl.ArtifactFuture):
+            return self._future_artifacts[node].id
+
+        elif isinstance(node, _dsl.Secret):
+            return self._secrets[key].id
         else:
-            # In normal circumstances, this should never happen
-            raise KeyError(node)  # pragma: no cover
+            return self._constants[key].id
 
 
 def _iter_nodes(
-    root_futures: t.Sequence[GraphNode],
+    root_futures: t.Sequence[DSLDataNode],
 ) -> t.Iterator[t.Union[_dsl.ArtifactFuture, _dsl.Constant]]:
     traversal_list = [*root_futures]
     traversed_nodes = set()
     while traversal_list:
         current_node = traversal_list.pop()
         # _make_key ensures that we traverse each node only once
         traversed_nodes.add(_make_key(current_node))
@@ -212,52 +381,52 @@
     if isinstance(imp, _dsl.DeferredGitImport):
         imp = imp.resolved()
 
     import_hash = _gen_id_hash(imp)
     id_ = _make_import_id(imp, import_hash)
 
     if isinstance(imp, _dsl.LocalImport):
-        return model.LocalImport(
+        return ir.LocalImport(
             id=id_,
         )
     elif isinstance(imp, _dsl.GitImport):
-        return model.GitImport(
+        return ir.GitImport(
             id=id_,
             repo_url=imp.repo_url,
             git_ref=imp.git_ref,
         )
     elif isinstance(imp, _dsl.GitImportWithAuth):
         url = _git_url_utils.parse_git_url(imp.repo_url)
         url.user = imp.username
         if imp.auth_secret is not None:
-            url.password = model.SecretNode(
+            url.password = ir.SecretNode(
                 id=f"secret-{id_}",
                 secret_name=imp.auth_secret.name,
                 secret_config=imp.auth_secret.config_name,
             )
-        return model.GitImport(
+        return ir.GitImport(
             id=id_,
             repo_url=url,
             git_ref=imp.git_ref,
         )
     elif isinstance(imp, _dsl.InlineImport):
-        return model.InlineImport(id=id_)
+        return ir.InlineImport(id=id_)
 
     elif isinstance(imp, _dsl.PythonImports):
         reqs: t.List[Requirement] = imp.resolved()
         deps = []
         for req in reqs:
-            x = model.PackageSpec(
+            x = ir.PackageSpec(
                 name=req.name,
                 extras=sorted(list(req.extras)),
                 version_constraints=sorted([str(spec) for spec in req.specifier]),
                 environment_markers=str(req.marker) if req.marker else "",
             )
             deps.append(x)
-        return model.PythonImports(id=id_, packages=deps, pip_options=[])
+        return ir.PythonImports(id=id_, packages=deps, pip_options=[])
 
     else:
         raise ValueError(f"Invalid DSL import type: {type(imp)}")
 
 
 def _make_resources_model(resources: _dsl.Resources, is_task=True):
     """Create a resources object of the IR based on a resources
@@ -268,33 +437,33 @@
         resources object from the IR
     """
     if resources.is_empty():
         return None
 
     if is_task and resources.nodes is not None:
         warnings.warn(
-            NodesInTaskResourcesWarning(
+            exceptions.NodesInTaskResourcesWarning(
                 "Tasks currently do not support the nodes resource."
             )
         )
         nodes = None
     else:
         nodes = resources.nodes
 
-    return model.Resources(
+    return ir.Resources(
         cpu=resources.cpu,
         memory=resources.memory,
         disk=resources.disk,
         gpu=resources.gpu,
         nodes=nodes,
     )
 
 
 def _make_data_aggregation_model(data_aggregation: _dsl.DataAggregation):
-    return model.DataAggregation(
+    return ir.DataAggregation(
         run=data_aggregation.run,
         resources=_make_resources_model(data_aggregation.resources),
     )
 
 
 def _qe_compliant_name(name: str) -> str:
     """Make a guess of a name that's compliant with QE.
@@ -315,62 +484,62 @@
 def _make_task_id(fn_name, suffix):
     return _qe_compliant_name(f"task-{fn_name}-{suffix}")
 
 
 def _make_parameters(parameters: t.Optional[OrderedDict]):
     if parameters is not None:
         return [
-            model.TaskParameter(name=p.name, kind=model.ParameterKind[p.kind.value])
+            ir.TaskParameter(name=p.name, kind=ir.ParameterKind[p.kind.value])
             for p in parameters.values()
         ]
     else:
         return None
 
 
-def _make_fn_ref(fn_ref: _dsl.FunctionRef) -> model.FunctionRef:
+def _make_fn_ref(fn_ref: _dsl.FunctionRef) -> ir.FunctionRef:
     if isinstance(fn_ref, _dsl.ModuleFunctionRef):
-        return model.ModuleFunctionRef(
+        return ir.ModuleFunctionRef(
             module=fn_ref.module,
             function_name=fn_ref.function_name,
             file_path=fn_ref.file_path,
             line_number=fn_ref.line_number,
         )
     elif isinstance(fn_ref, _dsl.FileFunctionRef):
-        return model.FileFunctionRef(
+        return ir.FileFunctionRef(
             file_path=fn_ref.file_path,
             function_name=fn_ref.function_name,
             line_number=fn_ref.line_number,
         )
     elif isinstance(fn_ref, _dsl.InlineFunctionRef):
         module = inspect.getmodule(fn_ref.fn)
         with serde.registered_module(module):
             encoded_fn = serde.serialize_pickle(fn_ref.fn)
-        return model.InlineFunctionRef(
+        return ir.InlineFunctionRef(
             function_name=fn_ref.function_name,
             encoded_function=encoded_fn,
         )
     else:
         raise NotImplementedError(f"Unknown FunctionRef {type(fn_ref)}")
 
 
 def _make_task_model(
     task: _dsl.TaskDef,
-    imports_dict: t.Dict[_dsl.Import, model.Import],
-) -> model.TaskDef:
+    imports_dict: t.Dict[_dsl.Import, ir.Import],
+) -> ir.TaskDef:
     # fn_ref and source_imports are completely resolved during
     # creation of import_models_dict. At this point every task should have
     # those variables set - and they are needed to make task model
     assert task._fn_ref is not None
     assert task._source_import is not None
 
     fn_ref_model = _make_fn_ref(task._fn_ref)
 
     source_import = imports_dict[task._source_import]
 
-    dependency_import_ids: t.Optional[t.List[model.ImportId]]
+    dependency_import_ids: t.Optional[t.List[ir.ImportId]]
     if task._dependency_imports is not None:
         # We need to keep track of the seen dependencies so we don't include duplicates.
         # Why don't we use a set? We currently treat the source_import separately and
         # we need to preserve the ordering of the dependency IDs.
         seen_ids = set([source_import.id])
         dependency_import_ids = []
         for imp in task._dependency_imports:
@@ -388,42 +557,32 @@
         fn_ref_model,
         source_import.id,
         dependency_import_ids,
         resources,
         parameters,
     )
 
-    return model.TaskDef(
+    return ir.TaskDef(
         id=_make_task_id(
             task.__name__,
             task_contents_hash,
         ),
         fn_ref=fn_ref_model,
+        output_metadata=ir.TaskOutputMetadata(
+            is_subscriptable=task._output_metadata.is_subscriptable,
+            n_outputs=task._output_metadata.n_outputs,
+        ),
         source_import_id=source_import.id,
         dependency_import_ids=dependency_import_ids,
         resources=resources,
         parameters=parameters,
         custom_image=task._custom_image,
     )
 
 
-def _make_artifact_node(
-    future_index: int, future: _dsl.ArtifactFuture
-) -> model.ArtifactNode:
-    return model.ArtifactNode(
-        id=_make_artifact_id(
-            source_task=future.invocation.task,
-            future_index=future_index,
-        ),
-        custom_name=future.custom_name,
-        serialization_format=model.ArtifactFormat(future.serialization_format.value),
-        artifact_index=future.output_index,
-    )
-
-
 def _get_nested_objects(obj) -> t.Iterable:
     """
     Figure out an object's neighbors in the reference graph using best-effort
     heuristics.
     """
     try:
         vs = vars(obj)
@@ -484,29 +643,29 @@
 
 def _preview_constant(constant: _dsl.Constant):
     return repr(constant)[:12]
 
 
 def _make_constant_node(
     constant_index: int, constant_value: _dsl.Constant
-) -> model.ConstantNode:
+) -> ir.ConstantNode:
     if isinstance(constant_value, _dsl.TaskDef):
         raise exceptions.WorkflowSyntaxError(
             f"`{constant_value.__name__}` is a task definition and should be called "
             "before returning.\n Did you mean to call it inside a workflow?"
         )
     try:
         # Piggyback on the serialization we already implemented for artifacts.
         # Adding support for pickle constants would require adding a separate
         # schema for constants with chunked values. For more info, see and
         # compare:
         # - orquestra.sdk.schema.ir.ConstantNode
         # - orquestra.sdk.schema.responses.JSONResult
         # - orquestra.sdk.schema.responses.PickleResult
-        result = serde.result_from_artifact(constant_value, model.ArtifactFormat.AUTO)
+        result = serde.result_from_artifact(constant_value, ir.ArtifactFormat.AUTO)
     except (TypeError, ValueError, NotImplementedError):
         futures = _find_futures_in_container(constant_value)
         task_fn_names = ", ".join(
             {f"`{fut.invocation.task._fn_name}()`" for fut in futures}
         )
         if task_fn_names:
             raise exceptions.WorkflowSyntaxError(
@@ -520,22 +679,22 @@
         else:
             raise exceptions.WorkflowSyntaxError(
                 "We couldn't serialize part of the workflow. Looks like you may have "
                 f"used a non-serializable object: {constant_value}"
             )
 
     if isinstance(result, responses.JSONResult):
-        return model.ConstantNodeJSON(
+        return ir.ConstantNodeJSON(
             id=f"constant-{constant_index}",
             value=result.value,
             value_preview=_preview_constant(constant_value),
             serialization_format=result.serialization_format,
         )
     elif isinstance(result, responses.PickleResult):
-        return model.ConstantNodePickle(
+        return ir.ConstantNodePickle(
             id=f"constant-{constant_index}",
             chunks=result.chunks,
             value_preview=_preview_constant(constant_value),
             serialization_format=result.serialization_format,
         )
     else:
         raise ValueError(
@@ -549,55 +708,58 @@
         return _qe_compliant_name(f"invocation-{invocation_i}-task-{task_name}")
     else:
         return _qe_compliant_name(
             f"name-{custom_name}-invocation-{invocation_i}-task-{task_name}"
         )
 
 
-def _sort_artifact_futures(artifact: _dsl.ArtifactFuture) -> int:
-    if artifact.output_index is None:
-        return -1
-    else:
-        return artifact.output_index
-
-
 def _make_invocation_model(
     invocation: _dsl.TaskInvocation,
     invocation_index: int,
-    task_models_dict: t.Dict[_dsl.TaskDef, model.TaskDef],
+    task_models_dict: t.Dict[_dsl.TaskDef, ir.TaskDef],
     graph: GraphTraversal,
 ):
-    args_ids = [graph.get_argument_id(arg) for arg in invocation.args]
+    args_ids = [graph.get_node_id(arg) for arg in invocation.args]
 
     kwargs_ids = {
-        arg_name: graph.get_argument_id(arg_val)
-        for arg_name, arg_val in invocation.kwargs
+        arg_name: graph.get_node_id(arg_val) for arg_name, arg_val in invocation.kwargs
     }
 
-    sorted_outputs = sorted(graph.invocations[invocation], key=_sort_artifact_futures)
-
-    return model.TaskInvocation(
+    return ir.TaskInvocation(
         id=_make_invocation_id(
             task_models_dict[invocation.task].fn_ref.function_name,
             invocation_index,
             invocation.custom_name,
         ),
         task_id=task_models_dict[invocation.task].id,
         args_ids=args_ids,
         kwargs_ids=kwargs_ids,
-        output_ids=[graph[output_future].id for output_future in sorted_outputs],
+        output_ids=graph.output_ids_for_invocation(invocation),
         resources=_make_resources_model(invocation.resources),
         custom_image=invocation.custom_image,
     )
 
 
+def extract_root_futures(wf_def: _workflow.WorkflowDef) -> t.Sequence[_dsl.Argument]:
+    """
+    Executes the ``wf_def`` function to get the workflow output futures.
+    """
+    with _exec_ctx.workflow_build():
+        futures = wf_def._fn(*wf_def._workflow_args, **wf_def._workflow_kwargs)
+
+    if not isinstance(futures, collections.abc.Sequence) or isinstance(futures, str):
+        return (futures,)
+    else:
+        return futures
+
+
 def flatten_graph(
     workflow_def: _workflow.WorkflowDef,
     futures: t.Sequence[t.Union[_dsl.ArtifactFuture, _dsl.Constant]],
-) -> model.WorkflowDef:
+) -> ir.WorkflowDef:
     """Traverse the nested linked list of futures and produce a flat graph.
 
     Each `dsl.ArtifactFuture` is mapped to a single `model.ArtifactNode`.
     Each `dsl.Constant` is mapped to a single `model.ConstantNode`.
     Each `dsl.TaskInvocation` is mapped to a single `model.TaskInvocation`.
 
     Unique task references from `dsl.TaskInvocation`s are mapped to `model.Task`s.
@@ -607,25 +769,28 @@
     node is referenced by multiple invocations.
     """
     root_futures = futures
 
     graph = GraphTraversal()
     graph.traverse(root_futures)
 
-    import_models_dict: t.Dict[_dsl.Import, model.Import] = {}
+    import_models_dict: t.Dict[_dsl.Import, ir.Import] = {}
 
     # this dict is used to store already processed deferred git imports in the WF
     # As deferred git imports are fetching repos inside model creation, this is used
     # to avoid git fetch spam for the same repos over and over.
-    cached_git_import_dict: t.Dict[t.Tuple, model.Import] = {}
-    for invocation in graph.invocations.keys():
+    cached_git_import_dict: t.Dict[t.Tuple, ir.Import] = {}
+    for invocation in graph.invocations:
         invocation.task._resolve_task_source_data(workflow_def.default_source_import)
-        invocation.task._resolve_task_dependencies(
-            workflow_def.default_dependency_imports
+        default_deps = (
+            tuple(workflow_def.default_dependency_imports)
+            if workflow_def.default_dependency_imports
+            else None
         )
+        invocation.task._resolve_task_dependencies(default_deps)
         for imp in [
             invocation.task._source_import,
             *(invocation.task._dependency_imports or []),
         ]:
             if imp not in import_models_dict:
                 if isinstance(imp, _dsl.DeferredGitImport):
                     cashe_key = (imp.local_repo_path, imp.git_ref)
@@ -634,82 +799,61 @@
                     else:
                         model_import = _make_import_model(imp)
                         import_models_dict[imp] = model_import
                         cached_git_import_dict[cashe_key] = model_import
                 else:
                     import_models_dict[imp] = _make_import_model(imp)
 
-    task_models_dict: t.Dict[_dsl.TaskDef, model.TaskDef] = {
+    task_models_dict: t.Dict[_dsl.TaskDef, ir.TaskDef] = {
         invocation.task: _make_task_model(invocation.task, import_models_dict)
-        for invocation in graph.invocations.keys()
+        for invocation in graph.invocations
     }
     # make sure we can execute tasks
     for task in task_models_dict:
         task.validate_task()
 
-    dsl_invocations = list(graph.invocations.keys())
+    dsl_invocations = list(graph.invocations)
 
-    invocation_models_dict: t.Dict[_dsl.TaskInvocation, model.TaskInvocation] = {
+    invocation_models_dict: t.Dict[_dsl.TaskInvocation, ir.TaskInvocation] = {
         dsl_invocation: _make_invocation_model(
             invocation=dsl_invocation,
             invocation_index=dsl_invocation_i,
             task_models_dict=task_models_dict,
             graph=graph,
         )
         for dsl_invocation_i, dsl_invocation in enumerate(dsl_invocations)
     }
 
-    output_ids: t.List[t.Union[model.ConstantNodeId, model.ArtifactNodeId]] = []
-    for output_future in futures:
-        output_id = graph.get_argument_id(output_future)
-        output_ids.append(output_id)
-
-    sdk_version_str = get_installed_version("orquestra-sdk")
-    parsed_sdk_version = parse_version(sdk_version_str)
-    sdk_version = model.Version(
-        original=sdk_version_str,
-        major=parsed_sdk_version.major,
-        minor=parsed_sdk_version.minor,
-        patch=parsed_sdk_version.micro,
-        is_prerelease=parsed_sdk_version.is_prerelease,
-    )
-    return model.WorkflowDef(
-        metadata=model.WorkflowMetadata(
+    sdk_version = get_current_sdk_version()
+    python_version = get_current_python_version()
+
+    return ir.WorkflowDef(
+        metadata=ir.WorkflowMetadata(
             sdk_version=sdk_version,
-            python_version=model.Version(
-                original=sys.version,
-                major=sys.version_info.major,
-                minor=sys.version_info.minor,
-                patch=sys.version_info.micro,
-                is_prerelease=sys.version_info.releaselevel != "final",
-            ),
+            python_version=python_version,
         ),
         resources=_make_resources_model(workflow_def._resources, is_task=False),
         # At the moment 'orq submit workflow-def <name>' assumes that the <name> is
         # the same as the underlying function. Orquestra Studio seems to get it from
         # the 'orq get workflow-def', so for now we have to keep .name attribute same
         # as the function name.
         name=workflow_def.name,
         fn_ref=_make_fn_ref(workflow_def.fn_ref),
         imports={
             import_node.id: import_node for import_node in import_models_dict.values()
         },
         tasks={task_model.id: task_model for task_model in task_models_dict.values()},
         artifact_nodes={
-            artifact_node.id: artifact_node
-            for artifact_node in graph.artifacts.values()
-        },
-        secret_nodes={
-            secret_node.id: secret_node for secret_node in graph.secrets.values()
+            artifact_node.id: artifact_node for artifact_node in graph.artifacts
         },
+        secret_nodes={secret_node.id: secret_node for secret_node in graph.secrets},
         constant_nodes={
-            constant_node.id: constant_node
-            for constant_node in graph.constants.values()
+            constant_node.id: constant_node for constant_node in graph.constants
         },
         task_invocations={
             invocation.id: invocation for invocation in invocation_models_dict.values()
         },
-        output_ids=output_ids,
+        output_ids=[graph.get_node_id(output_future) for output_future in futures],
         data_aggregation=_make_data_aggregation_model(workflow_def.data_aggregation)
         if workflow_def.data_aggregation
         else None,
     )
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_viz.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_viz.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ################################################################################
 # © Copyright 2022 Zapata Computing Inc.
 ################################################################################
 """
 Workflow visualization using graphviz.
 """
 
+import itertools
 import typing as t
 from dataclasses import dataclass
 
 import graphviz  # type: ignore
 
 from orquestra.sdk.schema import ir
 
@@ -83,29 +84,34 @@
                     f"{task_location}.{fn_name}(){line_no_suffix}",
                     task_inv.id,
                 ],
             )
         )
 
         # 2. Connect task with arguments
-        for arg_id in task_inv.args_ids:
+        for arg_id in itertools.chain(task_inv.args_ids, task_inv.kwargs_ids.values()):
             # We don't define a node here, because artifacts are declared with the
             # tasks that produce them (below), and workflow constants are defined
             # totally separately.
             edges.append((arg_id, task_inv.id))
 
         # 3. Connect task with outputs
         for artifact_id in task_inv.output_ids:
             artifact_nodes.append(Node(id=artifact_id, caption=[]))
             edges.append((task_inv.id, artifact_id))
 
     # 4. Add workflow constants
     for constant in wf_def.constant_nodes.values():
         artifact_nodes.append(Node(id=constant.id, caption=[constant.value_preview]))
 
+    aggregation_step_id = "aggregation_step"
+    artifact_nodes.append(Node(id=aggregation_step_id, caption=["outputs"]))
+    for wf_output in wf_def.output_ids:
+        edges.append((wf_output, aggregation_step_id))
+
     return BiGraph(nodes1=task_nodes, nodes2=artifact_nodes, edges=edges)
 
 
 def translate_to_graphviz(graph: BiGraph) -> graphviz.Digraph:
     """
     Builds a graphviz object based on the renderer-agnostic bigraph.
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/_workflow.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/_workflow.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 ################################################################################
 # © Copyright 2022-2023 Zapata Computing Inc.
 ################################################################################
 import ast
 import functools
 import inspect
 import warnings
-from collections.abc import Sequence
 from enum import Enum
 from pathlib import Path
 from types import FunctionType
 from typing import (
     Any,
     Callable,
     Dict,
@@ -23,18 +22,23 @@
     Union,
     overload,
 )
 
 from typing_extensions import ParamSpec
 
 import orquestra.sdk.schema.ir as ir
-from orquestra.sdk.exceptions import ConfigNameNotFoundError, WorkflowSyntaxError
+from orquestra.sdk.exceptions import (
+    ConfigNameNotFoundError,
+    ProjectInvalidError,
+    WorkflowSyntaxError,
+)
+from orquestra.sdk.schema.workflow_run import ProjectId, ProjectRef, WorkspaceId
 
 from .. import secrets
-from . import _api, _dsl, _exec_ctx, loader
+from . import _api, _dsl, loader
 from ._ast import CallVisitor, NodeReference, NodeReferenceType, normalize_indents
 from ._dsl import (
     DataAggregation,
     FunctionRef,
     Import,
     ImportTypes,
     Secret,
@@ -111,24 +115,16 @@
                 this workflow def has a "GitImport" and the git repo that contains it
                 has uncommitted changes.
             orquestra.sdk.exceptions.WorkflowSyntaxError: when there are no tasks
                 defined for this workflow.
         """
         from orquestra.sdk._base import _traversal
 
-        with _exec_ctx.workflow_build():
-            futures = self._fn(*self._workflow_args, **self._workflow_kwargs)
-
-        _futures: Sequence
-        if not isinstance(futures, Sequence) or isinstance(futures, str):
-            _futures = (futures,)
-        else:
-            _futures = futures
-
-        model = _traversal.flatten_graph(self, _futures)
+        futures = _traversal.extract_root_futures(self)
+        model = _traversal.flatten_graph(self, futures)
 
         if len(model.task_invocations) < 1:
             helpstr = f"The workflow '{model.name}' "
             if hasattr(model.fn_ref, "file_path"):  # If possible add the file and line.
                 helpstr += f"(defined at {model.fn_ref.file_path}"
                 if hasattr(model.fn_ref, "line_number"):
                     helpstr += f" line {model.fn_ref.line_number}"
@@ -163,32 +159,37 @@
         _dsl.DIRECT_EXECUTION = False
         return result
 
     def prepare(
         self,
         config: Union[_api.RuntimeConfig, str],
         project_dir: Optional[Union[str, Path]] = None,
+        workspace_id: Optional[WorkspaceId] = None,
+        project_id: Optional[ProjectId] = None,
     ) -> _api.WorkflowRun:
         """
         "Prepares" workflow for running. Call ".start()" on the result to
         schedule the workflow for execution.
 
         Args:
             config: SDK needs to know where to execute the workflow. The config
                 contains the required details. This can be a RuntimeConfig object, or
                 the name of a saved configuration.
             project_dir: the path to the project directory. If omitted, the current
                 working directory is used.
+            workspace_id: ID of the workspace for workflow - supported only on CE
+            project_id: ID of the project for workflow - supported only on CE
 
         Raises:
             ConfigNameNotFoundError: when the configuration has not been saved prior to
                 this point.
             orquestra.sdk.exceptions.DirtyGitRepo: (warning) when a task def used by
                 this workflow def has a "GitImport" and the git repo that contains it
                 has uncommitted changes.
+            ProjectInvalidError: when only 1 out of project and workspace is passed
         """
         _config: _api.RuntimeConfig
         if isinstance(config, _api.RuntimeConfig):
             _config = config
         elif isinstance(config, str):
             _config = _api.RuntimeConfig.load(config)
         else:
@@ -212,35 +213,54 @@
             runtime = _config._get_runtime(project_dir=project_dir)
 
         # In close future there will be multiple ways of figuring out the
         # appropriate runtime to use, based on `config`. Regardless of this
         # logic, the runtime should always be resolved.
         assert runtime is not None
 
+        _project: Optional[ProjectRef]
+        if project_id is not None and workspace_id is not None:
+            _project = ProjectRef(project_id=project_id, workspace_id=workspace_id)
+        elif project_id is None and workspace_id is None:
+            _project = None
+        else:
+            raise ProjectInvalidError(
+                "Invalid project ID. Either explicitely pass workspace_id "
+                "and project_id, or omit both"
+            )
+
         # The DirtyGitRepo warning can be raised here.
         wf_def_model = self.model
 
         return _api.WorkflowRun(
-            run_id=None, wf_def=wf_def_model, runtime=runtime, config=_config
+            run_id=None,
+            wf_def=wf_def_model,
+            runtime=runtime,
+            config=_config,
+            project=_project,
         )
 
     def run(
         self,
         config: Optional[Union[_api.RuntimeConfig, str]] = None,
         project_dir: Optional[Union[str, Path]] = None,
+        workspace_id: Optional[WorkspaceId] = None,
+        project_id: Optional[ProjectId] = None,
     ) -> _api.WorkflowRun:
         """
         Schedules workflow for execution. Shorthand for
         `workflow.prepare().start()`.
 
         Args:
             config: SDK needs to know where to execute the workflow. This
                 objects contains the required details.
             project_dir: the path to the project directory. If omitted, the current
                 working directory is used.
+            workspace_id: ID of the workspace for workflow - supported only on CE
+            project_id: ID of the project for workflow - supported only on CE
 
         Raises:
             orquestra.sdk.exceptions.DirtyGitRepo: (warning) when a task def used by
                 this workflow def has a "GitImport" and the git repo that contains it
                 has uncommitted changes.
         """
         # This exists for users who have gotten used to doing `run()`. Once this has
@@ -251,15 +271,20 @@
                 "Please specify the runtime configuration for this run. "
                 "The built in `local` and `in_process` configurations can be used by "
                 'calling `run.("local")` and `run("in_process")` respectively. '
                 "User defined configurations can be specified by providing the name "
                 "under which they are saved, or passing in the RuntimeConfig object "
                 "directly. "
             )
-        run = self.prepare(config, project_dir=project_dir)
+        run = self.prepare(
+            config,
+            project_dir=project_dir,
+            workspace_id=workspace_id,
+            project_id=project_id,
+        )
         run.start()
         return run
 
     def with_resources(
         self,
         *,
         cpu: Optional[Union[str, _dsl.Sentinel]] = _dsl.Sentinel.NO_UPDATE,
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/abc.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/abc.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 from abc import ABC, abstractmethod
 from datetime import timedelta
 from pathlib import Path
 
 from orquestra.sdk.schema.configs import RuntimeConfiguration
 from orquestra.sdk.schema.ir import TaskInvocationId, WorkflowDef
 from orquestra.sdk.schema.local_database import StoredWorkflowRun
+from orquestra.sdk.schema.responses import WorkflowResult
 from orquestra.sdk.schema.workflow_run import (
+    ProjectRef,
     State,
     WorkflowRun,
     WorkflowRunId,
     WorkflowRunMinimal,
 )
 
 
@@ -75,60 +77,72 @@
         cls, project_dir: Path, config: RuntimeConfiguration, verbose: bool
     ) -> "RuntimeInterface":
         """Returns an initilaised version of the class from a "Runtime options" JSON"""
         raise NotImplementedError()
 
     @abstractmethod
     def create_workflow_run(
-        self,
-        workflow_def: WorkflowDef,
+        self, workflow_def: WorkflowDef, project: t.Optional[ProjectRef]
     ) -> WorkflowRunId:
-        """Schedules a workflow definition for execution"""
+        """Schedules a workflow definition for execution
+
+        Args:
+            workflow_def: IR definition of workflow to be executed
+            project: project in which workflow is going to be executed
+                used currently only on CE runtime.
+                When omitted, WF will be scheduled at default project
+        """
         raise NotImplementedError()
 
     @abstractmethod
     def get_workflow_run_status(self, workflow_run_id: WorkflowRunId) -> WorkflowRun:
         """Gets the status of a workflow run"""
         raise NotImplementedError()
 
     @abstractmethod
     def get_workflow_run_outputs_non_blocking(
         self, workflow_run_id: WorkflowRunId
-    ) -> t.Sequence[ArtifactValue]:
+    ) -> t.Sequence[WorkflowResult]:
         """Non-blocking version of get_workflow_run_outputs.
 
         This method raises exceptions if the workflow output artifacts are not available
 
         Raises:
             WorkflowRunNotSucceeded if the workflow has not yet finished
         """
         raise NotImplementedError()
 
     @abstractmethod
     def get_available_outputs(
         self, workflow_run_id: WorkflowRunId
-    ) -> t.Dict[TaskInvocationId, t.Tuple[ArtifactValue, ...]]:
+    ) -> t.Dict[TaskInvocationId, WorkflowResult]:
         """Returns all available outputs for a workflow
 
         This method returns all available artifacts. When the workflow fails it returns
         artifacts only for the steps that did success. Might raise an exception if
         runtime doesn't support getting artifacts from in-progress workflow.
 
-        Either we have access to all outputs of a given task, or none. In other words,
-        the number of values in the tuple should always match the number of output IDs
-        in the corresponding task invocation.
+        Either we have access to all outputs of a given task, or none. If a given task
+        invocation didn't succeed yet, there shouldn't be an entry in the returned dict.
+
+        This method should return all output values for a task even if some of them
+        aren't used in the workflow function. Reasons:
+        - Users might be interested in the computed value after running, even though
+          the workflow didn't make an explicit use of it.
+        - Position in the task output tuple is significant. We can't just drop some of
+          the elements because this would shift indices.
 
         Careful: This method does NOT return status of a workflow. Verify it beforehand
         to make sure if workflow failed/succeeded/is running. You might get incomplete
         results
 
         Returns:
             A mapping with an entry for each task run in the workflow. The key is the
-                task's invocation ID. The value is a n-tuple, where n is the number of
-                task's outputs. If task has 1 output, this will be a 1-tuple.
+                task's invocation ID. The value is whatever the task function returned,
+                independent of the ``@task(n_outputs=...)`` value.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def stop_workflow_run(self, workflow_run_id: WorkflowRunId) -> None:
         """Stops a workflow run.
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_arg_resolvers.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_arg_resolvers.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_cli_logs.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_cli_logs.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_dumpers.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_dumpers.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_entry.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_entry.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_login/_login.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_login/_login.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_login/_login_server.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_login/_login_server.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_repos.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_repos.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 from orquestra import sdk
 from orquestra.sdk import exceptions
 from orquestra.sdk._base import _config, _db, loader
 from orquestra.sdk._base._driver._client import DriverClient
 from orquestra.sdk._base._qe import _client
 from orquestra.sdk._base.abc import ArtifactValue
+from orquestra.sdk.schema import _compat
 from orquestra.sdk.schema.configs import ConfigName, RuntimeName
 from orquestra.sdk.schema.ir import TaskInvocationId, WorkflowDef
 from orquestra.sdk.schema.workflow_run import (
     State,
     TaskRun,
     TaskRunId,
     WorkflowRun,
@@ -204,40 +205,59 @@
         return outputs
 
     def get_task_outputs(
         self,
         wf_run_id: WorkflowRunId,
         task_inv_id: TaskInvocationId,
         config_name: ConfigName,
-    ) -> t.Tuple[ArtifactValue]:
+    ) -> t.Tuple[ArtifactValue, ...]:
         """
-        Asks the runtime for task output values. This includes
+        Asks the runtime for task output values. The output is always a n-tuple where n
+        is the number of outputs in the task def metadata.
 
         Raises:
             orquestra.sdk.exceptions.NotFoundError: when the wf_run_id doesn't match a
                 known run ID.
             orquestra.sdk.exceptions.TaskInvocationNotFoundError: when task_inv_id
                 doesn't match the workflow definition.
             orquestra.sdk.exceptions.ConfigNameNotFoundError: when the named config is
                 not found in the file.
         """
         try:
             wf_run = sdk.WorkflowRun.by_id(wf_run_id, config_name)
         except (exceptions.NotFoundError, exceptions.ConfigNameNotFoundError):
             raise
 
-        artifacts = wf_run.get_artifacts()
         try:
-            task_outputs = artifacts[task_inv_id]
-        except KeyError as e:
+            task_run: sdk.TaskRun = _find_first(
+                lambda task: task.task_invocation_id == task_inv_id, wf_run.get_tasks()
+            )
+        except StopIteration as e:
             raise exceptions.TaskInvocationNotFoundError(
                 invocation_id=task_inv_id
             ) from e
 
-        return task_outputs
+        # TaskRun.get_outputs() returns whatever the task function returned, regardless
+        # of the number of ``@task(n_outputs=...)``. For presentation we need to somehow
+        # decide if we need to iterate over ``task_outputs`` or not. We base this logic
+        # on the IR.
+        task_outputs = task_run.get_outputs()
+
+        wf_def = wf_run.get_status_model().workflow_def
+        invocation = wf_def.task_invocations[task_inv_id]
+        task_def = wf_def.tasks[invocation.task_id]
+
+        if _compat.result_is_packed(task_def=task_def):
+            # We expect ``task_outputs`` to be an iterable already.
+            outputs_tuple = tuple(task_outputs)
+        else:
+            # ``task_outputs`` is likely to be a single object. We need to wrap it.
+            outputs_tuple = (task_outputs,)
+
+        return outputs_tuple
 
     def _get_wf_def_model(
         self, wf_run_id: WorkflowRunId, config_name: ConfigName
     ) -> WorkflowDef:
         """
         Raises:
             orquestra.sdk.exceptions.NotFoundError: when the wf_run_id doesn't match a
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_services/_down.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_services/_down.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_services/_status.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_services/_status.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_services/_up.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_services/_up.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_task/_logs.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_task/_logs.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_task/_results.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_task/_results.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_corq_format/color.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_corq_format/color.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_corq_format/per_command.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_corq_format/per_command.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_errors.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_errors.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_models.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_models.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_presenters.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_presenters.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_prompts.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_ui/_prompts.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_list.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_list.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_logs.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_logs.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_results.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_results.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_stop.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_stop.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_submit.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_submit.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_view.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/cli/_dorq/_workflow/_view.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/dispatch.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/dispatch.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/loader.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/loader.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_base/serde.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_base/serde.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,16 +15,42 @@
 from orquestra.sdk.schema import ir, responses
 
 CHUNK_SIZE = 40_000
 ENCODING = "base64"
 PICKLE_PROTOCOL = 4
 
 
+class _JSONTupleEncoder(json.JSONEncoder):
+    @staticmethod
+    def decode_tuple(obj):
+        if "__tuple__" in obj:
+            return tuple(obj["__values__"])
+        else:
+            return obj
+
+    @classmethod
+    def encode_tuple(cls, obj):
+        if isinstance(obj, tuple):
+            return {
+                "__tuple__": True,
+                "__values__": tuple(cls.encode_tuple(o) for o in obj),
+            }
+        elif isinstance(obj, list):
+            return [cls.encode_tuple(v) for v in obj]
+        elif isinstance(obj, dict):
+            return {k: cls.encode_tuple(v) for k, v in obj.items()}
+        else:
+            return obj
+
+    def encode(self, obj):
+        return super(_JSONTupleEncoder, self).encode(self.encode_tuple(obj))
+
+
 def _serialize_json(value: t.Any):
-    return json.dumps(value)
+    return json.dumps(value, cls=_JSONTupleEncoder)
 
 
 def _chunkify(s: str) -> t.List[str]:
     """
     Yaml/JSON parsers will fail if string is too large,
     so break it down into a list of strings where each chunk
     is no larger than CHUNK_SIZE
@@ -82,16 +108,26 @@
 
 
 @deserialize.register
 def _(result: responses.PickleResult) -> t.Any:
     return deserialize_pickle(result.chunks)
 
 
+@deserialize.register
+def _(result: ir.ConstantNodeJSON) -> t.Any:
+    return deserialize_constant(result)
+
+
+@deserialize.register
+def _(result: ir.ConstantNodePickle) -> t.Any:
+    return deserialize_constant(result)
+
+
 def deserialize_json(serialized_value: str) -> t.Any:
-    return json.loads(serialized_value)
+    return json.loads(serialized_value, object_hook=_JSONTupleEncoder.decode_tuple)
 
 
 def deserialize_pickle(chunks: t.List[str]) -> t.Any:
     chunks_str: str = "".join(chunks)
     return cloudpickle.loads(codecs.decode(chunks_str.encode(), ENCODING))
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_ray/_client.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_ray/_client.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_ray/_id_gen.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_ray/_id_gen.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/_ray/_ray_logs.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/_ray/_ray_logs.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/examples/exportable_wf.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/examples/exportable_wf.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/examples/workflow_defs.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/examples/workflow_defs.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/exceptions.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/exceptions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 ################################################################################
 # © Copyright 2022-2023 Zapata Computing Inc.
 ################################################################################
 import typing as t
 
-from orquestra.sdk.schema.ir import TaskInvocationId
+from orquestra.sdk.schema import ir
 from orquestra.sdk.schema.workflow_run import State
 
 
 class WorkflowSyntaxError(Exception):
     def __init__(self, msg: str):
         super().__init__(msg)
         self.msg = msg
 
 
+class VersionMismatch(Warning):
+    def __init__(self, msg: str, actual: ir.Version, needed: t.Optional[ir.Version]):
+        super().__init__(msg)
+        self.actual = actual
+        self.needed = needed
+
+
 class DirtyGitRepo(Warning):
     pass
 
 
 class BaseRuntimeError(Exception):
     def __init__(self, message: t.Optional[str] = None):
         super().__init__(message)
@@ -129,19 +136,25 @@
 
 
 class TaskInvocationNotFoundError(NotFoundError):
     """
     Raised when we can't find a Task Invocation that matches the provided ID.
     """
 
-    def __init__(self, invocation_id: TaskInvocationId):
+    def __init__(self, invocation_id: ir.TaskInvocationId):
         super().__init__()
         self.invocation_id = invocation_id
 
 
+class WorkflowResultsNotReadyError(NotFoundError):
+    """
+    Raised when a workflow has succeeded, but the results are not ready yet
+    """
+
+
 # Auth Errors
 class UnauthorizedError(BaseRuntimeError):
     pass
 
 
 # Ray Errors
 class RayActorNameClashError(BaseRuntimeError):
@@ -156,7 +169,16 @@
 class LoginURLUnavailableError(BaseRuntimeError):
     def __init__(self, base_uri: str):
         self.base_uri = base_uri
 
 
 class InProcessFromCLIError(NotFoundError):
     """Raised when the user requests the in-process runtime when using the CLI"""
+
+
+# Unsupported features
+class UnsupportedRuntimeFeature(Warning):
+    pass
+
+
+class ProjectInvalidError(BaseRuntimeError):
+    pass
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/kubernetes/quantity.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/kubernetes/quantity.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/packaging.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/packaging/_versions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 ################################################################################
-# © Copyright 2022 Zapata Computing Inc.
+# © Copyright 2022-2023 Zapata Computing Inc.
 ################################################################################
 import re
+import sys
 from typing import Any, Optional
 
 try:
     import importlib.metadata as metadata  # type: ignore
 except ModuleNotFoundError:  # pragma: no cover
     import importlib_metadata as metadata  # type: ignore  # pragma: no cover
 
+import packaging.version
+
 from orquestra.sdk import Import, PythonImports, TaskDef, exceptions
+from orquestra.sdk.schema import ir
 
 
 class PackagingError(exceptions.BaseRuntimeError):
     """Base error for any packaging errors"""
 
 
 def get_installed_version(package_name: str) -> str:
@@ -37,14 +41,44 @@
     """
     try:
         return metadata.version(package_name)
     except metadata.PackageNotFoundError as e:
         raise PackagingError(f"Package not found: {package_name}") from e
 
 
+def parse_version_str(version_str: str) -> ir.Version:
+    parsed_sdk_version = packaging.version.parse(version_str)
+    return ir.Version(
+        original=version_str,
+        major=parsed_sdk_version.major,
+        minor=parsed_sdk_version.minor,
+        patch=parsed_sdk_version.micro,
+        is_prerelease=parsed_sdk_version.is_prerelease,
+    )
+
+
+def get_installed_version_model(package_name: str) -> ir.Version:
+    sdk_version_str = get_installed_version(package_name)
+    return parse_version_str(sdk_version_str)
+
+
+def get_current_sdk_version() -> ir.Version:
+    return get_installed_version_model("orquestra-sdk")
+
+
+def get_current_python_version() -> ir.Version:
+    return ir.Version(
+        original=sys.version,
+        major=sys.version_info.major,
+        minor=sys.version_info.minor,
+        patch=sys.version_info.micro,
+        is_prerelease=sys.version_info.releaselevel != "final",
+    )
+
+
 def InstalledImport(
     *,
     package_name: str,
     version_match: Optional[str] = None,
     fallback: Optional[Import] = None,
 ) -> Import:
     """
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/schema/configs.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/schema/configs.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/schema/ir.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/schema/ir.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 The classes here are used only for purposes of schema definition. Every data
 structure here is JSON-serializable.
 """
 
 import enum
 import typing as t
+import warnings
 
 import pydantic
 from pydantic import BaseModel
 
 ImportId = str
 SecretNodeId = str
 
@@ -186,14 +187,30 @@
 class TaskParameter(BaseModel):
     name: ParameterName
     kind: ParameterKind
     # If we need more metadata related to parameters, like type hints or default values,
     # it should be added here.
 
 
+class TaskOutputMetadata(BaseModel):
+    """
+    Information about the data shape returned by a task function.
+    """
+
+    # If yes, it's possible to unpack the output in the workflow like:
+    # foo, bar = my_task()
+    #
+    # Separate from `n_outputs` to handle cases like:
+    # foo, = my_task()
+    is_subscriptable: bool
+
+    # Number of artifacts we can populate with the task results.
+    n_outputs: int
+
+
 class TaskDef(BaseModel):
     # workflow-unique ID used to refer from task invocations
     id: TaskDefId
 
     fn_ref: FunctionRef
 
     # `source_import_id` & `dependency_import_ids` are references to imports defined in
@@ -201,14 +218,20 @@
 
     # List of abstract inputs that the task requires, but without the values yet.
     # Kinda like function signature.
     # None means we do not know the parameters for this Task (e.g. an external task)
     # An empty list [] means a Task with no parameters
     parameters: t.Optional[t.List[TaskParameter]]
 
+    # Statically inferred from the task function. See also `TaskOutputMetadata`'s
+    # docstring.
+    # 'None' for IRs generated with orquestra-sdk<=0.45.1. Not empty for newer SDK
+    # versions.
+    output_metadata: t.Optional[TaskOutputMetadata] = None
+
     # ID of the import that contains the callable function
     source_import_id: ImportId
 
     # IDs of the imports that are needed at runtime to allow running the callable
     dependency_import_ids: t.Optional[t.List[ImportId]] = None
 
     resources: t.Optional[Resources] = None
@@ -238,34 +261,35 @@
 TaskInvocationId = str
 TaskNodeId = str
 ArtifactNodeId = str
 ConstantNodeId = str
 
 
 class ArtifactNode(BaseModel):
-    # Workflow-scope unique ID used to refer from task invocations
+    # Workflow-scope unique ID used to refer from task invocations. If the task has
+    # multiple outputs they will have distinct `id`s.
     id: ArtifactNodeId
 
     # artifact metadata below
 
     # Optional name that can be used if human-readable strings are needed. If present,
     # it's an addition to `id`, doesn't replace it.
     custom_name: t.Optional[str] = None
 
     # Tells runtime how to serialize artifact value after task invocation returns it.
     # At the moment it's unknown where exactly the artifacts will be persisted, but some
     # serialization will likely be needed somewhere.
     serialization_format: ArtifactFormat = ArtifactFormat.AUTO
 
-    # Tells the runtime the index of the Artifact from the TaskInvocation
-    # If None, then the TaskInvocation's result is not split
+    # Index of the variable when destructuring task result in the workflow function. If
+    # the workflow contained `foo, bar = my_task()`, `foo`'s index is 0 and `bar`'s
+    # index is 1. This is used by some runtimes to extract the artifact value from the
+    # output tuple.
     #
-    # We need this to support destructuring multi-output tasks when some
-    # of the output values are unused. For more info, see comments in:
-    # https://github.com/zapatacomputing/orquestra-workflow/pull/44
+    # `None` if the task result isn't destructured in the workflow function.
     artifact_index: t.Optional[int] = None
 
 
 class ConstantNodeJSON(BaseModel):
     """Piece of data that already exists at workflow submission time.
 
     The value is directly embedded in the workflow. To support arbitrary data shapes we
@@ -307,14 +331,16 @@
 
     # Human-readable string that can be rendered on the UI to represent the value.
     value_preview: pydantic.constr(max_length=12)  # type: ignore
 
 
 # General ConstantNode that can hold constants that are not JSON-serializable
 ConstantNode = t.Union[ConstantNodeJSON, ConstantNodePickle]
+# ID of a node that can be a task argument. Multiple node types can be task inputs.
+# This is contrary to the outputs; only artifact nodes can be task outputs.
 ArgumentId = t.Union[ArtifactNodeId, ConstantNodeId, SecretNodeId]
 
 
 class TaskInvocation(BaseModel):
     id: TaskInvocationId
 
     # What task should be executed.
@@ -387,7 +413,50 @@
 
     # Metadata defaults to None to allow older JSON to be loaded
     metadata: t.Optional[WorkflowMetadata] = None
 
     # The resources that are available for the workflow to use.
     # If none, the runtime will decide.
     resources: t.Optional[Resources] = None
+
+    @pydantic.validator("metadata", always=True)
+    def sdk_version_up_to_date(cls, v: t.Optional[WorkflowMetadata]):
+        # Workaround for circular imports
+        from orquestra.sdk import exceptions
+        from orquestra.sdk.packaging import _versions
+        from orquestra.sdk.schema import _compat
+
+        current_version = _versions.get_current_sdk_version()
+
+        if v is None:
+            warnings.warn(
+                exceptions.VersionMismatch(
+                    (
+                        "Attempting to read a workflow definition generated with an "
+                        "old version of Orquestra Workflow SDK. Please consider "
+                        "re-running your workflow or downgrading orquestra-sdk. "
+                        "For more information visit: https://docs.orquestra.io/docs/core/sdk/guides/version-compatibility.html"  # noqa: E501
+                    ),
+                    actual=current_version,
+                    needed=None,
+                )
+            )
+            return v
+
+        if not _compat.versions_are_compatible(
+            generated_at=v.sdk_version, current=current_version
+        ):
+            warnings.warn(
+                exceptions.VersionMismatch(
+                    (
+                        "Attempting to read a workflow definition generated with a "
+                        "different version of Orquestra Workflow SDK. "
+                        "Please consider re-running your workflow or installing "
+                        f"'orquestra-sdk=={v.sdk_version.original}'. "
+                        "For more information visit: https://docs.orquestra.io/docs/core/sdk/guides/version-compatibility.html"  # noqa: E501
+                    ),
+                    actual=current_version,
+                    needed=v.sdk_version,
+                )
+            )
+
+        return v
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/schema/local_database.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/schema/local_database.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/schema/responses.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/schema/responses.py`

 * *Files 6% similar despite different names*

```diff
@@ -162,14 +162,19 @@
 
 
 WorkflowResult = Annotated[
     t.Union[JSONResult, PickleResult], Field(discriminator="serialization_format")
 ]
 
 
+class ComputeEngineWorkflowResult(BaseModel):
+    results: t.Tuple[WorkflowResult, ...]
+    type: t.Literal["ComputeEngineWorkflowResult"] = "ComputeEngineWorkflowResult"
+
+
 class GetWorkflowRunResultsResponse(BaseModel):
     meta: ResponseMetadata
     workflow_run_id: str
     workflow_results: t.List[WorkflowResult]
 
 
 class GetArtifactsResponse(BaseModel):
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/schema/workflow_run.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/schema/workflow_run.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 from pydantic import BaseModel
 
 from orquestra.sdk.schema.ir import TaskInvocationId, WorkflowDef
 
 WorkflowRunId = str
 TaskRunId = str
+WorkspaceId = str
+ProjectId = str
 
 
 class State(enum.Enum):
     WAITING = "WAITING"
     RUNNING = "RUNNING"
     SUCCEEDED = "SUCCEEDED"
     TERMINATED = "TERMINATED"
@@ -60,7 +62,12 @@
 class WorkflowRun(WorkflowRunMinimal):
     """
     A full workflow run with TaskRuns and WorkflowRun status
     """
 
     task_runs: t.List[TaskRun]
     status: RunStatus
+
+
+class ProjectRef(BaseModel):
+    workspace_id: WorkspaceId
+    project_id: ProjectId
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/schema/yaml_model.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/schema/yaml_model.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/secrets/__init__.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/secrets/_api.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/secrets/_api.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/secrets/_auth.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/secrets/_auth.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/secrets/_client.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/secrets/_client.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/secrets/_exceptions.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/secrets/_exceptions.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/secrets/_models.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/secrets/_models.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra/sdk/v2/__init__.py` & `orquestra-sdk-0.47.0/src/orquestra/sdk/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/src/orquestra_sdk.egg-info/PKG-INFO` & `orquestra-sdk-0.47.0/src/orquestra_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orquestra-sdk
-Version: 0.46.0
+Version: 0.47.0
 Summary: "Compose Orquestra workflows using a Python DSL"
 Home-page: https://github.com/zapatacomputing/orquestra-workflow-sdk
 Author: Zapata Computing Inc.
 Author-email: info@zapatacomputing.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `orquestra-sdk-0.46.0/src/orquestra_sdk.egg-info/requires.txt` & `orquestra-sdk-0.47.0/src/orquestra_sdk.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 dill==0.3.6
 wrapt
 filelock>=3.3.2
 packaging>=21
 GitPython
 pip-api==0.0.30
 importlib_metadata~=4.0
-typing-extensions~=4.0
+typing-extensions>=4.1.0
 pyyaml
 requests~=2.28
 graphviz
 argcomplete
 click~=8.0
 cloup~=2.0
 inquirer~=3.0
```

### Comparing `orquestra-sdk-0.46.0/subtrees/z_quantum_actions/Makefile` & `orquestra-sdk-0.47.0/subtrees/z_quantum_actions/Makefile`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/subtrees/z_quantum_actions/README.rst` & `orquestra-sdk-0.47.0/subtrees/z_quantum_actions/README.rst`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/subtrees/z_quantum_actions/actions/publish-release/action.yml` & `orquestra-sdk-0.47.0/subtrees/z_quantum_actions/actions/publish-release/action.yml`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/subtrees/z_quantum_actions/bin/get_next_version.py` & `orquestra-sdk-0.47.0/subtrees/z_quantum_actions/bin/get_next_version.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/subtrees/z_quantum_actions/pyproject.toml` & `orquestra-sdk-0.47.0/subtrees/z_quantum_actions/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/subtrees/z_quantum_actions/sample_setup.py` & `orquestra-sdk-0.47.0/subtrees/z_quantum_actions/sample_setup.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/subtrees/z_quantum_actions/setup_extras.py` & `orquestra-sdk-0.47.0/subtrees/z_quantum_actions/setup_extras.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/subtrees/z_quantum_actions/tests/test_get_next_version.py` & `orquestra-sdk-0.47.0/subtrees/z_quantum_actions/tests/test_get_next_version.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml` & `orquestra-sdk-0.47.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/subtrees/z_quantum_actions/workflow-templates/publish_release.yml` & `orquestra-sdk-0.47.0/subtrees/z_quantum_actions/workflow-templates/publish_release.yml`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/subtrees/z_quantum_actions/workflow-templates/style.yml` & `orquestra-sdk-0.47.0/subtrees/z_quantum_actions/workflow-templates/style.yml`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/cli/dorq/task/test_task_logs.py` & `orquestra-sdk-0.47.0/tests/cli/dorq/task/test_task_logs.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/cli/dorq/task/test_task_results.py` & `orquestra-sdk-0.47.0/tests/cli/dorq/task/test_task_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
             # Mocks
             error_presenter = create_autospec(WrappedCorqOutputPresenter)
             artifact_presenter = create_autospec(ArtifactPresenter)
             dumper = create_autospec(TaskOutputDumper)
             wf_run_repo = create_autospec(WorkflowRunRepo)
 
-            fake_outputs = ["my_log_1", "my_log_2"]
+            fake_outputs = ["output val 1", "output val 2"]
             wf_run_repo.get_task_outputs.return_value = fake_outputs
 
             config_resolver = create_autospec(WFConfigResolver)
             config_resolver.resolve.return_value = resolved_config
 
             wf_run_resolver = create_autospec(WFRunResolver)
             wf_run_resolver.resolve_id.return_value = resolved_wf_run_id
@@ -143,15 +143,15 @@
             # details = create_autospec(DumpDetails)
             dump_details = "<dump details sentinel>"
             dumper = create_autospec(TaskOutputDumper)
             dumper.dump.return_value = dump_details
 
             wf_run_repo = create_autospec(WorkflowRunRepo)
 
-            fake_outputs = ["my_log_1", "my_log_2"]
+            fake_outputs = ["output val 1", "output val 2"]
             wf_run_repo.get_task_outputs.return_value = fake_outputs
 
             config_resolver = create_autospec(WFConfigResolver)
             config_resolver.resolve.return_value = resolved_config
 
             wf_run_resolver = create_autospec(WFRunResolver)
             wf_run_resolver.resolve_id.return_value = resolved_wf_run_id
```

### Comparing `orquestra-sdk-0.46.0/tests/cli/dorq/test_arg_resolvers.py` & `orquestra-sdk-0.47.0/tests/cli/dorq/test_arg_resolvers.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/cli/dorq/test_cli_logs.py` & `orquestra-sdk-0.47.0/tests/cli/dorq/test_cli_logs.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/cli/dorq/test_dumpers.py` & `orquestra-sdk-0.47.0/tests/cli/dorq/test_dumpers.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/cli/dorq/test_entrypoint.py` & `orquestra-sdk-0.47.0/tests/cli/dorq/test_entrypoint.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/cli/dorq/test_login.py` & `orquestra-sdk-0.47.0/tests/cli/dorq/test_login.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/cli/dorq/test_login_server.py` & `orquestra-sdk-0.47.0/tests/cli/dorq/test_login_server.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/cli/dorq/test_repos.py` & `orquestra-sdk-0.47.0/tests/cli/dorq/test_repos.py`

 * *Files 2% similar despite different names*

```diff
@@ -415,31 +415,40 @@
                         ir.TaskDef(
                             id="task1",
                             fn_ref=ir.ModuleFunctionRef(
                                 module="tasks",
                                 function_name="task_in_another_module",
                             ),
                             parameters=[],
+                            output_metadata=ir.TaskOutputMetadata(
+                                is_subscriptable=False, n_outputs=1
+                            ),
                             source_import_id="imp1",
                         ),
                         ir.TaskDef(
                             id="task2",
                             fn_ref=ir.FileFunctionRef(
                                 file_path="other_tasks.py",
                                 function_name="task_in_another_file",
                             ),
                             parameters=[],
+                            output_metadata=ir.TaskOutputMetadata(
+                                is_subscriptable=False, n_outputs=1
+                            ),
                             source_import_id="imp1",
                         ),
                         ir.TaskDef(
                             id="task3",
                             fn_ref=ir.InlineFunctionRef(
                                 function_name="inlined_task", encoded_function=[]
                             ),
                             parameters=[],
+                            output_metadata=ir.TaskOutputMetadata(
+                                is_subscriptable=False, n_outputs=1
+                            ),
                             source_import_id="imp1",
                         ),
                     ]
                 )
                 by_id = Mock(return_value=wf_run)
                 monkeypatch.setattr(sdk.WorkflowRun, "by_id", by_id)
 
@@ -466,22 +475,28 @@
                     [
                         ir.TaskDef(
                             id="task1",
                             fn_ref=ir.ModuleFunctionRef(
                                 module="tasks1", function_name=fn_name
                             ),
                             parameters=[],
+                            output_metadata=ir.TaskOutputMetadata(
+                                is_subscriptable=False, n_outputs=1
+                            ),
                             source_import_id="imp1",
                         ),
                         ir.TaskDef(
                             id="task2",
                             fn_ref=ir.ModuleFunctionRef(
                                 module="tasks2", function_name=fn_name
                             ),
                             parameters=[],
+                            output_metadata=ir.TaskOutputMetadata(
+                                is_subscriptable=False, n_outputs=1
+                            ),
                             source_import_id="imp1",
                         ),
                     ]
                 )
                 by_id = Mock(return_value=wf_run)
                 monkeypatch.setattr(sdk.WorkflowRun, "by_id", by_id)
 
@@ -535,50 +550,111 @@
 
                 # Then
                 with pytest.raises(type(exc)):
                     # When
                     _ = repo.get_task_inv_ids(wf_run_id, config_name, task_fn_name)
 
         class TestGetTaskOutputs:
-            @staticmethod
-            def test_passing_data(monkeypatch):
-                run_id = "wf.1"
-                inv_id = "inv1"
-                config_name = "<config sentinel>"
+            class TestHappyPath:
+                @staticmethod
+                def _make_wf_run(
+                    monkeypatch,
+                    inv_id: str,
+                    fake_task_run_outputs,
+                    task_meta: ir.TaskOutputMetadata,
+                ) -> sdk.WorkflowRun:
+                    task_run = create_autospec(sdk.TaskRun)
+                    task_run.task_invocation_id = inv_id
+                    task_run.get_outputs.return_value = fake_task_run_outputs
+
+                    task_def = create_autospec(ir.TaskDef)
+                    task_def_id = "task_def_1"
+                    task_def.output_metadata = task_meta
+
+                    inv = create_autospec(ir.TaskInvocation)
+                    inv.task_id = task_def_id
+
+                    wf_def = create_autospec(ir.WorkflowDef)
+                    wf_def.task_invocations = {inv_id: inv}
+                    wf_def.tasks = {task_def_id: task_def}
+
+                    wf_run = create_autospec(sdk.WorkflowRun)
+                    wf_run.get_tasks.return_value = {task_run}
+                    wf_run.get_status_model().workflow_def = wf_def
+
+                    by_id = Mock(return_value=wf_run)
+                    monkeypatch.setattr(sdk.WorkflowRun, "by_id", by_id)
+
+                    return wf_run
+
+                def test_single_output(self, monkeypatch):
+                    # Given
+                    run_id = "wf.1"
+                    inv_id = "inv1"
+                    config_name = "<config sentinel>"
+                    fake_output = "<task output sentinel>"
+
+                    self._make_wf_run(
+                        monkeypatch,
+                        inv_id=inv_id,
+                        fake_task_run_outputs=fake_output,
+                        task_meta=ir.TaskOutputMetadata(
+                            n_outputs=1,
+                            is_subscriptable=False,
+                        ),
+                    )
 
-                wf_run = Mock()
-                fake_outputs = ("<output sentinel 0>", "<output sentinel 1>")
-                wf_run.get_artifacts.return_value = {
-                    inv_id: fake_outputs,
-                }
+                    repo = _repos.WorkflowRunRepo()
 
-                by_id = Mock(return_value=wf_run)
-                monkeypatch.setattr(sdk.WorkflowRun, "by_id", by_id)
+                    # When
+                    outputs = repo.get_task_outputs(
+                        wf_run_id=run_id, task_inv_id=inv_id, config_name=config_name
+                    )
+
+                    # Then
+                    assert outputs == (fake_output,)
+
+                def test_multiple_outputs(self, monkeypatch):
+                    # Given
+                    run_id = "wf.1"
+                    inv_id = "inv1"
+                    config_name = "<config sentinel>"
+                    fake_outputs = ("<out1>", "<out2>")
+
+                    self._make_wf_run(
+                        monkeypatch,
+                        inv_id=inv_id,
+                        fake_task_run_outputs=fake_outputs,
+                        task_meta=ir.TaskOutputMetadata(
+                            n_outputs=2,
+                            is_subscriptable=True,
+                        ),
+                    )
 
-                repo = _repos.WorkflowRunRepo()
+                    repo = _repos.WorkflowRunRepo()
 
-                # When
-                outputs = repo.get_task_outputs(
-                    wf_run_id=run_id, task_inv_id=inv_id, config_name=config_name
-                )
+                    # When
+                    outputs = repo.get_task_outputs(
+                        wf_run_id=run_id, task_inv_id=inv_id, config_name=config_name
+                    )
 
-                # Then
-                assert outputs == fake_outputs
+                    # Then
+                    assert outputs == fake_outputs
 
             @staticmethod
             def test_invalid_inv_id(monkeypatch):
                 run_id = "wf.1"
                 inv_id = "inv1"
                 config_name = "<config sentinel>"
 
-                wf_run = Mock()
-                fake_outputs = ("<output sentinel 0>", "<output sentinel 1>")
-                wf_run.get_artifacts.return_value = {
-                    "non-existing-inv-id": fake_outputs,
-                }
+                task_run = create_autospec(sdk.TaskRun)
+                task_run.task_invocation_id = "<invalid inv ID>"
+
+                wf_run = create_autospec(sdk.WorkflowRun)
+                wf_run.get_tasks.return_value = {task_run}
 
                 by_id = Mock(return_value=wf_run)
                 monkeypatch.setattr(sdk.WorkflowRun, "by_id", by_id)
 
                 repo = _repos.WorkflowRunRepo()
 
                 # Then
```

### Comparing `orquestra-sdk-0.46.0/tests/cli/dorq/ui/data/wf_runs/running.txt` & `orquestra-sdk-0.47.0/tests/cli/dorq/ui/data/wf_runs/running.txt`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/cli/dorq/ui/test_errors.py` & `orquestra-sdk-0.47.0/tests/cli/dorq/ui/test_errors.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/cli/dorq/ui/test_presenters.py` & `orquestra-sdk-0.47.0/tests/cli/dorq/ui/test_presenters.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/cli/dorq/workflow/test_list.py` & `orquestra-sdk-0.47.0/tests/cli/dorq/workflow/test_list.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/cli/dorq/workflow/test_logs.py` & `orquestra-sdk-0.47.0/tests/cli/dorq/workflow/test_logs.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/cli/dorq/workflow/test_results.py` & `orquestra-sdk-0.47.0/tests/cli/dorq/workflow/test_results.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/cli/dorq/workflow/test_stop.py` & `orquestra-sdk-0.47.0/tests/cli/dorq/workflow/test_stop.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/cli/dorq/workflow/test_submit.py` & `orquestra-sdk-0.47.0/tests/cli/dorq/workflow/test_submit.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/cli/dorq/workflow/test_view.py` & `orquestra-sdk-0.47.0/tests/cli/dorq/workflow/test_view.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/conftest.py` & `orquestra-sdk-0.47.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/reloaders.py` & `orquestra-sdk-0.47.0/tests/reloaders.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/api/test_api_with_qe.py` & `orquestra-sdk-0.47.0/tests/runtime/api/test_api_with_qe.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/api/test_api_with_ray.py` & `orquestra-sdk-0.47.0/tests/runtime/api/test_api_with_ray.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/corq/data/cli_outputs/failed_wf_run.txt` & `orquestra-sdk-0.47.0/tests/runtime/corq/data/cli_outputs/failed_wf_run.txt`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/corq/data/responses/failed_wf_run.json` & `orquestra-sdk-0.47.0/tests/runtime/corq/data/responses/failed_wf_run.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998914930555556%*

 * *Differences: {"'workflow_runs'": "{0: {'workflow_def': {'tasks': {'task-generate-data-786a9eaf26': "*

 * *                    "{'output_metadata': OrderedDict([('is_subscriptable', True), ('n_outputs', "*

 * *                    "2)])}, 'task-train-model-6339962840': {'output_metadata': "*

 * *                    "OrderedDict([('is_subscriptable', False), ('n_outputs', 1)])}}}}}"}*

```diff
@@ -158,14 +158,18 @@
                             "file_path": "workflow_defs.py",
                             "function_name": "generate_data",
                             "line_number": 13,
                             "module": "workflow_defs",
                             "type": "MODULE_FUNCTION_REF"
                         },
                         "id": "task-generate-data-786a9eaf26",
+                        "output_metadata": {
+                            "is_subscriptable": true,
+                            "n_outputs": 2
+                        },
                         "parameters": [
                             {
                                 "kind": "POSITIONAL_OR_KEYWORD",
                                 "name": "size"
                             },
                             {
                                 "kind": "POSITIONAL_OR_KEYWORD",
@@ -189,14 +193,18 @@
                             "file_path": "workflow_defs.py",
                             "function_name": "train_model",
                             "line_number": 25,
                             "module": "workflow_defs",
                             "type": "MODULE_FUNCTION_REF"
                         },
                         "id": "task-train-model-6339962840",
+                        "output_metadata": {
+                            "is_subscriptable": false,
+                            "n_outputs": 1
+                        },
                         "parameters": [
                             {
                                 "kind": "POSITIONAL_OR_KEYWORD",
                                 "name": "x"
                             },
                             {
                                 "kind": "POSITIONAL_OR_KEYWORD",
```

### Comparing `orquestra-sdk-0.46.0/tests/runtime/corq/test_format.py` & `orquestra-sdk-0.47.0/tests/runtime/corq/test_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,15 @@
                 (
                     responses.GetWorkflowRunResponse,
                     DATA_DIR / "responses" / "failed_wf_run.json",
                     DATA_DIR / "cli_outputs" / "failed_wf_run.txt",
                 ),
             ],
         )
+        @pytest.mark.filterwarnings("ignore::orquestra.sdk.exceptions.VersionMismatch")
         def test_matches_recorded_output(
             capsys, resp_cls, resp_path: Path, recorded_output_path: Path
         ):
             # Given
             resp_model = resp_cls.parse_file(resp_path)
 
             # When
```

### Comparing `orquestra-sdk-0.46.0/tests/runtime/db/test_db.py` & `orquestra-sdk-0.47.0/tests/runtime/db/test_db.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/db/test_migration.py` & `orquestra-sdk-0.47.0/tests/runtime/db/test_migration.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/performance/conftest.py` & `orquestra-sdk-0.47.0/tests/runtime/performance/conftest.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/performance/test_cli_perf.py` & `orquestra-sdk-0.47.0/tests/runtime/performance/test_cli_perf.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/project_state.py` & `orquestra-sdk-0.47.0/tests/runtime/project_state.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/qe/test_qe_date_conversion.py` & `orquestra-sdk-0.47.0/tests/runtime/qe/test_qe_date_conversion.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/qe/test_qe_runtime.py` & `orquestra-sdk-0.47.0/tests/runtime/qe/test_qe_runtime.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,25 +11,34 @@
 from pathlib import Path
 from unittest.mock import MagicMock, Mock, PropertyMock
 
 import pytest
 import responses
 
 import orquestra.sdk as sdk
-import orquestra.sdk._base._db as _db
-import orquestra.sdk._base._qe._qe_runtime as _qe_runtime
 from orquestra.sdk import exceptions
+from orquestra.sdk._base import _db, serde
 from orquestra.sdk._base._conversions._yaml_exporter import (
     pydantic_to_yaml,
     workflow_to_yaml,
 )
+from orquestra.sdk._base._qe import _qe_runtime
 from orquestra.sdk._base._testing._example_wfs import my_workflow
 from orquestra.sdk.schema.configs import RuntimeConfiguration, RuntimeName
+from orquestra.sdk.schema.ir import ArtifactFormat, ArtifactNodeId, TaskInvocationId
 from orquestra.sdk.schema.local_database import StoredWorkflowRun
-from orquestra.sdk.schema.workflow_run import RunStatus, State, TaskRun, WorkflowRun
+from orquestra.sdk.schema.responses import JSONResult, PickleResult, WorkflowResult
+from orquestra.sdk.schema.workflow_run import (
+    ProjectRef,
+    RunStatus,
+    State,
+    TaskRun,
+    WorkflowRun,
+    WorkflowRunId,
+)
 
 QE_MINIMAL_CURRENT_REPRESENTATION: t.Dict[str, t.Any] = {
     "status": {
         "phase": "Succeeded",
         "startedAt": "1989-12-13T09:03:49Z",
         "finishedAt": "1989-12-13T09:05:14Z",
         "nodes": {
@@ -458,32 +467,45 @@
         monkeypatch.setattr(_db.WorkflowDB, "save_workflow_run", _save_workflow_run)
         mocked_responses.add(
             responses.POST,
             "http://localhost/v1/workflows",
             body=QE_RESPONSES["submit"],
         )
 
-        result = runtime.create_workflow_run(TEST_WORKFLOW)
+        result = runtime.create_workflow_run(TEST_WORKFLOW, None)
 
         _save_workflow_run.assert_called_once()
         assert result == "workflow-id"
 
+    def test_project_raises_warning(self, monkeypatch, runtime, mocked_responses):
+        _save_workflow_run = Mock()
+        monkeypatch.setattr(_db.WorkflowDB, "save_workflow_run", _save_workflow_run)
+        mocked_responses.add(
+            responses.POST,
+            "http://localhost/v1/workflows",
+            body=QE_RESPONSES["submit"],
+        )
+        with pytest.warns(expected_warning=exceptions.UnsupportedRuntimeFeature):
+            runtime.create_workflow_run(
+                TEST_WORKFLOW, project=ProjectRef(workspace_id="", project_id="")
+            )
+
     @staticmethod
     def test_exception_on_bad_request_too_large(monkeypatch, runtime, mocked_responses):
         _save_workflow_run = Mock()
         monkeypatch.setattr(_db.WorkflowDB, "save_workflow_run", _save_workflow_run)
         mocked_responses.add(
             responses.POST,
             "http://localhost/v1/workflows",
             status=400,
             body="Failed to run workflow : Request entity too large: limit is 3145728",
         )
 
         with pytest.raises(exceptions.WorkflowTooLargeError) as exc_info:
-            _ = runtime.create_workflow_run(TEST_WORKFLOW)
+            _ = runtime.create_workflow_run(TEST_WORKFLOW, None)
 
         _save_workflow_run.assert_not_called()
         assert "The submitted workflow is too large to be run on this cluster." in str(
             exc_info
         )
 
     @staticmethod
@@ -496,15 +518,15 @@
             responses.POST,
             "http://localhost/v1/workflows",
             status=400,
             body="some other submission failure",
         )
 
         with pytest.raises(exceptions.WorkflowSyntaxError) as exc_info:
-            _ = runtime.create_workflow_run(TEST_WORKFLOW)
+            _ = runtime.create_workflow_run(TEST_WORKFLOW, None)
 
         _save_workflow_run.assert_not_called()
         assert "some other submission failure" in str(exc_info)
 
     @staticmethod
     @pytest.mark.parametrize(
         "workflow_name",
@@ -525,105 +547,129 @@
         @sdk.workflow(custom_name=workflow_name)
         def BadNameWorkflow():
             return [simple_task()]
 
         workflow = BadNameWorkflow.model
 
         with pytest.raises(exceptions.InvalidWorkflowDefinitionError) as exc_info:
-            runtime.create_workflow_run(workflow)
+            runtime.create_workflow_run(workflow, None)
 
         assert f'Workflow name "{workflow_name}" is invalid' in str(exc_info)
 
     def test_yaml_to_stderr(
         self, monkeypatch, runtime_verbose, runtime, mocked_responses, capsys
     ):
         _save_workflow_run = Mock()
         monkeypatch.setattr(_db.WorkflowDB, "save_workflow_run", _save_workflow_run)
         mocked_responses.add(
             responses.POST,
             "http://localhost/v1/workflows",
             body=QE_RESPONSES["submit"],
         )
-        _ = runtime.create_workflow_run(TEST_WORKFLOW)
+        _ = runtime.create_workflow_run(TEST_WORKFLOW, None)
         captured_without_yaml = capsys.readouterr()
-        _ = runtime_verbose.create_workflow_run(TEST_WORKFLOW)
+        _ = runtime_verbose.create_workflow_run(TEST_WORKFLOW, None)
         captured_with_yaml = capsys.readouterr()
         yaml_wf = pydantic_to_yaml(workflow_to_yaml(TEST_WORKFLOW))
         assert yaml_wf in captured_with_yaml.err
         assert yaml_wf not in captured_without_yaml.err
 
 
+def _mock_artifact_resp(
+    responses,
+    wf_run_id: WorkflowRunId,
+    inv_id: TaskInvocationId,
+    art_id: ArtifactNodeId,
+    result_model: WorkflowResult,
+):
+    responses.add(
+        responses.GET,
+        f"http://localhost/v2/workflows/{wf_run_id}/step/{inv_id}/artifact/{art_id}",
+        content_type="application/x-gtar-compressed",
+        body=_make_result_bytes(dict(result_model)),
+    )
+
+
+def _make_pickle_result(artifact_value) -> PickleResult:
+    result = serde.result_from_artifact(
+        artifact_value, artifact_format=ArtifactFormat.ENCODED_PICKLE
+    )
+    assert isinstance(result, PickleResult), "Invalid serialization used"
+    return result
+
+
 class TestGetAvailableOutputs:
     def test_successful_workflow(self, monkeypatch, runtime, mocked_responses):
+        wf_run_id = "hello-there-abc123-r000"
         _get_workflow_run = Mock(
             return_value=StoredWorkflowRun(
-                workflow_run_id="hello-there-abc123-r000",
+                workflow_run_id=wf_run_id,
                 config_name="hello",
                 workflow_def=TEST_WORKFLOW,
             )
         )
         monkeypatch.setattr(_db.WorkflowDB, "get_workflow_run", _get_workflow_run)
-        mocked_responses.add(
-            responses.GET,
-            "http://localhost/v2/workflows/hello-there-abc123-r000/step/invocation-0-task-make-greeting-message/artifact/artifact-0-make-greeting-message",  # noqa
-            content_type="application/x-gtar-compressed",
-            body=_make_result_bytes(
-                {"value": '"hello, alex zapata!there"', "serialization_format": "JSON"}
-            ),
-        )
-        mocked_responses.add(
-            responses.GET,
-            "http://localhost/v2/workflows/hello-there-abc123-r000/step/invocation-1-task-multi-output-test/artifact/artifact-1-multi-output-test",  # noqa
-            content_type="application/x-gtar-compressed",
-            body=_make_result_bytes(
-                {"value": '"there"', "serialization_format": "JSON"}
-            ),
+
+        expected_inv_0 = JSONResult(value='"hello, alex zapata!there"')
+        _mock_artifact_resp(
+            mocked_responses,
+            wf_run_id=wf_run_id,
+            inv_id="invocation-0-task-make-greeting-message",
+            art_id="artifact-0-make-greeting-message",
+            result_model=expected_inv_0,
+        )
+        expected_inv_1 = _make_pickle_result(artifact_value=("hello", "there"))
+        _mock_artifact_resp(
+            mocked_responses,
+            wf_run_id=wf_run_id,
+            inv_id="invocation-1-task-multi-output-test",
+            art_id="artifact-3-multi-output-test",
+            result_model=expected_inv_1,
         )
 
         result = runtime.get_available_outputs("hello-there-abc123-r000")
 
         assert result == {
-            "invocation-0-task-make-greeting-message": ("hello, alex zapata!there",),
-            "invocation-1-task-multi-output-test": ("there",),
+            "invocation-0-task-make-greeting-message": expected_inv_0,
+            "invocation-1-task-multi-output-test": expected_inv_1,
         }
 
     def test_failed_workflow(self, monkeypatch, runtime, mocked_responses):
+        wf_run_id = "wf-3fmte-r000"
         _get_workflow_run = Mock(
             return_value=StoredWorkflowRun(
-                workflow_run_id="wf-3fmte-r000",
+                workflow_run_id=wf_run_id,
                 config_name="hello",
                 workflow_def=TEST_WORKFLOW,
             )
         )
         monkeypatch.setattr(_db.WorkflowDB, "get_workflow_run", _get_workflow_run)
 
-        mocked_responses.add(
-            responses.GET,
-            "http://localhost/v2/workflows/wf-3fmte-r000/step/invocation-0-task-make-greeting-message/artifact/artifact-0-make-greeting-message",  # noqa
-            content_type="application/x-gtar-compressed",
-            body=_make_result_bytes(
-                {"value": '"hello, alex zapata!there"', "serialization_format": "JSON"}
-            ),
+        expected_inv_0 = JSONResult(value='"hello, alex zapata!there"')
+        _mock_artifact_resp(
+            mocked_responses,
+            wf_run_id=wf_run_id,
+            inv_id="invocation-0-task-make-greeting-message",
+            art_id="artifact-0-make-greeting-message",
+            result_model=expected_inv_0,
         )
         mocked_responses.add(
             responses.GET,
-            "http://localhost/v2/workflows/wf-3fmte-r000/step/invocation-1-task-multi-output-test/artifact/artifact-1-multi-output-test",  # noqa
+            "http://localhost/v2/workflows/wf-3fmte-r000/step/invocation-1-task-multi-output-test/artifact/artifact-3-multi-output-test",  # noqa
             status=404,
             json={
                 "meta": {},
                 "message": "not found",
             },
         )
 
         result = runtime.get_available_outputs("wf-3fmte-r000")
         # There should be a result for 1 task that finish successfully
         assert len(result) == 1
-        assert result["invocation-0-task-make-greeting-message"] == (
-            "hello, alex zapata!there",
-        )
+        assert result["invocation-0-task-make-greeting-message"] == expected_inv_0
 
 
 class TestGetWorkflowRunStatus:
     def test_happy_path(self, monkeypatch, runtime, mocked_responses):
         _get_workflow_run = Mock(
             return_value=StoredWorkflowRun(
                 workflow_run_id="hello-there-abc123-r000",
@@ -859,15 +905,15 @@
             body=QE_RESPONSES["results_bytes"],
         )
 
         result = runtime.get_workflow_run_outputs_non_blocking(
             "hello-there-abc123-r000"
         )
 
-        assert result == ("hello, alex zapata!there",)
+        assert result == (JSONResult(value='"hello, alex zapata!there"'),)
 
     def test_get_workflow_run_outputs_non_blocking_fails(
         self, mock_workflow_db_location
     ):
         # Fake QE configuration
         config = RuntimeConfiguration(
             config_name="hello",
@@ -1347,15 +1393,15 @@
         monkeypatch.setattr(_db.WorkflowDB, "save_workflow_run", _save_workflow_run)
         mocked_responses.add(
             responses.POST,
             "http://localhost/v1/workflows",
             status=error_code,
         )
         with pytest.raises(expected_exception) as exc_info:
-            runtime.create_workflow_run(TEST_WORKFLOW)
+            runtime.create_workflow_run(TEST_WORKFLOW, None)
         for telltale in telltales:
             assert telltale in str(exc_info)
         _save_workflow_run.assert_not_called()
 
     def test_get_workflow_run_status(
         self,
         error_code,
```

### Comparing `orquestra-sdk-0.46.0/tests/runtime/qe/test_response_parsers.py` & `orquestra-sdk-0.47.0/tests/runtime/qe/test_response_parsers.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/qe/test_tar_extraction.py` & `orquestra-sdk-0.47.0/tests/runtime/qe/test_tar_extraction.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/ray/conftest.py` & `orquestra-sdk-0.47.0/tests/runtime/ray/conftest.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/ray/data/ml_demo/workflow_defs.py` & `orquestra-sdk-0.47.0/tests/runtime/ray/data/ml_demo/workflow_defs.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/ray/data/module_level_function/workflow_defs.py` & `orquestra-sdk-0.47.0/tests/runtime/ray/data/module_level_function/workflow_defs.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/ray/data/passing_closures/workflow_defs.py` & `orquestra-sdk-0.47.0/tests/runtime/ray/data/passing_closures/workflow_defs.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/ray/data/python_package/python_package_dependent_workflow.json` & `orquestra-sdk-0.47.0/tests/runtime/ray/data/python_package/python_package_dependent_workflow.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8327132936507936%*

 * *Differences: {"'constant_nodes'": "{'constant-0': {'chunks': "*

 * *                     "['gASVeAAAAAAAAACMFnBvbGFycy5kYXRhZnJhbWUuZnJhbWWUjAlEYXRhRnJhbWWUk5QpgZRdlIwU\\ncG9sYXJzLnNlcmllcy5zZXJpZXOUjAZTZXJpZXOUk5QpgZRDIKNkbmFtZWFhaGRhdGF0eXBlZUlu\\ndDY0ZnZhbHVlc4EVlGJhYi4=\\n']}}",*

 * * "'fn_ref'": "{'file_path': 'tests/runtime/ray/data/python_package/original_workflow.py', "*

 * *             "'line_number': 14}",*

 * * "'imports'": "{'python-import-4b988e935a': OrderedDict([('id', 'python-import-4b988e935a'), "*

 * *              "('package […]*

```diff
@@ -6,98 +6,105 @@
             "id": "artifact-0-my-fn",
             "serialization_format": "AUTO"
         }
     },
     "constant_nodes": {
         "constant-0": {
             "chunks": [
-                "gASVqAAAAAAAAACMFnBvbGFycy5kYXRhZnJhbWUuZnJhbWWUjAlEYXRhRnJhbWWUk5QpgZRdlIwU\ncG9sYXJzLnNlcmllcy5zZXJpZXOUjAZTZXJpZXOUk5QpgZRDUAMAAAAAAAAABAAAAAAAAABuYW1l\nAQAAAAAAAABhCAAAAAAAAABkYXRhdHlwZQgAAAAGAAAAAAAAAHZhbHVlcwEAAAAAAAAAARUAAAAA\nAAAAlGJhYi4=\n"
+                "gASVeAAAAAAAAACMFnBvbGFycy5kYXRhZnJhbWUuZnJhbWWUjAlEYXRhRnJhbWWUk5QpgZRdlIwU\ncG9sYXJzLnNlcmllcy5zZXJpZXOUjAZTZXJpZXOUk5QpgZRDIKNkbmFtZWFhaGRhdGF0eXBlZUlu\ndDY0ZnZhbHVlc4EVlGJhYi4=\n"
             ],
             "id": "constant-0",
             "serialization_format": "ENCODED_PICKLE",
             "value_preview": "shape: (1, 1"
         }
     },
     "data_aggregation": null,
     "fn_ref": {
-        "file_path": "a.py",
+        "file_path": "tests/runtime/ray/data/python_package/original_workflow.py",
         "function_name": "wf",
-        "line_number": 11,
+        "line_number": 14,
         "module": "__main__",
         "type": "MODULE_FUNCTION_REF"
     },
     "imports": {
         "inline-import-1": {
             "id": "inline-import-1",
             "type": "INLINE_IMPORT"
         },
-        "python-import-e0459ec73a": {
-            "id": "python-import-e0459ec73a",
+        "python-import-4b988e935a": {
+            "id": "python-import-4b988e935a",
             "packages": [
                 {
                     "environment_markers": "",
                     "extras": [],
                     "name": "polars",
-                    "version_constraints": []
+                    "version_constraints": [
+                        "==0.17.3"
+                    ]
                 }
             ],
             "pip_options": [],
             "type": "PYTHON_IMPORT"
         }
     },
     "metadata": {
         "python_version": {
             "is_prerelease": false,
             "major": 3,
             "minor": 8,
-            "original": "3.8.12 (default, Jun 28 2022, 14:32:09) \n[Clang 13.1.6 (clang-1316.0.21.2.5)]",
+            "original": "3.8.12 (default, Apr 28 2022, 11:46:59) \n[Clang 12.0.5 (clang-1205.0.22.9)]",
             "patch": 12
         },
         "sdk_version": {
             "is_prerelease": true,
             "major": 0,
             "minor": 45,
-            "original": "0.45.2.dev11+gf708e3b",
+            "original": "0.45.2.dev18+ga73915e.d20230405",
             "patch": 2
         }
     },
     "name": "wf",
     "output_ids": [
         "artifact-0-my-fn"
     ],
+    "resources": null,
     "secret_nodes": {},
     "task_invocations": {
         "invocation-0-task-my-fn": {
             "args_ids": [
                 "constant-0"
             ],
             "custom_image": "zapatacomputing/orquestra-default:v0.0.0",
             "id": "invocation-0-task-my-fn",
             "kwargs_ids": {},
             "output_ids": [
                 "artifact-0-my-fn"
             ],
             "resources": null,
-            "task_id": "task-my-fn-d3914c5e63"
+            "task_id": "task-my-fn-55d017d1e7"
         }
     },
     "tasks": {
-        "task-my-fn-d3914c5e63": {
+        "task-my-fn-55d017d1e7": {
             "custom_image": "zapatacomputing/orquestra-default:v0.0.0",
             "dependency_import_ids": [
-                "python-import-e0459ec73a"
+                "python-import-4b988e935a"
             ],
             "fn_ref": {
                 "encoded_function": [
-                    "gASVtAMAAAAAAACMF2Nsb3VkcGlja2xlLmNsb3VkcGlja2xllIwOX21ha2VfZnVuY3Rpb26Uk5Qo\naACMDV9idWlsdGluX3R5cGWUk5SMCENvZGVUeXBllIWUUpQoSwFLAEsASwFLAktDQwh8AKAAoQBT\nAJROhZSMBGl0ZW2UhZSMAmRmlIWUjARhLnB5lIwFbXlfZm6USwRDAgAFlCkpdJRSlH2UKIwLX19w\nYWNrYWdlX1+UTowIX19uYW1lX1+UjAhfX21haW5fX5SMCF9fZmlsZV9flGgOdU5OTnSUUpSMHGNs\nb3VkcGlja2xlLmNsb3VkcGlja2xlX2Zhc3SUjBJfZnVuY3Rpb25fc2V0c3RhdGWUk5RoGX2UKIwX\nX1Rhc2tEZWZfX3Nka190YXNrX2JvZHmUaBmMBmZuX3JlZpSMGG9ycXVlc3RyYS5zZGsuX2Jhc2Uu\nX2RzbJSMEUlubGluZUZ1bmN0aW9uUmVmlJOUaA9oGYaUgZSMDXNvdXJjZV9pbXBvcnSUaCCMDElu\nbGluZUltcG9ydJSTlCmBlIwPb3V0cHV0X21ldGFkYXRhlGggjBJUYXNrT3V0cHV0TWV0YWRhdGGU\nk5SJSwGGlIGUjApwYXJhbWV0ZXJzlIwLY29sbGVjdGlvbnOUjAtPcmRlcmVkRGljdJSTlClSlGgM\naCCMDVRhc2tQYXJhbWV0ZXKUk5RoDGggjA1QYXJhbWV0ZXJLaW5klJOUjBVQT1NJVElPTkFMX09S\nX0tFWVdPUkSUhZRSlIaUgZRzjBJkZXBlbmRlbmN5X2ltcG9ydHOUaCCMDVB5dGhvbkltcG9ydHOU\nk5QpgZR9lCiMDXVzZV9maWxlX3BhdGiUiYwIcGFja2FnZXOUjAZwb2xhcnOUhZR1YoWUjAlyZXNv\ndXJjZXOUaCCMCVJlc291cmNlc5STlChOTk5OdJSBlIwMY3VzdG9tX2ltYWdllIwoemFwYXRhY29t\ncHV0aW5nL29ycXVlc3RyYS1kZWZhdWx0OnYwLjAuMJSMC2N1c3RvbV9uYW1llE51fZQoaBVoD4wM\nX19xdWFsbmFtZV9flGgPjA9fX2Fubm90YXRpb25zX1+UfZSMDl9fa3dkZWZhdWx0c19flE6MDF9f\nZGVmYXVsdHNfX5ROjApfX21vZHVsZV9flGgWjAdfX2RvY19flE6MC19fY2xvc3VyZV9flE6MF19j\nbG91ZHBpY2tsZV9zdWJtb2R1bGVzlF2UjAtfX2dsb2JhbHNfX5R9lHWGlIZSMC4=\n"
+                    "gASVQgQAAAAAAACMF2Nsb3VkcGlja2xlLmNsb3VkcGlja2xllIwOX21ha2VfZnVuY3Rpb26Uk5Qo\naACMDV9idWlsdGluX3R5cGWUk5SMCENvZGVUeXBllIWUUpQoSwFLAEsASwFLAktDQwh8AKAAoQBT\nAJROhZSMBGl0ZW2UhZSMAmRmlIWUjDp0ZXN0cy9ydW50aW1lL3JheS9kYXRhL3B5dGhvbl9wYWNr\nYWdlL29yaWdpbmFsX3dvcmtmbG93LnB5lIwFbXlfZm6USwZDAgAFlCkpdJRSlH2UKIwLX19wYWNr\nYWdlX1+UTowIX19uYW1lX1+UjAhfX21haW5fX5SMCF9fZmlsZV9flGgOdU5OTnSUUpSMHGNsb3Vk\ncGlja2xlLmNsb3VkcGlja2xlX2Zhc3SUjBJfZnVuY3Rpb25fc2V0c3RhdGWUk5RoGX2UKIwXX1Rh\nc2tEZWZfX3Nka190YXNrX2JvZHmUaBmMB19mbl9yZWaUjBhvcnF1ZXN0cmEuc2RrLl9iYXNlLl9k\nc2yUjBFJbmxpbmVGdW5jdGlvblJlZpSTlGgPaBmGlIGUjAhfZm5fbmFtZZRoD4wQX291dHB1dF9t\nZXRhZGF0YZRoIIwSVGFza091dHB1dE1ldGFkYXRhlJOUiUsBhpSBlIwLX3BhcmFtZXRlcnOUjAtj\nb2xsZWN0aW9uc5SMC09yZGVyZWREaWN0lJOUKVKUaAxoIIwNVGFza1BhcmFtZXRlcpSTlGgMaCCM\nDVBhcmFtZXRlcktpbmSUk5SMFVBPU0lUSU9OQUxfT1JfS0VZV09SRJSFlFKUhpSBlHOMCl9yZXNv\ndXJjZXOUaCCMCVJlc291cmNlc5STlChOTk5OTnSUgZSMDV9jdXN0b21faW1hZ2WUjCh6YXBhdGFj\nb21wdXRpbmcvb3JxdWVzdHJhLWRlZmF1bHQ6djAuMC4wlIwMX2N1c3RvbV9uYW1llE6ME19kZXBl\nbmRlbmN5X2ltcG9ydHOUaCCMDVB5dGhvbkltcG9ydHOUk5QpgZR9lCiMBV9maWxllE6MCV9wYWNr\nYWdlc5SMDnBvbGFycz09MC4xNy4zlIWUdWKFlIwfX3VzZV9kZWZhdWx0X2RlcGVuZGVuY3lfaW1w\nb3J0c5SJjA5fc291cmNlX2ltcG9ydJRoIIwMSW5saW5lSW1wb3J0lJOUKYGUjBpfdXNlX2RlZmF1\nbHRfc291cmNlX2ltcG9ydJSJdX2UKGgVaA+MDF9fcXVhbG5hbWVfX5RoD4wPX19hbm5vdGF0aW9u\nc19flH2UjA5fX2t3ZGVmYXVsdHNfX5ROjAxfX2RlZmF1bHRzX1+UTowKX19tb2R1bGVfX5RoFowH\nX19kb2NfX5ROjAtfX2Nsb3N1cmVfX5ROjBdfY2xvdWRwaWNrbGVfc3VibW9kdWxlc5RdlIwLX19n\nbG9iYWxzX1+UfZR1hpSGUjAu\n"
                 ],
                 "function_name": "my_fn",
                 "type": "INLINE_FUNCTION_REF"
             },
-            "id": "task-my-fn-d3914c5e63",
+            "id": "task-my-fn-55d017d1e7",
+            "output_metadata": {
+                "is_subscriptable": false,
+                "n_outputs": 1
+            },
             "parameters": [
                 {
                     "kind": "POSITIONAL_OR_KEYWORD",
                     "name": "df"
                 }
             ],
             "resources": null,
```

### Comparing `orquestra-sdk-0.46.0/tests/runtime/ray/ray_logs/data/ray_temp/session_2023-02-09_12-23-55_156174_25782/logs/worker1.err` & `orquestra-sdk-0.47.0/tests/runtime/ray/ray_logs/data/ray_temp/session_2023-02-09_12-23-55_156174_25782/logs/worker1.err`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/ray/ray_logs/data/ray_temp/session_2023-02-09_12-23-55_156174_25782/logs/worker3.err` & `orquestra-sdk-0.47.0/tests/runtime/ray/ray_logs/data/ray_temp/session_2023-02-09_12-23-55_156174_25782/logs/worker3.err`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/ray/ray_logs/test_ray_logs.py` & `orquestra-sdk-0.47.0/tests/runtime/ray/ray_logs/test_ray_logs.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/ray/test_client.py` & `orquestra-sdk-0.47.0/tests/runtime/ray/test_client.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/ray/test_integration.py` & `orquestra-sdk-0.47.0/tests/runtime/ray/test_integration.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from orquestra import sdk
 from orquestra.sdk import exceptions
 from orquestra.sdk._base._testing import _example_wfs
 from orquestra.sdk._base.abc import RuntimeInterface
 from orquestra.sdk._ray import _client, _dag, _ray_logs
 from orquestra.sdk.schema import configs, ir
+from orquestra.sdk.schema.responses import JSONResult
 from orquestra.sdk.schema.workflow_run import State, WorkflowRunId
 
 
 @pytest.fixture(scope="module")
 def runtime(
     shared_ray_conn, tmp_path_factory: pytest.TempPathFactory, change_db_location
 ):
@@ -75,46 +76,46 @@
         """
 
         # Ray mishandles log file handlers and we get "_io.FileIO [closed]"
         # unraisable exceptions. Last tested with Ray 2.2.0.
         @pytest.mark.filterwarnings("ignore::pytest.PytestUnraisableExceptionWarning")
         def test_running_same_workflow_def_twice(self, runtime: _dag.RayRuntime):
             wf_def = _example_wfs.multioutput_wf.model
-            run_id1 = runtime.create_workflow_run(wf_def)
-            run_id2 = runtime.create_workflow_run(wf_def)
+            run_id1 = runtime.create_workflow_run(wf_def, None)
+            run_id2 = runtime.create_workflow_run(wf_def, None)
 
             assert run_id1 != run_id2
 
             _wait_to_finish_wf(run_id1, runtime)
             _wait_to_finish_wf(run_id2, runtime)
             output1 = runtime.get_workflow_run_outputs_non_blocking(run_id1)
             output2 = runtime.get_workflow_run_outputs_non_blocking(run_id2)
 
             assert output1 == output2
 
         def test_sets_context(self, runtime: _dag.RayRuntime):
             wf_def = _example_wfs.wf_with_exec_ctx().model
 
             # when
-            run_id = runtime.create_workflow_run(wf_def)
+            run_id = runtime.create_workflow_run(wf_def, None)
 
             # then
             _wait_to_finish_wf(run_id, runtime)
             outputs = runtime.get_workflow_run_outputs_non_blocking(run_id)
-            assert outputs == ("RAY",)
+            assert outputs == (JSONResult(value='"RAY"'),)
 
         def test_sets_run_id_from_env(
             self, monkeypatch: pytest.MonkeyPatch, runtime: _dag.RayRuntime
         ):
             wf_def = _example_wfs.multioutput_wf.model
             # Appending the normal run ID to prevent collisions
             global_wf_run_id = "run_id_from_env" + _dag._generate_wf_run_id(wf_def)
             monkeypatch.setenv("GLOBAL_WF_RUN_ID", global_wf_run_id)
 
-            run_id = runtime.create_workflow_run(wf_def)
+            run_id = runtime.create_workflow_run(wf_def, None)
 
             runtime.stop_workflow_run(run_id)
             assert run_id == global_wf_run_id
 
     class TestGetWorkflowRunStatus:
         """
         Tests that validate .get_workflow_run_status().
@@ -125,15 +126,15 @@
             """
             Verifies that we report status correctly before workflow ends.
             It's difficult to synchronize, so there's a bunch of ifs in this
             test.
             """
             # Given
             wf_def = _example_wfs.greet_wf.model
-            run_id = runtime.create_workflow_run(wf_def)
+            run_id = runtime.create_workflow_run(wf_def, None)
 
             # When
             run = runtime.get_workflow_run_status(run_id)
 
             # Then
             assert run.id == run_id
             assert run.status.state in {State.WAITING, State.RUNNING, State.SUCCEEDED}
@@ -174,15 +175,15 @@
 
             Note: Ray sometimes suffers from race conditions between blocking
             on the output, and returning workflow status "completed". This is
             why this test is repeated a couple of times.
             """
             # Given
             wf_def = _example_wfs.greet_wf.model
-            run_id = runtime.create_workflow_run(wf_def)
+            run_id = runtime.create_workflow_run(wf_def, None)
 
             # Block until wf completes
             _wait_to_finish_wf(run_id, runtime)
 
             # When
             run = runtime.get_workflow_run_status(run_id)
 
@@ -223,15 +224,15 @@
                 ▼
                [3] => won't run
                 │
                 ▼
             [return]
             """
             wf_def = _example_wfs.exception_wf_with_multiple_values.model
-            run_id = runtime.create_workflow_run(wf_def)
+            run_id = runtime.create_workflow_run(wf_def, None)
 
             _wait_to_finish_wf(run_id, runtime)
 
             wf_run = runtime.get_workflow_run_status(run_id)
 
             assert wf_run.status.state == State.FAILED
             assert _count_task_runs(wf_run, State.FAILED) == 1
@@ -242,16 +243,16 @@
         """
         Tests that validate .list_workflow_runs().
         """
 
         def test_two_runs(self, runtime: _dag.RayRuntime):
             # Given
             wf_def = _example_wfs.greet_wf.model
-            run_id1 = runtime.create_workflow_run(wf_def)
-            run_id2 = runtime.create_workflow_run(wf_def)
+            run_id1 = runtime.create_workflow_run(wf_def, None)
+            run_id2 = runtime.create_workflow_run(wf_def, None)
 
             # When
             wf_runs = runtime.list_workflow_runs()
 
             # Then
             wf_run_ids = {run.id for run in wf_runs}
             assert run_id1 in wf_run_ids
@@ -276,27 +277,27 @@
                ▼
             """
             triggers = [tmp_path / f"trigger{i}.txt" for i in range(2)]
 
             wf = _example_wfs.serial_wf_with_file_triggers(
                 triggers, task_timeout=2.0
             ).model
-            wf_run_id = runtime.create_workflow_run(wf)
+            wf_run_id = runtime.create_workflow_run(wf, None)
             wf_run = runtime.get_workflow_run_status(wf_run_id)
             assert wf_run.status.state == State.RUNNING
 
             runtime.stop_workflow_run(wf_run_id)
 
             wf_run = runtime.get_workflow_run_status(wf_run_id)
             assert wf_run.status.state == State.TERMINATED
 
         def test_on_finished_workflow(self, runtime: _dag.RayRuntime, tmp_path):
 
             wf = _example_wfs.multioutput_task_wf.model
-            wf_run_id = runtime.create_workflow_run(wf)
+            wf_run_id = runtime.create_workflow_run(wf, None)
             _wait_to_finish_wf(wf_run_id, runtime)
             # ensure wf has finished
             status = runtime.get_workflow_run_status(wf_run_id)
             assert status.status.state == State.SUCCEEDED
 
             runtime.stop_workflow_run(wf_run_id)
             status = runtime.get_workflow_run_status(wf_run_id)
@@ -306,25 +307,27 @@
     class TestGetWorkflowRunOutputsNonBlocking:
         """
         Tests that validate get_workflow_run_outputs_non_blocking
         """
 
         def test_happy_path(self, runtime: _dag.RayRuntime):
             wf_def = _example_wfs.greet_wf.model
-            run_id = runtime.create_workflow_run(wf_def)
+            run_id = runtime.create_workflow_run(wf_def, None)
 
             _wait_to_finish_wf(run_id, runtime)
 
             outputs = runtime.get_workflow_run_outputs_non_blocking(run_id)
 
-            assert outputs == ("yooooo emiliano from zapata computing",)
+            assert outputs == (
+                JSONResult(value='"yooooo emiliano from zapata computing"'),
+            )
 
         def test_failed_workflow(self, runtime: _dag.RayRuntime):
             wf_def = _example_wfs.exception_wf_with_multiple_values().model
-            run_id = runtime.create_workflow_run(wf_def)
+            run_id = runtime.create_workflow_run(wf_def, None)
 
             _wait_to_finish_wf(run_id, runtime)
 
             with pytest.raises(exceptions.WorkflowRunNotSucceeded):
                 runtime.get_workflow_run_outputs_non_blocking(run_id)
 
         def test_in_progress_workflow(self, runtime: _dag.RayRuntime, tmp_path):
@@ -340,15 +343,15 @@
                ▼
             """
             triggers = [tmp_path / f"trigger{i}.txt" for i in range(2)]
 
             wf = _example_wfs.serial_wf_with_file_triggers(
                 triggers, task_timeout=2.0
             ).model
-            run_id = runtime.create_workflow_run(wf)
+            run_id = runtime.create_workflow_run(wf, None)
 
             assert runtime.get_workflow_run_status(run_id).status.state == State.RUNNING
             with pytest.raises(exceptions.WorkflowRunNotSucceeded):
                 runtime.get_workflow_run_outputs_non_blocking(run_id)
 
             # let the workers complete the workflow
             triggers[0].write_text("triggered")
@@ -371,33 +374,33 @@
                 ▼
                [3] => won't run
                 │
                 ▼
             [return]
             """
             wf_def = _example_wfs.exception_wf_with_multiple_values().model
-            run_id = runtime.create_workflow_run(wf_def)
+            run_id = runtime.create_workflow_run(wf_def, None)
 
             _wait_to_finish_wf(run_id, runtime)
 
             wf_run = runtime.get_workflow_run_status(run_id)
-            outputs = runtime.get_available_outputs(run_id)
+            inv_artifacts = runtime.get_available_outputs(run_id)
             if wf_run.status.state != State.FAILED:
                 pytest.fail(
                     "The workflow was supposed to fail, but it didn't. "
                     f"Wf run: {wf_run}"
                 )
 
-            # Expect only one finished task.
-            assert len(outputs) == 1
+            # Expect only one finished task invocation.
+            assert len(inv_artifacts) == 1
 
-            # The outputs dict has an entry for each task invocation. Each entry's value
-            # should be a tuple.
-            inv_output = list(outputs.values())[0]
-            assert inv_output == (58,)
+            # The outputs dict has an entry for each task invocation. The value is
+            # whatever the task returned; in this example it's a single int.
+            task_output = list(inv_artifacts.values())[0]
+            assert task_output == JSONResult(value="58")
 
         def test_after_one_task_finishes(self, runtime: _dag.RayRuntime, tmp_path):
             """
             Workflow graph in the scenario under test:
               [ ]  => finished
                │
                │
@@ -416,15 +419,15 @@
 
             # Let the first task finish quickly
             triggers[0].write_text("triggered")
 
             wf = _example_wfs.serial_wf_with_file_triggers(
                 triggers, task_timeout=2.0
             ).model
-            wf_run_id = runtime.create_workflow_run(wf)
+            wf_run_id = runtime.create_workflow_run(wf, None)
 
             # Await completion of the first task
             loop_start = time.time()
             while True:
                 wf_run = runtime.get_workflow_run_status(wf_run_id)
                 if wf_run.status.state not in {State.RUNNING, State.SUCCEEDED}:
                     pytest.fail(f"Unexpected wf run state: {wf_run}")
@@ -441,100 +444,138 @@
                     pytest.fail(
                         f"Timeout when awaiting for workflow finish. Full run: {wf_run}"
                     )
 
                 time.sleep(0.2)
 
             # When
-            outputs = runtime.get_available_outputs(wf_run_id)
+            outputs_dict = runtime.get_available_outputs(wf_run_id)
 
             # Then
-            assert len(outputs) == len(succeeded_runs)
+            assert len(outputs_dict) == len(succeeded_runs)
 
             # let the workers complete the workflow
             triggers[1].write_text("triggered")
             triggers[2].write_text("triggered")
 
 
 @pytest.mark.slow
+# Ray mishandles log file handlers and we get "_io.FileIO [closed]"
+# unraisable exceptions. Last tested with Ray 2.3.0.
+@pytest.mark.filterwarnings("ignore::pytest.PytestUnraisableExceptionWarning")
 @pytest.mark.parametrize(
     "wf,expected_outputs,expected_intermediate",
     [
         (
             _example_wfs.greet_wf,
-            ("yooooo emiliano from zapata computing",),
+            (JSONResult(value='"yooooo emiliano from zapata computing"'),),
             {
                 "invocation-0-task-make-greeting": (
-                    "yooooo emiliano from zapata computing",
+                    JSONResult(value='"yooooo emiliano from zapata computing"')
                 )
             },
         ),
         (
             _example_wfs.complicated_wf,
-            ("yooooo emiliano Zapata from Zapata computing",),
+            (JSONResult(value='"yooooo emiliano Zapata from Zapata computing"'),),
             {
                 "invocation-0-task-make-greeting": (
-                    ("yooooo emiliano Zapata from Zapata computing",)
+                    JSONResult(value='"yooooo emiliano Zapata from Zapata computing"')
                 ),
-                "invocation-1-task-capitalize": ("Zapata computing",),
-                "invocation-2-task-concat": ("emiliano Zapata",),
-                "invocation-3-task-capitalize": ("Zapata",),
+                "invocation-1-task-capitalize": JSONResult(value='"Zapata computing"'),
+                "invocation-2-task-concat": JSONResult(value='"emiliano Zapata"'),
+                "invocation-3-task-capitalize": JSONResult(value='"Zapata"'),
             },
         ),
         (
             _example_wfs.multioutput_wf,
-            ("Emiliano Zapata", "Zapata computing"),
+            (
+                JSONResult(value='"Emiliano Zapata"'),
+                JSONResult(value='"Zapata computing"'),
+            ),
             {
-                "invocation-0-task-capitalize": ("Zapata computing",),
-                "invocation-1-task-make-company-name": ("zapata computing",),
-                "invocation-2-task-concat": ("Emiliano Zapata",),
-                "invocation-3-task-capitalize": ("Zapata",),
+                "invocation-0-task-capitalize": JSONResult(value='"Zapata computing"'),
+                "invocation-1-task-make-company-name": JSONResult(
+                    value='"zapata computing"'
+                ),
+                "invocation-2-task-concat": JSONResult(value='"Emiliano Zapata"'),
+                "invocation-3-task-capitalize": JSONResult(value='"Zapata"'),
             },
         ),
         (
             _example_wfs.multioutput_task_wf,
-            ("Zapata", "Computing", "Computing", ("Zapata", "Computing")),
+            (
+                # Unpacked outputs
+                JSONResult(value='"Zapata"'),
+                JSONResult(value='"Computing"'),
+                # First output discarded
+                JSONResult(value='"Computing"'),
+                # Second output discarded
+                JSONResult(value='"Zapata"'),
+                # Returning both packed and unpacked outputs
+                JSONResult(
+                    value='{"__tuple__": true, "__values__": ["Zapata", "Computing"]}'
+                ),
+                JSONResult(value='"Zapata"'),
+                JSONResult(value='"Computing"'),
+            ),
             {
-                # The outputs for invocation 1 and 2 should be just a single tuple, not
-                # tuple-in-tuple. TODO: change it when working on
-                # https://zapatacomputing.atlassian.net/browse/ORQSDK-695.
-                "invocation-0-task-multioutput-task": (("Zapata", "Computing"),),
-                "invocation-1-task-multioutput-task": (("Zapata", "Computing"),),
-                "invocation-2-task-multioutput-task": ("Zapata", "Computing"),
+                # We expect all task outputs for each task invocation, regardless of
+                # unpacking in the workflow. For more info, see
+                # `RuntimeInterface.get_available_outputs()`.
+                "invocation-0-task-multioutput-task": JSONResult(
+                    value='{"__tuple__": true, "__values__": ["Zapata", "Computing"]}'
+                ),
+                "invocation-1-task-multioutput-task": JSONResult(
+                    value='{"__tuple__": true, "__values__": ["Zapata", "Computing"]}'
+                ),
+                "invocation-2-task-multioutput-task": JSONResult(
+                    value='{"__tuple__": true, "__values__": ["Zapata", "Computing"]}'
+                ),
+                "invocation-3-task-multioutput-task": JSONResult(
+                    value='{"__tuple__": true, "__values__": ["Zapata", "Computing"]}'
+                ),
             },
         ),
         (
             _example_wfs.greet_wf_kw,
-            ("yooooo emiliano from zapata computing",),
+            (JSONResult(value='"yooooo emiliano from zapata computing"'),),
             {
                 "invocation-0-task-make-greeting": (
-                    "yooooo emiliano from zapata computing",
+                    JSONResult(value='"yooooo emiliano from zapata computing"')
                 )
             },
         ),
         (
             _example_wfs.wf_using_inline_imports,
-            ("Emiliano Zapata", "Zapata computing"),
+            (
+                JSONResult(value='"Emiliano Zapata"'),
+                JSONResult(value='"Zapata computing"'),
+            ),
             {
-                "invocation-0-task-capitalize-inline": ("Zapata computing",),
-                "invocation-1-task-make-company-name": ("zapata computing",),
-                "invocation-2-task-concat": ("Emiliano Zapata",),
-                "invocation-3-task-capitalize-inline": ("Zapata",),
+                "invocation-0-task-capitalize-inline": JSONResult(
+                    value='"Zapata computing"'
+                ),
+                "invocation-1-task-make-company-name": JSONResult(
+                    value='"zapata computing"'
+                ),
+                "invocation-2-task-concat": JSONResult(value='"Emiliano Zapata"'),
+                "invocation-3-task-capitalize-inline": JSONResult(value='"Zapata"'),
             },
         ),
     ],
 )
 def test_run_and_get_output(
     runtime: _dag.RayRuntime, wf, expected_outputs, expected_intermediate
 ):
     """
     Verifies methods for getting outputs, both the "final" and "intermediate".
     """
     # Given
-    run_id = runtime.create_workflow_run(wf.model)
+    run_id = runtime.create_workflow_run(wf.model, None)
     _wait_to_finish_wf(run_id, runtime)
 
     # When
     wf_results = runtime.get_workflow_run_outputs_non_blocking(run_id)
     intermediate_outputs = runtime.get_available_outputs(run_id)
 
     # Then
@@ -550,14 +591,18 @@
 #   scanning.
 @pytest.mark.slow
 # Ray mishandles log file handlers and we get "_io.FileIO [closed]"
 # unraisable exceptions. Last tested with Ray 2.3.0.
 @pytest.mark.filterwarnings("ignore::pytest.PytestUnraisableExceptionWarning")
 class Test3rdPartyLibraries:
     @staticmethod
+    # We're reading a serialized workflow def. The SDK version inside that JSON is
+    # likely to be different from the one we're using for development. The SDK shows a
+    # warning when deserializing a workflow def like this.
+    @pytest.mark.filterwarnings("ignore::orquestra.sdk.exceptions.VersionMismatch")
     def test_constants_and_inline_imports(runtime: _dag.RayRuntime):
         """
         This test uses already generated workflow def from json file. If necessary, it
         can be recreated using ./data/python_package/original_workflow.py
 
         This function tests 2 things
         1. Proper package installation. Python Package defined in task definition should
@@ -577,21 +622,21 @@
 
         path_to_json = Path(__file__).parent.joinpath(
             "data/python_package/python_package_dependent_workflow.json"
         )
         wf = ir.WorkflowDef.parse_file(path_to_json)
 
         # When
-        run_id = runtime.create_workflow_run(wf)
+        run_id = runtime.create_workflow_run(wf, None)
         # This test is notoriously slow to run, especially on local machines.
         _wait_to_finish_wf(run_id, runtime, timeout=10 * 60.0)
         wf_result = runtime.get_workflow_run_outputs_non_blocking(run_id)
 
         # Then
-        assert wf_result == (21,)
+        assert wf_result == (JSONResult(value=("21")),)
 
         # this package should be only used inside ray env
         with pytest.raises(ModuleNotFoundError):
             import polars  # type: ignore # noqa
 
     @staticmethod
     def test_git_import_inside_ray(monkeypatch, runtime: _dag.RayRuntime):
@@ -599,21 +644,23 @@
         # This package should not be installed before running test
         with pytest.raises(ModuleNotFoundError):
             import piccup  # type: ignore # noqa
 
         monkeypatch.setenv(name="ORQ_RAY_DOWNLOAD_GIT_IMPORTS", value="1")
 
         # When
-        run_id = runtime.create_workflow_run(_example_wfs.wf_using_git_imports.model)
+        run_id = runtime.create_workflow_run(
+            _example_wfs.wf_using_git_imports.model, None
+        )
         # This test is notoriously slow to run, especially on local machines.
         _wait_to_finish_wf(run_id, runtime, timeout=10 * 60.0)
         wf_result = runtime.get_workflow_run_outputs_non_blocking(run_id)
 
         # Then
-        assert wf_result == (2,)
+        assert wf_result == (JSONResult(value=("2")),)
 
         # this package should be only used inside ray env
         with pytest.raises(ModuleNotFoundError):
             import piccup  # type: ignore # noqa
 
 
 @pytest.mark.slow
@@ -654,15 +701,15 @@
     The tests' boundary: `[DirectRayReader]-[task code]`
     """
 
     @staticmethod
     def run_and_await_wf(
         runtime: RuntimeInterface, wf: ir.WorkflowDef
     ) -> WorkflowRunId:
-        run_id = runtime.create_workflow_run(wf)
+        run_id = runtime.create_workflow_run(wf, None)
         _wait_to_finish_wf(run_id, runtime)
 
         return run_id
 
     def test_get_workflow_logs(self, shared_ray_conn, runtime, wf, tell_tale: str):
         """
         Submit a workflow, wait for it to finish, get wf logs, look for the test
@@ -724,15 +771,15 @@
     """
     # Given
     wf = _example_wfs.wf_with_log("Unique log line").model
     tell_tale = "Unique log line"
     ray_params = shared_ray_conn
     reader = _ray_logs.DirectRayReader(Path(ray_params._temp_dir))
 
-    run_id = runtime.create_workflow_run(wf)
+    run_id = runtime.create_workflow_run(wf, None)
     _wait_to_finish_wf(run_id, runtime)
 
     # When
     logs_dict = reader.get_workflow_logs(wf_run_id=run_id)
 
     # Then
     # First check for the tell_tale in all log lines
@@ -763,15 +810,15 @@
     wf_def = _example_wfs.greet_wf.model
     task_id = list(wf_def.tasks.keys())[0]
 
     # ignoring mypy, this is supposed to be module fn repo
     wf_def.tasks[task_id].fn_ref.module = "nope"  # type: ignore
 
     # when
-    wf_id = runtime.create_workflow_run(wf_def)
+    wf_id = runtime.create_workflow_run(wf_def, None)
     _wait_to_finish_wf(wf_id, runtime)
 
     # then
     assert runtime.get_workflow_run_status(wf_id).status.state == State.FAILED
     assert (
         runtime.get_workflow_run_status(wf_id).task_runs[0].status.state == State.FAILED
     )
@@ -811,15 +858,15 @@
         def wf():
             return dump_ids()
 
         wf_model = wf().model
 
         # When
         # The function-under-test is called inside the workflow.
-        wf_run_id = runtime.create_workflow_run(wf_model)
+        wf_run_id = runtime.create_workflow_run(wf_model, None)
         _wait_to_finish_wf(wf_run_id, runtime)
 
         # Precondition
         wf_run = runtime.get_workflow_run_status(wf_run_id)
         assert wf_run.status.state == State.SUCCEEDED
 
         # Then
```

### Comparing `orquestra-sdk-0.46.0/tests/runtime/ray/test_logger.py` & `orquestra-sdk-0.47.0/tests/runtime/ray/test_logger.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/test_config.py` & `orquestra-sdk-0.47.0/tests/runtime/test_config.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/test_log_adapter.py` & `orquestra-sdk-0.47.0/tests/runtime/test_log_adapter.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/test_services.py` & `orquestra-sdk-0.47.0/tests/runtime/test_services.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/runtime/test_services_integration.py` & `orquestra-sdk-0.47.0/tests/runtime/test_services_integration.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/api/test_config.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/api/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,14 +303,16 @@
         @staticmethod
         def test_default_file_location(tmp_default_config_json):
             config_names = api_cfg.RuntimeConfig.list_configs()
 
             assert config_names == [name for name in TEST_CONFIGS_DICT] + list(
                 _config.UNIQUE_CONFIGS
             )
+            # this config name should appear only when proper env var is set
+            assert _config.AUTO_CONFIG_NAME not in config_names
 
         @staticmethod
         def test_custom_file_location(
             tmp_config_json: Path, monkeypatch: pytest.MonkeyPatch
         ):
             monkeypatch.setenv("ORQ_CONFIG_PATH", str(tmp_config_json))
 
@@ -334,14 +336,21 @@
             with open(patch_config_location / "config.json", "w") as f:
                 json.dump({}, f)
 
             config_names = api_cfg.RuntimeConfig.list_configs()
 
             assert config_names == list(_config.UNIQUE_CONFIGS)
 
+        @staticmethod
+        def test_auto_config_name(monkeypatch, tmp_config_json):
+            monkeypatch.setenv("ORQUESTRA_PASSPORT_FILE", "some_file_path")
+            config_names = api_cfg.RuntimeConfig.list_configs()
+
+            assert _config.AUTO_CONFIG_NAME in config_names
+
     class TestLoad:
         @pytest.mark.parametrize("config_name", [name for name in TEST_CONFIGS_DICT])
         class TestLoadSuccess:
             @staticmethod
             def test_with_default_file_path(tmp_default_config_json, config_name):
                 config = api_cfg.RuntimeConfig.load(config_name)
 
@@ -372,14 +381,39 @@
         def test_invalid_name(tmp_config_json: Path, monkeypatch: pytest.MonkeyPatch):
             monkeypatch.setenv("ORQ_CONFIG_PATH", str(tmp_config_json))
             with pytest.raises(ConfigNameNotFoundError):
                 api_cfg.RuntimeConfig.load(
                     "non-existing",
                 )
 
+        class TestAutoConfig:
+            def test_on_cluster(self, monkeypatch, tmp_path):
+                token = "the best token you have ever seen"
+                pass_file = tmp_path / "pass.port"
+                pass_file.write_text(token)
+                monkeypatch.setenv("ORQUESTRA_PASSPORT_FILE", str(pass_file))
+
+                cfg = api_cfg.RuntimeConfig.load(
+                    "auto",
+                )
+
+                assert cfg.token == token
+
+            def test_on_local_env(self):
+                assert api_cfg.RuntimeConfig.load("auto") == api_cfg.RuntimeConfig.load(
+                    "local"
+                )
+
+            def test_no_file(self, monkeypatch):
+                monkeypatch.setenv("ORQUESTRA_PASSPORT_FILE", "non-existing-path")
+                with pytest.raises(FileNotFoundError):
+                    api_cfg.RuntimeConfig.load(
+                        "auto",
+                    )
+
     class TestLoadDefault:
         @staticmethod
         def test_with_default_file_path(tmp_default_config_json):
             config = api_cfg.RuntimeConfig.load_default()
 
             default_config_params = TEST_CONFIGS_DICT[
                 TEST_CONFIG_JSON["default_config_name"]
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/api/test_task_run.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/api/test_task_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 import typing as t
 from unittest.mock import MagicMock, Mock, create_autospec
 
 import pytest
 
-from orquestra.sdk._base import _api, _workflow
+from orquestra.sdk._base import _api, _workflow, serde
 from orquestra.sdk._base.abc import RuntimeInterface
 from orquestra.sdk.exceptions import TaskRunNotFound
 from orquestra.sdk.schema import ir
 from orquestra.sdk.schema.workflow_run import RunStatus, State
 from orquestra.sdk.schema.workflow_run import TaskRun as TaskRunModel
 from orquestra.sdk.schema.workflow_run import WorkflowRun as WorkflowRunModel
 
@@ -214,16 +214,16 @@
                 pytest.param("inv2", (21, 38), id="multi_param_invocation"),
             ],
         )
         def test_get_output_finished(wf_def_model, inv_id: str, exp_output):
             # Given
             runtime = create_autospec(RuntimeInterface)
             runtime.get_available_outputs.return_value = {
-                "inv1": (42,),
-                "inv2": (21, 38),
+                "inv1": serde.result_from_artifact(42, ir.ArtifactFormat.AUTO),
+                "inv2": serde.result_from_artifact((21, 38), ir.ArtifactFormat.AUTO),
             }
 
             task_run = _api.TaskRun(
                 task_run_id="a_run",
                 task_invocation_id=inv_id,
                 workflow_run_id="wf.1",
                 runtime=runtime,
@@ -375,14 +375,23 @@
     class TestGetInput:
         @staticmethod
         @pytest.mark.parametrize(
             "workflow, expected_args, expected_kwargs",
             [
                 ("simple_wf_one_task_inline", [], {}),
                 ("wf_single_task_with_const_parent", [21], {}),
+                (
+                    "wf_single_task_with_secret_parent",
+                    [
+                        ir.SecretNode(
+                            id="secret-0", secret_name="test", secret_config=None
+                        )
+                    ],
+                    {},
+                ),
                 ("wf_single_task_with_const_parent_kwargs", [], {"kwargs": 36}),
                 ("wf_single_task_with_const_parent_args_kwargs", [21], {"kwargs": 36}),
             ],
         )
         def test_const_as_parent(workflow, expected_args, expected_kwargs):
             # given
             from ..data import task_run_workflow_defs
@@ -442,15 +451,18 @@
             wf_def = wf_for_input_test().model
             # find the task with 1 arg and 0 kwarg args. It is the one at the top
             first_inv_id = self._find_task_by_args_and_kwargs_number(1, 0, wf_def)
             # find the task with 1 arg and 1 kwarg. 2nd task that finished
             second_inv_2 = self._find_task_by_args_and_kwargs_number(1, 1, wf_def)
 
             runtime = MagicMock(RuntimeInterface)
-            runtime_outputs = {first_inv_id: (15,), second_inv_2: (25,)}
+            runtime_outputs = {
+                first_inv_id: serde.result_from_artifact(15, ir.ArtifactFormat.AUTO),
+                second_inv_2: serde.result_from_artifact(25, ir.ArtifactFormat.AUTO),
+            }
             runtime.get_available_outputs.return_value = runtime_outputs
             wf_run_id = "wf.3"
 
             task_runs = [
                 _api.TaskRun(
                     task_run_id=f"run_{inv_id}",
                     task_invocation_id=inv_id,
@@ -484,15 +496,20 @@
 
             # find the task with 0 arg and 0 kwarg args
             first_inv_id = self._find_task_by_args_and_kwargs_number(0, 0, wf_def)
             # find the task with 1 arg and 1 kwarg args. 2nd task with that finished
             second_inv_id = self._find_task_by_args_and_kwargs_number(1, 0, wf_def)
 
             runtime = MagicMock(RuntimeInterface)
-            runtime_outputs = {first_inv_id: (21, 36), second_inv_id: (25,)}
+            runtime_outputs = {
+                first_inv_id: serde.result_from_artifact(
+                    (21, 36), ir.ArtifactFormat.AUTO
+                ),
+                second_inv_id: serde.result_from_artifact(25, ir.ArtifactFormat.AUTO),
+            }
             runtime.get_available_outputs.return_value = runtime_outputs
 
             task_run = _api.TaskRun(
                 task_run_id=f"run_{second_inv_id}",
                 task_invocation_id=second_inv_id,
                 workflow_run_id=wf_run_id,
                 runtime=runtime,
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/api/test_wf_run.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/api/test_wf_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,32 +5,34 @@
 Tests for orquestra.sdk._base._api._wf_run.
 """
 
 import itertools
 import json
 import time
 import typing as t
+from contextlib import suppress as do_not_raise
 from datetime import timedelta
 from unittest.mock import DEFAULT, MagicMock, Mock, PropertyMock, create_autospec
 
 import pytest
 
-from orquestra.sdk._base import _api, _workflow
+from orquestra.sdk._base import _api, _workflow, serde
 from orquestra.sdk._base.abc import RuntimeInterface
 from orquestra.sdk.exceptions import (
+    ProjectInvalidError,
     UnauthorizedError,
     WorkflowRunCanNotBeTerminated,
     WorkflowRunNotFinished,
     WorkflowRunNotFoundError,
     WorkflowRunNotStarted,
 )
 from orquestra.sdk.schema import ir
 from orquestra.sdk.schema.configs import RuntimeName
 from orquestra.sdk.schema.local_database import StoredWorkflowRun
-from orquestra.sdk.schema.workflow_run import RunStatus, State
+from orquestra.sdk.schema.workflow_run import ProjectRef, RunStatus, State
 from orquestra.sdk.schema.workflow_run import TaskRun as TaskRunModel
 
 from ..data.complex_serialization.workflow_defs import (
     capitalize,
     join_strings,
     wf_pass_tuple,
 )
@@ -64,29 +66,29 @@
 
     class TestTwoStepForm:
         @staticmethod
         def test_pass_builtin_config_name_no_file():
             run = wf_pass_tuple().run("in_process")
             results = run.get_results()
 
-            assert results == 3
+            assert results == (3,)
 
         @staticmethod
         def test_pass_builtin_config_name_with_file(tmp_default_config_json):
             run = wf_pass_tuple().run("in_process")
             results = run.get_results()
 
-            assert results == 3
+            assert results == (3,)
 
         def test_single_run(self):
             run = wf_pass_tuple().prepare("in_process")
             run.start()
             results = run.get_results()
 
-            assert results == 3
+            assert results == (3,)
 
         def test_multiple_starts(self):
             run = wf_pass_tuple().prepare("in_process")
 
             run.start()
             results1 = run.get_results()
 
@@ -96,24 +98,24 @@
             assert results1 == results2
 
     class TestShorthand:
         def test_single_run(self):
             run = wf_pass_tuple().run("in_process")
             results = run.get_results()
 
-            assert results == 3
+            assert results == (3,)
 
     class TestWithConfig:
         @staticmethod
         def test_pass_config():
             config = _api.RuntimeConfig.in_process()
             run = wf_pass_tuple().run(config)
             results = run.get_results()
 
-            assert results == 3
+            assert results == (3,)
 
 
 class TestWorkflowRun:
     @staticmethod
     @pytest.fixture
     def sample_wf_def() -> _workflow.WorkflowDef:
         @_workflow.workflow
@@ -128,15 +130,17 @@
     @staticmethod
     @pytest.fixture
     def mock_runtime(sample_wf_def):
         runtime = create_autospec(RuntimeInterface, name="runtime")
         # For getting workflow ID
         runtime.create_workflow_run.return_value = "wf_pass_tuple-1"
         # For getting workflow outputs
-        runtime.get_workflow_run_outputs_non_blocking.return_value = "woohoo!"
+        runtime.get_workflow_run_outputs_non_blocking.return_value = (
+            serde.result_from_artifact("woohoo!", ir.ArtifactFormat.AUTO),
+        )
         # for simulating a workflow running
         succeeded_run_model = Mock(name="succeeded wf run model")
 
         # Default value is "SUCCEEDED"
         succeeded_run_model.status.state = State.SUCCEEDED
         runtime.get_workflow_run_status.return_value = succeeded_run_model
         # Use side effects to simulate a running workflow
@@ -149,17 +153,17 @@
                 running_wf_run_model,
             ),
             itertools.repeat(DEFAULT),
         )
 
         # got getting task run artifacts
         runtime.get_available_outputs.return_value = {
-            "task_run1": "woohoo!",
-            "task_run2": "another",
-            "task_run3": 123,
+            "task_run1": serde.result_from_artifact("woohoo!", ir.ArtifactFormat.AUTO),
+            "task_run2": serde.result_from_artifact("another", ir.ArtifactFormat.AUTO),
+            "task_run3": serde.result_from_artifact(123, ir.ArtifactFormat.AUTO),
         }
 
         wf_def_model = sample_wf_def.model
         task_invs = list(wf_def_model.task_invocations.values())
         # Get logs, the runtime interface returns invocation IDs
         runtime.get_workflow_logs.return_value = {
             task_invs[0].id: ["woohoo!\n"],
@@ -474,27 +478,27 @@
             # Given
             run.start()
             # When
             results = run.get_results(wait=True)
             # Then
             assert mock_runtime.get_workflow_run_status.call_count >= 1
             assert results is not None
-            assert results == "woohoo!"
+            assert results == ("woohoo!",)
 
         @staticmethod
         def test_waits_when_wait_is_explicitly_false(run, mock_runtime):
             # Remove RUNNING in mock
             mock_runtime.get_workflow_run_status.side_effect = None
             # Given
             run.start()
             # When
             results = run.get_results(wait=False)
             # Then
             assert results is not None
-            assert results == "woohoo!"
+            assert results == ("woohoo!",)
             assert mock_runtime.get_workflow_run_status.call_count == 1
 
     class TestGetArtifacts:
         @staticmethod
         def test_raises_exception_if_workflow_not_started(run):
             # When
             with pytest.raises(WorkflowRunNotStarted) as exc_info:
@@ -517,18 +521,18 @@
                 [sdk.WorkflowRun]->[RuntimeInterface]
                                  ->[ir.WorkflowDef]
             """
             # Given
             runtime = create_autospec(RuntimeInterface)
 
             # The RuntimeInterface's contract for get_available_outputs is
-            # to always return tuple as the dict value.
+            # to return whatever the task function returned.
             runtime.get_available_outputs.return_value = {
-                "inv1": (42,),
-                "inv2": (21, 38),
+                "inv1": serde.result_from_artifact(42, ir.ArtifactFormat.AUTO),
+                "inv2": serde.result_from_artifact((21, 38), ir.ArtifactFormat.AUTO),
             }
 
             mock_inv1 = create_autospec(ir.TaskInvocation)
             mock_inv1.output_ids = ["art1"]
 
             mock_inv2 = create_autospec(ir.TaskInvocation)
             mock_inv2.output_ids = ["art2", "art3"]
@@ -753,7 +757,33 @@
         # Given
         # When
         _ = _api.list_workflow_runs("mocked_config", state=State.SUCCEEDED)
         # Then
         mock_config_runtime.list_workflow_runs.assert_called_with(
             limit=None, max_age=None, state=State.SUCCEEDED
         )
+
+
+@pytest.mark.parametrize(
+    "workspace_id, project_id, raises, expected",
+    [
+        ("a", "b", do_not_raise(), ProjectRef(workspace_id="a", project_id="b")),
+        ("a", None, pytest.raises(ProjectInvalidError), None),
+        (None, "b", pytest.raises(ProjectInvalidError), None),
+        (None, None, do_not_raise(), None),
+    ],
+)
+class TestProjectId:
+    def test_prepare(self, workspace_id, project_id, raises, expected):
+        with raises:
+            wf = wf_pass_tuple().prepare(
+                "in_process", workspace_id=workspace_id, project_id=project_id
+            )
+            assert wf._project == expected
+
+    def test_run(self, workspace_id, project_id, raises, expected, monkeypatch):
+        monkeypatch.setattr(_api._wf_run.WorkflowRun, "start", Mock())
+        with raises:
+            wf = wf_pass_tuple().run(
+                "in_process", workspace_id=workspace_id, project_id=project_id
+            )
+            assert wf._project == expected
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/conftest.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/conftest.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/additional-metrics.yml` & `orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/additional-metrics.yml`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 steps:
 
 - name: step-0-steps-ml-tutorial-3-exercise-steps-generate-data-step
   passed: []
   config:
     runtime:
+      customImage: zapatacomputing/orquestra-default:v0.0.0
       language: python3
       imports: [orq-wor-sdk, tut-orq-skl]
       parameters:
         file: orq-wor-sdk/src/orquestra/sdk/_base/dispatch.py
         function: exec_task_fn
   inputs:
   - __sdk_fn_ref_dict:
@@ -52,14 +53,15 @@
   - name: data
     type: workflow-result-dict
 
 - name: step-1-steps-ml-tutorial-3-exercise-steps-preprocess-data-step
   passed: [step-0-steps-ml-tutorial-3-exercise-steps-generate-data-step]
   config:
     runtime:
+      customImage: zapatacomputing/orquestra-default:v0.0.0
       language: python3
       imports: [orq-wor-sdk, tut-orq-skl]
       parameters:
         file: orq-wor-sdk/src/orquestra/sdk/_base/dispatch.py
         function: exec_task_fn
   inputs:
   - __sdk_fn_ref_dict:
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/basics.yml` & `orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/basics_with_data_aggregation.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # workflow example inspired by https://docs.orquestra.io/quantum-engine/workflow-basics/
 apiVersion: io.orquestra.workflow/1.0.0
 
-name: basics
+dataAggregation:
+  resources:
+    cpu: '1'
+    disk: '1'
+    gpu: '1'
+    memory: '1'
+  run: true
+
+name: basics-with-data-aggregation
 
 imports:
 
 - name: tut-0-wel
   type: git
   parameters:
     commit: "master"
@@ -18,23 +26,25 @@
 
 steps:
 
 - name: step-0-welcome-welcome
   passed: []
   config:
     runtime:
+      customImage: zapatacomputing/orquestra-nvidia:v0.0.0
       language: python3
       imports: [orq-wor-sdk, tut-0-wel]
       parameters:
         file: orq-wor-sdk/src/orquestra/sdk/_base/dispatch.py
         function: exec_task_fn
     resources:
       cpu: "1000m"
       memory: "1Gi"
       disk: "15Gi"
+      gpu: "1"
   inputs:
   - __sdk_fn_ref_dict:
       module: welcome
       function_name: welcome
       file_path: welcome.py
       line_number: 7
       type: MODULE_FUNCTION_REF
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/basics_file_ref.yml` & `orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/basics_file_ref.yml`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 steps:
 
 - name: step-0-welcome-welcome
   passed: []
   config:
     runtime:
+      customImage: zapatacomputing/orquestra-default:v0.0.0
       language: python3
       imports: [orq-wor-sdk, tut-0-wel]
       parameters:
         file: orq-wor-sdk/src/orquestra/sdk/_base/dispatch.py
         function: exec_task_fn
     resources:
       cpu: "1000m"
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/basics_with_data_aggregation.yml` & `orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/python_import.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,64 @@
-# workflow example inspired by https://docs.orquestra.io/quantum-engine/workflow-basics/
 apiVersion: io.orquestra.workflow/1.0.0
-
-dataAggregation:
-  resources:
-    cpu: '1'
-    disk: '1'
-    gpu: '1'
-    memory: '1'
-  run: true
-
-name: basics-with-data-aggregation
-
 imports:
-
-- name: tut-0-wel
-  type: git
+- name: eva-wor
   parameters:
-    commit: "master"
-    repository: "git@github.com:zapatacomputing/tutorial-0-welcome"
+    commit: morawiec/test
+    repository: git@github.com:zapatacomputing/evangelism-workflows.git
+  type: git
 - name: orq-wor-sdk
   parameters:
     commit: main
     repository: git@github.com:zapatacomputing/orquestra-workflow-sdk.git
   type: git
+- name: py
+  parameters:
+    requirements: 'numpy==1.21.5
 
+    pip'
+  type: python-requirements
+name: python-import
 steps:
-
-- name: step-0-welcome-welcome
-  passed: []
-  config:
+- config:
     runtime:
+      customImage: zapatacomputing/orquestra-default:v0.0.0
+      imports:
+      - eva-wor
+      - orq-wor-sdk
+      - py
       language: python3
-      imports: [orq-wor-sdk, tut-0-wel]
       parameters:
         file: orq-wor-sdk/src/orquestra/sdk/_base/dispatch.py
         function: exec_task_fn
-    resources:
-      cpu: "1000m"
-      memory: "1Gi"
-      disk: "15Gi"
-      gpu: "1"
   inputs:
   - __sdk_fn_ref_dict:
-      module: welcome
-      function_name: welcome
-      file_path: welcome.py
-      line_number: 7
+      file_path: workflow_defs.py
+      function_name: my_task
+      line_number: 36
+      module: workflow_defs
       type: MODULE_FUNCTION_REF
     type: sdk-metadata
   - __sdk_output_node_dicts:
-    - id: 'artifact-0-welcome'
-      custom_name: 'welcome'
-      serialization_format: 'AUTO'
-      artifact_index: null
+    - artifact_index: null
+      custom_name: null
+      id: artifact-0-my-task
+      serialization_format: AUTO
     type: sdk-metadata
-  - __sdk_additional_sys_paths: ["step/tut-0-wel"]
+  - __sdk_additional_sys_paths:
+    - step/eva-wor
     type: sdk-metadata
-  - __sdk_positional_args_ids: []
+  - __sdk_positional_args_ids:
+    - constant-0
     type: sdk-metadata
+  - constant-0:
+      serialization_format: JSON
+      value: 'null'
+    type: workflow-result-dict
+  name: invocation-0-task-my-task
   outputs:
-  - name: welcome
+  - name: artifact-0-my-task
     type: workflow-result-dict
-
+  passed: []
 types:
 - sdk-metadata
 - workflow-result-dict
 - workflow-secret-dict
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/basics_with_gpu.yml` & `orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/basics.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # workflow example inspired by https://docs.orquestra.io/quantum-engine/workflow-basics/
 apiVersion: io.orquestra.workflow/1.0.0
 
-name: basics-with-gpu
+name: basics
 
 imports:
 
 - name: tut-0-wel
   type: git
   parameters:
     commit: "master"
@@ -18,24 +18,24 @@
 
 steps:
 
 - name: step-0-welcome-welcome
   passed: []
   config:
     runtime:
+      customImage: zapatacomputing/orquestra-default:v0.0.0
       language: python3
       imports: [orq-wor-sdk, tut-0-wel]
       parameters:
         file: orq-wor-sdk/src/orquestra/sdk/_base/dispatch.py
         function: exec_task_fn
     resources:
       cpu: "1000m"
       memory: "1Gi"
       disk: "15Gi"
-      gpu: "1"
   inputs:
   - __sdk_fn_ref_dict:
       module: welcome
       function_name: welcome
       file_path: welcome.py
       line_number: 7
       type: MODULE_FUNCTION_REF
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/custom_json.yml` & `orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/custom_json.yml`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 steps:
 
 - name: invocation-0-task-0-last-element
   passed: []
   config:
     runtime:
+      customImage: zapatacomputing/orquestra-default:v0.0.0
       language: python3
       imports: [orq-wor-sdk]
       parameters:
         file: orq-wor-sdk/src/orquestra/sdk/_base/dispatch.py
         function: exec_task_fn
     resources:
       cpu: "1000m"
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/exportable_wf.yml` & `orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/multi_task_outputs.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,92 +1,87 @@
 # workflow example inspired by https://docs.orquestra.io/quantum-engine/workflow-basics/
 apiVersion: io.orquestra.workflow/1.0.0
 
-name: my-workflow
+name: multiple-task-outputs
 
 imports:
 
 - name: orq-wor-sdk
-  type: git
   parameters:
-    repository: "git@github.com:zapatacomputing/orquestra-workflow-sdk.git"
     commit: main
+    repository: git@github.com:zapatacomputing/orquestra-workflow-sdk.git
+  type: git
 
 steps:
-- config:
+- name: invocation-0-task-multi-output
+  passed: []
+  config:
     runtime:
+      customImage: zapatacomputing/orquestra-default:v0.0.0
       language: python3
-      customImage: "zapatacomputing/orquestra-default:v0.0.0"
       imports: [orq-wor-sdk]
       parameters:
         file: orq-wor-sdk/src/orquestra/sdk/_base/dispatch.py
         function: exec_task_fn
   inputs:
   - __sdk_fn_ref_dict:
       module: orquestra.sdk.examples.exportable_wf
-      function_name: make_greeting
+      function_name: multi_output_test
       file_path: src/orquestra/sdk/examples/exportable_wf.py
-      line_number: 23
+      line_number: 0
       type: MODULE_FUNCTION_REF
     type: sdk-metadata
   - __sdk_output_node_dicts:
-    - id: 'artifact-0-make-greeting'
+    - id: 'artifact-0-multi-output'
       custom_name: null
       serialization_format: 'AUTO'
-      artifact_index: null
+      artifact_index: 0
+    - id: 'artifact-1-multi-output'
+      custom_name: null
+      serialization_format: 'AUTO'
+      artifact_index: 1
     type: sdk-metadata
   - __sdk_additional_sys_paths: ["step/orq-wor-sdk"]
     type: sdk-metadata
   - __sdk_positional_args_ids: []
     type: sdk-metadata
-  - first:
-      serialization_format: "JSON"
-      value: '"alex"'
-    type: workflow-result-dict
-  - last:
-      serialization_format: "JSON"
-      value: '"zapata"'
-    type: workflow-result-dict
-  - additional_message: ((invocation-1-task-multi-output-test.artifact-1-multi-output-test))
-    type: workflow-result-dict
-  name: invocation-0-task-make-greeting
   outputs:
-  - name: artifact-0-make-greeting
+  - name: artifact-0-multi-output
     type: workflow-result-dict
-  passed:
-  - invocation-1-task-multi-output-test
-- config:
+  - name: artifact-1-multi-output
+    type: workflow-result-dict
+- name: invocation-1-task-multi-output
+  passed: []
+  config:
     runtime:
+      customImage: zapatacomputing/orquestra-default:v0.0.0
       language: python3
-      customImage: "zapatacomputing/orquestra-default:v0.0.0"
       imports: [orq-wor-sdk]
       parameters:
         file: orq-wor-sdk/src/orquestra/sdk/_base/dispatch.py
         function: exec_task_fn
   inputs:
   - __sdk_fn_ref_dict:
       module: orquestra.sdk.examples.exportable_wf
       function_name: multi_output_test
       file_path: src/orquestra/sdk/examples/exportable_wf.py
-      line_number: 33
+      line_number: 0
       type: MODULE_FUNCTION_REF
     type: sdk-metadata
   - __sdk_output_node_dicts:
-    - id: 'artifact-1-multi-output-test'
+    - id: 'artifact-2-multi-output'
       custom_name: null
       serialization_format: 'AUTO'
       artifact_index: 1
     type: sdk-metadata
   - __sdk_additional_sys_paths: ["step/orq-wor-sdk"]
     type: sdk-metadata
   - __sdk_positional_args_ids: []
     type: sdk-metadata
-  name: invocation-1-task-multi-output-test
   outputs:
-  - name: artifact-1-multi-output-test
+  - name: artifact-2-multi-output
     type: workflow-result-dict
-  passed: []
 
 types:
 - sdk-metadata
 - workflow-result-dict
 - workflow-secret-dict
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/inline_function.yml` & `orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/inline_function.yml`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 steps:
 
 - name: step-0-welcome-welcome
   passed: []
   config:
     runtime:
+      customImage: zapatacomputing/orquestra-default:v0.0.0
       language: python3
       imports: [orq-wor-sdk]
       parameters:
         file: orq-wor-sdk/src/orquestra/sdk/_base/dispatch.py
         function: exec_task_fn
   inputs:
   - __sdk_fn_ref_dict:
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/main_test.json` & `orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/main_test.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955357142857143%*

 * *Differences: {"'tasks'": "{'task-0-local-test': {'output_metadata': OrderedDict([('is_subscriptable', False), "*

 * *            "('n_outputs', 1)])}}"}*

```diff
@@ -52,14 +52,18 @@
                 "file_path": "examples/hello_v2.py",
                 "function_name": "capitalize",
                 "line_number": 6,
                 "module": "examples.hello_v2",
                 "type": "MODULE_FUNCTION_REF"
             },
             "id": "task-0-local-test",
+            "output_metadata": {
+                "is_subscriptable": false,
+                "n_outputs": 1
+            },
             "parameters": [
                 {
                     "kind": "POSITIONAL_OR_KEYWORD",
                     "name": "text"
                 }
             ],
             "resources": null,
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/main_test.yml` & `orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/main_test.yml`

 * *Files 25% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     commit: main
     repository: git@github.com:zapatacomputing/orquestra-workflow-sdk.git
   type: git
 name: small
 steps:
 - config:
     runtime:
+      customImage: zapatacomputing/orquestra-default:v0.0.0
       imports:
       - orq-wor-sdk
       language: python3
       parameters:
         file: orq-wor-sdk/src/orquestra/sdk/_base/dispatch.py
         function: exec_task_fn
   inputs:
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/multi_task_outputs.yml` & `orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/multi_task_outputs_as_inputs.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # workflow example inspired by https://docs.orquestra.io/quantum-engine/workflow-basics/
 apiVersion: io.orquestra.workflow/1.0.0
 
-name: multiple-task-outputs
+name: multiple-task-outputs-as-inputs
 
 imports:
 
 - name: orq-wor-sdk
   parameters:
     commit: main
     repository: git@github.com:zapatacomputing/orquestra-workflow-sdk.git
   type: git
 
 steps:
 - name: invocation-0-task-multi-output
   passed: []
   config:
     runtime:
+      customImage: zapatacomputing/orquestra-default:v0.0.0
       language: python3
       imports: [orq-wor-sdk]
       parameters:
         file: orq-wor-sdk/src/orquestra/sdk/_base/dispatch.py
         function: exec_task_fn
   inputs:
   - __sdk_fn_ref_dict:
@@ -45,17 +46,18 @@
     type: sdk-metadata
   outputs:
   - name: artifact-0-multi-output
     type: workflow-result-dict
   - name: artifact-1-multi-output
     type: workflow-result-dict
 - name: invocation-1-task-multi-output
-  passed: []
+  passed: [invocation-0-task-multi-output]
   config:
     runtime:
+      customImage: zapatacomputing/orquestra-default:v0.0.0
       language: python3
       imports: [orq-wor-sdk]
       parameters:
         file: orq-wor-sdk/src/orquestra/sdk/_base/dispatch.py
         function: exec_task_fn
   inputs:
   - __sdk_fn_ref_dict:
@@ -69,16 +71,20 @@
     - id: 'artifact-2-multi-output'
       custom_name: null
       serialization_format: 'AUTO'
       artifact_index: 1
     type: sdk-metadata
   - __sdk_additional_sys_paths: ["step/orq-wor-sdk"]
     type: sdk-metadata
-  - __sdk_positional_args_ids: []
+  - __sdk_positional_args_ids: [artifact-0-multi-output, artifact-1-multi-output]
     type: sdk-metadata
+  - artifact-0-multi-output: ((invocation-0-task-multi-output.artifact-0-multi-output))
+    type: workflow-result-dict
+  - artifact-1-multi-output: ((invocation-0-task-multi-output.artifact-1-multi-output))
+    type: workflow-result-dict
   outputs:
   - name: artifact-2-multi-output
     type: workflow-result-dict
 
 types:
 - sdk-metadata
 - workflow-result-dict
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/multi_task_outputs_as_inputs.yml` & `orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/exportable_wf.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,106 @@
 # workflow example inspired by https://docs.orquestra.io/quantum-engine/workflow-basics/
 apiVersion: io.orquestra.workflow/1.0.0
 
-name: multiple-task-outputs-as-inputs
+name: my-workflow
 
 imports:
 
 - name: orq-wor-sdk
+  type: git
   parameters:
+    repository: "git@github.com:zapatacomputing/orquestra-workflow-sdk.git"
     commit: main
-    repository: git@github.com:zapatacomputing/orquestra-workflow-sdk.git
-  type: git
 
 steps:
-- name: invocation-0-task-multi-output
-  passed: []
-  config:
+- config:
     runtime:
+      customImage: zapatacomputing/orquestra-default:v0.0.0
       language: python3
+      customImage: "zapatacomputing/orquestra-default:v0.0.0"
       imports: [orq-wor-sdk]
       parameters:
         file: orq-wor-sdk/src/orquestra/sdk/_base/dispatch.py
         function: exec_task_fn
   inputs:
   - __sdk_fn_ref_dict:
       module: orquestra.sdk.examples.exportable_wf
-      function_name: multi_output_test
+      function_name: make_greeting
       file_path: src/orquestra/sdk/examples/exportable_wf.py
-      line_number: 0
+      line_number: 23
       type: MODULE_FUNCTION_REF
     type: sdk-metadata
   - __sdk_output_node_dicts:
-    - id: 'artifact-0-multi-output'
+    - id: 'artifact-0-make-greeting'
       custom_name: null
       serialization_format: 'AUTO'
-      artifact_index: 0
-    - id: 'artifact-1-multi-output'
-      custom_name: null
-      serialization_format: 'AUTO'
-      artifact_index: 1
+      artifact_index: null
     type: sdk-metadata
   - __sdk_additional_sys_paths: ["step/orq-wor-sdk"]
     type: sdk-metadata
   - __sdk_positional_args_ids: []
     type: sdk-metadata
-  outputs:
-  - name: artifact-0-multi-output
+  - first:
+      serialization_format: "JSON"
+      value: '"alex"'
     type: workflow-result-dict
-  - name: artifact-1-multi-output
+  - last:
+      serialization_format: "JSON"
+      value: '"zapata"'
     type: workflow-result-dict
-- name: invocation-1-task-multi-output
-  passed: [invocation-0-task-multi-output]
-  config:
+  - additional_message: ((invocation-1-task-multi-output-test.artifact-2-multi-output-test))
+    type: workflow-result-dict
+  name: invocation-0-task-make-greeting
+  outputs:
+  - name: artifact-0-make-greeting
+    type: workflow-result-dict
+  passed:
+  - invocation-1-task-multi-output-test
+- config:
     runtime:
+      customImage: zapatacomputing/orquestra-default:v0.0.0
       language: python3
+      customImage: "zapatacomputing/orquestra-default:v0.0.0"
       imports: [orq-wor-sdk]
       parameters:
         file: orq-wor-sdk/src/orquestra/sdk/_base/dispatch.py
         function: exec_task_fn
   inputs:
   - __sdk_fn_ref_dict:
       module: orquestra.sdk.examples.exportable_wf
       function_name: multi_output_test
       file_path: src/orquestra/sdk/examples/exportable_wf.py
-      line_number: 0
+      line_number: 33
       type: MODULE_FUNCTION_REF
     type: sdk-metadata
   - __sdk_output_node_dicts:
-    - id: 'artifact-2-multi-output'
+    - id: 'artifact-1-multi-output-test'
+      custom_name: null
+      serialization_format: 'AUTO'
+      artifact_index: 0
+    - id: 'artifact-2-multi-output-test'
       custom_name: null
       serialization_format: 'AUTO'
       artifact_index: 1
+    - id: 'artifact-3-multi-output-test'
+      custom_name: null
+      serialization_format: 'AUTO'
+      artifact_index: null
     type: sdk-metadata
   - __sdk_additional_sys_paths: ["step/orq-wor-sdk"]
     type: sdk-metadata
-  - __sdk_positional_args_ids: [artifact-0-multi-output, artifact-1-multi-output]
+  - __sdk_positional_args_ids: []
     type: sdk-metadata
-  - artifact-0-multi-output: ((invocation-0-task-multi-output.artifact-0-multi-output))
+  name: invocation-1-task-multi-output-test
+  outputs:
+  - name: artifact-1-multi-output-test
     type: workflow-result-dict
-  - artifact-1-multi-output: ((invocation-0-task-multi-output.artifact-1-multi-output))
+  - name: artifact-2-multi-output-test
     type: workflow-result-dict
-  outputs:
-  - name: artifact-2-multi-output
+  - name: artifact-3-multi-output-test
     type: workflow-result-dict
+  passed: []
 
 types:
 - sdk-metadata
 - workflow-result-dict
 - workflow-secret-dict
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/positional.yml` & `orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/positional.yml`

 * *Files 15% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 steps:
 
 - name: invocation-0-task-0-capitalize
   passed: []
   config:
     runtime:
+      customImage: zapatacomputing/orquestra-default:v0.0.0
       language: python3
       imports: [orq-wor-sdk]
       parameters:
         file: orq-wor-sdk/src/orquestra/sdk/_base/dispatch.py
         function: exec_task_fn
     resources:
       cpu: "1000m"
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/conversions/data/positional_artifact.yml` & `orquestra-sdk-0.47.0/tests/sdk/v2/conversions/data/positional_artifact.yml`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 steps:
 
 - name: invocation-0-task-0-capitalize
   passed: []
   config:
     runtime:
+      customImage: zapatacomputing/orquestra-default:v0.0.0
       language: python3
       imports: [orq-wor-sdk]
       parameters:
         file: orq-wor-sdk/src/orquestra/sdk/_base/dispatch.py
         function: exec_task_fn
     resources:
       cpu: "1000m"
@@ -52,14 +53,15 @@
   - name: artifact-0-capitalize
     type: workflow-result-dict
 
 - name: invocation-1-task-0-capitalize
   passed: ["invocation-0-task-0-capitalize"]
   config:
     runtime:
+      customImage: zapatacomputing/orquestra-default:v0.0.0
       language: python3
       imports: [orq-wor-sdk]
       parameters:
         file: orq-wor-sdk/src/orquestra/sdk/_base/dispatch.py
         function: exec_task_fn
     resources:
       cpu: "1000m"
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/conversions/test_ids.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/conversions/test_ids.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/conversions/test_imports.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/conversions/test_imports.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/conversions/test_yaml_exporter.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/conversions/test_yaml_exporter.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,916 +14,975 @@
 from orquestra.sdk.examples import exportable_wf
 
 
 def _model_dict(model_obj):
     return json.loads(model_obj.json(exclude_none=True))
 
 
-WORKFLOW_WITH_POSITIONAL_ARGS = model.WorkflowDef(
-    name="positional",
-    fn_ref=model.ModuleFunctionRef(
-        module="does_not.exist",
-        function_name="positional",
-        file_path="does_not/exist.py",
-        line_number=13,
-    ),
-    imports={
-        "orquestra-sdk": model.GitImport(
-            id="orquestra-sdk",
-            repo_url="git@github.com:zapatacomputing/orquestra-workflow-sdk.git",
-            git_ref="main",
-        ),
-    },
-    tasks={
-        "task-0-capitalize": model.TaskDef(
-            id="task-0-capitalize",
-            fn_ref=model.ModuleFunctionRef(
-                module="examples.hello_v2",
-                function_name="capitalize",
-                file_path="examples/hello_v2.py",
-                line_number=11,
-            ),
-            parameters=[
-                model.TaskParameter(
-                    name="text", kind=model.ParameterKind.POSITIONAL_OR_KEYWORD
-                ),
-            ],
-            source_import_id="orquestra-sdk",
-            dependency_import_ids=[],
-            resources=model.Resources(
-                cpu="1000m",
-                memory="1Gi",
-                disk="15Gi",
+def _make_workflow_with_positional_args():
+    return model.WorkflowDef(
+        name="positional",
+        fn_ref=model.ModuleFunctionRef(
+            module="does_not.exist",
+            function_name="positional",
+            file_path="does_not/exist.py",
+            line_number=13,
+        ),
+        imports={
+            "orquestra-sdk": model.GitImport(
+                id="orquestra-sdk",
+                repo_url="git@github.com:zapatacomputing/orquestra-workflow-sdk.git",
+                git_ref="main",
+            ),
+        },
+        tasks={
+            "task-0-capitalize": model.TaskDef(
+                id="task-0-capitalize",
+                fn_ref=model.ModuleFunctionRef(
+                    module="examples.hello_v2",
+                    function_name="capitalize",
+                    file_path="examples/hello_v2.py",
+                    line_number=11,
+                ),
+                parameters=[
+                    model.TaskParameter(
+                        name="text", kind=model.ParameterKind.POSITIONAL_OR_KEYWORD
+                    ),
+                ],
+                output_metadata=model.TaskOutputMetadata(
+                    is_subscriptable=False, n_outputs=1
+                ),
+                source_import_id="orquestra-sdk",
+                dependency_import_ids=[],
+                resources=model.Resources(
+                    cpu="1000m",
+                    memory="1Gi",
+                    disk="15Gi",
+                ),
             ),
-        ),
-    },
-    artifact_nodes={
-        "artifact-0-capitalize": model.ArtifactNode(
-            id="artifact-0-capitalize",
-        ),
-    },
-    constant_nodes={
-        "constant-0": model.ConstantNodeJSON(
-            id="constant-0",
-            value='"hello"',
-            value_preview="'hello'",
-        ),
-    },
-    task_invocations={
-        "invocation-0-task-0-capitalize": model.TaskInvocation(
-            id="invocation-0-task-0-capitalize",
-            task_id="task-0-capitalize",
-            args_ids=[
-                "constant-0",
-            ],
-            kwargs_ids={},
-            output_ids=["artifact-0-capitalize"],
-        ),
-    },
-    output_ids=["artifact-0-capitalize"],
-)
+        },
+        artifact_nodes={
+            "artifact-0-capitalize": model.ArtifactNode(
+                id="artifact-0-capitalize",
+            ),
+        },
+        constant_nodes={
+            "constant-0": model.ConstantNodeJSON(
+                id="constant-0",
+                value='"hello"',
+                value_preview="'hello'",
+            ),
+        },
+        task_invocations={
+            "invocation-0-task-0-capitalize": model.TaskInvocation(
+                id="invocation-0-task-0-capitalize",
+                task_id="task-0-capitalize",
+                args_ids=[
+                    "constant-0",
+                ],
+                kwargs_ids={},
+                output_ids=["artifact-0-capitalize"],
+            ),
+        },
+        output_ids=["artifact-0-capitalize"],
+    )
 
 
-WORKFLOW_WITH_POSITIONAL_ARTIFACT_ARGS = model.WorkflowDef(
-    name="positional_artifact",
-    fn_ref=model.ModuleFunctionRef(
-        module="does_not.exist",
-        function_name="positional",
-        file_path="does_not/exist.py",
-        line_number=13,
-    ),
-    imports={
-        "orquestra-sdk": model.GitImport(
-            id="orquestra-sdk",
-            repo_url="git@github.com:zapatacomputing/orquestra-workflow-sdk.git",
-            git_ref="main",
-        ),
-    },
-    tasks={
-        "task-0-capitalize": model.TaskDef(
-            id="task-0-capitalize",
-            fn_ref=model.ModuleFunctionRef(
-                module="examples.hello_v2",
-                function_name="capitalize",
-                file_path="examples/hello_v2.py",
-                line_number=11,
-            ),
-            parameters=[
-                model.TaskParameter(
-                    name="text", kind=model.ParameterKind.POSITIONAL_OR_KEYWORD
-                ),
-            ],
-            source_import_id="orquestra-sdk",
-            dependency_import_ids=[],
-            resources=model.Resources(
-                cpu="1000m",
-                memory="1Gi",
-                disk="15Gi",
+def _make_workflow_with_positional_artifact_args():
+    return model.WorkflowDef(
+        name="positional_artifact",
+        fn_ref=model.ModuleFunctionRef(
+            module="does_not.exist",
+            function_name="positional",
+            file_path="does_not/exist.py",
+            line_number=13,
+        ),
+        imports={
+            "orquestra-sdk": model.GitImport(
+                id="orquestra-sdk",
+                repo_url="git@github.com:zapatacomputing/orquestra-workflow-sdk.git",
+                git_ref="main",
+            ),
+        },
+        tasks={
+            "task-0-capitalize": model.TaskDef(
+                id="task-0-capitalize",
+                fn_ref=model.ModuleFunctionRef(
+                    module="examples.hello_v2",
+                    function_name="capitalize",
+                    file_path="examples/hello_v2.py",
+                    line_number=11,
+                ),
+                parameters=[
+                    model.TaskParameter(
+                        name="text", kind=model.ParameterKind.POSITIONAL_OR_KEYWORD
+                    ),
+                ],
+                output_metadata=model.TaskOutputMetadata(
+                    is_subscriptable=False, n_outputs=1
+                ),
+                source_import_id="orquestra-sdk",
+                dependency_import_ids=[],
+                resources=model.Resources(
+                    cpu="1000m",
+                    memory="1Gi",
+                    disk="15Gi",
+                ),
             ),
-        ),
-    },
-    artifact_nodes={
-        "artifact-0-capitalize": model.ArtifactNode(
-            id="artifact-0-capitalize",
-        ),
-        "artifact-1-capitalize": model.ArtifactNode(
-            id="artifact-1-capitalize",
-        ),
-    },
-    constant_nodes={
-        "constant-0": model.ConstantNodeJSON(
-            id="constant-0",
-            value='"hello"',
-            value_preview="'hello'",
-        ),
-    },
-    task_invocations={
-        "invocation-0-task-0-capitalize": model.TaskInvocation(
-            id="invocation-0-task-0-capitalize",
-            task_id="task-0-capitalize",
-            args_ids=[
-                "constant-0",
-            ],
-            kwargs_ids={},
-            output_ids=["artifact-0-capitalize"],
-        ),
-        "invocation-1-task-0-capitalize": model.TaskInvocation(
-            id="invocation-1-task-0-capitalize",
-            task_id="task-0-capitalize",
-            args_ids=[
-                "artifact-0-capitalize",
-            ],
-            kwargs_ids={},
-            output_ids=["artifact-1-capitalize"],
-        ),
-    },
-    output_ids=["artifact-1-capitalize"],
-)
+        },
+        artifact_nodes={
+            "artifact-0-capitalize": model.ArtifactNode(
+                id="artifact-0-capitalize",
+            ),
+            "artifact-1-capitalize": model.ArtifactNode(
+                id="artifact-1-capitalize",
+            ),
+        },
+        constant_nodes={
+            "constant-0": model.ConstantNodeJSON(
+                id="constant-0",
+                value='"hello"',
+                value_preview="'hello'",
+            ),
+        },
+        task_invocations={
+            "invocation-0-task-0-capitalize": model.TaskInvocation(
+                id="invocation-0-task-0-capitalize",
+                task_id="task-0-capitalize",
+                args_ids=[
+                    "constant-0",
+                ],
+                kwargs_ids={},
+                output_ids=["artifact-0-capitalize"],
+            ),
+            "invocation-1-task-0-capitalize": model.TaskInvocation(
+                id="invocation-1-task-0-capitalize",
+                task_id="task-0-capitalize",
+                args_ids=[
+                    "artifact-0-capitalize",
+                ],
+                kwargs_ids={},
+                output_ids=["artifact-1-capitalize"],
+            ),
+        },
+        output_ids=["artifact-1-capitalize"],
+    )
 
 
-WORKFLOW_WITH_CUSTOM_JSON_ARGS = model.WorkflowDef(
-    name="custom-json",
-    fn_ref=model.ModuleFunctionRef(
-        module="does_not.exist",
-        function_name="custom_json",
-        file_path="does_not/exist.py",
-        line_number=13,
-    ),
-    imports={
-        "orquestra-sdk": model.GitImport(
-            id="orquestra-sdk",
-            repo_url="git@github.com:zapatacomputing/orquestra-workflow-sdk.git",
-            git_ref="main",
-        ),
-    },
-    tasks={
-        "task-0-last-element": model.TaskDef(
-            id="task-0-last-element",
-            fn_ref=model.ModuleFunctionRef(
-                module="examples.hello_v2",
-                function_name="last_element",
-                file_path="examples/hello_v2.py",
-                line_number=11,
-            ),
-            parameters=[
-                model.TaskParameter(
-                    name="text", kind=model.ParameterKind.POSITIONAL_OR_KEYWORD
-                ),
-            ],
-            source_import_id="orquestra-sdk",
-            dependency_import_ids=[],
-            resources=model.Resources(
-                cpu="1000m",
-                memory="1Gi",
-                disk="15Gi",
+def _make_workflow_with_custom_json_args():
+    return model.WorkflowDef(
+        name="custom-json",
+        fn_ref=model.ModuleFunctionRef(
+            module="does_not.exist",
+            function_name="custom_json",
+            file_path="does_not/exist.py",
+            line_number=13,
+        ),
+        imports={
+            "orquestra-sdk": model.GitImport(
+                id="orquestra-sdk",
+                repo_url="git@github.com:zapatacomputing/orquestra-workflow-sdk.git",
+                git_ref="main",
+            ),
+        },
+        tasks={
+            "task-0-last-element": model.TaskDef(
+                id="task-0-last-element",
+                fn_ref=model.ModuleFunctionRef(
+                    module="examples.hello_v2",
+                    function_name="last_element",
+                    file_path="examples/hello_v2.py",
+                    line_number=11,
+                ),
+                parameters=[
+                    model.TaskParameter(
+                        name="text", kind=model.ParameterKind.POSITIONAL_OR_KEYWORD
+                    ),
+                ],
+                output_metadata=model.TaskOutputMetadata(
+                    is_subscriptable=False, n_outputs=1
+                ),
+                source_import_id="orquestra-sdk",
+                dependency_import_ids=[],
+                resources=model.Resources(
+                    cpu="1000m",
+                    memory="1Gi",
+                    disk="15Gi",
+                ),
             ),
-        ),
-    },
-    artifact_nodes={
-        "artifact-0-last-element": model.ArtifactNode(
-            id="artifact-0-last-element",
-        ),
-    },
-    constant_nodes={
-        "constant-0": model.ConstantNodeJSON(
-            id="constant-0",
-            value="[1, 2, 3, 4, 5]",
-            value_preview="[1, 2, 3, 4,",
-        ),
-    },
-    task_invocations={
-        "invocation-0-task-0-last-element": model.TaskInvocation(
-            id="invocation-0-task-0-last-element",
-            task_id="task-0-last-element",
-            args_ids=[
-                "constant-0",
-            ],
-            kwargs_ids={},
-            output_ids=["artifact-0-last-element"],
-        ),
-    },
-    output_ids=["artifact-0-last-element"],
-)
+        },
+        artifact_nodes={
+            "artifact-0-last-element": model.ArtifactNode(
+                id="artifact-0-last-element",
+            ),
+        },
+        constant_nodes={
+            "constant-0": model.ConstantNodeJSON(
+                id="constant-0",
+                value="[1, 2, 3, 4, 5]",
+                value_preview="[1, 2, 3, 4,",
+            ),
+        },
+        task_invocations={
+            "invocation-0-task-0-last-element": model.TaskInvocation(
+                id="invocation-0-task-0-last-element",
+                task_id="task-0-last-element",
+                args_ids=[
+                    "constant-0",
+                ],
+                kwargs_ids={},
+                output_ids=["artifact-0-last-element"],
+            ),
+        },
+        output_ids=["artifact-0-last-element"],
+    )
 
 
-WORKFLOW_WITH_PICKLED_ARGS = model.WorkflowDef(
-    name="pickled",
-    fn_ref=model.ModuleFunctionRef(
-        module="does_not.exist",
-        function_name="pickled",
-        file_path="does_not/exist.py",
-        line_number=13,
-    ),
-    imports={
-        "orquestra-sdk": model.GitImport(
-            id="orquestra-sdk",
-            repo_url="git@github.com:zapatacomputing/orquestra-workflow-sdk.git",
-            git_ref="main",
-        ),
-    },
-    tasks={
-        "task-0-capitalize": model.TaskDef(
-            id="task-0-capitalize",
-            fn_ref=model.ModuleFunctionRef(
-                module="examples.hello_v2",
-                function_name="capitalize",
-                file_path="examples/hello_v2.py",
-                line_number=11,
-            ),
-            parameters=[
-                model.TaskParameter(
-                    name="text", kind=model.ParameterKind.POSITIONAL_OR_KEYWORD
-                ),
-            ],
-            source_import_id="orquestra-sdk",
-            dependency_import_ids=[],
-            resources=model.Resources(
-                cpu="1000m",
-                memory="1Gi",
-                disk="15Gi",
+def _make_workflow_with_pickled_args():
+    return model.WorkflowDef(
+        name="pickled",
+        fn_ref=model.ModuleFunctionRef(
+            module="does_not.exist",
+            function_name="pickled",
+            file_path="does_not/exist.py",
+            line_number=13,
+        ),
+        imports={
+            "orquestra-sdk": model.GitImport(
+                id="orquestra-sdk",
+                repo_url="git@github.com:zapatacomputing/orquestra-workflow-sdk.git",
+                git_ref="main",
+            ),
+        },
+        tasks={
+            "task-0-capitalize": model.TaskDef(
+                id="task-0-capitalize",
+                fn_ref=model.ModuleFunctionRef(
+                    module="examples.hello_v2",
+                    function_name="capitalize",
+                    file_path="examples/hello_v2.py",
+                    line_number=11,
+                ),
+                parameters=[
+                    model.TaskParameter(
+                        name="text", kind=model.ParameterKind.POSITIONAL_OR_KEYWORD
+                    ),
+                ],
+                output_metadata=model.TaskOutputMetadata(
+                    is_subscriptable=False, n_outputs=1
+                ),
+                source_import_id="orquestra-sdk",
+                dependency_import_ids=[],
+                resources=model.Resources(
+                    cpu="1000m",
+                    memory="1Gi",
+                    disk="15Gi",
+                ),
             ),
-        ),
-    },
-    artifact_nodes={
-        "artifact-0-capitalize": model.ArtifactNode(
-            id="artifact-0-capitalize",
-        ),
-    },
-    constant_nodes={
-        "constant-0": model.ConstantNodePickle(
-            id="constant-0",
-            chunks=[
-                "gASVLQAAAAAAAACMCmRpbGwuX2RpbGyUjApfbG9hZF90eXBllJOUjAZvYmplY3SUhZRSlCmBlC4=\\n"  # noqa: E501'
-            ],
-            value_preview="<object obje",
-            serialization_format=model.ArtifactFormat.ENCODED_PICKLE,
-        ),
-    },
-    task_invocations={
-        "invocation-0-task-0-capitalize": model.TaskInvocation(
-            id="invocation-0-task-0-capitalize",
-            task_id="task-0-capitalize",
-            args_ids=[
-                "constant-0",
-            ],
-            kwargs_ids={},
-            output_ids=["artifact-0-capitalize"],
-        ),
-    },
-    output_ids=["artifact-0-capitalize"],
-)
+        },
+        artifact_nodes={
+            "artifact-0-capitalize": model.ArtifactNode(
+                id="artifact-0-capitalize",
+            ),
+        },
+        constant_nodes={
+            "constant-0": model.ConstantNodePickle(
+                id="constant-0",
+                chunks=[
+                    "gASVLQAAAAAAAACMCmRpbGwuX2RpbGyUjApfbG9hZF90eXBllJOUjAZvYmplY3SUhZRSlCmBlC4=\\n"  # noqa: E501'
+                ],
+                value_preview="<object obje",
+                serialization_format=model.ArtifactFormat.ENCODED_PICKLE,
+            ),
+        },
+        task_invocations={
+            "invocation-0-task-0-capitalize": model.TaskInvocation(
+                id="invocation-0-task-0-capitalize",
+                task_id="task-0-capitalize",
+                args_ids=[
+                    "constant-0",
+                ],
+                kwargs_ids={},
+                output_ids=["artifact-0-capitalize"],
+            ),
+        },
+        output_ids=["artifact-0-capitalize"],
+    )
 
 
-BASICS_WORKFLOW = model.WorkflowDef(
-    name="basics",
-    fn_ref=model.ModuleFunctionRef(
-        module="does_not.exist",
-        function_name="basics",
-        file_path="does_not/exist.py",
-        line_number=13,
-    ),
-    imports={
-        "welcome-to-orquestra": model.GitImport(
-            id="welcome-to-orquestra",
-            repo_url="git@github.com:zapatacomputing/tutorial-0-welcome",
-            git_ref="master",
-        ),
-    },
-    tasks={
-        "welcome-welcome": model.TaskDef(
-            id="welcome-welcome",
-            fn_ref=model.ModuleFunctionRef(
-                module="welcome",
-                function_name="welcome",
-                file_path="welcome.py",
-                line_number=7,
-            ),
-            parameters=[],
-            source_import_id="welcome-to-orquestra",
-            dependency_import_ids=[],
-            resources=model.Resources(
-                cpu="1000m",
-                memory="1Gi",
-                disk="15Gi",
+def _make_basics_workflow():
+    return model.WorkflowDef(
+        name="basics",
+        fn_ref=model.ModuleFunctionRef(
+            module="does_not.exist",
+            function_name="basics",
+            file_path="does_not/exist.py",
+            line_number=13,
+        ),
+        imports={
+            "welcome-to-orquestra": model.GitImport(
+                id="welcome-to-orquestra",
+                repo_url="git@github.com:zapatacomputing/tutorial-0-welcome",
+                git_ref="master",
+            ),
+        },
+        tasks={
+            "welcome-welcome": model.TaskDef(
+                id="welcome-welcome",
+                fn_ref=model.ModuleFunctionRef(
+                    module="welcome",
+                    function_name="welcome",
+                    file_path="welcome.py",
+                    line_number=7,
+                ),
+                parameters=[],
+                output_metadata=model.TaskOutputMetadata(
+                    is_subscriptable=False, n_outputs=1
+                ),
+                source_import_id="welcome-to-orquestra",
+                dependency_import_ids=[],
+                resources=model.Resources(
+                    cpu="1000m",
+                    memory="1Gi",
+                    disk="15Gi",
+                ),
             ),
-        ),
-    },
-    artifact_nodes={
-        "artifact-0-welcome": model.ArtifactNode(
-            id="artifact-0-welcome",
-            custom_name="welcome",
-        ),
-    },
-    constant_nodes={},
-    task_invocations={
-        "step-0-welcome-welcome": model.TaskInvocation(
-            id="step-0-welcome-welcome",
-            task_id="welcome-welcome",
-            args_ids=[],
-            kwargs_ids={},
-            output_ids=["artifact-0-welcome"],
-        ),
-    },
-    output_ids=["artifact-0-welcome"],
-)
-
-BASICS_WORKFLOW_WITH_GPU = model.WorkflowDef(
-    name="basics-with-gpu",
-    fn_ref=model.ModuleFunctionRef(
-        module="does_not.exist",
-        function_name="basics",
-        file_path="does_not/exist.py",
-        line_number=13,
-    ),
-    imports={
-        "welcome-to-orquestra": model.GitImport(
-            id="welcome-to-orquestra",
-            repo_url="git@github.com:zapatacomputing/tutorial-0-welcome",
-            git_ref="master",
-        ),
-    },
-    tasks={
-        "welcome-welcome": model.TaskDef(
-            id="welcome-welcome",
-            fn_ref=model.ModuleFunctionRef(
-                module="welcome",
-                function_name="welcome",
-                file_path="welcome.py",
-                line_number=7,
-            ),
-            parameters=[],
-            source_import_id="welcome-to-orquestra",
-            dependency_import_ids=[],
-            resources=model.Resources(
-                cpu="1000m",
-                memory="1Gi",
-                disk="15Gi",
-                gpu="1",
+        },
+        artifact_nodes={
+            "artifact-0-welcome": model.ArtifactNode(
+                id="artifact-0-welcome",
+                custom_name="welcome",
+            ),
+        },
+        constant_nodes={},
+        task_invocations={
+            "step-0-welcome-welcome": model.TaskInvocation(
+                id="step-0-welcome-welcome",
+                task_id="welcome-welcome",
+                args_ids=[],
+                kwargs_ids={},
+                output_ids=["artifact-0-welcome"],
             ),
-        ),
-    },
-    artifact_nodes={
-        "artifact-0-welcome": model.ArtifactNode(
-            id="artifact-0-welcome",
-            custom_name="welcome",
-        ),
-    },
-    constant_nodes={},
-    task_invocations={
-        "step-0-welcome-welcome": model.TaskInvocation(
-            id="step-0-welcome-welcome",
-            task_id="welcome-welcome",
-            args_ids=[],
-            kwargs_ids={},
-            output_ids=["artifact-0-welcome"],
-        ),
-    },
-    output_ids=["artifact-0-welcome"],
-)
+        },
+        output_ids=["artifact-0-welcome"],
+    )
 
-BASICS_FILE_REF_WORKFLOW = model.WorkflowDef(
-    name="basics-file-ref",
-    fn_ref=model.FileFunctionRef(
-        function_name="basics",
-        file_path="welcome.py",
-        line_number=13,
-    ),
-    imports={
-        "welcome-to-orquestra": model.GitImport(
-            id="welcome-to-orquestra",
-            repo_url="git@github.com:zapatacomputing/tutorial-0-welcome",
-            git_ref="master",
-        ),
-    },
-    tasks={
-        "welcome-welcome": model.TaskDef(
-            id="welcome-welcome",
-            fn_ref=model.FileFunctionRef(
-                function_name="welcome",
-                file_path="welcome.py",
-                line_number=7,
-            ),
-            parameters=[],
-            source_import_id="welcome-to-orquestra",
-            dependency_import_ids=[],
-            resources=model.Resources(
-                cpu="1000m",
-                memory="1Gi",
-                disk="15Gi",
+
+def _make_basics_workflow_with_gpu():
+    return model.WorkflowDef(
+        name="basics-with-gpu",
+        fn_ref=model.ModuleFunctionRef(
+            module="does_not.exist",
+            function_name="basics",
+            file_path="does_not/exist.py",
+            line_number=13,
+        ),
+        imports={
+            "welcome-to-orquestra": model.GitImport(
+                id="welcome-to-orquestra",
+                repo_url="git@github.com:zapatacomputing/tutorial-0-welcome",
+                git_ref="master",
+            ),
+        },
+        tasks={
+            "welcome-welcome": model.TaskDef(
+                id="welcome-welcome",
+                fn_ref=model.ModuleFunctionRef(
+                    module="welcome",
+                    function_name="welcome",
+                    file_path="welcome.py",
+                    line_number=7,
+                ),
+                parameters=[],
+                output_metadata=model.TaskOutputMetadata(
+                    is_subscriptable=False, n_outputs=1
+                ),
+                source_import_id="welcome-to-orquestra",
+                dependency_import_ids=[],
+                resources=model.Resources(
+                    cpu="1000m",
+                    memory="1Gi",
+                    disk="15Gi",
+                    gpu="1",
+                ),
             ),
-        ),
-    },
-    artifact_nodes={
-        "artifact-0-welcome": model.ArtifactNode(
-            id="artifact-0-welcome",
-            custom_name="welcome",
-        ),
-    },
-    constant_nodes={},
-    task_invocations={
-        "step-0-welcome-welcome": model.TaskInvocation(
-            id="step-0-welcome-welcome",
-            task_id="welcome-welcome",
-            args_ids=[],
-            kwargs_ids={},
-            output_ids=["artifact-0-welcome"],
-        ),
-    },
-    output_ids=["artifact-0-welcome"],
-)
+        },
+        artifact_nodes={
+            "artifact-0-welcome": model.ArtifactNode(
+                id="artifact-0-welcome",
+                custom_name="welcome",
+            ),
+        },
+        constant_nodes={},
+        task_invocations={
+            "step-0-welcome-welcome": model.TaskInvocation(
+                id="step-0-welcome-welcome",
+                task_id="welcome-welcome",
+                args_ids=[],
+                kwargs_ids={},
+                output_ids=["artifact-0-welcome"],
+            ),
+        },
+        output_ids=["artifact-0-welcome"],
+    )
 
 
-ADDITIONAL_METRICS = model.WorkflowDef(
-    name="additional-metrics",
-    fn_ref=model.ModuleFunctionRef(
-        module="does_not.exist",
-        function_name="additional_metrics",
-        file_path="does_not/exist.py",
-        line_number=13,
-    ),
-    imports={
-        "sklearn-component": model.GitImport(
-            id="sklearn-component",
-            repo_url=(
-                "git@github.com:zapatacomputing" "/tutorial-orquestra-sklearn.git"
+def _make_basics_file_ref_workflow():
+    return model.WorkflowDef(
+        name="basics-file-ref",
+        fn_ref=model.FileFunctionRef(
+            function_name="basics",
+            file_path="welcome.py",
+            line_number=13,
+        ),
+        imports={
+            "welcome-to-orquestra": model.GitImport(
+                id="welcome-to-orquestra",
+                repo_url="git@github.com:zapatacomputing/tutorial-0-welcome",
+                git_ref="master",
+            ),
+        },
+        tasks={
+            "welcome-welcome": model.TaskDef(
+                id="welcome-welcome",
+                fn_ref=model.FileFunctionRef(
+                    function_name="welcome",
+                    file_path="welcome.py",
+                    line_number=7,
+                ),
+                parameters=[],
+                output_metadata=model.TaskOutputMetadata(
+                    is_subscriptable=False, n_outputs=1
+                ),
+                source_import_id="welcome-to-orquestra",
+                dependency_import_ids=[],
+                resources=model.Resources(
+                    cpu="1000m",
+                    memory="1Gi",
+                    disk="15Gi",
+                ),
             ),
-            git_ref="master",
-        ),
-    },
-    tasks={
-        ("steps-ml-tutorial-3-exercise-steps-generate-data-step"): model.TaskDef(
-            # I know this is mouthful, but the idea was to use the fully
-            # qualified python module name. In this example, the module
-            # would be "steps.ml_tutorial_3_exercise_steps"
-            # https://github.com/zapatacomputing/tutorial-orquestra-sklearn/tree/master/steps
-            id="steps-ml-tutorial-3-exercise-steps-generate-data-step",
-            fn_ref=model.ModuleFunctionRef(
-                module="steps.ml_tutorial_3_exercise_steps",
-                function_name="generate_data_step",
-                file_path="steps/ml_tutorial_3_exercise_steps.py",
-                line_number=4,
-            ),
-            parameters=[
-                model.TaskParameter(
-                    name="dataset_name", kind=model.ParameterKind.POSITIONAL_OR_KEYWORD
-                )
-            ],
-            source_import_id="sklearn-component",
-            dependency_import_ids=[],
-            resources=None,
-        ),
-        ("steps-ml-tutorial-3-exercise-steps-preprocess-data-step"): model.TaskDef(
-            id="steps-ml-tutorial-3-exercise-steps-preprocess-data-step",
-            fn_ref=model.ModuleFunctionRef(
-                module="steps.ml_tutorial_3_exercise_steps",
-                function_name="preprocess_data_step",
-                file_path="steps/ml_tutorial_3_exercise_steps.py",
-                line_number=10,
-            ),
-            parameters=[
-                model.TaskParameter(
-                    name="data", kind=model.ParameterKind.POSITIONAL_OR_KEYWORD
-                )
-            ],
-            source_import_id="sklearn-component",
-            dependency_import_ids=[],
-            resources=None,
-        ),
-    },
-    artifact_nodes={
-        "artifact-0-generate-data-step": model.ArtifactNode(
-            id="artifact-0-generate-data-step",
-            custom_name="data",
-        ),
-        "artifact-1-preprocess-data": model.ArtifactNode(
-            id="artifact-1-preprocess-data",
-            custom_name="features",
-        ),
-        "artifact-2-preprocess-data": model.ArtifactNode(
-            id="artifact-2-preprocess-data",
-            custom_name="labels",
-        ),
-    },
-    constant_nodes={
-        "literal-0": model.ConstantNodeJSON(
-            id="literal-0",
-            value='"simple_dataset"',
-            value_preview="simple_datas",
-            serialization_format=model.ArtifactFormat.JSON,
-        ),
-    },
-    task_invocations={
-        (
-            "step-0-steps-ml-tutorial-3-exercise-steps-generate-data-step"
-        ): model.TaskInvocation(
-            id=("step-0-steps-ml-tutorial-3-exercise-steps" "-generate-data-step"),
-            task_id="steps-ml-tutorial-3-exercise-steps-generate-data-step",
-            args_ids=[],
-            kwargs_ids={"dataset_name": "literal-0"},
-            output_ids=["artifact-0-generate-data-step"],
-        ),
-        (
-            "step-1-steps-ml-tutorial-3-exercise-steps-preprocess-data-step"
-        ): model.TaskInvocation(
-            id="step-1-steps-ml-tutorial-3-exercise-steps-preprocess-data-step",
-            task_id="steps-ml-tutorial-3-exercise-steps-preprocess-data-step",
-            args_ids=[],
-            kwargs_ids={"data": "artifact-0-generate-data-step"},
-            output_ids=[
-                "artifact-1-preprocess-data",
-                "artifact-2-preprocess-data",
-            ],
-        ),
-    },
-    output_ids=["artifact-1-preprocess-data"],
-)
+        },
+        artifact_nodes={
+            "artifact-0-welcome": model.ArtifactNode(
+                id="artifact-0-welcome",
+                custom_name="welcome",
+            ),
+        },
+        constant_nodes={},
+        task_invocations={
+            "step-0-welcome-welcome": model.TaskInvocation(
+                id="step-0-welcome-welcome",
+                task_id="welcome-welcome",
+                args_ids=[],
+                kwargs_ids={},
+                output_ids=["artifact-0-welcome"],
+            ),
+        },
+        output_ids=["artifact-0-welcome"],
+    )
 
 
-MULTIPLE_TASK_OUTPUTS = model.WorkflowDef(
-    name="multiple-task-outputs",
-    fn_ref=model.ModuleFunctionRef(
-        module="test.v2.test_traversal",
-        function_name="multiple_task_outputs",
-        file_path="tests/sdk/v2/test_traversal.py",
-        line_number=0,
-        type="MODULE_FUNCTION_REF",
-    ),
-    imports={
-        "my_import": model.GitImport(
-            id="my_import",
-            repo_url="git@github.com:zapatacomputing/orquestra-workflow-sdk.git",
-            git_ref="main",
-        ),
-    },
-    tasks={
-        "task-multi-output-99daf1a352": model.TaskDef(
-            id="task-multi-output-99daf1a352",
-            fn_ref=model.ModuleFunctionRef(
-                module="orquestra.sdk.examples.exportable_wf",
-                function_name="multi_output_test",
-                file_path="src/orquestra/sdk/examples/exportable_wf.py",
-                line_number=0,
+def _make_additional_metrics():
+    return model.WorkflowDef(
+        name="additional-metrics",
+        fn_ref=model.ModuleFunctionRef(
+            module="does_not.exist",
+            function_name="additional_metrics",
+            file_path="does_not/exist.py",
+            line_number=13,
+        ),
+        imports={
+            "sklearn-component": model.GitImport(
+                id="sklearn-component",
+                repo_url=(
+                    "git@github.com:zapatacomputing" "/tutorial-orquestra-sklearn.git"
+                ),
+                git_ref="master",
             ),
-            parameters=[],
-            source_import_id="my_import",
-        )
-    },
-    artifact_nodes={
-        "artifact-0-multi-output": model.ArtifactNode(
-            id="artifact-0-multi-output",
-            artifact_index=0,
-        ),
-        "artifact-1-multi-output": model.ArtifactNode(
-            id="artifact-1-multi-output",
-            artifact_index=1,
-        ),
-        "artifact-2-multi-output": model.ArtifactNode(
-            id="artifact-2-multi-output",
-            artifact_index=1,
-        ),
-    },
-    constant_nodes={},
-    task_invocations={
-        "invocation-0-task-multi-output": model.TaskInvocation(
-            id="invocation-0-task-multi-output",
-            task_id="task-multi-output-99daf1a352",
-            args_ids=[],
-            kwargs_ids={},
-            output_ids=["artifact-0-multi-output", "artifact-1-multi-output"],
-        ),
-        "invocation-1-task-multi-output": model.TaskInvocation(
-            id="invocation-1-task-multi-output",
-            task_id="task-multi-output-99daf1a352",
-            args_ids=[],
-            kwargs_ids={},
-            output_ids=["artifact-2-multi-output"],
-        ),
-    },
-    output_ids=[
-        "artifact-0-multi-output",
-        "artifact-1-multi-output",
-        "artifact-2-multi-output",
-    ],
-)
-
-MULTIPLE_TASK_OUTPUTS_AS_INPUTS = model.WorkflowDef(
-    name="multiple-task-outputs-as-inputs",
-    fn_ref=model.ModuleFunctionRef(
-        module="test.v2.test_traversal",
-        function_name="multiple_task_outputs",
-        file_path="tests/sdk/v2/test_traversal.py",
-        line_number=0,
-        type="MODULE_FUNCTION_REF",
-    ),
-    imports={
-        "my_import": model.GitImport(
-            id="my_import",
-            repo_url="git@github.com:zapatacomputing/orquestra-workflow-sdk.git",
-            git_ref="main",
-        ),
-    },
-    tasks={
-        "task-multi-output-99daf1a352": model.TaskDef(
-            id="task-multi-output-99daf1a352",
-            fn_ref=model.ModuleFunctionRef(
-                module="orquestra.sdk.examples.exportable_wf",
-                function_name="multi_output_test",
-                file_path="src/orquestra/sdk/examples/exportable_wf.py",
-                line_number=0,
+        },
+        tasks={
+            ("steps-ml-tutorial-3-exercise-steps-generate-data-step"): model.TaskDef(
+                # I know this is mouthful, but the idea was to use the fully
+                # qualified python module name. In this example, the module
+                # would be "steps.ml_tutorial_3_exercise_steps"
+                # https://github.com/zapatacomputing/tutorial-orquestra-sklearn/tree/master/steps
+                id="steps-ml-tutorial-3-exercise-steps-generate-data-step",
+                fn_ref=model.ModuleFunctionRef(
+                    module="steps.ml_tutorial_3_exercise_steps",
+                    function_name="generate_data_step",
+                    file_path="steps/ml_tutorial_3_exercise_steps.py",
+                    line_number=4,
+                ),
+                parameters=[
+                    model.TaskParameter(
+                        name="dataset_name",
+                        kind=model.ParameterKind.POSITIONAL_OR_KEYWORD,
+                    )
+                ],
+                output_metadata=model.TaskOutputMetadata(
+                    is_subscriptable=True, n_outputs=2
+                ),
+                source_import_id="sklearn-component",
+                dependency_import_ids=[],
+                resources=None,
+            ),
+            ("steps-ml-tutorial-3-exercise-steps-preprocess-data-step"): model.TaskDef(
+                id="steps-ml-tutorial-3-exercise-steps-preprocess-data-step",
+                fn_ref=model.ModuleFunctionRef(
+                    module="steps.ml_tutorial_3_exercise_steps",
+                    function_name="preprocess_data_step",
+                    file_path="steps/ml_tutorial_3_exercise_steps.py",
+                    line_number=10,
+                ),
+                parameters=[
+                    model.TaskParameter(
+                        name="data", kind=model.ParameterKind.POSITIONAL_OR_KEYWORD
+                    )
+                ],
+                output_metadata=model.TaskOutputMetadata(
+                    is_subscriptable=True, n_outputs=2
+                ),
+                source_import_id="sklearn-component",
+                dependency_import_ids=[],
+                resources=None,
+            ),
+        },
+        artifact_nodes={
+            "artifact-0-generate-data-step": model.ArtifactNode(
+                id="artifact-0-generate-data-step",
+                custom_name="data",
+            ),
+            "artifact-1-preprocess-data": model.ArtifactNode(
+                id="artifact-1-preprocess-data",
+                custom_name="features",
+            ),
+            "artifact-2-preprocess-data": model.ArtifactNode(
+                id="artifact-2-preprocess-data",
+                custom_name="labels",
+            ),
+        },
+        constant_nodes={
+            "literal-0": model.ConstantNodeJSON(
+                id="literal-0",
+                value='"simple_dataset"',
+                value_preview="simple_datas",
+                serialization_format=model.ArtifactFormat.JSON,
             ),
-            parameters=[],
-            source_import_id="my_import",
-        )
-    },
-    artifact_nodes={
-        "artifact-0-multi-output": model.ArtifactNode(
-            id="artifact-0-multi-output",
-            artifact_index=0,
-        ),
-        "artifact-1-multi-output": model.ArtifactNode(
-            id="artifact-1-multi-output",
-            artifact_index=1,
-        ),
-        "artifact-2-multi-output": model.ArtifactNode(
-            id="artifact-2-multi-output",
-            artifact_index=1,
-        ),
-    },
-    constant_nodes={},
-    task_invocations={
-        "invocation-0-task-multi-output": model.TaskInvocation(
-            id="invocation-0-task-multi-output",
-            task_id="task-multi-output-99daf1a352",
-            args_ids=[],
-            kwargs_ids={},
-            output_ids=["artifact-0-multi-output", "artifact-1-multi-output"],
-        ),
-        "invocation-1-task-multi-output": model.TaskInvocation(
-            id="invocation-1-task-multi-output",
-            task_id="task-multi-output-99daf1a352",
-            args_ids=["artifact-0-multi-output", "artifact-1-multi-output"],
-            kwargs_ids={},
-            output_ids=["artifact-2-multi-output"],
-        ),
-    },
-    output_ids=[
-        "artifact-2-multi-output",
-    ],
-)
+        },
+        task_invocations={
+            (
+                "step-0-steps-ml-tutorial-3-exercise-steps-generate-data-step"
+            ): model.TaskInvocation(
+                id=("step-0-steps-ml-tutorial-3-exercise-steps" "-generate-data-step"),
+                task_id="steps-ml-tutorial-3-exercise-steps-generate-data-step",
+                args_ids=[],
+                kwargs_ids={"dataset_name": "literal-0"},
+                output_ids=["artifact-0-generate-data-step"],
+            ),
+            (
+                "step-1-steps-ml-tutorial-3-exercise-steps-preprocess-data-step"
+            ): model.TaskInvocation(
+                id="step-1-steps-ml-tutorial-3-exercise-steps-preprocess-data-step",
+                task_id="steps-ml-tutorial-3-exercise-steps-preprocess-data-step",
+                args_ids=[],
+                kwargs_ids={"data": "artifact-0-generate-data-step"},
+                output_ids=[
+                    "artifact-1-preprocess-data",
+                    "artifact-2-preprocess-data",
+                ],
+            ),
+        },
+        output_ids=["artifact-1-preprocess-data"],
+    )
 
 
-DATA_AGGREGATION_SETTINGS = model.WorkflowDef(
-    name="basics-with-data-aggregation",
-    fn_ref=model.ModuleFunctionRef(
-        module="does_not.exist",
-        function_name="basics",
-        file_path="does_not/exist.py",
-        line_number=13,
-    ),
-    imports={
-        "welcome-to-orquestra": model.GitImport(
-            id="welcome-to-orquestra",
-            repo_url="git@github.com:zapatacomputing/tutorial-0-welcome",
-            git_ref="master",
-        ),
-    },
-    tasks={
-        "welcome-welcome": model.TaskDef(
-            id="welcome-welcome",
-            fn_ref=model.ModuleFunctionRef(
-                module="welcome",
-                function_name="welcome",
-                file_path="welcome.py",
-                line_number=7,
-            ),
-            parameters=[],
-            source_import_id="welcome-to-orquestra",
-            dependency_import_ids=[],
-            resources=model.Resources(
-                cpu="1000m",
-                memory="1Gi",
-                disk="15Gi",
-                gpu="1",
+def _make_multiple_task_outputs():
+    return model.WorkflowDef(
+        name="multiple-task-outputs",
+        fn_ref=model.ModuleFunctionRef(
+            module="test.v2.test_traversal",
+            function_name="multiple_task_outputs",
+            file_path="tests/sdk/v2/test_traversal.py",
+            line_number=0,
+            type="MODULE_FUNCTION_REF",
+        ),
+        imports={
+            "my_import": model.GitImport(
+                id="my_import",
+                repo_url="git@github.com:zapatacomputing/orquestra-workflow-sdk.git",
+                git_ref="main",
+            ),
+        },
+        tasks={
+            "task-multi-output-99daf1a352": model.TaskDef(
+                id="task-multi-output-99daf1a352",
+                fn_ref=model.ModuleFunctionRef(
+                    module="orquestra.sdk.examples.exportable_wf",
+                    function_name="multi_output_test",
+                    file_path="src/orquestra/sdk/examples/exportable_wf.py",
+                    line_number=0,
+                ),
+                parameters=[],
+                output_metadata=model.TaskOutputMetadata(
+                    is_subscriptable=True, n_outputs=2
+                ),
+                source_import_id="my_import",
+            )
+        },
+        artifact_nodes={
+            "artifact-0-multi-output": model.ArtifactNode(
+                id="artifact-0-multi-output",
+                artifact_index=0,
+            ),
+            "artifact-1-multi-output": model.ArtifactNode(
+                id="artifact-1-multi-output",
+                artifact_index=1,
+            ),
+            "artifact-2-multi-output": model.ArtifactNode(
+                id="artifact-2-multi-output",
+                artifact_index=1,
+            ),
+        },
+        constant_nodes={},
+        task_invocations={
+            "invocation-0-task-multi-output": model.TaskInvocation(
+                id="invocation-0-task-multi-output",
+                task_id="task-multi-output-99daf1a352",
+                args_ids=[],
+                kwargs_ids={},
+                output_ids=["artifact-0-multi-output", "artifact-1-multi-output"],
+            ),
+            "invocation-1-task-multi-output": model.TaskInvocation(
+                id="invocation-1-task-multi-output",
+                task_id="task-multi-output-99daf1a352",
+                args_ids=[],
+                kwargs_ids={},
+                output_ids=["artifact-2-multi-output"],
+            ),
+        },
+        output_ids=[
+            "artifact-0-multi-output",
+            "artifact-1-multi-output",
+            "artifact-2-multi-output",
+        ],
+    )
+
+
+def _make_multiple_task_outputs_as_inputs():
+    return model.WorkflowDef(
+        name="multiple-task-outputs-as-inputs",
+        fn_ref=model.ModuleFunctionRef(
+            module="test.v2.test_traversal",
+            function_name="multiple_task_outputs",
+            file_path="tests/sdk/v2/test_traversal.py",
+            line_number=0,
+            type="MODULE_FUNCTION_REF",
+        ),
+        imports={
+            "my_import": model.GitImport(
+                id="my_import",
+                repo_url="git@github.com:zapatacomputing/orquestra-workflow-sdk.git",
+                git_ref="main",
+            ),
+        },
+        tasks={
+            "task-multi-output-99daf1a352": model.TaskDef(
+                id="task-multi-output-99daf1a352",
+                fn_ref=model.ModuleFunctionRef(
+                    module="orquestra.sdk.examples.exportable_wf",
+                    function_name="multi_output_test",
+                    file_path="src/orquestra/sdk/examples/exportable_wf.py",
+                    line_number=0,
+                ),
+                parameters=[],
+                output_metadata=model.TaskOutputMetadata(
+                    is_subscriptable=True, n_outputs=2
+                ),
+                source_import_id="my_import",
+            )
+        },
+        artifact_nodes={
+            "artifact-0-multi-output": model.ArtifactNode(
+                id="artifact-0-multi-output",
+                artifact_index=0,
+            ),
+            "artifact-1-multi-output": model.ArtifactNode(
+                id="artifact-1-multi-output",
+                artifact_index=1,
+            ),
+            "artifact-2-multi-output": model.ArtifactNode(
+                id="artifact-2-multi-output",
+                artifact_index=1,
+            ),
+        },
+        constant_nodes={},
+        task_invocations={
+            "invocation-0-task-multi-output": model.TaskInvocation(
+                id="invocation-0-task-multi-output",
+                task_id="task-multi-output-99daf1a352",
+                args_ids=[],
+                kwargs_ids={},
+                output_ids=["artifact-0-multi-output", "artifact-1-multi-output"],
+            ),
+            "invocation-1-task-multi-output": model.TaskInvocation(
+                id="invocation-1-task-multi-output",
+                task_id="task-multi-output-99daf1a352",
+                args_ids=["artifact-0-multi-output", "artifact-1-multi-output"],
+                kwargs_ids={},
+                output_ids=["artifact-2-multi-output"],
+            ),
+        },
+        output_ids=[
+            "artifact-2-multi-output",
+        ],
+    )
+
+
+def _make_data_aggregation_settings():
+    return model.WorkflowDef(
+        name="basics-with-data-aggregation",
+        fn_ref=model.ModuleFunctionRef(
+            module="does_not.exist",
+            function_name="basics",
+            file_path="does_not/exist.py",
+            line_number=13,
+        ),
+        imports={
+            "welcome-to-orquestra": model.GitImport(
+                id="welcome-to-orquestra",
+                repo_url="git@github.com:zapatacomputing/tutorial-0-welcome",
+                git_ref="master",
+            ),
+        },
+        tasks={
+            "welcome-welcome": model.TaskDef(
+                id="welcome-welcome",
+                fn_ref=model.ModuleFunctionRef(
+                    module="welcome",
+                    function_name="welcome",
+                    file_path="welcome.py",
+                    line_number=7,
+                ),
+                parameters=[],
+                output_metadata=model.TaskOutputMetadata(
+                    is_subscriptable=False, n_outputs=1
+                ),
+                source_import_id="welcome-to-orquestra",
+                dependency_import_ids=[],
+                resources=model.Resources(
+                    cpu="1000m",
+                    memory="1Gi",
+                    disk="15Gi",
+                    gpu="1",
+                ),
             ),
+        },
+        artifact_nodes={
+            "artifact-0-welcome": model.ArtifactNode(
+                id="artifact-0-welcome",
+                custom_name="welcome",
+            ),
+        },
+        constant_nodes={},
+        task_invocations={
+            "step-0-welcome-welcome": model.TaskInvocation(
+                id="step-0-welcome-welcome",
+                task_id="welcome-welcome",
+                args_ids=[],
+                kwargs_ids={},
+                output_ids=["artifact-0-welcome"],
+            ),
+        },
+        output_ids=["artifact-0-welcome"],
+        data_aggregation=model.DataAggregation(
+            run=True, resources=model.Resources(cpu="1", memory="1", disk="1", gpu="1")
         ),
-    },
-    artifact_nodes={
-        "artifact-0-welcome": model.ArtifactNode(
-            id="artifact-0-welcome",
-            custom_name="welcome",
-        ),
-    },
-    constant_nodes={},
-    task_invocations={
-        "step-0-welcome-welcome": model.TaskInvocation(
-            id="step-0-welcome-welcome",
-            task_id="welcome-welcome",
-            args_ids=[],
-            kwargs_ids={},
-            output_ids=["artifact-0-welcome"],
-        ),
-    },
-    output_ids=["artifact-0-welcome"],
-    data_aggregation=model.DataAggregation(
-        run=True, resources=model.Resources(cpu="1", memory="1", disk="1", gpu="1")
-    ),
-)
+    )
 
 
-INLINE_TASK = model.WorkflowDef(
-    name="basics",
-    fn_ref=model.ModuleFunctionRef(
-        module="does_not.exist",
-        function_name="basics",
-        file_path="does_not/exist.py",
-        line_number=13,
-    ),
-    imports={
-        "welcome-to-orquestra": model.GitImport(
-            id="welcome-to-orquestra",
-            repo_url="git@github.com:zapatacomputing/tutorial-0-welcome",
-            git_ref="master",
-        ),
-        "inline-import-0": model.InlineImport(
-            id="inline-import-0",
-        ),
-    },
-    tasks={
-        "welcome-welcome": model.TaskDef(
-            id="task-capitalize-inline-8bba29c9af",
-            fn_ref=model.InlineFunctionRef(
-                function_name="capitalize_inline",
-                encoded_function=[
-                    "gANjZGlsbC5fZGlsbApfY3JlYXRlX2Z1bmN0aW9uCnEAKGNkaWxsLl9kaWxsCl9jcmVhdGVfY29k\n"  # noqa: E501'
-                    "ZQpxAShLAUsASwBLAUsCS0NDCHwAoAChAFMAcQJOhXEDWAoAAABjYXBpdGFsaXplcQSFcQVYBAAA\n"  # noqa: E501'
-                    "AHRleHRxBoVxB1hFAAAAL1VzZXJzL3NlYmFzdGlhbm1vcmF3aWVjL2dpdC9vcnF1ZXN0cmEtc2Rr\n"  # noqa: E501'
-                    "L3Rlc3RzL3YyL3Rlc3RfdHJhdmVyc2FsLnB5cQhYEQAAAGNhcGl0YWxpemVfaW5saW5lcQlLakMC\n"  # noqa: E501'
-                    "AARxCikpdHELUnEMfXENWAgAAABfX25hbWVfX3EOWBcAAAB0ZXN0cy52Mi50ZXN0X3RyYXZlcnNh\n"  # noqa: E501'
-                    "bHEPc2gJTk50cRBScRF9cRIoWBcAAABfVGFza0RlZl9fc2RrX3Rhc2tfYm9keXETaBFYBgAAAGZu\n"  # noqa: E501'
-                    "X3JlZnEUY2RpbGwuX2RpbGwKX2NyZWF0ZV9uYW1lZHR1cGxlCnEVWBEAAABJbmxpbmVGdW5jdGlv\n"  # noqa: E501'
-                    "blJlZnEWWA0AAABmdW5jdGlvbl9uYW1lcRdYAgAAAGZucRiGcRlYFQAAAG9ycXVlc3RyYS5zZGsu\n"  # noqa: E501'
-                    "djIuX2RzbHEah3EbUnEcaAloEYZxHYFxHlgNAAAAc291cmNlX2ltcG9ydHEfaBVYDAAAAElubGlu\n"  # noqa: E501'
-                    "ZUltcG9ydHEgKWgah3EhUnEiKYFxI1gPAAAAb3V0cHV0X21ldGFkYXRhcSRoFVgSAAAAVGFza091\n"  # noqa: E501'
-                    "dHB1dE1ldGFkYXRhcSVYEAAAAGlzX3N1YnNjcmlwdGFibGVxJlgJAAAAbl9vdXRwdXRzcSeGcSho\n"  # noqa: E501'
-                    "GodxKVJxKolLAYZxK4FxLFgKAAAAcGFyYW1ldGVyc3EtY2NvbGxlY3Rpb25zCk9yZGVyZWREaWN0\n"  # noqa: E501'
-                    "CnEuKVJxL2gGaBVYDQAAAFRhc2tQYXJhbWV0ZXJxMFgEAAAAbmFtZXExWAQAAABraW5kcTKGcTNo\n"  # noqa: E501'
-                    "GodxNFJxNWgGY29ycXVlc3RyYS5zZGsudjIuX2RzbApQYXJhbWV0ZXJLaW5kCnE2WBUAAABQT1NJ\n"  # noqa: E501'
-                    "VElPTkFMX09SX0tFWVdPUkRxN4VxOFJxOYZxOoFxO3NYEgAAAGRlcGVuZGVuY3lfaW1wb3J0c3E8\n"  # noqa: E501'
-                    "TlgJAAAAcmVzb3VyY2VzcT1OWAwAAABjdXN0b21faW1hZ2VxPlgoAAAAemFwYXRhY29tcHV0aW5n\n"  # noqa: E501'
-                    "L29ycXVlc3RyYS1kZWZhdWx0OnYwLjAuMHE/WAsAAABjdXN0b21fbmFtZXFATnV9cUFYDwAAAF9f\n"  # noqa: E501'
-                    "YW5ub3RhdGlvbnNfX3FCfXFDaAZjZGlsbC5fZGlsbApfbG9hZF90eXBlCnFEWAMAAABzdHJxRYVx\n"  # noqa: E501'
-                    "RlJxR3NzhnFIYi4=\n"
+def _make_inline_task():
+    return model.WorkflowDef(
+        name="basics",
+        fn_ref=model.ModuleFunctionRef(
+            module="does_not.exist",
+            function_name="basics",
+            file_path="does_not/exist.py",
+            line_number=13,
+        ),
+        imports={
+            "welcome-to-orquestra": model.GitImport(
+                id="welcome-to-orquestra",
+                repo_url="git@github.com:zapatacomputing/tutorial-0-welcome",
+                git_ref="master",
+            ),
+            "inline-import-0": model.InlineImport(
+                id="inline-import-0",
+            ),
+        },
+        tasks={
+            "welcome-welcome": model.TaskDef(
+                id="task-capitalize-inline-8bba29c9af",
+                fn_ref=model.InlineFunctionRef(
+                    function_name="capitalize_inline",
+                    encoded_function=[
+                        "gANjZGlsbC5fZGlsbApfY3JlYXRlX2Z1bmN0aW9uCnEAKGNkaWxsLl9kaWxsCl9jcmVhdGVfY29k\n"  # noqa: E501'
+                        "ZQpxAShLAUsASwBLAUsCS0NDCHwAoAChAFMAcQJOhXEDWAoAAABjYXBpdGFsaXplcQSFcQVYBAAA\n"  # noqa: E501'
+                        "AHRleHRxBoVxB1hFAAAAL1VzZXJzL3NlYmFzdGlhbm1vcmF3aWVjL2dpdC9vcnF1ZXN0cmEtc2Rr\n"  # noqa: E501'
+                        "L3Rlc3RzL3YyL3Rlc3RfdHJhdmVyc2FsLnB5cQhYEQAAAGNhcGl0YWxpemVfaW5saW5lcQlLakMC\n"  # noqa: E501'
+                        "AARxCikpdHELUnEMfXENWAgAAABfX25hbWVfX3EOWBcAAAB0ZXN0cy52Mi50ZXN0X3RyYXZlcnNh\n"  # noqa: E501'
+                        "bHEPc2gJTk50cRBScRF9cRIoWBcAAABfVGFza0RlZl9fc2RrX3Rhc2tfYm9keXETaBFYBgAAAGZu\n"  # noqa: E501'
+                        "X3JlZnEUY2RpbGwuX2RpbGwKX2NyZWF0ZV9uYW1lZHR1cGxlCnEVWBEAAABJbmxpbmVGdW5jdGlv\n"  # noqa: E501'
+                        "blJlZnEWWA0AAABmdW5jdGlvbl9uYW1lcRdYAgAAAGZucRiGcRlYFQAAAG9ycXVlc3RyYS5zZGsu\n"  # noqa: E501'
+                        "djIuX2RzbHEah3EbUnEcaAloEYZxHYFxHlgNAAAAc291cmNlX2ltcG9ydHEfaBVYDAAAAElubGlu\n"  # noqa: E501'
+                        "ZUltcG9ydHEgKWgah3EhUnEiKYFxI1gPAAAAb3V0cHV0X21ldGFkYXRhcSRoFVgSAAAAVGFza091\n"  # noqa: E501'
+                        "dHB1dE1ldGFkYXRhcSVYEAAAAGlzX3N1YnNjcmlwdGFibGVxJlgJAAAAbl9vdXRwdXRzcSeGcSho\n"  # noqa: E501'
+                        "GodxKVJxKolLAYZxK4FxLFgKAAAAcGFyYW1ldGVyc3EtY2NvbGxlY3Rpb25zCk9yZGVyZWREaWN0\n"  # noqa: E501'
+                        "CnEuKVJxL2gGaBVYDQAAAFRhc2tQYXJhbWV0ZXJxMFgEAAAAbmFtZXExWAQAAABraW5kcTKGcTNo\n"  # noqa: E501'
+                        "GodxNFJxNWgGY29ycXVlc3RyYS5zZGsudjIuX2RzbApQYXJhbWV0ZXJLaW5kCnE2WBUAAABQT1NJ\n"  # noqa: E501'
+                        "VElPTkFMX09SX0tFWVdPUkRxN4VxOFJxOYZxOoFxO3NYEgAAAGRlcGVuZGVuY3lfaW1wb3J0c3E8\n"  # noqa: E501'
+                        "TlgJAAAAcmVzb3VyY2VzcT1OWAwAAABjdXN0b21faW1hZ2VxPlgoAAAAemFwYXRhY29tcHV0aW5n\n"  # noqa: E501'
+                        "L29ycXVlc3RyYS1kZWZhdWx0OnYwLjAuMHE/WAsAAABjdXN0b21fbmFtZXFATnV9cUFYDwAAAF9f\n"  # noqa: E501'
+                        "YW5ub3RhdGlvbnNfX3FCfXFDaAZjZGlsbC5fZGlsbApfbG9hZF90eXBlCnFEWAMAAABzdHJxRYVx\n"  # noqa: E501'
+                        "RlJxR3NzhnFIYi4=\n"
+                    ],
+                ),
+                parameters=[
+                    model.TaskParameter(
+                        name="text", kind=model.ParameterKind.POSITIONAL_OR_KEYWORD
+                    )
                 ],
-            ),
-            parameters=[
-                model.TaskParameter(
-                    name="text", kind=model.ParameterKind.POSITIONAL_OR_KEYWORD
-                )
-            ],
-            source_import_id="inline-import-0",
-        )
-    },
-    artifact_nodes={
-        "artifact-0-welcome": model.ArtifactNode(
-            id="artifact-0-welcome",
-            custom_name="welcome",
-        ),
-    },
-    constant_nodes={},
-    task_invocations={
-        "step-0-welcome-welcome": model.TaskInvocation(
-            id="step-0-welcome-welcome",
-            task_id="welcome-welcome",
-            args_ids=[],
-            kwargs_ids={},
-            output_ids=["artifact-0-welcome"],
+                output_metadata=model.TaskOutputMetadata(
+                    is_subscriptable=False, n_outputs=1
+                ),
+                source_import_id="inline-import-0",
+            )
+        },
+        artifact_nodes={
+            "artifact-0-welcome": model.ArtifactNode(
+                id="artifact-0-welcome",
+                custom_name="welcome",
+            ),
+        },
+        constant_nodes={},
+        task_invocations={
+            "step-0-welcome-welcome": model.TaskInvocation(
+                id="step-0-welcome-welcome",
+                task_id="welcome-welcome",
+                args_ids=[],
+                kwargs_ids={},
+                output_ids=["artifact-0-welcome"],
+            ),
+        },
+        output_ids=["artifact-0-welcome"],
+        data_aggregation=model.DataAggregation(
+            run=True, resources=model.Resources(cpu="1", memory="1", disk="1", gpu="1")
         ),
-    },
-    output_ids=["artifact-0-welcome"],
-    data_aggregation=model.DataAggregation(
-        run=True, resources=model.Resources(cpu="1", memory="1", disk="1", gpu="1")
-    ),
-)
+    )
 
 
-PYTHON_REQUIREMENTS = model.WorkflowDef(
-    name="python-import",
-    fn_ref=model.ModuleFunctionRef(
-        module="workflow_defs",
-        function_name="wf",
-        file_path="workflow_defs.py",
-        line_number=44,
-        type="MODULE_FUNCTION_REF",
-    ),
-    imports={
-        "hello_zapata": model.GitImport(
-            id="hello_zapata",
-            repo_url="git@github.com:zapatacomputing/evangelism-workflows.git",
-            git_ref="morawiec/test",
-            type="GIT_IMPORT",
-        ),
-        "git-1871174d6e_github_com_zapatacomputing_orquestra_sdk": model.GitImport(
-            id="git-1871174d6e_github_com_zapatacomputing_orquestra_sdk",
-            repo_url="git@github.com:zapatacomputing/orquestra-workflow-sdk.git",
-            git_ref="main",
-            type="GIT_IMPORT",
-        ),
-        "python-import-86be3435bb": model.PythonImports(
-            id="python-import-86be3435bb",
-            packages=[
-                model.PackageSpec(
-                    name="numpy",
-                    extras=[],
-                    version_constraints=["==1.21.5"],
-                    environment_markers="",
-                ),
-                model.PackageSpec(
-                    name="pip",
-                    extras=[],
-                    version_constraints=[],
-                    environment_markers="",
-                ),
-            ],
-            pip_options=[],
-            type="PYTHON_IMPORT",
-        ),
-    },
-    tasks={
-        "task-my-task-ed08df330d": model.TaskDef(
-            id="task-my-task-ed08df330d",
-            fn_ref=model.ModuleFunctionRef(
-                module="workflow_defs",
-                function_name="my_task",
-                file_path="workflow_defs.py",
-                line_number=36,
-                type="MODULE_FUNCTION_REF",
-            ),
-            parameters=[
-                model.TaskParameter(
-                    name="prev", kind=model.ParameterKind.POSITIONAL_OR_KEYWORD
-                )
-            ],
-            source_import_id="hello_zapata",
-            dependency_import_ids=[
-                "git-1871174d6e_github_com_zapatacomputing_orquestra_sdk",
-                "python-import-86be3435bb",
-            ],
-            resources=None,
-            custom_image="zapatacomputing/orquestra-default:v0.0.0",
-        )
-    },
-    artifact_nodes={
-        "artifact-0-my-task": model.ArtifactNode(
-            id="artifact-0-my-task",
-            custom_name=None,
-            serialization_format=model.ArtifactFormat.AUTO,
-            artifact_index=None,
-        )
-    },
-    constant_nodes={
-        "constant-0": model.ConstantNodeJSON(
-            id="constant-0",
-            value="null",
-            serialization_format=model.ArtifactFormat.JSON,
-            value_preview="None",
-        )
-    },
-    task_invocations={
-        "invocation-0-task-my-task": model.TaskInvocation(
-            id="invocation-0-task-my-task",
-            task_id="task-my-task-ed08df330d",
-            args_ids=["constant-0"],
-            kwargs_ids={},
-            output_ids=["artifact-0-my-task"],
-            resources=None,
-        )
-    },
-    output_ids=["artifact-0-my-task"],
-    data_aggregation=None,
-)
+def _make_python_requirements():
+    return model.WorkflowDef(
+        name="python-import",
+        fn_ref=model.ModuleFunctionRef(
+            module="workflow_defs",
+            function_name="wf",
+            file_path="workflow_defs.py",
+            line_number=44,
+            type="MODULE_FUNCTION_REF",
+        ),
+        imports={
+            "hello_zapata": model.GitImport(
+                id="hello_zapata",
+                repo_url="git@github.com:zapatacomputing/evangelism-workflows.git",
+                git_ref="morawiec/test",
+                type="GIT_IMPORT",
+            ),
+            "git-1871174d6e_github_com_zapatacomputing_orquestra_sdk": model.GitImport(
+                id="git-1871174d6e_github_com_zapatacomputing_orquestra_sdk",
+                repo_url="git@github.com:zapatacomputing/orquestra-workflow-sdk.git",
+                git_ref="main",
+                type="GIT_IMPORT",
+            ),
+            "python-import-86be3435bb": model.PythonImports(
+                id="python-import-86be3435bb",
+                packages=[
+                    model.PackageSpec(
+                        name="numpy",
+                        extras=[],
+                        version_constraints=["==1.21.5"],
+                        environment_markers="",
+                    ),
+                    model.PackageSpec(
+                        name="pip",
+                        extras=[],
+                        version_constraints=[],
+                        environment_markers="",
+                    ),
+                ],
+                pip_options=[],
+                type="PYTHON_IMPORT",
+            ),
+        },
+        tasks={
+            "task-my-task-ed08df330d": model.TaskDef(
+                id="task-my-task-ed08df330d",
+                fn_ref=model.ModuleFunctionRef(
+                    module="workflow_defs",
+                    function_name="my_task",
+                    file_path="workflow_defs.py",
+                    line_number=36,
+                    type="MODULE_FUNCTION_REF",
+                ),
+                parameters=[
+                    model.TaskParameter(
+                        name="prev", kind=model.ParameterKind.POSITIONAL_OR_KEYWORD
+                    )
+                ],
+                output_metadata=model.TaskOutputMetadata(
+                    is_subscriptable=False, n_outputs=1
+                ),
+                source_import_id="hello_zapata",
+                dependency_import_ids=[
+                    "git-1871174d6e_github_com_zapatacomputing_orquestra_sdk",
+                    "python-import-86be3435bb",
+                ],
+                resources=None,
+                custom_image="zapatacomputing/orquestra-default:v0.0.0",
+            )
+        },
+        artifact_nodes={
+            "artifact-0-my-task": model.ArtifactNode(
+                id="artifact-0-my-task",
+                custom_name=None,
+                serialization_format=model.ArtifactFormat.AUTO,
+                artifact_index=None,
+            )
+        },
+        constant_nodes={
+            "constant-0": model.ConstantNodeJSON(
+                id="constant-0",
+                value="null",
+                serialization_format=model.ArtifactFormat.JSON,
+                value_preview="None",
+            )
+        },
+        task_invocations={
+            "invocation-0-task-my-task": model.TaskInvocation(
+                id="invocation-0-task-my-task",
+                task_id="task-my-task-ed08df330d",
+                args_ids=["constant-0"],
+                kwargs_ids={},
+                output_ids=["artifact-0-my-task"],
+                resources=None,
+            )
+        },
+        output_ids=["artifact-0-my-task"],
+        data_aggregation=None,
+    )
 
 
 @pytest.fixture
 def override_semver(monkeypatch):
     version_mock = Mock(return_value="main")
     monkeypatch.setattr(_imports, "_get_package_version_tag", version_mock)
 
@@ -931,118 +990,127 @@
 DATA_PATH = Path("tests/sdk/v2/conversions/data")
 
 
 class TestWorkflowToYAML:
     @pytest.mark.parametrize(
         "workflow,ref_yaml_path",
         [
-            (WORKFLOW_WITH_POSITIONAL_ARGS, DATA_PATH / "positional.yml"),
+            (_make_workflow_with_positional_args, DATA_PATH / "positional.yml"),
             (
-                WORKFLOW_WITH_POSITIONAL_ARTIFACT_ARGS,
+                _make_workflow_with_positional_artifact_args,
                 DATA_PATH / "positional_artifact.yml",
             ),
-            (WORKFLOW_WITH_CUSTOM_JSON_ARGS, DATA_PATH / "custom_json.yml"),
-            (BASICS_WORKFLOW, DATA_PATH / "basics.yml"),
-            (BASICS_WORKFLOW_WITH_GPU, DATA_PATH / "basics_with_gpu.yml"),
-            (BASICS_FILE_REF_WORKFLOW, DATA_PATH / "basics_file_ref.yml"),
-            (ADDITIONAL_METRICS, DATA_PATH / "additional-metrics.yml"),
-            (MULTIPLE_TASK_OUTPUTS, DATA_PATH / "multi_task_outputs.yml"),
+            (_make_workflow_with_custom_json_args, DATA_PATH / "custom_json.yml"),
+            (_make_basics_workflow, DATA_PATH / "basics.yml"),
+            (_make_basics_workflow_with_gpu, DATA_PATH / "basics_with_gpu.yml"),
+            (_make_basics_file_ref_workflow, DATA_PATH / "basics_file_ref.yml"),
+            (_make_additional_metrics, DATA_PATH / "additional-metrics.yml"),
+            (_make_multiple_task_outputs, DATA_PATH / "multi_task_outputs.yml"),
             (
-                MULTIPLE_TASK_OUTPUTS_AS_INPUTS,
+                _make_multiple_task_outputs_as_inputs,
                 DATA_PATH / "multi_task_outputs_as_inputs.yml",
             ),
             (
-                DATA_AGGREGATION_SETTINGS,
+                _make_data_aggregation_settings,
                 DATA_PATH / "basics_with_data_aggregation.yml",
             ),
-            (INLINE_TASK, DATA_PATH / "inline_function.yml"),
-            (PYTHON_REQUIREMENTS, DATA_PATH / "python_import.yml"),
+            (_make_inline_task, DATA_PATH / "inline_function.yml"),
+            (_make_python_requirements, DATA_PATH / "python_import.yml"),
         ],
     )
+    @pytest.mark.filterwarnings("ignore::orquestra.sdk.exceptions.VersionMismatch")
     def test_matches_ref_file(self, override_semver, workflow, ref_yaml_path):
+        wf_model = workflow()
         with ref_yaml_path.open() as f:
             ref_yaml_contents = yaml.safe_load(f)
 
         assert (
-            _model_dict(yaml_converter.workflow_to_yaml(workflow)) == ref_yaml_contents
+            _model_dict(yaml_converter.workflow_to_yaml(wf_model)) == ref_yaml_contents
         )
 
     @pytest.mark.parametrize(
         "workflow",
         [
-            WORKFLOW_WITH_PICKLED_ARGS,
+            _make_workflow_with_pickled_args,
         ],
     )
+    @pytest.mark.filterwarnings("ignore::orquestra.sdk.exceptions.VersionMismatch")
     def test_for_pickled_constants(self, override_semver, workflow):
         """
         This method check if is possible to create the yaml representation of a workflow
         that contains constant nodes with pickled values.
 
         Params
             workflow: model.WorkflowDef = A workflow definition
         """
-        _ = yaml_converter.workflow_to_yaml(workflow)
+        wf_model = workflow()
+        _ = yaml_converter.workflow_to_yaml(wf_model)
 
 
-OVERRIDE_WORKFLOW = model.WorkflowDef(
-    name="basics",
-    fn_ref=model.ModuleFunctionRef(
-        module="does_not.exist",
-        function_name="basics",
-        file_path="does_not/exist.py",
-        line_number=13,
-    ),
-    imports={
-        "welcome-to-orquestra": model.GitImport(
-            id="welcome-to-orquestra",
-            repo_url="git@github.com:zapatacomputing/tutorial-0-welcome",
-            git_ref="master",
-        ),
-    },
-    tasks={
-        "welcome-welcome": model.TaskDef(
-            id="welcome-welcome",
-            fn_ref=model.ModuleFunctionRef(
-                module="welcome",
-                function_name="welcome",
-                file_path="welcome.py",
-                line_number=7,
-            ),
-            parameters=[],
-            source_import_id="welcome-to-orquestra",
-            dependency_import_ids=[],
-            resources=model.Resources(
-                cpu="1000m",
-                memory="1Gi",
-                disk="15Gi",
+def _make_override_workflow():
+    return model.WorkflowDef(
+        name="basics",
+        fn_ref=model.ModuleFunctionRef(
+            module="does_not.exist",
+            function_name="basics",
+            file_path="does_not/exist.py",
+            line_number=13,
+        ),
+        imports={
+            "welcome-to-orquestra": model.GitImport(
+                id="welcome-to-orquestra",
+                repo_url="git@github.com:zapatacomputing/tutorial-0-welcome",
+                git_ref="master",
+            ),
+        },
+        tasks={
+            "welcome-welcome": model.TaskDef(
+                id="welcome-welcome",
+                fn_ref=model.ModuleFunctionRef(
+                    module="welcome",
+                    function_name="welcome",
+                    file_path="welcome.py",
+                    line_number=7,
+                ),
+                parameters=[],
+                output_metadata=model.TaskOutputMetadata(
+                    is_subscriptable=False, n_outputs=1
+                ),
+                source_import_id="welcome-to-orquestra",
+                dependency_import_ids=[],
+                resources=model.Resources(
+                    cpu="1000m",
+                    memory="1Gi",
+                    disk="15Gi",
+                ),
             ),
-        ),
-    },
-    artifact_nodes={
-        "artifact-0-welcome": model.ArtifactNode(
-            id="artifact-0-welcome",
-            custom_name="welcome",
-        ),
-    },
-    constant_nodes={},
-    task_invocations={
-        "step-0-welcome-welcome": model.TaskInvocation(
-            id="step-0-welcome-welcome",
-            task_id="welcome-welcome",
-            args_ids=[],
-            kwargs_ids={},
-            output_ids=["artifact-0-welcome"],
-        ),
-    },
-    output_ids=["artifact-0-welcome"],
-)
+        },
+        artifact_nodes={
+            "artifact-0-welcome": model.ArtifactNode(
+                id="artifact-0-welcome",
+                custom_name="welcome",
+            ),
+        },
+        constant_nodes={},
+        task_invocations={
+            "step-0-welcome-welcome": model.TaskInvocation(
+                id="step-0-welcome-welcome",
+                task_id="welcome-welcome",
+                args_ids=[],
+                kwargs_ids={},
+                output_ids=["artifact-0-welcome"],
+            ),
+        },
+        output_ids=["artifact-0-welcome"],
+    )
 
 
+@pytest.mark.filterwarnings("ignore::orquestra.sdk.exceptions.VersionMismatch")
 def test_workflow_to_yaml_override_git_ref():
-    workflow = OVERRIDE_WORKFLOW
+    workflow = _make_override_workflow()
     ref_yaml_path = DATA_PATH / "basics.yml"
 
     with ref_yaml_path.open() as f:
         ref_yaml_contents = yaml.safe_load(f)
 
     ref_yaml_contents["imports"][1]["parameters"]["commit"] = "v0.26.0"
 
@@ -1076,75 +1144,82 @@
 
     with open(yaml_path) as f:
         ref_yaml_contents = yaml.safe_load(f)
 
     assert _model_dict(yaml_converter.workflow_to_yaml(workflow)) == ref_yaml_contents
 
 
+@pytest.mark.filterwarnings("ignore::orquestra.sdk.exceptions.VersionMismatch")
 def test_main(override_semver, monkeypatch, capsys):
     with (DATA_PATH / "main_test.json").open() as json_f:
         monkeypatch.setattr("sys.stdin", json_f)
         yaml_converter.main()
         captured = capsys.readouterr()
         with (DATA_PATH / "main_test.yml").open() as yaml_f:
             assert captured.out.strip() == yaml_f.read().strip()
 
 
-PLAIN_WORKFLOW = model.WorkflowDef(
-    name="plain",
-    fn_ref=model.ModuleFunctionRef(
-        module="does_not.exist",
-        function_name="plain",
-        file_path="does_not/exist.py",
-        line_number=13,
-    ),
-    imports={
-        "hello": model.GitImport(
-            id="hello",
-            repo_url="git@github.com:zapatacomputing/hello-world.git",
-            git_ref="main",
-        ),
-    },
-    tasks={
-        "task-0_hello": model.TaskDef(
-            id="task-0_hello",
-            fn_ref=model.ModuleFunctionRef(
-                module="does_not.matter",
-                function_name="hello",
-                file_path="does_not/matter.py",
-                line_number=1,
-            ),
-            parameters=[],
-            source_import_id="orquestra-sdk",
-            dependency_import_ids=[],
-            resources=model.Resources(
-                cpu="1000m",
-                memory="1Gi",
-                disk="15Gi",
-                gpu="1",
+def _make_plain_workflow():
+    return model.WorkflowDef(
+        name="plain",
+        fn_ref=model.ModuleFunctionRef(
+            module="does_not.exist",
+            function_name="plain",
+            file_path="does_not/exist.py",
+            line_number=13,
+        ),
+        imports={
+            "hello": model.GitImport(
+                id="hello",
+                repo_url="git@github.com:zapatacomputing/hello-world.git",
+                git_ref="main",
+            ),
+        },
+        tasks={
+            "task-0_hello": model.TaskDef(
+                id="task-0_hello",
+                fn_ref=model.ModuleFunctionRef(
+                    module="does_not.matter",
+                    function_name="hello",
+                    file_path="does_not/matter.py",
+                    line_number=1,
+                ),
+                parameters=[],
+                output_metadata=model.TaskOutputMetadata(
+                    is_subscriptable=False, n_outputs=1
+                ),
+                source_import_id="orquestra-sdk",
+                dependency_import_ids=[],
+                resources=model.Resources(
+                    cpu="1000m",
+                    memory="1Gi",
+                    disk="15Gi",
+                    gpu="1",
+                ),
             ),
-        ),
-    },
-    artifact_nodes={
-        "artifact-0_hello": model.ArtifactNode(
-            id="artifact-0_hello",
-        ),
-    },
-    constant_nodes={},
-    task_invocations={
-        "invocation-0_task-0_hello": model.TaskInvocation(
-            id="invocation-0_task-0_hello",
-            task_id="task-0_hello",
-            args_ids=[],
-            kwargs_ids={},
-            output_ids=["artifact-0_hello"],
-        ),
-    },
-    output_ids=["artifact-0_hello"],
-)
+        },
+        artifact_nodes={
+            "artifact-0_hello": model.ArtifactNode(
+                id="artifact-0_hello",
+            ),
+        },
+        constant_nodes={},
+        task_invocations={
+            "invocation-0_task-0_hello": model.TaskInvocation(
+                id="invocation-0_task-0_hello",
+                task_id="task-0_hello",
+                args_ids=[],
+                kwargs_ids={},
+                output_ids=["artifact-0_hello"],
+            ),
+        },
+        output_ids=["artifact-0_hello"],
+    )
 
 
+@pytest.mark.filterwarnings("ignore::orquestra.sdk.exceptions.VersionMismatch")
 def test_workflow_with_invalid_package_version(monkeypatch):
+    wf_model = _make_plain_workflow()
     version_mock = Mock(side_effect=_imports.PackageVersionError("mock", "mocked"))
     monkeypatch.setattr(_imports, "_get_package_version_tag", version_mock)
     with pytest.raises(RuntimeError):
-        _ = yaml_converter.workflow_to_yaml(PLAIN_WORKFLOW)
+        _ = yaml_converter.workflow_to_yaml(wf_model)
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/data/complex_serialization/workflow_defs.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/data/complex_serialization/workflow_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,31 +48,34 @@
 
 
 @sdk.task
 def invoke_callables(fns: t.List[t.Callable]) -> t.List[t.Any]:
     return [fn() for fn in fns]
 
 
-@sdk.task(n_outputs=1)
+@sdk.task
 def generate_simple_callable(num: int = 1) -> t.Callable:
     def _inner():
         return 42 + num
 
     return _inner
 
 
-@sdk.task(n_outputs=2)
+@sdk.task
 def generate_simple_callables(num: int = 1) -> t.List[t.Callable]:
     def _inner_1():
         return 42 + num
 
     def _inner_2():
         return 43 + num
 
-    return [_inner_1, _inner_2]
+    # We want the task to have one output. It's content will be a list.
+    callables = [_inner_1, _inner_2]
+
+    return callables
 
 
 class HasNum(t.Protocol):
     num: int
 
 
 @sdk.task
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/data/configs.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/data/configs.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/data/sample_project/workflow_defs_no_raise.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/data/sample_project/workflow_defs_no_raise.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/data/task_run_workflow_defs.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/data/task_run_workflow_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,19 @@
 
 @sdk.workflow
 def wf_single_task_with_const_parent():
     return [return_num(21)]
 
 
 @sdk.workflow
+def wf_single_task_with_secret_parent():
+    return [return_num(sdk.secrets.get("test"))]
+
+
+@sdk.workflow
 def wf_single_task_with_const_parent_kwargs():
     return [args_kwargs(**{"kwargs": 36})]
 
 
 @sdk.workflow
 def wf_single_task_with_const_parent_args_kwargs():
     return [args_kwargs(21, **{"kwargs": 36})]
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/dirs.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/dirs.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/driver/resp_mocks.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/driver/resp_mocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     TaskInvocationID,
     TaskRunID,
     WorkflowDefID,
     WorkflowRunID,
 )
 from orquestra.sdk._base.serde import result_from_artifact
 from orquestra.sdk.schema.ir import ArtifactFormat, WorkflowDef
+from orquestra.sdk.schema.responses import ComputeEngineWorkflowResult
 from orquestra.sdk.schema.workflow_run import RunStatus, TaskRun
 
 # --- Helpers ---
 # These helpers are used to reduce code duplication when creating test responses
 
 PLATFORM_TIME_FORMAT = "%Y-%m-%dT%H:%M:%S.%fZ"
 
@@ -236,15 +237,29 @@
             "80ba3786-70c0-11ed-a1eb-0242ac120002",
             "80ba3a88-70c0-11ed-a1eb-0242ac120002",
             "80ba3c7c-70c0-11ed-a1eb-0242ac120002",
         ]
     }
 
 
-def make_get_wf_run_result_response(result_obj: Any):
+def make_get_wf_run_result_response(result_list: List[Any]):
+    """
+    Based on:
+        https://github.com/zapatacomputing/workflow-driver/blob/main/openapi/src/resources/run-result.yaml#L13
+    """
+
+    return ComputeEngineWorkflowResult(
+        results=[
+            result_from_artifact(result_obj, ArtifactFormat.AUTO).dict()
+            for result_obj in result_list
+        ]
+    ).json()
+
+
+def make_get_wf_run_result_legacy_response(result_obj: Any):
     """
     Based on:
         https://github.com/zapatacomputing/workflow-driver/blob/main/openapi/src/resources/run-result.yaml#L13
     """
 
     return result_from_artifact(result_obj, ArtifactFormat.AUTO).dict()
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/driver/test_ce_runtime.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/driver/test_ce_runtime.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,32 @@
 # © Copyright 2022-2023 Zapata Computing Inc.
 ################################################################################
 from datetime import timedelta
 from pathlib import Path
-from unittest.mock import DEFAULT, MagicMock, Mock, call
+from unittest.mock import DEFAULT, MagicMock, Mock, call, create_autospec
 
 import pytest
 
 from orquestra.sdk import exceptions
+from orquestra.sdk._base import serde
 from orquestra.sdk._base._driver import _ce_runtime, _client, _exceptions, _models
 from orquestra.sdk._base._testing._example_wfs import (
     my_workflow,
     workflow_parametrised_with_resources,
     workflow_with_different_resources,
 )
 from orquestra.sdk.schema.configs import RuntimeConfiguration, RuntimeName
-from orquestra.sdk.schema.responses import JSONResult
-from orquestra.sdk.schema.workflow_run import State, WorkflowRunId
-
-
-@pytest.fixture
-def runtime(mock_workflow_db_location):
-    # Fake CE configuration
-    config = RuntimeConfiguration(
-        config_name="hello",
-        runtime_name=RuntimeName.QE_REMOTE,
-        runtime_options={"uri": "http://localhost", "token": "blah"},
-    )
-    # Return a runtime object
-    return _ce_runtime.CERuntime(config)
-
-
-@pytest.fixture
-def runtime_verbose(tmp_path):
-    (tmp_path / ".orquestra").mkdir(exist_ok=True)
-    # Fake QE configuration
-    config = RuntimeConfiguration(
-        config_name="hello",
-        runtime_name=RuntimeName.QE_REMOTE,
-        runtime_options={"uri": "http://localhost", "token": "blah"},
-    )
-    # Return a runtime object
-    return _ce_runtime.CERuntime(config, True)
+from orquestra.sdk.schema.ir import ArtifactFormat, WorkflowDef
+from orquestra.sdk.schema.responses import ComputeEngineWorkflowResult, JSONResult
+from orquestra.sdk.schema.workflow_run import (
+    RunStatus,
+    State,
+    WorkflowRun,
+    WorkflowRunId,
+)
 
 
 class TestInitialization:
     @pytest.mark.parametrize("proj_dir", [".", Path(".")])
     @pytest.mark.parametrize("verbose", [True, False])
     def test_passing_project_dir_and_config_obj(self, proj_dir, verbose):
         """
@@ -94,31 +76,51 @@
 
 
 @pytest.fixture
 def workflow_run_id():
     return "00000000-0000-0000-0000-000000000000"
 
 
+@pytest.fixture
+def workflow_run_status(workflow_run_id: WorkflowRunId):
+    def _workflow_run(state: State):
+        workflow_def_mock = create_autospec(WorkflowDef)
+        return WorkflowRun(
+            id=workflow_run_id,
+            workflow_def=workflow_def_mock,
+            task_runs=[],
+            status=RunStatus(
+                state=state,
+                start_time=None,
+                end_time=None,
+            ),
+        )
+
+    return _workflow_run
+
+
 class TestCreateWorkflowRun:
     def test_happy_path(
         self,
         mocked_client: MagicMock,
         runtime: _ce_runtime.CERuntime,
         workflow_def_id: str,
         workflow_run_id: str,
     ):
         # Given
         mocked_client.create_workflow_def.return_value = workflow_def_id
         mocked_client.create_workflow_run.return_value = workflow_run_id
 
         # When
-        wf_run_id = runtime.create_workflow_run(my_workflow.model)
+        wf_run_id = runtime.create_workflow_run(my_workflow.model, None)
 
         # Then
-        mocked_client.create_workflow_def.assert_called_once_with(my_workflow.model)
+        mocked_client.create_workflow_def.assert_called_once_with(
+            my_workflow.model, None
+        )
         mocked_client.create_workflow_run.assert_called_once_with(
             workflow_def_id,
             _models.Resources(cpu=None, memory=None, gpu=None, nodes=None),
         )
         assert isinstance(wf_run_id, WorkflowRunId)
         assert (
             wf_run_id == workflow_run_id
@@ -134,15 +136,15 @@
         ):
             # Given
             mocked_client.create_workflow_def.return_value = workflow_def_id
             mocked_client.create_workflow_run.return_value = workflow_run_id
 
             # When
             _ = runtime.create_workflow_run(
-                workflow_parametrised_with_resources(memory="10Gi").model
+                workflow_parametrised_with_resources(memory="10Gi").model, None
             )
 
             # Then
             mocked_client.create_workflow_run.assert_called_once_with(
                 workflow_def_id,
                 _models.Resources(cpu=None, memory="10Gi", gpu=None, nodes=None),
             )
@@ -156,15 +158,15 @@
         ):
             # Given
             mocked_client.create_workflow_def.return_value = workflow_def_id
             mocked_client.create_workflow_run.return_value = workflow_run_id
 
             # When
             _ = runtime.create_workflow_run(
-                workflow_parametrised_with_resources(cpu="1000m").model
+                workflow_parametrised_with_resources(cpu="1000m").model, None
             )
 
             # Then
             mocked_client.create_workflow_run.assert_called_once_with(
                 workflow_def_id,
                 _models.Resources(cpu="1000m", memory=None, gpu=None, nodes=None),
             )
@@ -178,15 +180,15 @@
         ):
             # Given
             mocked_client.create_workflow_def.return_value = workflow_def_id
             mocked_client.create_workflow_run.return_value = workflow_run_id
 
             # When
             _ = runtime.create_workflow_run(
-                workflow_parametrised_with_resources(gpu="1").model
+                workflow_parametrised_with_resources(gpu="1").model, None
             )
 
             # Then
             mocked_client.create_workflow_run.assert_called_once_with(
                 workflow_def_id,
                 _models.Resources(cpu=None, memory=None, gpu="1", nodes=None),
             )
@@ -199,15 +201,17 @@
             workflow_run_id: str,
         ):
             # Given
             mocked_client.create_workflow_def.return_value = workflow_def_id
             mocked_client.create_workflow_run.return_value = workflow_run_id
 
             # When
-            _ = runtime.create_workflow_run(workflow_with_different_resources().model)
+            _ = runtime.create_workflow_run(
+                workflow_with_different_resources().model, None
+            )
 
             # Then
             mocked_client.create_workflow_run.assert_called_once_with(
                 workflow_def_id,
                 _models.Resources(cpu="5000m", memory="3G", gpu="1", nodes=None),
             )
 
@@ -222,15 +226,16 @@
             mocked_client.create_workflow_def.return_value = workflow_def_id
             mocked_client.create_workflow_run.return_value = workflow_run_id
 
             # When
             _ = runtime.create_workflow_run(
                 my_workflow()
                 .with_resources(cpu="1", memory="1.5G", gpu="1", nodes=20)
-                .model
+                .model,
+                None,
             )
 
             # Then
             mocked_client.create_workflow_run.assert_called_once_with(
                 workflow_def_id,
                 _models.Resources(cpu="1", memory="1.5G", gpu="1", nodes=20),
             )
@@ -242,27 +247,27 @@
             # Given
             mocked_client.create_workflow_def.side_effect = (
                 _exceptions.InvalidWorkflowDef("message", "detail")
             )
 
             # When
             with pytest.raises(exceptions.WorkflowSyntaxError):
-                _ = runtime.create_workflow_run(my_workflow.model)
+                _ = runtime.create_workflow_run(my_workflow.model, None)
 
         def test_unknown_http(
             self, mocked_client: MagicMock, runtime: _ce_runtime.CERuntime
         ):
             # Given
             mocked_client.create_workflow_def.side_effect = (
                 _exceptions.UnknownHTTPError(MagicMock())
             )
 
             # When
             with pytest.raises(_exceptions.UnknownHTTPError):
-                _ = runtime.create_workflow_run(my_workflow.model)
+                _ = runtime.create_workflow_run(my_workflow.model, None)
 
         @pytest.mark.parametrize(
             "failure_exc", [_exceptions.InvalidTokenError, _exceptions.ForbiddenError]
         )
         def test_auth_failure(
             self,
             mocked_client: MagicMock,
@@ -270,15 +275,15 @@
             failure_exc: Exception,
         ):
             # Given
             mocked_client.create_workflow_def.side_effect = failure_exc
 
             # When
             with pytest.raises(exceptions.UnauthorizedError):
-                _ = runtime.create_workflow_run(my_workflow.model)
+                _ = runtime.create_workflow_run(my_workflow.model, None)
 
     class TestWorkflowRunFailure:
         @pytest.fixture
         def mocked_client(self, mocked_client: MagicMock, workflow_def_id: str):
             mocked_client.create_workflow_def.return_value = workflow_def_id
             return mocked_client
 
@@ -290,27 +295,27 @@
             # Given
             mocked_client.create_workflow_run.side_effect = (
                 _exceptions.InvalidWorkflowRunRequest("message", "detail")
             )
 
             # When
             with pytest.raises(exceptions.WorkflowRunNotStarted):
-                _ = runtime.create_workflow_run(my_workflow.model)
+                _ = runtime.create_workflow_run(my_workflow.model, None)
 
         def test_unknown_http(
             self, mocked_client: MagicMock, runtime: _ce_runtime.CERuntime
         ):
             # Given
             mocked_client.create_workflow_run.side_effect = (
                 _exceptions.UnknownHTTPError(MagicMock())
             )
 
             # When
             with pytest.raises(_exceptions.UnknownHTTPError):
-                _ = runtime.create_workflow_run(my_workflow.model)
+                _ = runtime.create_workflow_run(my_workflow.model, None)
 
         @pytest.mark.parametrize(
             "failure_exc", [_exceptions.InvalidTokenError, _exceptions.ForbiddenError]
         )
         def test_auth_failure(
             self,
             mocked_client: MagicMock,
@@ -318,15 +323,15 @@
             failure_exc: Exception,
         ):
             # Given
             mocked_client.create_workflow_run.side_effect = failure_exc
 
             # When
             with pytest.raises(exceptions.UnauthorizedError):
-                _ = runtime.create_workflow_run(my_workflow.model)
+                _ = runtime.create_workflow_run(my_workflow.model, None)
 
 
 class TestGetWorkflowRunStatus:
     def test_happy_path(
         self,
         mocked_client: MagicMock,
         runtime: _ce_runtime.CERuntime,
@@ -413,43 +418,49 @@
         self,
         mocked_client: MagicMock,
         runtime: _ce_runtime.CERuntime,
         workflow_run_id: str,
     ):
         # Given
         mocked_client.get_workflow_run_results.return_value = ["result_id"]
-        mocked_client.get_workflow_run_result.return_value = JSONResult(value="[1]")
+        mocked_client.get_workflow_run_result.return_value = (
+            ComputeEngineWorkflowResult(results=[JSONResult(value="[1]")])
+        )
 
         # When
         results = runtime.get_workflow_run_outputs_non_blocking(workflow_run_id)
 
         # Then
         mocked_client.get_workflow_run_results.assert_called_once_with(workflow_run_id)
         mocked_client.get_workflow_run_result.assert_has_calls([call("result_id")])
-        assert results == (1,)
+        assert results == (JSONResult(value="[1]"),)
 
     def test_happy_path_tuple(
         self,
         mocked_client: MagicMock,
         runtime: _ce_runtime.CERuntime,
         workflow_run_id: str,
     ):
         # Given
-        mocked_client.get_workflow_run_results.return_value = ["result_id"]
-        # Currently, the result is JSON serialised, which means the tuple information
-        # is discarded
-        mocked_client.get_workflow_run_result.return_value = JSONResult(value="[1, 2]")
+        mocked_client.get_workflow_run_results.return_value = [
+            "result_id",
+        ]
+        mocked_client.get_workflow_run_result.side_effect = [
+            ComputeEngineWorkflowResult(
+                results=[JSONResult(value="1"), JSONResult(value="2")],
+            )
+        ]
 
         # When
         results = runtime.get_workflow_run_outputs_non_blocking(workflow_run_id)
 
         # Then
         mocked_client.get_workflow_run_results.assert_called_once_with(workflow_run_id)
         mocked_client.get_workflow_run_result.assert_has_calls([call("result_id")])
-        assert results == (1, 2)
+        assert results == (JSONResult(value="1"), JSONResult(value="2"))
 
     class TestGetWorkflowRunResultsFailure:
         def test_bad_workflow_run_id(
             self,
             mocked_client: MagicMock,
             runtime: _ce_runtime.CERuntime,
             workflow_run_id: str,
@@ -472,26 +483,72 @@
             mocked_client.get_workflow_run_results.side_effect = (
                 _exceptions.WorkflowRunNotFound(workflow_run_id)
             )
             # When
             with pytest.raises(exceptions.WorkflowRunNotFoundError):
                 _ = runtime.get_workflow_run_outputs_non_blocking(workflow_run_id)
 
-        def test_no_results(
+        def test_no_results_not_succeeded(
             self,
             mocked_client: MagicMock,
             runtime: _ce_runtime.CERuntime,
             workflow_run_id: str,
+            workflow_run_status,
         ):
             # Given
             mocked_client.get_workflow_run_results.return_value = []
+            mocked_client.get_workflow_run.return_value = workflow_run_status(
+                State.RUNNING
+            )
             # When
             with pytest.raises(exceptions.WorkflowRunNotSucceeded):
                 _ = runtime.get_workflow_run_outputs_non_blocking(workflow_run_id)
 
+        def test_no_results_succeeded(
+            self,
+            monkeypatch: pytest.MonkeyPatch,
+            mocked_client: MagicMock,
+            runtime: _ce_runtime.CERuntime,
+            workflow_run_id: str,
+            workflow_run_status,
+        ):
+            # Given
+            mocked_client.get_workflow_run_results.return_value = []
+            mocked_client.get_workflow_run.return_value = workflow_run_status(
+                State.SUCCEEDED
+            )
+            monkeypatch.setattr(_ce_runtime._retry.time, "sleep", Mock())
+            # When
+            with pytest.raises(exceptions.WorkflowResultsNotReadyError):
+                _ = runtime.get_workflow_run_outputs_non_blocking(workflow_run_id)
+
+            # We should try a few times if the results were not ready
+            assert mocked_client.get_workflow_run_results.call_count == 5
+
+        def test_eventually_get_results(
+            self,
+            monkeypatch: pytest.MonkeyPatch,
+            mocked_client: MagicMock,
+            runtime: _ce_runtime.CERuntime,
+            workflow_run_id: str,
+            workflow_run_status,
+        ):
+            # Given
+            mocked_client.get_workflow_run_results.side_effect = [[], [], [Mock()]]
+            mocked_client.get_workflow_run.return_value = workflow_run_status(
+                State.SUCCEEDED
+            )
+            monkeypatch.setattr(_ce_runtime.serde, "deserialize", lambda x: x)
+            monkeypatch.setattr(_ce_runtime._retry.time, "sleep", Mock())
+            # When
+            _ = runtime.get_workflow_run_outputs_non_blocking(workflow_run_id)
+
+            # We should have the results after 3 attempts
+            assert mocked_client.get_workflow_run_results.call_count == 3
+
         def test_unknown_http(
             self,
             mocked_client: MagicMock,
             runtime: _ce_runtime.CERuntime,
             workflow_run_id: str,
         ):
             # Given
@@ -564,32 +621,32 @@
         self,
         mocked_client: MagicMock,
         runtime: _ce_runtime.CERuntime,
         workflow_run_id: str,
     ):
         # Given
         mocked_client.get_workflow_run_artifacts.return_value = {
-            f"{workflow_run_id}@task-inv-1": ["wf-art-1", "wf-art-2"],
+            f"{workflow_run_id}@task-inv-1": ["wf-art-1"],
             f"{workflow_run_id}@task-inv-2": ["wf-art-3"],
         }
         mocked_client.get_workflow_run_artifact.return_value = JSONResult(value="1")
 
         # When
         results = runtime.get_available_outputs(workflow_run_id)
 
         # Then
         mocked_client.get_workflow_run_artifacts.assert_called_once_with(
             workflow_run_id
         )
         mocked_client.get_workflow_run_artifact.assert_has_calls(
-            [call("wf-art-1"), call("wf-art-2"), call("wf-art-3")]
+            [call("wf-art-1"), call("wf-art-3")]
         )
         assert results == {
-            "task-inv-1": (1, 1),
-            "task-inv-2": (1,),
+            "task-inv-1": JSONResult(value="1"),
+            "task-inv-2": JSONResult(value="1"),
         }
 
     class TestGetWorkflowRunArtifactsFailure:
         def test_bad_workflow_run_id(
             self,
             mocked_client: MagicMock,
             runtime: _ce_runtime.CERuntime,
@@ -662,15 +719,15 @@
             with pytest.raises(exceptions.UnauthorizedError):
                 _ = runtime.get_available_outputs(workflow_run_id)
 
     class TestGetWorkflowRunArtifactFailure:
         @pytest.fixture
         def mocked_client(self, mocked_client: MagicMock, workflow_run_id):
             mocked_client.get_workflow_run_artifacts.return_value = {
-                f"{workflow_run_id}@task-inv-1": ["wf-art-1", "wf-art-2"],
+                f"{workflow_run_id}@task-inv-1": ["wf-art-1"],
                 f"{workflow_run_id}@task-inv-2": ["wf-art-3"],
             }
             return mocked_client
 
         def test_any_failure(
             self,
             mocked_client: MagicMock,
@@ -684,71 +741,68 @@
             results = runtime.get_available_outputs(workflow_run_id)
 
             # Then
             mocked_client.get_workflow_run_artifacts.assert_called_once_with(
                 workflow_run_id
             )
             mocked_client.get_workflow_run_artifact.assert_has_calls(
-                [call("wf-art-1"), call("wf-art-2"), call("wf-art-3")]
+                [call("wf-art-1"), call("wf-art-3")]
             )
             assert results == {}
 
         def test_returns_successful_artifacts_after_failure(
             self,
             mocked_client: MagicMock,
             runtime: _ce_runtime.CERuntime,
             workflow_run_id: str,
         ):
             # Given
             mocked_client.get_workflow_run_artifact.return_value = JSONResult(value="1")
             mocked_client.get_workflow_run_artifact.side_effect = (
                 DEFAULT,
-                DEFAULT,
                 Exception,
             )
 
             # When
             results = runtime.get_available_outputs(workflow_run_id)
 
             # Then
             mocked_client.get_workflow_run_artifacts.assert_called_once_with(
                 workflow_run_id
             )
             mocked_client.get_workflow_run_artifact.assert_has_calls(
-                [call("wf-art-1"), call("wf-art-2"), call("wf-art-3")]
+                [call("wf-art-1"), call("wf-art-3")]
             )
-            assert results == {"task-inv-1": (1, 1)}
+            assert results == {"task-inv-1": JSONResult(value="1")}
 
         def test_continues_after_failure(
             self,
             mocked_client: MagicMock,
             runtime: _ce_runtime.CERuntime,
             workflow_run_id: str,
         ):
             # Given
             mocked_client.get_workflow_run_artifact.return_value = JSONResult(value="1")
             mocked_client.get_workflow_run_artifact.side_effect = (
                 Exception,
                 DEFAULT,
-                DEFAULT,
             )
 
             # When
             results = runtime.get_available_outputs(workflow_run_id)
 
             # Then
             mocked_client.get_workflow_run_artifacts.assert_called_once_with(
                 workflow_run_id
             )
             mocked_client.get_workflow_run_artifact.assert_has_calls(
-                [call("wf-art-1"), call("wf-art-2"), call("wf-art-3")]
+                [call("wf-art-1"), call("wf-art-3")]
             )
             assert results == {
-                "task-inv-1": (1,),
-                "task-inv-2": (1,),
+                "task-inv-2": JSONResult(value="1"),
             }
 
         def test_unknown_http(
             self,
             mocked_client: MagicMock,
             runtime: _ce_runtime.CERuntime,
             workflow_run_id: str,
@@ -762,15 +816,15 @@
             results = runtime.get_available_outputs(workflow_run_id)
 
             # Then
             mocked_client.get_workflow_run_artifacts.assert_called_once_with(
                 workflow_run_id
             )
             mocked_client.get_workflow_run_artifact.assert_has_calls(
-                [call("wf-art-1"), call("wf-art-2"), call("wf-art-3")]
+                [call("wf-art-1"), call("wf-art-3")]
             )
             assert results == {}
 
         @pytest.mark.parametrize(
             "failure_exc", [_exceptions.InvalidTokenError, _exceptions.ForbiddenError]
         )
         def test_auth_failure(
@@ -787,15 +841,15 @@
             results = runtime.get_available_outputs(workflow_run_id)
 
             # Then
             mocked_client.get_workflow_run_artifacts.assert_called_once_with(
                 workflow_run_id
             )
             mocked_client.get_workflow_run_artifact.assert_has_calls(
-                [call("wf-art-1"), call("wf-art-2"), call("wf-art-3")]
+                [call("wf-art-1"), call("wf-art-3")]
             )
             assert results == {}
 
 
 class TestStopWorkflowRun:
     def test_happy_path(
         self,
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/driver/test_client.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/driver/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import orquestra.sdk as sdk
 from orquestra.sdk._base._driver import _exceptions
 from orquestra.sdk._base._driver._client import DriverClient, Paginated
 from orquestra.sdk._base._driver._models import Resources
 from orquestra.sdk.schema.ir import WorkflowDef
 from orquestra.sdk.schema.responses import JSONResult, PickleResult
-from orquestra.sdk.schema.workflow_run import RunStatus, State, TaskRun
+from orquestra.sdk.schema.workflow_run import ProjectRef, RunStatus, State, TaskRun
 
 from . import resp_mocks
 
 
 @pytest.fixture
 def mocked_responses():
     with responses.RequestsMock() as rsps:
@@ -375,32 +375,47 @@
                 return endpoint_mocker_base(
                     responses.POST,
                     f"{base_uri}/api/workflow-definitions",
                     default_status_code=201,
                 )
 
             @staticmethod
+            @pytest.mark.parametrize(
+                "project,params",
+                [
+                    (None, {}),
+                    (
+                        ProjectRef(workspace_id="a", project_id="b"),
+                        {"workspaceId": "a", "projectId": "b"},
+                    ),
+                ],
+            )
             def test_params_encoding(
                 endpoint_mocker,
                 client: DriverClient,
                 workflow_def_id,
                 workflow_def: WorkflowDef,
+                project,
+                params,
             ):
                 """
                 Verifies that params are correctly sent to the server.
                 """
                 endpoint_mocker(
                     json=resp_mocks.make_create_wf_def_response(id_=workflow_def_id),
-                    match=[responses.matchers.json_params_matcher(workflow_def.dict())],
+                    match=[
+                        responses.matchers.json_params_matcher(workflow_def.dict()),
+                        responses.matchers.query_param_matcher(params),
+                    ],
                     # Based on:
                     # https://github.com/zapatacomputing/workflow-driver/blob/2b353476d5b0161da31584533be208611a131bdc/openapi/src/resources/workflow-definitions.yaml#L42
                     status=201,
                 )
 
-                client.create_workflow_def(workflow_def)
+                client.create_workflow_def(workflow_def, project)
 
                 # The assertion is done by mocked_responses
 
             @staticmethod
             def test_sets_auth(
                 endpoint_mocker,
                 client: DriverClient,
@@ -416,15 +431,15 @@
                     ],
                     # Based on:
                     # https://github.com/zapatacomputing/workflow-driver/blob/2b353476d5b0161da31584533be208611a131bdc/openapi/src/resources/workflow-definitions.yaml#L42
                     status=201,
                     json=resp_mocks.make_create_wf_def_response(id_=workflow_def_id),
                 )
 
-                client.create_workflow_def(workflow_def)
+                client.create_workflow_def(workflow_def, None)
 
                 # The assertion is done by mocked_responses
 
             @staticmethod
             def test_invalid_definition(
                 endpoint_mocker,
                 client: DriverClient,
@@ -434,53 +449,53 @@
                     # Specified in:
                     # https://github.com/zapatacomputing/workflow-driver/blob/6270a214fff40f53d7b25ec967f2e7875eb296e3/openapi/src/resources/workflow-definitions.yaml#L50
                     status=400,
                     json=resp_mocks.make_error_response("Bad definition", "details"),
                 )
 
                 with pytest.raises(_exceptions.InvalidWorkflowDef):
-                    client.create_workflow_def(workflow_def)
+                    client.create_workflow_def(workflow_def, None)
 
             @staticmethod
             def test_unauthorized(
                 endpoint_mocker, client: DriverClient, workflow_def: WorkflowDef
             ):
                 endpoint_mocker(
                     # https://github.com/zapatacomputing/workflow-driver/blob/6270a214fff40f53d7b25ec967f2e7875eb296e3/openapi/src/resources/workflow-definitions.yaml#L56
                     status=401,
                 )
 
                 with pytest.raises(_exceptions.InvalidTokenError):
-                    client.create_workflow_def(workflow_def)
+                    client.create_workflow_def(workflow_def, None)
 
             @staticmethod
             def test_forbidden(
                 endpoint_mocker, client: DriverClient, workflow_def: WorkflowDef
             ):
                 endpoint_mocker(
                     # Specified in:
                     # https://github.com/zapatacomputing/workflow-driver/blob/6270a214fff40f53d7b25ec967f2e7875eb296e3/openapi/src/resources/workflow-definitions.yaml#L58
                     status=403,
                 )
 
                 with pytest.raises(_exceptions.ForbiddenError):
-                    _ = client.create_workflow_def(workflow_def)
+                    _ = client.create_workflow_def(workflow_def, None)
 
             @staticmethod
             def test_unknown_error(
                 endpoint_mocker, client: DriverClient, workflow_def: WorkflowDef
             ):
                 endpoint_mocker(
                     # Specified in:
                     # https://github.com/zapatacomputing/workflow-driver/blob/2b353476d5b0161da31584533be208611a131bdc/openapi/src/resources/workflow-definitions.yaml#L52
                     status=500,
                 )
 
                 with pytest.raises(_exceptions.UnknownHTTPError):
-                    _ = client.create_workflow_def(workflow_def)
+                    _ = client.create_workflow_def(workflow_def, None)
 
         class TestDelete:
             @staticmethod
             @pytest.fixture
             def endpoint_mocker(endpoint_mocker_base, base_uri: str, workflow_def_id):
                 """
                 Returns a helper for mocking requests. Assumes that most of the tests
@@ -1479,38 +1494,22 @@
                     f"{base_uri}/api/run-results/{workflow_run_result_id}",
                     # Specified in:
                     # https://github.com/zapatacomputing/workflow-driver/blob/6270a214fff40f53d7b25ec967f2e7875eb296e3/openapi/src/resources/run-result.yaml#L11
                     default_status_code=200,
                 )
 
             @staticmethod
-            @pytest.mark.parametrize("obj", [None, 100, "hello", np.eye(10)])
-            def test_objects(
-                endpoint_mocker,
-                client: DriverClient,
-                workflow_run_result_id: str,
-                obj: Any,
-            ):
-                endpoint_mocker(
-                    json=resp_mocks.make_get_wf_run_result_response(obj),
-                )
-
-                result = client.get_workflow_run_result(workflow_run_result_id)
-
-                assert isinstance(result, (JSONResult, PickleResult))
-
-            @staticmethod
             def test_sets_auth(
                 endpoint_mocker,
                 client: DriverClient,
                 token: str,
                 workflow_run_result_id: str,
             ):
                 endpoint_mocker(
-                    json=resp_mocks.make_get_wf_run_result_response(None),
+                    json=resp_mocks.make_get_wf_run_result_legacy_response(None),
                     match=[
                         responses.matchers.header_matcher(
                             {"Authorization": f"Bearer {token}"}
                         )
                     ],
                 )
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/project_state.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/project_state.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/sample_wfs.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/sample_wfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,11 +28,11 @@
 def integer_division(a, b):
     return a // b, a % b
 
 
 @sdk.workflow
 def wf(param: int):
     floor, remainder = integer_division(param, 3)
-    floor_plus_6 = add(floor, 6)
+    floor_plus_6 = add(a=floor, b=6)
     remainder_plus_3 = inc(inc_2(remainder))
 
     return floor_plus_6, remainder_plus_3
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/secrets/resp_mocks.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/secrets/resp_mocks.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/secrets/test_api.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/secrets/test_api.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/secrets/test_auth.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/secrets/test_auth.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/secrets/test_client.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/secrets/test_client.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/secrets/test_importing.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/secrets/test_importing.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/test_api_tutorial_scripts.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/test_api_tutorial_scripts.py`

 * *Files 14% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
 @pytest.mark.slow
 def test_quickstart(capsys, _examples_dir):
     command = f"{PYTHON_EXECUTABLE} {_examples_dir}/quickstart.py"
     result_status = run_command(command, shell=True, stdout=True)
     captured = capsys.readouterr()
 
-    expected_output = "Hello Orquestra!"
+    expected_output = "('Hello Orquestra!',)"
 
     assert result_status, (
         f"Process {command} did not complete successfully."
         + "=" * 80
         + f"\nSTDOUT:\n{captured.out}"
         + "=" * 80
         + f"\nSTDERR:\n{captured.err}"
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/test_artifact_future_methods.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/test_artifact_future_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import typing as t
 
 import pytest
 
 import orquestra.sdk as sdk
 from orquestra.sdk import exceptions
 from orquestra.sdk._base import _workflow
-from orquestra.sdk._base._dsl import DEFAULT_IMAGE, ArtifactFuture
+from orquestra.sdk._base._dsl import ArtifactFuture
 
 _TaskResourcesArgs = t.TypedDict(
     "_TaskResourcesArgs",
     {
         "cpu": t.Optional[str],
         "memory": t.Optional[str],
         "disk": t.Optional[str],
@@ -318,15 +318,15 @@
         assert len(set(invocation.task_id for invocation in invocations)) == 1
 
         assert invocations[0].resources is not None
         assert invocations[0].resources.dict() == TASK_RESOURCES_EXPECTED
         assert invocations[0].custom_image == CUSTOM_IMAGE_NOT_DEFAULT["custom_image"]
 
         assert invocations[1].resources is None
-        assert invocations[1].custom_image is DEFAULT_IMAGE
+        assert invocations[1].custom_image is None
 
     @staticmethod
     def test_artifact_with_resources_workflow_model():
         """Check that the resources assignment is done properly
         and there is a correct amount of tasks, task_invocations and
         artifact futures
         """
@@ -355,15 +355,15 @@
         assert len(wf_model.artifact_nodes) == 2
 
         invocations = [*wf_model.task_invocations.values()]
         assert len(set(invocation.task_id for invocation in invocations)) == 1
         assert invocations[0].custom_image == CUSTOM_IMAGE_NOT_DEFAULT["custom_image"]
 
         assert invocations[1].resources == invocations[0].resources
-        assert invocations[1].custom_image == DEFAULT_IMAGE
+        assert invocations[1].custom_image is None
 
     @staticmethod
     def test_artifact_with_resources_and_custom_image_workflow_model():
         """Check that the resources and custom mage assignment is done properly
         and there is a correct amount of tasks, task_invocations and
         artifact futures
         """
@@ -375,8 +375,8 @@
         invocations = [*wf_model.task_invocations.values()]
         assert len(set(invocation.task_id for invocation in invocations)) == 1
         assert invocations[0].resources is not None
         assert invocations[0].resources.dict() == TASK_RESOURCES_EXPECTED
         assert invocations[0].custom_image == CUSTOM_IMAGE_NOT_DEFAULT["custom_image"]
 
         assert invocations[1].resources is None
-        assert invocations[1].custom_image is DEFAULT_IMAGE
+        assert invocations[1].custom_image is None
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/test_ast.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/test_ast.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/test_config.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/test_config.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/test_constant_nodes_serialization.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/test_constant_nodes_serialization.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/test_dispatch.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/test_dispatch_integration.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/test_dispatch_integration.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/test_dsl.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/test_dsl.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,36 +185,14 @@
 def test_task_no_linenumber_if_source_inaccessible():
     task_no_source.__code__ = task_no_source.__code__.replace(co_filename="fake")
     local_task = _dsl.task(task_no_source)
     assert isinstance(local_task._fn_ref, _dsl.ModuleFunctionRef)
     assert local_task._fn_ref.line_number is None
 
 
-def test_external_file_task_calling():
-    external_task = _dsl.external_file_task(
-        file_path="hello/there.py",
-        function="general_kenobi",
-        repo_url="example.com/obi-wan",
-        n_outputs=1,
-    )
-    with pytest.raises(ValueError):
-        external_task._TaskDef__sdk_task_body()
-
-
-def test_external_module_task_calling():
-    external_task = _dsl.external_module_task(
-        module="orquestra.hello.there",
-        function="general_kenobi",
-        repo_url="example.com/obi-wan",
-        n_outputs=1,
-    )
-    with pytest.raises(ValueError):
-        external_task._TaskDef__sdk_task_body()
-
-
 @pytest.mark.parametrize("num_outputs", [1, 100, 2])
 def test_returning_multiple_outputs_from_tasks(num_outputs):
     @sdk.task(n_outputs=num_outputs)
     def _local_task():
         return ("hello" for _ in range(num_outputs))
 
     futures = [f for f in _local_task()]
@@ -238,26 +216,14 @@
     with pytest.raises(ValueError):
 
         @sdk.task(n_outputs=num_outputs)
         def _local_task():
             return "hello", "there"
 
 
-def test_external_tasks_warn_empty_n_outputs():
-    with pytest.warns(UserWarning):
-        _dsl.external_file_task(
-            file_path="./hello.py", repo_url="example.com", function="hello"
-        )
-
-    with pytest.warns(UserWarning):
-        _dsl.external_module_task(
-            module="orquestra.sdk", repo_url="example.com", function="hello"
-        )
-
-
 def test_accessing_deprecated_n_outputs():
     @sdk.task
     def _local_task():
         return 0, 1
 
     with pytest.warns(DeprecationWarning):
         assert _local_task.n_outputs == _local_task._output_metadata.n_outputs == 2
@@ -346,36 +312,32 @@
     with pytest.raises(TypeError):
         results[index]
 
 
 def test_resourced_task_with_custom_gpu_image():
     @sdk.task(
         resources=_dsl.Resources("1000m", "1Gi", "10Gi", "1"),
-        custom_image=_dsl.GPU_IMAGE,
+        custom_image="zapatacomputing/custom_image_not_real",
     )
     def _local_task():
         return "hello"
 
     hello = _local_task()
-    assert hello.invocation.task._custom_image == _dsl.GPU_IMAGE
-
-
-def test_resourced_task_with_default_gpu_image():
-    future = _resourced_task()
-
-    assert future.invocation.task._custom_image == _dsl.GPU_IMAGE
+    assert (
+        hello.invocation.task._custom_image == "zapatacomputing/custom_image_not_real"
+    )
 
 
 def test_task_with_default_image():
     @sdk.task()
     def _local_task():
         return "hello"
 
     hello = _local_task()
-    assert hello.invocation.task._custom_image == _dsl.DEFAULT_IMAGE
+    assert hello.invocation.task._custom_image is None
 
 
 @pytest.fixture
 def my_fake_repo_setup(tmp_path):
     """Setup a fake repo containing a commit."""
 
     repo_dir = tmp_path / "non-repo"
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/test_env.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/test_env.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/test_git_url_utils.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/test_git_url_utils.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/test_graphs.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/test_graphs.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/test_in_process_runtime.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/test_in_process_runtime.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 from datetime import datetime, timedelta, timezone
 from unittest.mock import create_autospec
 
 import pytest
 
 from orquestra import sdk
 from orquestra.sdk import exceptions
+from orquestra.sdk._base import serde
 from orquestra.sdk._base._in_process_runtime import InProcessRuntime
 from orquestra.sdk._base._testing._example_wfs import wf_with_secrets
 from orquestra.sdk.schema import ir
-from orquestra.sdk.schema.workflow_run import State, WorkflowRunId
+from orquestra.sdk.schema.workflow_run import ProjectRef, State, WorkflowRunId
 from orquestra.sdk.secrets import _client, _models
 
 from .data.complex_serialization.workflow_defs import (
     wf_pass_callables_from_task,
     wf_pass_tuple,
 )
 
@@ -68,43 +69,45 @@
     tmp_default_config_json, monkeypatch: pytest.MonkeyPatch, runtime: InProcessRuntime
 ):
     mocked_secret = _models.SecretDefinition(name="a-secret", value="mocked")
     get_secret = create_autospec(_client.SecretsClient.get_secret)
     get_secret.return_value = mocked_secret
     monkeypatch.setattr(_client.SecretsClient, "get_secret", get_secret)
 
-    run_id = runtime.create_workflow_run(wf_with_secrets().model)
+    run_id = runtime.create_workflow_run(wf_with_secrets().model, None)
     result = runtime.get_workflow_run_outputs_non_blocking(run_id)
 
-    assert result == "Mocked"
+    assert result == (serde.result_from_artifact("Mocked", ir.ArtifactFormat.AUTO),)
 
 
 class TestQueriesAfterRunning:
     """
     Submits a well-known workflow and tests the "query" methods.
     """
 
     @staticmethod
     @pytest.fixture
     def run_id(runtime: InProcessRuntime, wf_def) -> WorkflowRunId:
-        run_id = runtime.create_workflow_run(wf_def)
+        run_id = runtime.create_workflow_run(wf_def, None)
         return run_id
 
     class TestGetWorkflowRunOutputs:
         @staticmethod
         def test_output_values(runtime, run_id):
-            assert runtime.get_workflow_run_outputs_non_blocking(run_id) == 3
+            assert runtime.get_workflow_run_outputs_non_blocking(run_id) == (
+                serde.result_from_artifact(3, ir.ArtifactFormat.AUTO),
+            )
 
         @staticmethod
         def test_multiple_runs(runtime):
             wf_def1 = wf_pass_tuple().model
             wf_def2 = wf_pass_callables_from_task().model
 
-            run_id1 = runtime.create_workflow_run(wf_def1)
-            run_id2 = runtime.create_workflow_run(wf_def2)
+            run_id1 = runtime.create_workflow_run(wf_def1, None)
+            run_id2 = runtime.create_workflow_run(wf_def2, None)
 
             outputs1 = runtime.get_workflow_run_outputs_non_blocking(run_id1)
             outputs2 = runtime.get_workflow_run_outputs_non_blocking(run_id2)
 
             assert run_id1 != run_id2
             assert outputs1 != outputs2
 
@@ -112,42 +115,46 @@
         @staticmethod
         def test_single_task_output(runtime, run_id):
             """
             The 'run_id' fixture is a result of submitting a workflow def with a
             single-output task.
             """
             assert runtime.get_available_outputs(run_id) == {
-                "invocation-0-task-sum-tuple-numbers": (3,)
+                "invocation-0-task-sum-tuple-numbers": serde.result_from_artifact(
+                    3, ir.ArtifactFormat.AUTO
+                )
             }
 
         class TestMultipleTaskOutputs:
             @staticmethod
-            # See ticket: https://zapatacomputing.atlassian.net/browse/ORQSDK-695
-            @pytest.mark.xfail(reason="Some artifact IDs are missing for TaskInvoation")
             def test_some_unused(runtime, wf_def_unused_outputs):
-                run_id = runtime.create_workflow_run(wf_def_unused_outputs)
+                run_id = runtime.create_workflow_run(wf_def_unused_outputs, None)
 
                 assert runtime.get_available_outputs(run_id) == {
-                    "invocation-0-task-two-outputs": (6, 4)
+                    "invocation-0-task-two-outputs": serde.result_from_artifact(
+                        (6, 4), ir.ArtifactFormat.AUTO
+                    ),
                 }
 
             @staticmethod
             def test_all_used(runtime, wf_def_all_used):
-                run_id = runtime.create_workflow_run(wf_def_all_used)
+                run_id = runtime.create_workflow_run(wf_def_all_used, None)
 
                 assert runtime.get_available_outputs(run_id) == {
-                    "invocation-0-task-two-outputs": (6, 4)
+                    "invocation-0-task-two-outputs": serde.result_from_artifact(
+                        (6, 4), ir.ArtifactFormat.AUTO
+                    ),
                 }
 
 
 class TestStop:
     @staticmethod
     def test_existing_run(runtime, wf_def):
         # Given
-        run_id = runtime.create_workflow_run(wf_def)
+        run_id = runtime.create_workflow_run(wf_def, None)
 
         # When
         runtime.stop_workflow_run(run_id)
 
         # Then
         # Not much. We expect the above to be a noop.
 
@@ -162,64 +169,64 @@
             runtime.stop_workflow_run(run_id)
 
 
 class TestListWorkflowRuns:
     @staticmethod
     def test_happy_path(runtime, wf_def):
         # Given
-        _ = runtime.create_workflow_run(wf_def)
-        _ = runtime.create_workflow_run(wf_def)
+        _ = runtime.create_workflow_run(wf_def, None)
+        _ = runtime.create_workflow_run(wf_def, None)
 
         # When
         wf_runs = runtime.list_workflow_runs()
 
         # Then
         assert len(wf_runs) == 2
 
     @staticmethod
     def test_limit(runtime, wf_def):
         # Given
-        _ = runtime.create_workflow_run(wf_def)
-        _ = runtime.create_workflow_run(wf_def)
+        _ = runtime.create_workflow_run(wf_def, None)
+        _ = runtime.create_workflow_run(wf_def, None)
 
         # When
         wf_runs = runtime.list_workflow_runs(limit=1)
 
         # Then
         assert len(wf_runs) == 1
 
     @staticmethod
     def test_state_running(runtime, wf_def):
         # Given
-        _ = runtime.create_workflow_run(wf_def)
+        _ = runtime.create_workflow_run(wf_def, None)
 
         # When
         wf_runs = runtime.list_workflow_runs(state=State.RUNNING)
 
         # Then
         # It doesn't make sense to get a running workflow from this runtime
         assert len(wf_runs) == 0
 
     @staticmethod
     def test_state_succeeded(runtime, wf_def):
         # Given
-        _ = runtime.create_workflow_run(wf_def)
+        _ = runtime.create_workflow_run(wf_def, None)
 
         # When
         wf_runs = runtime.list_workflow_runs(state=State.SUCCEEDED)
 
         # Then
         # It doesn't make sense to get a running workflow from this runtime
         assert len(wf_runs) == 1
 
     @staticmethod
     def test_max_age(runtime, wf_def):
         # Given
-        run_id = runtime.create_workflow_run(wf_def)
-        _ = runtime.create_workflow_run(wf_def)
+        run_id = runtime.create_workflow_run(wf_def, None)
+        _ = runtime.create_workflow_run(wf_def, None)
         runtime._start_time_store[run_id] = datetime.now(timezone.utc) - timedelta(
             days=1
         )
 
         # When
         wf_runs = runtime.list_workflow_runs(max_age=timedelta(minutes=1))
 
@@ -235,7 +242,15 @@
         [
             InProcessRuntime.from_runtime_configuration,
         ],
     )
     def test_raises(runtime, method):
         with pytest.raises(NotImplementedError):
             method(runtime)
+
+
+def test_project_raises_warning(runtime, wf_def):
+    # Given
+    with pytest.warns(expected_warning=exceptions.UnsupportedRuntimeFeature):
+        _ = runtime.create_workflow_run(
+            wf_def, project=ProjectRef(workspace_id="", project_id="")
+        )
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/test_loader.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/test_loader.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/test_packaging.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/test_packaging.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,111 +1,127 @@
 ################################################################################
 # © Copyright 2022 Zapata Computing Inc.
 ################################################################################
 from unittest.mock import Mock
 
 import pytest
 
-import orquestra.sdk as sdk
-import orquestra.sdk.packaging as packaging
+from orquestra import sdk
+from orquestra.sdk import packaging
+from orquestra.sdk.packaging import _versions
+
+try:
+    import importlib.metadata as metadata  # type: ignore
+except ModuleNotFoundError:
+    import importlib_metadata as metadata  # type: ignore
 
 
 class TestGetInstalledVersion:
     @staticmethod
     def test_successful_call(monkeypatch):
         # Given
-        metadata_version = Mock(return_value="1.2.3")
-        monkeypatch.setattr(packaging.metadata, "version", metadata_version)
+        monkeypatch.setattr(metadata, "version", Mock(return_value="1.2.3"))
         # When
         version = packaging.get_installed_version("some-package")
         # Then
         assert version == "1.2.3"
 
     @staticmethod
     def test_package_not_found(monkeypatch):
         # Given
-        metadata_version = Mock(side_effect=packaging.metadata.PackageNotFoundError)
-        monkeypatch.setattr(packaging.metadata, "version", metadata_version)
+        monkeypatch.setattr(
+            metadata, "version", Mock(side_effect=metadata.PackageNotFoundError)
+        )
         # When
         with pytest.raises(packaging.PackagingError) as exc_info:
             _ = packaging.get_installed_version("some-package")
         # Then
         assert exc_info.match("Package not found: some-package")
 
 
 class TestInstalledImport:
     @staticmethod
     def test_package_found(monkeypatch):
         # Given
-        get_version = Mock(return_value="1.2.3")
-        monkeypatch.setattr(packaging, "get_installed_version", get_version)
+        monkeypatch.setattr(
+            _versions, "get_installed_version", Mock(return_value="1.2.3")
+        )
         # When
         imp = packaging.InstalledImport(package_name="some-package")
         # Then
         assert isinstance(imp, sdk.PythonImports)
         assert len(imp._packages) == 1
         assert imp._packages[0] == "some-package==1.2.3"
 
     @staticmethod
     def test_package_not_found(monkeypatch):
         # Given
-        get_version = Mock(side_effect=packaging.PackagingError("Package not found:"))
-        monkeypatch.setattr(packaging, "get_installed_version", get_version)
+        monkeypatch.setattr(
+            _versions,
+            "get_installed_version",
+            Mock(side_effect=packaging.PackagingError("Package not found:")),
+        )
         # When
         with pytest.raises(packaging.PackagingError) as exc_info:
             _ = packaging.InstalledImport(package_name="some-package")
         # Then
         assert exc_info.match("Package not found:")
 
     @staticmethod
     def test_package_not_found_fallback(monkeypatch):
         # Given
-        get_version = Mock(side_effect=packaging.PackagingError("Package not found:"))
-        monkeypatch.setattr(packaging, "get_installed_version", get_version)
+        monkeypatch.setattr(
+            _versions,
+            "get_installed_version",
+            Mock(side_effect=packaging.PackagingError("Package not found:")),
+        )
         fallback = sdk.GithubImport("zapatacomputing/orquestra-workflow-sdk")
         # When
         imp = packaging.InstalledImport(package_name="some-package", fallback=fallback)
         # Then
         assert imp == fallback
 
     @staticmethod
     def test_package_version_matches(monkeypatch):
         # Given
-        get_version = Mock(return_value="1.2.3")
-        monkeypatch.setattr(packaging, "get_installed_version", get_version)
+        monkeypatch.setattr(
+            _versions, "get_installed_version", Mock(return_value="1.2.3")
+        )
         # When
         imp = packaging.InstalledImport(
             package_name="some-package", version_match="[0-9].[0-9].[0-9]"
         )
         # Then
         assert isinstance(imp, sdk.PythonImports)
         assert len(imp._packages) == 1
         assert imp._packages[0] == "some-package==1.2.3"
 
     @staticmethod
     def test_package_version_does_not_match(monkeypatch):
         # Given
-        get_version = Mock(return_value="1.2.3")
-        monkeypatch.setattr(packaging, "get_installed_version", get_version)
+        monkeypatch.setattr(
+            _versions, "get_installed_version", Mock(return_value="1.2.3")
+        )
         # When
         with pytest.raises(packaging.PackagingError) as exc_info:
             _ = packaging.InstalledImport(
                 package_name="some-package", version_match="xxx"
             )
         # Then
         assert exc_info.match(
             "Package version mismatch: some-package==1.2.3\n"
             'Expected version to match "xxx"'
         )
 
     @staticmethod
     def test_package_version_does_not_match_fallback(monkeypatch):
         # Given
-        get_version = Mock(return_value="1.2.3")
-        monkeypatch.setattr(packaging, "get_installed_version", get_version)
+        monkeypatch.setattr(
+            _versions, "get_installed_version", Mock(return_value="1.2.3")
+        )
         fallback = sdk.GithubImport("zapatacomputing/orquestra-workflow-sdk")
         # When
         imp = packaging.InstalledImport(
             package_name="some-package",
             version_match="xxx",
             fallback=fallback,
         )
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/test_serde.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/test_serde.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,26 @@
 import numpy.testing
 import pytest
 from pydantic.error_wrappers import ValidationError
 
 import orquestra.sdk as sdk
 from orquestra.sdk._base import serde
 from orquestra.sdk.schema import ir
+from orquestra.sdk.schema.responses import JSONResult
 
 ROUNDTRIP_EXAMPLES = [
     None,
     "hello",
     {"foo": "bar"},
     {"foo": "bar", "baz": ["qux", "qux"]},
     {"a_float": 0.123},
+    (1, 2, 3, 4),
+    (1, 2, 3, (1, 2, 3)),
+    {"hello": (1, 2, 3)},
+    ["a", 1, (1, 2, 3)],
 ]
 
 
 def test_sdk_can_be_serialised():
     def sdk_pickle_by_ref():
         sdk
 
@@ -94,14 +99,29 @@
         return "hello there"
 
     serialized = serde.serialize_pickle(fun)
 
     assert fun() == (serde.deserialize_pickle(serialized))()
 
 
+def test_tuple_magic():
+    # Given
+    serialised = serde.result_from_artifact((1, 2, 3), ir.ArtifactFormat.JSON)
+    assert isinstance(serialised, JSONResult)
+
+    # When
+    result_dict = json.loads(serialised.value)
+
+    # Then
+    assert "__tuple__" in result_dict
+    assert result_dict["__tuple__"]
+    assert "__values__" in result_dict
+    assert result_dict["__values__"] == [1, 2, 3]
+
+
 @pytest.mark.parametrize(
     "package_spec, expected",
     [
         (
             ir.PackageSpec(
                 name="package",
                 extras=[],
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/test_task_ast_parsing.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/test_task_ast_parsing.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/test_traversal.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/test_traversal.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 import typing as t
 from contextlib import nullcontext as does_not_raise
 from unittest.mock import Mock
 
 import git
 import pytest
 
-import orquestra.sdk.schema.ir as model
+import orquestra.sdk.schema.ir as ir
 from orquestra.sdk import exceptions, secrets
-from orquestra.sdk._base import _dsl, _traversal, _workflow, serde
+from orquestra.sdk._base import _dsl, _traversal, _workflow, dispatch, serde
+from orquestra.sdk.packaging import _versions
 
 from .data.complex_serialization.workflow_defs import (
     generate_object_with_num,
     generate_simple_callable,
     generate_simple_callables,
     get_object_id,
     get_object_num,
@@ -132,18 +133,23 @@
 
 @_dsl.task
 def pickled(value):
     pass
 
 
 @_dsl.task(n_outputs=2)
-def multi_output():
+def two_outputs():
     pass
 
 
+@_dsl.task
+def three_outputs():
+    return "a", "b", "c"
+
+
 dupe_import = _dsl.GithubImport("zapatacomputing/test")
 
 
 @_dsl.task(source_import=dupe_import, dependency_imports=[dupe_import])
 def duplicate_deps():
     pass
 
@@ -234,40 +240,14 @@
 @_workflow.workflow
 def no_tasks():
     first = "emiliano"
     last = "zapata"
     return [first, last]
 
 
-# Exposing a function from PyPI-available library
-numpy_eye = _dsl.external_module_task(
-    module="numpy",
-    function="eye",
-    repo_url="git@github.com:numpy/numpy.git",
-    n_outputs=1,
-)
-
-
-# Exposing a function that's only available by git checkout
-generate_random_graph_erdos_renyi = _dsl.external_file_task(
-    file_path="src/python/zquantum/core/graph.py",
-    function="generate_random_graph_erdos_renyi",
-    repo_url="https://github.com/zapatacomputing/z-quantum-core",
-    git_ref="dev",
-    n_outputs=1,
-)
-
-
-@_workflow.workflow
-def external_task_usage():
-    graph = generate_random_graph_erdos_renyi(10, 0.2)
-    array = numpy_eye(2, 2)
-    return [graph, array]
-
-
 @_workflow.workflow
 def wf_with_git_deps():
     """Single task invocation. The task's source import is local, but it has a
     git-based dependency.
     """
     graph = generate_graph()
     return [graph]
@@ -298,21 +278,45 @@
 @_workflow.workflow
 def unhashable_constants():
     names = ["emiliano", "zapata"]
     return [join_strings(names)]
 
 
 @_workflow.workflow
-def multiple_task_outputs():
-    a, b = multi_output()
-    _, c = multi_output()
+def two_task_outputs():
+    a, b = two_outputs()
+    _, c = two_outputs()
     return [a, b, c]
 
 
 @_workflow.workflow
+def two_task_outputs_all_used():
+    a, b = two_outputs()
+    return a, b
+
+
+@_workflow.workflow
+def two_task_outputs_packed_returned():
+    packed = two_outputs()
+    a, b = packed
+    return a, b, packed
+
+
+@_workflow.workflow
+def three_task_outputs():
+    foo1, bar1, baz1 = three_outputs()
+    _, bar2, baz2 = three_outputs()
+    foo3, bar3, _ = three_outputs()
+    _, bar4, _ = three_outputs()
+    foo5, _, baz5 = three_outputs()
+
+    return foo1, bar1, baz1, bar2, baz2, foo3, bar3, bar4, foo5, baz5
+
+
+@_workflow.workflow
 def constant_return():
     a = simple_task(1)
     return [42, a]
 
 
 @_workflow.workflow
 def constant_collisions():
@@ -366,15 +370,15 @@
 @_workflow.workflow
 def workflow_with_secret():
     secret = secrets.get("my_secret")
     return simple_task(secret)
 
 
 def _id_from_wf(param):
-    if isinstance(param, (_workflow.WorkflowDef, model.WorkflowDef)):
+    if isinstance(param, (_workflow.WorkflowDef, ir.WorkflowDef)):
         return param.name
 
 
 def _first(iterable):
     return next(iter(iterable))
 
 
@@ -404,35 +408,35 @@
         source_import = wf.imports[task.source_import_id]
 
         assert task.dependency_import_ids is not None
         assert len(task.dependency_import_ids) == 1
         dep_import = wf.imports[task.dependency_import_ids[0]]
 
         # main assertions
-        assert isinstance(source_import, model.LocalImport)
-        assert isinstance(dep_import, model.GitImport)
+        assert isinstance(source_import, ir.LocalImport)
+        assert isinstance(dep_import, ir.GitImport)
 
     def test_setting_invocation_metadata(self):
         # preconditions
         wf = resources_invocation.model
         with_inv_meta, with_task_meta, no_meta = [
             invocation
             for output_id in wf.output_ids
             for invocation in wf.task_invocations.values()
             if output_id in invocation.output_ids
         ]
 
         # main assertions
-        assert with_inv_meta.resources == model.Resources(
+        assert with_inv_meta.resources == ir.Resources(
             cpu="2000m",
             memory="10Gi",
             disk=None,
             gpu=None,
         )
-        assert with_task_meta.resources == model.Resources(
+        assert with_task_meta.resources == ir.Resources(
             cpu="1000m",
             memory=None,
             disk=None,
             gpu=None,
         )
 
         assert no_meta.resources is None
@@ -445,15 +449,15 @@
         assert len(wf.output_ids) == 2
         assert wf.output_ids[0] in wf.constant_nodes
 
     def test_equal_constants_different_types(self):
         wf = constant_collisions.model
         constant_nodes = []
         for constant_node in wf.constant_nodes.values():
-            assert isinstance(constant_node, model.ConstantNodeJSON)
+            assert isinstance(constant_node, ir.ConstantNodeJSON)
             constant_nodes.append(constant_node)
 
         serialised_constants = [con.value for con in constant_nodes]
         assert len(wf.constant_nodes) == 3
         assert "true" in serialised_constants
         assert "1" in serialised_constants
         assert "1.0" in serialised_constants
@@ -494,15 +498,15 @@
         assert len(wf.constant_nodes) == 1
 
     def test_workflow_with_inline(self):
         wf = wf_with_inline.model
 
         assert len(wf.imports) == 1
         (imp,) = wf.imports.values()
-        assert isinstance(imp, model.InlineImport)
+        assert isinstance(imp, ir.InlineImport)
 
         assert len(wf.tasks) == 1
         (task_def,) = wf.tasks.values()
         assert task_def.source_import_id == imp.id
 
     def test_duplicate_deps(self):
         wf = dupe_import_wf.model
@@ -553,26 +557,21 @@
         ),
         (
             multiple_tasks,
             [capitalize, uppercase],
             ["Emiliano", "ZAPATA"],
             does_not_raise(),
         ),
-        (
-            external_task_usage,
-            [generate_random_graph_erdos_renyi, numpy_eye],
-            None,
-            does_not_raise(),
-        ),
         (daisy_chain, [increment], [44], does_not_raise()),
         (wf_with_git_deps, [generate_graph], None, does_not_raise()),
         (arg_test, [task_arg_test], None, does_not_raise()),
         (unhashable_constants, [join_strings], ["emilianozapata"], does_not_raise()),
         (resources_invocation, [capitalize_resourced], None, does_not_raise()),
-        (multiple_task_outputs, [multi_output], None, does_not_raise()),
+        (two_task_outputs, [two_outputs], None, does_not_raise()),
+        (three_task_outputs, [three_outputs], None, does_not_raise()),
         (wf_object_id, [get_object_id], None, does_not_raise()),
         (wf_objects_id, [get_objects_id], None, does_not_raise()),
         (wf_pass_callable, [invoke_callable], [43], does_not_raise()),
         (
             wf_pass_callable_from_task,
             [generate_simple_callable, invoke_callable],
             [43],
@@ -606,21 +605,24 @@
             ["hellohello"],
             pytest.raises(exceptions.WorkflowSyntaxError),
         ),
     ],
     ids=_id_from_wf,
 )
 class TestWorkflowsTasksProperties:
+    @staticmethod
     def test_wf_imports_are_task_imports(
-        self,
         workflow_template: _workflow.WorkflowTemplate,
         task_defs: t.Sequence[_dsl.TaskDef],
         outputs: t.List,
         expectation: ContextManager,
     ):
+        """
+        Import IDs refered from task defs should be part of wf def IR.
+        """
         with expectation:
             wf = workflow_template.model
             wf_import_ids = set(wf.imports.keys())
 
             # refers to tasks embedded inside workflow model
             task_import_ids_embedded = {
                 import_id
@@ -629,59 +631,102 @@
                     task.source_import_id,
                     *(task.dependency_import_ids or []),
                 ]
             }
 
             assert task_import_ids_embedded == wf_import_ids
 
+    @staticmethod
     def test_task_ids_match_invocations(
-        self,
         workflow_template: _workflow.WorkflowTemplate,
         task_defs: t.Sequence[_dsl.TaskDef],
         outputs: t.List,
         expectation: ContextManager,
     ):
+        """
+        Task def referenced from invocation should be part of the workflow def.
+        """
         with expectation:
             wf = workflow_template.model
-            assert set(wf.tasks.keys()) == {
-                invocation.task_id for invocation in wf.task_invocations.values()
-            }
+            task_def_ids = set(wf.tasks.keys())
 
+            for inv in wf.task_invocations.values():
+                assert inv.task_id in task_def_ids
+
+    @staticmethod
     def test_number_of_invocations(
-        self,
         workflow_template: _workflow.WorkflowTemplate,
         task_defs: t.Sequence[_dsl.TaskDef],
         outputs: t.List,
         expectation: ContextManager,
     ):
+        """
+        Number of task defs shouldn't exceed the number of invocations. Reasoning: each
+        task def should be invoked at least once.
+        """
         with expectation:
             wf = workflow_template.model
-            assert len(wf.task_invocations) >= len(wf.tasks)
+            assert len(wf.tasks) <= len(wf.task_invocations)
 
+    @staticmethod
     def test_invocation_outputs_are_unique(
-        self,
         workflow_template: _workflow.WorkflowTemplate,
         task_defs: t.Sequence[_dsl.TaskDef],
         outputs: t.List,
         expectation: ContextManager,
     ):
+        """
+        A given node ID should be only produced by a single task invocation.
+        """
         with expectation:
             wf = workflow_template.model
-            seen_ids: t.Set[model.ArtifactNodeId] = set()
+            seen_ids: t.Set[ir.ArtifactNodeId] = set()
             for invocation in wf.task_invocations.values():
                 assert set(invocation.output_ids).isdisjoint(seen_ids)
                 seen_ids.update(invocation.output_ids)
 
+    @staticmethod
+    def test_n_invocation_outputs_matches_task_def(
+        workflow_template: _workflow.WorkflowTemplate,
+        task_defs: t.Sequence[_dsl.TaskDef],
+        outputs: t.List,
+        expectation: ContextManager,
+    ):
+        """
+        Number of task invocation output IDs should correspond to task def's outputs.
+        """
+        with expectation:
+            wf_def = workflow_template.model
+            for inv in wf_def.task_invocations.values():
+                task_def_model = wf_def.tasks[inv.task_id]
+                task_def_obj = dispatch.locate_fn_ref(task_def_model.fn_ref)
+                # We assume that `fn_ref` points to a @task() decorated function.
+                assert isinstance(task_def_obj, _dsl.TaskDef)
+
+                if task_def_obj._output_metadata.is_subscriptable:
+                    # n + 1 artifacts for n-output task def:
+                    # - one artifact for each output to handle unpacking
+                    # - one artifact overall to handle using non-unpacked future
+                    assert (
+                        len(inv.output_ids)
+                        == task_def_obj._output_metadata.n_outputs + 1
+                    )
+                else:
+                    assert len(inv.output_ids) == 1
+
+    @staticmethod
     def test_no_hanging_inputs(
-        self,
         workflow_template: _workflow.WorkflowTemplate,
         task_defs: t.Sequence[_dsl.TaskDef],
         outputs: t.List,
         expectation: ContextManager,
     ):
+        """
+        Node IDs used as task inputs should point to constants or task outputs.
+        """
         with expectation:
             wf = workflow_template.model
             constant_ids = set(wf.constant_nodes.keys())
             output_ids = {
                 output_id
                 for invocation in wf.task_invocations.values()
                 for output_id in invocation.output_ids
@@ -698,127 +743,143 @@
             kwarg_input_ids = {
                 input_id
                 for invocation in wf.task_invocations.values()
                 for input_id in invocation.kwargs_ids.values()
             }
             assert kwarg_input_ids.issubset(filled_ids)
 
+    @staticmethod
     def test_constants_can_be_read(
-        self,
         workflow_template: _workflow.WorkflowTemplate,
         task_defs: t.Sequence[_dsl.TaskDef],
         outputs: t.List,
         expectation: ContextManager,
     ):
+        """
+        It should be possible to deserialize constant nodes embedded in the IR using
+        ``serde``.
+        """
         with expectation:
             wf = workflow_template.model
             for constant in wf.constant_nodes.values():
                 constant_dict = json.loads(constant.json())
                 _ = serde.value_from_result_dict(constant_dict)
 
+    @staticmethod
     def test_no_hanging_wf_outputs(
-        self,
         workflow_template: _workflow.WorkflowTemplate,
         task_defs: t.Sequence[_dsl.TaskDef],
         outputs: t.List,
         expectation: ContextManager,
     ):
+        """
+        IDs of the workflow output artifacts should be a subset of task invocation
+        output IDs.
+        """
         with expectation:
             wf = workflow_template.model
             task_output_ids = {
                 output_id
                 for invocation in wf.task_invocations.values()
                 for output_id in invocation.output_ids
             }
             assert set(wf.output_ids).issubset(task_output_ids)
 
+    @staticmethod
     def test_local_run(
-        self,
         workflow_template: _workflow.WorkflowTemplate,
         task_defs: t.Sequence[_dsl.TaskDef],
         outputs: t.List,
         expectation: ContextManager,
     ):
+        """
+        Running the workflow in-process should produce the expected outputs.
+        """
         wf = workflow_template
         if outputs:
             assert outputs == wf().local_run()
 
 
-CAPITALIZE_TASK_DEF = model.TaskDef(
+CAPITALIZE_TASK_DEF = ir.TaskDef(
     id=AnyMatchingStr(r"task-capitalize-\w{10}"),
-    fn_ref=model.ModuleFunctionRef(
+    fn_ref=ir.ModuleFunctionRef(
         module="tests.sdk.v2.test_traversal",
         function_name="capitalize",
         file_path="tests/sdk/v2/test_traversal.py",
         line_number=AnyPositiveInt(),
     ),
+    output_metadata=ir.TaskOutputMetadata(is_subscriptable=False, n_outputs=1),
     parameters=[
-        model.TaskParameter(name="text", kind=model.ParameterKind.POSITIONAL_OR_KEYWORD)
+        ir.TaskParameter(name="text", kind=ir.ParameterKind.POSITIONAL_OR_KEYWORD)
     ],
     source_import_id=AnyMatchingStr(r"local-\w{10}"),
-    custom_image=_dsl.DEFAULT_IMAGE,
+    custom_image=None,
 )
 
-CAPITALIZE_INLINE_TASK_DEF = model.TaskDef(
+CAPITALIZE_INLINE_TASK_DEF = ir.TaskDef(
     id=AnyMatchingStr(r"task-capitalize-inline-\w{10}"),
-    fn_ref=model.InlineFunctionRef(
+    fn_ref=ir.InlineFunctionRef(
         function_name="capitalize_inline",
         encoded_function=[AnyMatchingStr(r".*")],  # dont test actual encoding here
     ),
+    output_metadata=ir.TaskOutputMetadata(is_subscriptable=False, n_outputs=1),
     parameters=[
-        model.TaskParameter(name="text", kind=model.ParameterKind.POSITIONAL_OR_KEYWORD)
+        ir.TaskParameter(name="text", kind=ir.ParameterKind.POSITIONAL_OR_KEYWORD)
     ],
     source_import_id=AnyMatchingStr(r"inline-import-\w{1}"),
-    custom_image=_dsl.DEFAULT_IMAGE,
+    custom_image=None,
 )
 
-GIT_TASK_DEF = model.TaskDef(
+GIT_TASK_DEF = ir.TaskDef(
     id=AnyMatchingStr(r"task-git-task-\w{10}"),
-    fn_ref=model.ModuleFunctionRef(
+    fn_ref=ir.ModuleFunctionRef(
         module="tests.sdk.v2.test_traversal",
         function_name="git_task",
         file_path="tests/sdk/v2/test_traversal.py",
         line_number=AnyPositiveInt(),
     ),
+    output_metadata=ir.TaskOutputMetadata(is_subscriptable=False, n_outputs=1),
     parameters=[],
     source_import_id=AnyMatchingStr(r"git-\w{10}_hello"),
-    custom_image=_dsl.DEFAULT_IMAGE,
+    custom_image=None,
 )
 
 
-GENERATE_GRAPH_TASK_DEF = model.TaskDef(
+GENERATE_GRAPH_TASK_DEF = ir.TaskDef(
     id=AnyMatchingStr(r"task-generate-graph-\w{10}"),
-    fn_ref=model.ModuleFunctionRef(
+    fn_ref=ir.ModuleFunctionRef(
         module="tests.sdk.v2.test_traversal",
         function_name="generate_graph",
         file_path="tests/sdk/v2/test_traversal.py",
         line_number=AnyPositiveInt(),
     ),
+    output_metadata=ir.TaskOutputMetadata(is_subscriptable=False, n_outputs=1),
     parameters=[],
     source_import_id=AnyMatchingStr(r"local-\w{10}"),
     dependency_import_ids=[
         AnyMatchingStr(r"git-\w{10}_github_com_zapatacomputing_orquestra_workflow_sdk")
     ],
-    custom_image=_dsl.DEFAULT_IMAGE,
+    custom_image=None,
 )
 
-PYTHON_IMPORTS_MANUAL_TASK_DEF = model.TaskDef(
+PYTHON_IMPORTS_MANUAL_TASK_DEF = ir.TaskDef(
     id=AnyMatchingStr(r"task-python-imports-manual-\w{10}"),
-    fn_ref=model.ModuleFunctionRef(
+    fn_ref=ir.ModuleFunctionRef(
         module="tests.sdk.v2.test_traversal",
         function_name="python_imports_manual",
         file_path="tests/sdk/v2/test_traversal.py",
         line_number=AnyPositiveInt(),
     ),
+    output_metadata=ir.TaskOutputMetadata(is_subscriptable=False, n_outputs=1),
     parameters=[
-        model.TaskParameter(name="text", kind=model.ParameterKind.POSITIONAL_OR_KEYWORD)
+        ir.TaskParameter(name="text", kind=ir.ParameterKind.POSITIONAL_OR_KEYWORD)
     ],
     source_import_id=AnyMatchingStr(r"local-\w{10}"),
     dependency_import_ids=[AnyMatchingStr(r"python-import-\w{10}")],
-    custom_image=_dsl.DEFAULT_IMAGE,
+    custom_image=None,
 )
 
 
 @pytest.mark.parametrize(
     "task_def, has_arg, expected_model",
     [
         (capitalize, True, CAPITALIZE_TASK_DEF),
@@ -878,15 +939,15 @@
     imp = _dsl.GitImportWithAuth(
         repo_url=original_url,
         git_ref=git_ref,
         username=user,
         auth_secret=_dsl.Secret(secret_name),
     )
     imp_model = _traversal._make_import_model(imp)
-    assert isinstance(imp_model, model.GitImport)
+    assert isinstance(imp_model, ir.GitImport)
     assert imp_model.git_ref == git_ref
     assert imp_model.repo_url.original_url == original_url
     assert imp_model.repo_url.user == user
     assert imp_model.repo_url.password is not None
     assert imp_model.repo_url.password.secret_name == secret_name
 
 
@@ -1105,15 +1166,15 @@
     assert len(wf.constant_nodes) == 0
     assert wf.secret_nodes["secret-0"].secret_name == "my_secret"
 
 
 def test_metadata_on_release(monkeypatch: pytest.MonkeyPatch):
     # Given
     mocked_installed_version = Mock(return_value="22.42.0")
-    monkeypatch.setattr(_traversal, "get_installed_version", mocked_installed_version)
+    monkeypatch.setattr(_versions, "get_installed_version", mocked_installed_version)
 
     # When
     wf = workflow().model
 
     # Then
     assert wf.metadata is not None
     assert wf.metadata.sdk_version.major == 22
@@ -1121,15 +1182,15 @@
     assert wf.metadata.sdk_version.patch == 0
     assert not wf.metadata.sdk_version.is_prerelease
 
 
 def test_metadata_on_dev(monkeypatch: pytest.MonkeyPatch):
     # Given
     mocked_installed_version = Mock(return_value="22.42.0.dev1+gitAABBCC.20230101")
-    monkeypatch.setattr(_traversal, "get_installed_version", mocked_installed_version)
+    monkeypatch.setattr(_versions, "get_installed_version", mocked_installed_version)
 
     # When
     wf = workflow().model
 
     # Then
     assert wf.metadata is not None
     assert wf.metadata.sdk_version.major == 22
@@ -1187,13 +1248,94 @@
 
         wf_model = wf_with_default_imports.model
         task_model = list(wf_model.tasks.values())[0]
         assert task_model.dependency_import_ids
         dep_import = wf_model.imports[task_model.dependency_import_ids[0]]
         source_import = wf_model.imports[task_model.source_import_id]
 
-        assert isinstance(dep_import, model.GitImport)
-        assert isinstance(source_import, model.GitImport)
+        assert isinstance(dep_import, ir.GitImport)
+        assert isinstance(source_import, ir.GitImport)
         assert dep_import.git_ref == expectation[0]
         assert dep_import.repo_url.original_url == expectation[1]
         assert source_import.git_ref == expectation[2]
         assert source_import.repo_url.original_url == expectation[3]
+
+
+class TestGraphTraversal:
+    """
+    Unit tests for GraphTraversal class. Contains edge cases identified while
+    integrating with other components.
+    """
+
+    @staticmethod
+    def test_all_used():
+        """
+        In this case the artifact indices were funky.
+        """
+        # Given
+        graph = _traversal.GraphTraversal()
+        futures = _traversal.extract_root_futures(two_task_outputs_all_used())
+
+        # When
+        graph.traverse(futures)
+
+        # Then
+        assert list(graph.artifacts) == [
+            ir.ArtifactNode(
+                id="artifact-0-two-outputs",
+                artifact_index=0,
+            ),
+            ir.ArtifactNode(
+                id="artifact-1-two-outputs",
+                artifact_index=1,
+            ),
+            # We expect a non-unpacked artifact node even though we instanteneously
+            # unpack it to other futures.
+            ir.ArtifactNode(
+                id="artifact-2-two-outputs",
+                artifact_index=None,
+            ),
+        ]
+
+    @staticmethod
+    def test_packed_and_unpacked():
+        # Given
+        graph = _traversal.GraphTraversal()
+        wf = two_task_outputs_packed_returned()
+        futures = _traversal.extract_root_futures(wf)
+
+        # When
+        graph.traverse(futures)
+
+        # Then
+        assert list(graph.artifacts) == [
+            ir.ArtifactNode(
+                id="artifact-0-two-outputs",
+                artifact_index=0,
+            ),
+            ir.ArtifactNode(
+                id="artifact-1-two-outputs",
+                artifact_index=1,
+            ),
+            ir.ArtifactNode(
+                id="artifact-2-two-outputs",
+                artifact_index=None,
+            ),
+        ]
+
+    @staticmethod
+    def test_non_subscriptable_output():
+        # Given
+        graph = _traversal.GraphTraversal()
+        wf = single_invocation()
+        futures = _traversal.extract_root_futures(wf)
+
+        # When
+        graph.traverse(futures)
+
+        # Then
+        assert list(graph.artifacts) == [
+            ir.ArtifactNode(
+                id="artifact-0-capitalize",
+                artifact_index=None,
+            ),
+        ]
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/test_viz.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/test_viz.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     """
     Test boundary: [ir.WorkflowDef]-[_viz.DiGraph]
     """
 
     @staticmethod
     def test_example_nodes_edges():
         """ """
+        aggregate_step_name = "aggregation_step"
         wf_def = sample_wfs.wf(123).model
         graph = _viz.wf_def_graph(wf_def)
 
         assert graph.nodes1 == [
             _viz.Node(
                 id="invocation-0-task-inc",
                 caption=["tests.sdk.v2.sample_wfs.inc():17", "invocation-0-task-inc"],
@@ -34,30 +35,36 @@
                 ],
             ),
             _viz.Node(
                 id="invocation-3-task-add",
                 caption=["tests.sdk.v2.sample_wfs.add():12", "invocation-3-task-add"],
             ),
         ]
+
         assert graph.nodes2 == [
             _viz.Node(id="artifact-0-inc", caption=[]),
             _viz.Node(id="artifact-1-inc-2", caption=[]),
-            _viz.Node(id="artifact-4-integer-division", caption=[]),
             _viz.Node(id="artifact-2-integer-division", caption=[]),
-            _viz.Node(id="artifact-3-add", caption=[]),
+            _viz.Node(id="artifact-3-integer-division", caption=[]),
+            _viz.Node(id="artifact-4-integer-division", caption=[]),
+            _viz.Node(id="artifact-5-add", caption=[]),
             _viz.Node(id="constant-0", caption=["3"]),
             _viz.Node(id="constant-1", caption=["123"]),
             _viz.Node(id="constant-2", caption=["6"]),
+            _viz.Node(id=aggregate_step_name, caption=["outputs"]),
         ]
         assert graph.edges == [
             ("artifact-1-inc-2", "invocation-0-task-inc"),
             ("invocation-0-task-inc", "artifact-0-inc"),
-            ("artifact-2-integer-division", "invocation-1-task-inc-2"),
+            ("artifact-3-integer-division", "invocation-1-task-inc-2"),
             ("invocation-1-task-inc-2", "artifact-1-inc-2"),
             ("constant-1", "invocation-2-task-integer-division"),
             ("constant-0", "invocation-2-task-integer-division"),
-            ("invocation-2-task-integer-division", "artifact-4-integer-division"),
             ("invocation-2-task-integer-division", "artifact-2-integer-division"),
-            ("artifact-4-integer-division", "invocation-3-task-add"),
+            ("invocation-2-task-integer-division", "artifact-3-integer-division"),
+            ("invocation-2-task-integer-division", "artifact-4-integer-division"),
+            ("artifact-2-integer-division", "invocation-3-task-add"),
             ("constant-2", "invocation-3-task-add"),
-            ("invocation-3-task-add", "artifact-3-add"),
+            ("invocation-3-task-add", "artifact-5-add"),
+            ("artifact-5-add", aggregate_step_name),
+            ("artifact-0-inc", aggregate_step_name),
         ]
```

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/test_workflow.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/test_workflow.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/test_workflow_ast_parsing.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/test_workflow_ast_parsing.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/typing/full_example.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/typing/full_example.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/typing/test_typing.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/typing/test_typing.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/sdk/v2/typing/workflow/assign_model.py` & `orquestra-sdk-0.47.0/tests/sdk/v2/typing/workflow/assign_model.py`

 * *Files identical despite different names*

### Comparing `orquestra-sdk-0.46.0/tests/workflow/test_generating_schema.py` & `orquestra-sdk-0.47.0/tests/workflow/test_generating_schema.py`

 * *Files identical despite different names*

