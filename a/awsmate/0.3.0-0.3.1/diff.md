# Comparing `tmp/awsmate-0.3.0.tar.gz` & `tmp/awsmate-0.3.1.tar.gz`

## Comparing `awsmate-0.3.0.tar` & `awsmate-0.3.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 awsmate-0.3.0/.readthedocs.yaml
--rw-r--r--   0        0        0     5489 2020-02-02 00:00:00.000000 awsmate-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 awsmate-0.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 awsmate-0.3.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 awsmate-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 awsmate-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 awsmate-0.3.0/.github/workflows/tests.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/requirements.txt
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/apigateway.rst
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/awsmate.rst
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/changelog.rst
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/code_of_conduct.rst
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/conf.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/contributing.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/eventbridge.rst
--rw-r--r--   0        0        0    12601 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/example_application.rst
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/genindex.rst
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/index.rst
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/lambdafunction.rst
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/logger.rst
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/readme.rst
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/release_process.rst
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/s3.rst
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/testing.rst
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/_static/flyout.js
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/_static/theme.css
--rwxr-xr-x   0        0        0     1607 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/_templates/layout.html
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/check_terraform
--rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/deploy.sh
--rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/undeploy.sh
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/variables.tfvars
--rwxr-xr-x   0        0        0     1102 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/src/lambda_apigateway_returns_403.py
--rwxr-xr-x   0        0        0     1808 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/src/lambda_apigateway_returns_500.py
--rwxr-xr-x   0        0        0     3738 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/src/lambda_apigateway_returns_okay.py
--rwxr-xr-x   0        0        0      465 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/src/lambda_eventbridge_scheduler.py
--rwxr-xr-x   0        0        0      394 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/src/lambda_logger.py
--rwxr-xr-x   0        0        0      742 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/src/lambda_s3_notification.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/00-provider.tf
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/00-variables.tf
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/01-lambda-iam-role.tf
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/02-awsmate-lambda-layer.tf
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/03-apigateway-lambda-functions.tf
--rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/04-apigateway.tf
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/05-eventbridge-lambda-functions.tf
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/06-eventbridge-iam-role.tf
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/07-eventbridge-scheduler.tf
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/08-s3-bucket.tf
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/09-s3-lambda-functions.tf
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/10-logger-lambda-functions.tf
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 awsmate-0.3.0/src/awsmate/__init__.py
--rw-r--r--   0        0        0    52826 2020-02-02 00:00:00.000000 awsmate-0.3.0/src/awsmate/apigateway.py
--rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 awsmate-0.3.0/src/awsmate/eventbridge.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 awsmate-0.3.0/src/awsmate/lambdafunction.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 awsmate-0.3.0/src/awsmate/logger.py
--rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 awsmate-0.3.0/src/awsmate/s3.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 awsmate-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0    34262 2020-02-02 00:00:00.000000 awsmate-0.3.0/tests/unit/test_apigateway.py
--rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 awsmate-0.3.0/tests/unit/test_eventbridge.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 awsmate-0.3.0/tests/unit/test_lambdafunction.py
--rw-r--r--   0        0        0    15684 2020-02-02 00:00:00.000000 awsmate-0.3.0/tests/unit/test_s3.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 awsmate-0.3.0/.gitignore
--rw-r--r--   0        0        0    13827 2020-02-02 00:00:00.000000 awsmate-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 awsmate-0.3.0/README.md
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 awsmate-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 awsmate-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 awsmate-0.3.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     6137 2020-02-02 00:00:00.000000 awsmate-0.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 awsmate-0.3.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 awsmate-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 awsmate-0.3.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 awsmate-0.3.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 awsmate-0.3.1/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/requirements.txt
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/apigateway.rst
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/awsmate.rst
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/changelog.rst
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/code_of_conduct.rst
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/conf.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/contributing.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/eventbridge.rst
+-rw-r--r--   0        0        0    12611 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/example_application.rst
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/genindex.rst
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/index.rst
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/lambdafunction.rst
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/logger.rst
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/readme.rst
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/release_process.rst
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/s3.rst
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/testing.rst
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/_static/flyout.js
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/_static/theme.css
+-rwxr-xr-x   0        0        0     1607 2020-02-02 00:00:00.000000 awsmate-0.3.1/docs/source/_templates/layout.html
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/check_terraform
+-rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/deploy.sh
+-rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/undeploy.sh
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/variables.tfvars
+-rwxr-xr-x   0        0        0     1102 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/src/lambda_apigateway_returns_403.py
+-rwxr-xr-x   0        0        0     1808 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/src/lambda_apigateway_returns_500.py
+-rwxr-xr-x   0        0        0     3738 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/src/lambda_apigateway_returns_okay.py
+-rwxr-xr-x   0        0        0      465 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/src/lambda_eventbridge_scheduler.py
+-rwxr-xr-x   0        0        0      394 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/src/lambda_logger.py
+-rwxr-xr-x   0        0        0      742 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/src/lambda_s3_notification.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/00-provider.tf
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/00-variables.tf
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/01-lambda-iam-role.tf
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/02-awsmate-lambda-layer.tf
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/03-apigateway-lambda-functions.tf
+-rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/04-apigateway.tf
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/05-eventbridge-lambda-functions.tf
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/06-eventbridge-iam-role.tf
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/07-eventbridge-scheduler.tf
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/08-s3-bucket.tf
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/09-s3-lambda-functions.tf
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 awsmate-0.3.1/example/tf/10-logger-lambda-functions.tf
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 awsmate-0.3.1/src/awsmate/__init__.py
+-rw-r--r--   0        0        0    52826 2020-02-02 00:00:00.000000 awsmate-0.3.1/src/awsmate/apigateway.py
+-rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 awsmate-0.3.1/src/awsmate/eventbridge.py
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 awsmate-0.3.1/src/awsmate/lambdafunction.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 awsmate-0.3.1/src/awsmate/logger.py
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 awsmate-0.3.1/src/awsmate/s3.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 awsmate-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0    34262 2020-02-02 00:00:00.000000 awsmate-0.3.1/tests/unit/test_apigateway.py
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 awsmate-0.3.1/tests/unit/test_eventbridge.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 awsmate-0.3.1/tests/unit/test_lambdafunction.py
+-rw-r--r--   0        0        0    15684 2020-02-02 00:00:00.000000 awsmate-0.3.1/tests/unit/test_s3.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 awsmate-0.3.1/.gitignore
+-rw-r--r--   0        0        0    13827 2020-02-02 00:00:00.000000 awsmate-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 awsmate-0.3.1/README.md
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 awsmate-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 awsmate-0.3.1/PKG-INFO
```

### Comparing `awsmate-0.3.0/CHANGELOG.md` & `awsmate-0.3.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,46 @@
 All notable changes to this project are documented in this file.
 
+## [0.3.1] - 2023-04-28
+
+### Added
+
+*nothing*
+
+### Changed
+
+- Example application
+    - Terraform version upgrade
+
+- Documentation
+    - wording
+    - README structure
+
+### Deprecated
+
+*nothing*
+
+### Removed
+
+*nothing*
+
+### Fixed
+
+- Code
+    - ``awsmate.lambdafunction.LambdaEvent.__init__()``: fixed error message if passed parameter is not a ``dict``
+    - ``awsmate.s3.LambdaNotificationEvent.object_url()``: fixed missing return type hint
+
+- Documentation
+    - example application: protected `curl` URLs with quotes so that the shell does not interpret `&`
+    - example application: fixed typos in some example URLs
+
+### Security
+
+*nothing*
+
 ## [0.3.0] - 2023-04-17
 
 ### Added
 
 - Code
     - added class ``awsmate.apigateway.HttpServerError``
     - added class ``awsmate.apigateway.HttpError``, which is the base class of ``awsmate.apigateway.HttpClientError`` and ``awsmate.apigateway.HttpServerError``
```

### Comparing `awsmate-0.3.0/CODE_OF_CONDUCT.md` & `awsmate-0.3.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/CONTRIBUTING.md` & `awsmate-0.3.1/CONTRIBUTING.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 ## Did you write a patch that fixes a bug?
 
 * Open a new GitHub pull request with the patch.
 
 * Ensure the PR description clearly describes the problem and solution. Include the relevant issue number if applicable.
 
-* Before submitting, feel free to [open a discussion](https://github.com/shlublu/awsmate/discussions/new/choose "new discussion on awsmate forum") to let us know about your patch, or to ask any question you would like.
+* Before submitting, feel free to [open a discussion](https://github.com/shlublu/awsmate/discussions/new/choose "new discussion on awsmate board") to let us know about your patch, or to ask any question you would like.
 
 ## Did you fix whitespace, format code, or make some refactoring?
 
 Such changes are welcome! Please just let us know why this change would be an improvement by filling the PR description.
 
 ## Do you intend to add a new feature or change an existing one?
 
-* Suggest your change in the [discussion forum](https://github.com/shlublu/awsmate/discussions/new?category=ideas "new idea on awsmate forum").
+* Suggest your change in the [discussion board](https://github.com/shlublu/awsmate/discussions/new?category=ideas "new idea on awsmate board").
 
 * After having collected some feedback, feel free to [open a precise feature request](https://github.com/shlublu/awsmate/issues/new?assignees=&labels=&template=feature_request.md&title= "new feature request on awsmate bugtracker").
 
 ## Do you have questions about the source code or the use of the library?
 
-* Ask any question you would like in [the discussion forum](https://github.com/shlublu/awsmate/discussions/new/choose "new discussion on awsmate forum").
+* Ask any question you would like in [the discussion board](https://github.com/shlublu/awsmate/discussions/new/choose "new discussion on awsmate board").
 
 ## Do you want to contribute to the documentation?
 
 You are very welcome! Please proceed the same way as described above for bug fixing an features requests.
 
 Thank you so much!
```

### Comparing `awsmate-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md` & `awsmate-0.3.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/.github/workflows/tests.yaml` & `awsmate-0.3.1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/docs/source/apigateway.rst` & `awsmate-0.3.1/docs/source/apigateway.rst`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/docs/source/conf.py` & `awsmate-0.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/docs/source/example_application.rst` & `awsmate-0.3.1/docs/source/example_application.rst`

 * *Files 0% similar despite different names*

```diff
@@ -109,16 +109,16 @@
 
 * Use
 
     The ``<endpoint_url>`` placeholder below need replacing by the actual value returned by ``./deploy.sh``, as seen in :ref:`section "Deployment" <Deployment>` above.
 
     * Route "okay": ``lambda_apigateway_returns_okay.py``
         * Command-line with ``curl`` 
-            * ``curl -v -X <method> https://<endpoint_url>/okay/<any path>?<any url parameter>=<any value> --data '<any JSON payload>' --header '<any name>: <any value>'`` 
-            * Example: ``curl -v -X POST https://<endpoint_url>/okay/lets/go?someParam=someValue --data '{ "someKey": 42 }' --header 'X-example: 42'``
+            * ``curl -v -X <method> 'https://<endpoint_url>/okay/<any path>?<any url parameter>=<any value>' --data '<any JSON payload>' --header '<any name>: <any value>'`` 
+            * Example: ``curl -v -X POST 'https://<endpoint_url>/okay/lets/go?someParam=someValue' --data '{ "someKey": 42 }' --header 'X-example: 42'``
             * Returns 200 with a JSON payload that contains the result of all methods of ``awsmate.apigateway.LambdaProxyEvent`` plus the raw event received from AWS API Gateway.
             * Demonstrates
                 * the use of all methods of :class:`awsmate.apigateway.LambdaProxyEvent`,
                 * the use of the HTTP response builder :func:`awsmate.apigateway.build_http_response`
             * Tip: play with the ``Accept`` and ``Accept-Encoding`` headers, play with the routes, play with the URL parameters
         * With a web browser
             * ``https://<endpoint_url>/okay/<any path>?<any url parameter>=<any value>``
@@ -129,30 +129,30 @@
                 * the use of the ``custom_transformers`` (here: HTML transformation of the API response) described in :doc:`the apigateway module documentation <apigateway>`,
                 * the use of ``extra_headers`` (here: to handle CORS) with :func:`awsmate.apigateway.build_http_response`,
                 * the ``gzip`` built-in functionality of :func:`awsmate.apigateway.build_http_response` based on the ``Accept-Encoding`` header (unless your browser does not accept gzip!),
                 * the handling of preferences submitted through ``Accept*`` headers in `weighted quality value syntax <https://developer.mozilla.org/en-US/docs/Web/HTTP/Content_negotiation>`_.
             * Tip: think of how you could localize the returned content depending on the ``Accept-Language`` header submitted by the browser
     * Route "forbidden": ``lambda_apigateway_returns_403.py``
         * Command-line with ``curl`` 
-            * ``curl -v -X GET https://<endpoint_url>/forbidden' --header '<any name>: <any value>'`` 
-            * Example: ``curl -v -X GET https://<endpoint_url>/forbidden``
+            * ``curl -v -X GET 'https://<endpoint_url>/forbidden' --header '<any name>: <any value>'`` 
+            * Example: ``curl -v -X GET 'https://<endpoint_url>/forbidden'``
             * Returns 403 with a JSON payload that explains the access is forbidden
             * Logs an error message in AWS Cloudwatch. See :ref:`section "Logger features" <LoggerFeatures>` below for further details.
             * Demonstrates
                 * the use of the HTTP response builder :func:`awsmate.apigateway.build_http_client_error_response`
         * With a web browser
             * ``https://<endpoint_url>/forbidden``
             * Example: ``https://<endpoint_url>/forbidden``
             * Returns an HTML page that is an HTML transformation of the JSON payload described in the command-line example just above.
             * Demonstrates 
                 * the same of the above plus the same extras seen with the "okay" route above
     * Route "crash": ``lambda_apigateway_returns_500.py``
         * Command-line with ``curl`` 
-            * ``curl -v -X GET https://<endpoint_url>/crash' --header '<any name>: <any value>'`` 
-            * Example: ``curl -v -X GET https://<endpoint_url>/crash``
+            * ``curl -v -X GET 'https://<endpoint_url>/crash' --header '<any name>: <any value>'`` 
+            * Example: ``curl -v -X GET 'https://<endpoint_url>/crash'``
             * Returns 500 with a JSON payload explaining that an internal error occurred
             * Logs a complete stack trace of this crash in AWS Cloudwatch. See :ref:`section "Logger features" <LoggerFeatures>` below for further details.
             * Demonstrates
                 * the use of the HTTP response builder :func:`awsmate.apigateway.build_http_server_error_response` 
                 * how not to reveal the cause of the crash to the end user (which would be a security breach) while logging it for debugging purposes
         * With a web browser
             * ``https://<endpoint_url>/crash``
```

### Comparing `awsmate-0.3.0/docs/source/release_process.rst` & `awsmate-0.3.1/docs/source/release_process.rst`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
    * ``/src/awsmate/__init.py__``: ``__version__ = 'x.y.z'``
    * ``Changelog``: new empty section
 * Set the project's development status classifier in ``/pyproject.toml``
 * ...do the job...
 * ...test the job...
 * Update the changelog, including the release date
 * PR and merge into master
+* checkout/pull master and delete dev branch
 * Set commit tag
 * PyPi release: as per https://packaging.python.org/en/latest/tutorials/packaging-projects/
    * python3 -m pip install --upgrade build
    * python3 -m build
    * python3 -m pip install --upgrade twine
    * python3 -m twine upload dist/awsmate-<x.y.z>* (use __token__)
 * Readthedocs: maintain versions (help in https://docs.readthedocs.io/en/stable/tutorial/)
```

### Comparing `awsmate-0.3.0/docs/source/_static/flyout.js` & `awsmate-0.3.1/docs/source/_static/flyout.js`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/docs/source/_templates/layout.html` & `awsmate-0.3.1/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/example/check_terraform` & `awsmate-0.3.1/example/check_terraform`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 }
 
 notSupportedArch () {
   echo >&1 "Sorry, Terraform $TERRAFORM_VERSION is unlikely to be available for this architecture."
   exit 1
 }
 
-TERRAFORM_VERSION='1.4.4'
+TERRAFORM_VERSION='1.4.5'
 
 BUILD_DIR='.build'
 
 EXE_EXT=''
 OS_PART=''
 ARCH_PART=''
```

### Comparing `awsmate-0.3.0/example/src/lambda_apigateway_returns_403.py` & `awsmate-0.3.1/example/src/lambda_apigateway_returns_403.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/example/src/lambda_apigateway_returns_500.py` & `awsmate-0.3.1/example/src/lambda_apigateway_returns_500.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/example/src/lambda_apigateway_returns_okay.py` & `awsmate-0.3.1/example/src/lambda_apigateway_returns_okay.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/example/src/lambda_s3_notification.py` & `awsmate-0.3.1/example/src/lambda_s3_notification.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/example/tf/01-lambda-iam-role.tf` & `awsmate-0.3.1/example/tf/01-lambda-iam-role.tf`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/example/tf/03-apigateway-lambda-functions.tf` & `awsmate-0.3.1/example/tf/03-apigateway-lambda-functions.tf`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/example/tf/04-apigateway.tf` & `awsmate-0.3.1/example/tf/04-apigateway.tf`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/example/tf/05-eventbridge-lambda-functions.tf` & `awsmate-0.3.1/example/tf/05-eventbridge-lambda-functions.tf`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/example/tf/06-eventbridge-iam-role.tf` & `awsmate-0.3.1/example/tf/06-eventbridge-iam-role.tf`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/example/tf/08-s3-bucket.tf` & `awsmate-0.3.1/example/tf/08-s3-bucket.tf`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/example/tf/09-s3-lambda-functions.tf` & `awsmate-0.3.1/example/tf/09-s3-lambda-functions.tf`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/example/tf/10-logger-lambda-functions.tf` & `awsmate-0.3.1/example/tf/10-logger-lambda-functions.tf`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/src/awsmate/apigateway.py` & `awsmate-0.3.1/src/awsmate/apigateway.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/src/awsmate/eventbridge.py` & `awsmate-0.3.1/src/awsmate/eventbridge.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/src/awsmate/lambdafunction.py` & `awsmate-0.3.1/src/awsmate/lambdafunction.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,11 +47,11 @@
         --------
         >>> def lambda_handler(raw_event, context):
         >>>     from awsmate.lambdafunction import LambdaEvent
         >>>     event = LambdaEvent(raw_event)                
         """
         
         if not isinstance(event_object, dict):
-            raise TypeError(f"eventObject should be a dict. Here: {str(type(event_object))}.")
+            raise TypeError(f"event_object should be a dict. Here: {str(type(event_object))}.")
 
         self._event = event_object
```

### Comparing `awsmate-0.3.0/src/awsmate/logger.py` & `awsmate-0.3.1/src/awsmate/logger.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/src/awsmate/s3.py` & `awsmate-0.3.1/src/awsmate/s3.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         >>> event.objet_etag()
         '8b38dac3b5c48c44704ec934eabae5a2'
         """
         
         return self._object_structure().get('eTag', None)
     
 
-    def object_url(self):
+    def object_url(self) -> str:
         """
         Returns the complete URL of the S3 object that is the subject of this notification.
 
         The returned value is URL decoded.
 
         Returns
         -------
```

### Comparing `awsmate-0.3.0/tests/unit/test_apigateway.py` & `awsmate-0.3.1/tests/unit/test_apigateway.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/tests/unit/test_eventbridge.py` & `awsmate-0.3.1/tests/unit/test_eventbridge.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/tests/unit/test_lambdafunction.py` & `awsmate-0.3.1/tests/unit/test_lambdafunction.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,8 +36,8 @@
 
 def test_LambdaEvent_init_raisesIfEventObjectIsNotADict():
     event = "not a dict"
 
     with pytest.raises(TypeError) as exceptionInfo:
         lf.LambdaEvent(event) # type: ignore
 
-    assert exceptionInfo.value.args[0] == f"eventObject should be a dict. Here: {str(type(event))}."
+    assert exceptionInfo.value.args[0] == f"event_object should be a dict. Here: {str(type(event))}."
```

### Comparing `awsmate-0.3.0/tests/unit/test_s3.py` & `awsmate-0.3.1/tests/unit/test_s3.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/LICENSE.txt` & `awsmate-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `awsmate-0.3.0/README.md` & `awsmate-0.3.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,97 +1,124 @@
-00000000: 6061 7773 6d61 7465 6020 6973 2061 2063  `awsmate` is a c
-00000010: 6f6d 7061 6e69 6f6e 2066 6f72 2079 6f75  ompanion for you
-00000020: 7220 4157 5320 6465 7665 6c6f 706d 656e  r AWS developmen
-00000030: 7473 2069 6e20 5079 7468 6f6e 2e0a 4974  ts in Python..It
-00000040: 2070 726f 7669 6465 7320 796f 7520 7769   provides you wi
-00000050: 7468 2068 656c 7065 7220 636f 6465 2074  th helper code t
-00000060: 6861 7420 6661 6369 6c69 7461 7465 7320  hat facilitates 
-00000070: 7468 6520 7573 6520 6f66 2076 6172 696f  the use of vario
-00000080: 7573 2041 5753 2073 6572 7669 6365 732e  us AWS services.
-00000090: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
-000000a0: 6e0a 0a2a 2043 6f6d 6d61 6e64 206c 696e  n..* Command lin
-000000b0: 653a 2060 7069 7033 2069 6e73 7461 6c6c  e: `pip3 install
-000000c0: 2061 7773 6d61 7465 600a 2a20 5b50 7950   awsmate`.* [PyP
-000000d0: 4920 7061 6765 5d28 6874 7470 733a 2f2f  I page](https://
-000000e0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-000000f0: 2f61 7773 6d61 7465 2f20 2261 7773 6d61  /awsmate/ "awsma
-00000100: 7465 2050 7950 4920 7061 6765 2229 0a0a  te PyPI page")..
-00000110: 2323 2044 6f63 756d 656e 7461 7469 6f6e  ## Documentation
-00000120: 0a0a 5468 6520 636f 6d70 6c65 7465 2064  ..The complete d
-00000130: 6f63 756d 656e 7461 7469 6f6e 2069 7320  ocumentation is 
-00000140: 6176 6169 6c61 626c 6520 6174 205b 5265  available at [Re
-00000150: 6164 5468 6544 6f63 735d 2868 7474 7073  adTheDocs](https
-00000160: 3a2f 2f61 7773 6d61 7465 2e72 6561 6474  ://awsmate.readt
-00000170: 6865 646f 6373 2e69 6f2f 2022 6177 736d  hedocs.io/ "awsm
-00000180: 6174 6520 646f 6375 6d65 6e74 6174 696f  ate documentatio
-00000190: 6e22 292e 0a0a 446f 6375 6d65 6e74 6174  n")...Documentat
-000001a0: 696f 6e20 7374 6174 7573 3a20 5b21 5b44  ion status: [![D
-000001b0: 6f63 756d 656e 7461 7469 6f6e 2073 7461  ocumentation sta
-000001c0: 7475 735d 2868 7474 7073 3a2f 2f72 6561  tus](https://rea
-000001d0: 6474 6865 646f 6373 2e6f 7267 2f70 726f  dthedocs.org/pro
-000001e0: 6a65 6374 732f 6177 736d 6174 652f 6261  jects/awsmate/ba
-000001f0: 6467 652f 3f76 6572 7369 6f6e 3d6c 6174  dge/?version=lat
-00000200: 6573 7429 5d28 6874 7470 733a 2f2f 6177  est)](https://aw
-00000210: 736d 6174 652e 7265 6164 7468 6564 6f63  smate.readthedoc
-00000220: 732e 696f 2f65 6e2f 6c61 7465 7374 2f3f  s.io/en/latest/?
-00000230: 6261 6467 653d 6c61 7465 7374 290a 0a23  badge=latest)..#
-00000240: 2320 4578 616d 706c 6520 6170 706c 6963  # Example applic
-00000250: 6174 696f 6e0a 0a41 6e20 6578 616d 706c  ation..An exampl
-00000260: 6520 6170 706c 6963 6174 696f 6e20 6973  e application is
-00000270: 2061 7661 696c 6162 6c65 2074 6f20 6465   available to de
-00000280: 6d6f 6e73 7472 6174 6520 7468 6520 6d61  monstrate the ma
-00000290: 696e 2066 6561 7475 7265 7320 6f66 2074  in features of t
-000002a0: 6869 7320 6c69 6272 6172 792e 2049 7420  his library. It 
-000002b0: 6973 2064 6f63 756d 656e 7465 6420 5b69  is documented [i
-000002c0: 6e20 7468 6973 2063 6861 7074 6572 5d28  n this chapter](
-000002d0: 6874 7470 733a 2f2f 6177 736d 6174 652e  https://awsmate.
-000002e0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-000002f0: 6e2f 6c61 7465 7374 2f65 7861 6d70 6c65  n/latest/example
-00000300: 5f61 7070 6c69 6361 7469 6f6e 2e68 746d  _application.htm
-00000310: 6c29 2e0a 0a23 2320 4973 7375 6573 0a0a  l)...## Issues..
-00000320: 5368 6f75 6c64 2079 6f75 2065 6e63 6f75  Should you encou
-00000330: 6e74 6572 2061 6e79 2062 7567 206f 7220  nter any bug or 
-00000340: 7072 6f62 6c65 6d20 6f66 2061 6e79 206b  problem of any k
-00000350: 696e 642c 2070 6c65 6173 6520 6665 656c  ind, please feel
-00000360: 2066 7265 6520 746f 206f 7065 6e20 616e   free to open an
-00000370: 2069 7373 7565 2061 6363 6f72 6469 6e67   issue according
-00000380: 2074 6f20 6f75 7220 5b63 6f6e 7472 6962   to our [contrib
-00000390: 7574 696f 6e20 6775 6964 656c 696e 6573  ution guidelines
-000003a0: 5d28 6874 7470 733a 2f2f 6177 736d 6174  ](https://awsmat
-000003b0: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
-000003c0: 2f65 6e2f 6c61 7465 7374 2f63 6f6e 7472  /en/latest/contr
-000003d0: 6962 7574 696e 672e 6874 6d6c 292e 0a0a  ibuting.html)...
-000003e0: 5465 7374 7320 7374 6174 7573 3a20 215b  Tests status: ![
-000003f0: 7465 7374 7320 7374 6174 7573 5d28 6874  tests status](ht
-00000400: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000410: 2f73 686c 7562 6c75 2f61 7773 6d61 7465  /shlublu/awsmate
-00000420: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000430: 7773 2f74 6573 7473 2e79 616d 6c2f 6261  ws/tests.yaml/ba
-00000440: 6467 652e 7376 673f 6272 616e 6368 3d6d  dge.svg?branch=m
-00000450: 6173 7465 7229 0a0a 2323 204c 6963 656e  aster)..## Licen
-00000460: 7365 0a0a 5468 6973 2070 726f 6a65 6374  se..This project
-00000470: 2069 7320 6c69 6365 6e73 6564 2075 6e64   is licensed und
-00000480: 6572 2074 6865 2045 5552 4f50 4541 4e20  er the EUROPEAN 
-00000490: 554e 494f 4e20 5055 424c 4943 204c 4943  UNION PUBLIC LIC
-000004a0: 454e 4345 2028 4555 504c 2920 762e 2031  ENCE (EUPL) v. 1
-000004b0: 2e32 2c20 7768 6963 6820 6973 2063 6f6d  .2, which is com
-000004c0: 7061 7469 626c 6520 7769 7468 2074 6865  patible with the
-000004d0: 206d 616a 6f72 6974 7920 6f66 206f 7065   majority of ope
-000004e0: 6e20 736f 7572 6365 206c 6963 656e 6365  n source licence
-000004f0: 732e 0a0a 2a20 5b56 6965 7720 616c 6c20  s...* [View all 
-00000500: 7472 616e 736c 6174 696f 6e73 5d28 6874  translations](ht
-00000510: 7470 733a 2f2f 6a6f 696e 7570 2e65 632e  tps://joinup.ec.
-00000520: 6575 726f 7061 2e65 752f 636f 6c6c 6563  europa.eu/collec
-00000530: 7469 6f6e 2f65 7570 6c2f 6575 706c 2d74  tion/eupl/eupl-t
-00000540: 6578 742d 6575 706c 2d31 3220 2254 7261  ext-eupl-12 "Tra
-00000550: 6e73 6c61 7469 6f6e 7320 6f66 2074 6865  nslations of the
-00000560: 2045 5550 4c2d 312e 3222 290a 2a20 5b4f   EUPL-1.2").* [O
-00000570: 5349 2043 6f6d 7061 7469 6269 6c69 7479  SI Compatibility
-00000580: 206d 6174 7269 785d 2868 7474 7073 3a2f   matrix](https:/
-00000590: 2f6a 6f69 6e75 702e 6563 2e65 7572 6f70  /joinup.ec.europ
-000005a0: 612e 6575 2f63 6f6c 6c65 6374 696f 6e2f  a.eu/collection/
-000005b0: 6575 706c 2f6d 6174 7269 782d 6575 706c  eupl/matrix-eupl
-000005c0: 2d63 6f6d 7061 7469 626c 652d 6f70 656e  -compatible-open
-000005d0: 2d73 6f75 7263 652d 6c69 6365 6e63 6573  -source-licences
-000005e0: 2022 436f 6d70 6174 6962 696c 6974 7920   "Compatibility 
-000005f0: 6d61 7472 6978 206f 6620 7468 6520 4555  matrix of the EU
-00000600: 504c 2d31 2e32 2229 0a                   PL-1.2").
+00000000: 5b21 5b56 6572 7369 6f6e 5d28 6874 7470  [![Version](http
+00000010: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000020: 696f 2f70 7970 692f 762f 6177 736d 6174  io/pypi/v/awsmat
+00000030: 6529 5d28 6874 7470 733a 2f2f 7079 7069  e)](https://pypi
+00000040: 2e6f 7267 2f70 726f 6a65 6374 2f61 7773  .org/project/aws
+00000050: 6d61 7465 2f20 2250 726f 6a65 6374 2070  mate/ "Project p
+00000060: 6167 6520 2d20 5079 5049 2229 0a5b 215b  age - PyPI").[![
+00000070: 5079 7468 6f6e 5d28 6874 7470 733a 2f2f  Python](https://
+00000080: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000090: 7970 692f 7079 7665 7273 696f 6e73 2f61  ypi/pyversions/a
+000000a0: 7773 6d61 7465 295d 2868 7474 7073 3a2f  wsmate)](https:/
+000000b0: 2f67 6974 6875 622e 636f 6d2f 7368 6c75  /github.com/shlu
+000000c0: 626c 752f 6177 736d 6174 652f 7472 6565  blu/awsmate/tree
+000000d0: 2f6d 6173 7465 722f 7372 632f 6177 736d  /master/src/awsm
+000000e0: 6174 6520 2253 6f75 7263 6520 636f 6465  ate "Source code
+000000f0: 202d 2047 6974 6875 6222 290a 5b21 5b4c   - Github").[![L
+00000100: 6963 656e 7365 5d28 6874 7470 733a 2f2f  icense](https://
+00000110: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
+00000120: 6974 6875 622f 6c69 6365 6e73 652f 7368  ithub/license/sh
+00000130: 6c75 626c 752f 6177 736d 6174 6529 5d28  lublu/awsmate)](
+00000140: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000150: 6f6d 2f73 686c 7562 6c75 2f61 7773 6d61  om/shlublu/awsma
+00000160: 7465 2f62 6c6f 622f 6d61 7374 6572 2f4c  te/blob/master/L
+00000170: 4943 454e 5345 2e74 7874 2022 4c69 6365  ICENSE.txt "Lice
+00000180: 6e73 6520 2d20 4769 7468 7562 2229 0a5b  nse - Github").[
+00000190: 215b 5465 7374 735d 2868 7474 7073 3a2f  ![Tests](https:/
+000001a0: 2f67 6974 6875 622e 636f 6d2f 7368 6c75  /github.com/shlu
+000001b0: 626c 752f 6177 736d 6174 652f 6163 7469  blu/awsmate/acti
+000001c0: 6f6e 732f 776f 726b 666c 6f77 732f 7465  ons/workflows/te
+000001d0: 7374 732e 7961 6d6c 2f62 6164 6765 2e73  sts.yaml/badge.s
+000001e0: 7667 3f62 7261 6e63 683d 6d61 7374 6572  vg?branch=master
+000001f0: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00000200: 622e 636f 6d2f 7368 6c75 626c 752f 6177  b.com/shlublu/aw
+00000210: 736d 6174 652f 6163 7469 6f6e 7320 2257  smate/actions "W
+00000220: 6f72 6b66 6c6f 7773 202d 2047 6974 6875  orkflows - Githu
+00000230: 6222 290a 5b21 5b44 6f63 756d 656e 7461  b").[![Documenta
+00000240: 7469 6f6e 5d28 6874 7470 733a 2f2f 7265  tion](https://re
+00000250: 6164 7468 6564 6f63 732e 6f72 672f 7072  adthedocs.org/pr
+00000260: 6f6a 6563 7473 2f61 7773 6d61 7465 2f62  ojects/awsmate/b
+00000270: 6164 6765 2f3f 7665 7273 696f 6e3d 6c61  adge/?version=la
+00000280: 7465 7374 295d 2868 7474 7073 3a2f 2f61  test)](https://a
+00000290: 7773 6d61 7465 2e72 6561 6474 6865 646f  wsmate.readthedo
+000002a0: 6373 2e69 6f2f 2022 446f 6375 6d65 6e74  cs.io/ "Document
+000002b0: 6174 696f 6e20 2d20 5265 6164 5468 6544  ation - ReadTheD
+000002c0: 6f63 732e 696f 2229 0a0a 0a60 6177 736d  ocs.io")...`awsm
+000002d0: 6174 6560 2069 7320 6120 636f 6d70 616e  ate` is a compan
+000002e0: 696f 6e20 666f 7220 796f 7572 2041 5753  ion for your AWS
+000002f0: 2064 6576 656c 6f70 6d65 6e74 7320 696e   developments in
+00000300: 2050 7974 686f 6e2e 0a49 7420 7072 6f76   Python..It prov
+00000310: 6964 6573 2079 6f75 2077 6974 6820 6865  ides you with he
+00000320: 6c70 6572 2063 6f64 6520 7468 6174 2066  lper code that f
+00000330: 6163 696c 6974 6174 6573 2074 6865 2075  acilitates the u
+00000340: 7365 206f 6620 7661 7269 6f75 7320 4157  se of various AW
+00000350: 5320 7365 7276 6963 6573 2e0a 0a23 2320  S services...## 
+00000360: 496e 7374 616c 6c61 7469 6f6e 0a0a 2a20  Installation..* 
+00000370: 436f 6d6d 616e 6420 6c69 6e65 3a20 6070  Command line: `p
+00000380: 6970 3320 696e 7374 616c 6c20 6177 736d  ip3 install awsm
+00000390: 6174 6560 0a2a 205b 5079 5049 2070 6167  ate`.* [PyPI pag
+000003a0: 655d 2868 7474 7073 3a2f 2f70 7970 692e  e](https://pypi.
+000003b0: 6f72 672f 7072 6f6a 6563 742f 6177 736d  org/project/awsm
+000003c0: 6174 652f 2022 5079 5049 2070 6167 6522  ate/ "PyPI page"
+000003d0: 290a 0a23 2320 446f 6375 6d65 6e74 6174  )..## Documentat
+000003e0: 696f 6e0a 0a54 6865 2063 6f6d 706c 6574  ion..The complet
+000003f0: 6520 646f 6375 6d65 6e74 6174 696f 6e20  e documentation 
+00000400: 6973 2061 7661 696c 6162 6c65 2061 7420  is available at 
+00000410: 5b52 6561 6454 6865 446f 6373 5d28 6874  [ReadTheDocs](ht
+00000420: 7470 733a 2f2f 6177 736d 6174 652e 7265  tps://awsmate.re
+00000430: 6164 7468 6564 6f63 732e 696f 2f20 2244  adthedocs.io/ "D
+00000440: 6f63 756d 656e 7461 7469 6f6e 202d 2052  ocumentation - R
+00000450: 6561 6454 6865 446f 6373 2e69 6f22 292e  eadTheDocs.io").
+00000460: 0a0a 2323 2045 7861 6d70 6c65 2061 7070  ..## Example app
+00000470: 6c69 6361 7469 6f6e 0a0a 416e 2065 7861  lication..An exa
+00000480: 6d70 6c65 2061 7070 6c69 6361 7469 6f6e  mple application
+00000490: 2069 7320 6176 6169 6c61 626c 6520 746f   is available to
+000004a0: 2064 656d 6f6e 7374 7261 7465 2074 6865   demonstrate the
+000004b0: 206d 6169 6e20 6665 6174 7572 6573 206f   main features o
+000004c0: 6620 7468 6973 206c 6962 7261 7279 2e20  f this library. 
+000004d0: 4974 2069 7320 646f 6375 6d65 6e74 6564  It is documented
+000004e0: 205b 696e 2074 6869 7320 6368 6170 7465   [in this chapte
+000004f0: 725d 2868 7474 7073 3a2f 2f61 7773 6d61  r](https://awsma
+00000500: 7465 2e72 6561 6474 6865 646f 6373 2e69  te.readthedocs.i
+00000510: 6f2f 656e 2f6c 6174 6573 742f 6578 616d  o/en/latest/exam
+00000520: 706c 655f 6170 706c 6963 6174 696f 6e2e  ple_application.
+00000530: 6874 6d6c 292e 0a0a 2323 2049 7373 7565  html)...## Issue
+00000540: 730a 0a53 686f 756c 6420 796f 7520 656e  s..Should you en
+00000550: 636f 756e 7465 7220 616e 7920 6275 6720  counter any bug 
+00000560: 6f72 2070 726f 626c 656d 206f 6620 616e  or problem of an
+00000570: 7920 6b69 6e64 2c20 706c 6561 7365 2066  y kind, please f
+00000580: 6565 6c20 6672 6565 2074 6f20 6f70 656e  eel free to open
+00000590: 2061 6e20 6973 7375 6520 6163 636f 7264   an issue accord
+000005a0: 696e 6720 746f 206f 7572 205b 636f 6e74  ing to our [cont
+000005b0: 7269 6275 7469 6f6e 2067 7569 6465 6c69  ribution guideli
+000005c0: 6e65 735d 2868 7474 7073 3a2f 2f61 7773  nes](https://aws
+000005d0: 6d61 7465 2e72 6561 6474 6865 646f 6373  mate.readthedocs
+000005e0: 2e69 6f2f 656e 2f6c 6174 6573 742f 636f  .io/en/latest/co
+000005f0: 6e74 7269 6275 7469 6e67 2e68 746d 6c29  ntributing.html)
+00000600: 2e0a 0a23 2320 4c69 6365 6e73 650a 0a54  ...## License..T
+00000610: 6869 7320 7072 6f6a 6563 7420 6973 206c  his project is l
+00000620: 6963 656e 7365 6420 756e 6465 7220 7468  icensed under th
+00000630: 6520 4555 524f 5045 414e 2055 4e49 4f4e  e EUROPEAN UNION
+00000640: 2050 5542 4c49 4320 4c49 4345 4e43 4520   PUBLIC LICENCE 
+00000650: 2845 5550 4c29 2076 2e20 312e 322c 2077  (EUPL) v. 1.2, w
+00000660: 6869 6368 2069 7320 636f 6d70 6174 6962  hich is compatib
+00000670: 6c65 2077 6974 6820 7468 6520 6d61 6a6f  le with the majo
+00000680: 7269 7479 206f 6620 6f70 656e 2073 6f75  rity of open sou
+00000690: 7263 6520 6c69 6365 6e63 6573 2e0a 0a2a  rce licences...*
+000006a0: 205b 5669 6577 2061 6c6c 2074 7261 6e73   [View all trans
+000006b0: 6c61 7469 6f6e 735d 2868 7474 7073 3a2f  lations](https:/
+000006c0: 2f6a 6f69 6e75 702e 6563 2e65 7572 6f70  /joinup.ec.europ
+000006d0: 612e 6575 2f63 6f6c 6c65 6374 696f 6e2f  a.eu/collection/
+000006e0: 6575 706c 2f65 7570 6c2d 7465 7874 2d65  eupl/eupl-text-e
+000006f0: 7570 6c2d 3132 2022 5472 616e 736c 6174  upl-12 "Translat
+00000700: 696f 6e73 206f 6620 7468 6520 4555 504c  ions of the EUPL
+00000710: 2d31 2e32 2229 0a2a 205b 4f53 4920 436f  -1.2").* [OSI Co
+00000720: 6d70 6174 6962 696c 6974 7920 6d61 7472  mpatibility matr
+00000730: 6978 5d28 6874 7470 733a 2f2f 6a6f 696e  ix](https://join
+00000740: 7570 2e65 632e 6575 726f 7061 2e65 752f  up.ec.europa.eu/
+00000750: 636f 6c6c 6563 7469 6f6e 2f65 7570 6c2f  collection/eupl/
+00000760: 6d61 7472 6978 2d65 7570 6c2d 636f 6d70  matrix-eupl-comp
+00000770: 6174 6962 6c65 2d6f 7065 6e2d 736f 7572  atible-open-sour
+00000780: 6365 2d6c 6963 656e 6365 7320 2243 6f6d  ce-licences "Com
+00000790: 7061 7469 6269 6c69 7479 206d 6174 7269  patibility matri
+000007a0: 7820 6f66 2074 6865 2045 5550 4c2d 312e  x of the EUPL-1.
+000007b0: 3222 290a                                2").
```

### Comparing `awsmate-0.3.0/pyproject.toml` & `awsmate-0.3.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build" 
 
 [project]
 name = "awsmate"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
     { name="Vincent Poulain (Shlublu)", email="shlublu@yahoo.fr" },
 ]
 description = "A companion for your AWS Python developments."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Intended Audience :: Developers",
     "Development Status :: 3 - Alpha",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)"
 ]
 keywords = ["python", "aws", "aws-apigateway", "aws-eventbridge", "aws-lambda", "aws-s3"]
 
 [project.urls]
 "Repository" = "https://github.com/shlublu/awsmate"
```

### Comparing `awsmate-0.3.0/PKG-INFO` & `awsmate-0.3.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,57 @@
 Metadata-Version: 2.1
 Name: awsmate
-Version: 0.3.0
+Version: 0.3.1
 Summary: A companion for your AWS Python developments.
 Project-URL: Repository, https://github.com/shlublu/awsmate
 Project-URL: Documentation, https://awsmate.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/shlublu/awsmate/issues
 Project-URL: Changelog, https://github.com/shlublu/awsmate/blob/master/CHANGELOG.md
 Author-email: "Vincent Poulain (Shlublu)" <shlublu@yahoo.fr>
 License-File: LICENSE.txt
 Keywords: aws,aws-apigateway,aws-eventbridge,aws-lambda,aws-s3,python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
+[![Version](https://img.shields.io/pypi/v/awsmate)](https://pypi.org/project/awsmate/ "Project page - PyPI")
+[![Python](https://img.shields.io/pypi/pyversions/awsmate)](https://github.com/shlublu/awsmate/tree/master/src/awsmate "Source code - Github")
+[![License](https://img.shields.io/github/license/shlublu/awsmate)](https://github.com/shlublu/awsmate/blob/master/LICENSE.txt "License - Github")
+[![Tests](https://github.com/shlublu/awsmate/actions/workflows/tests.yaml/badge.svg?branch=master)](https://github.com/shlublu/awsmate/actions "Workflows - Github")
+[![Documentation](https://readthedocs.org/projects/awsmate/badge/?version=latest)](https://awsmate.readthedocs.io/ "Documentation - ReadTheDocs.io")
+
+
 `awsmate` is a companion for your AWS developments in Python.
 It provides you with helper code that facilitates the use of various AWS services.
 
 ## Installation
 
 * Command line: `pip3 install awsmate`
-* [PyPI page](https://pypi.org/project/awsmate/ "awsmate PyPI page")
+* [PyPI page](https://pypi.org/project/awsmate/ "PyPI page")
 
 ## Documentation
 
-The complete documentation is available at [ReadTheDocs](https://awsmate.readthedocs.io/ "awsmate documentation").
-
-Documentation status: [![Documentation status](https://readthedocs.org/projects/awsmate/badge/?version=latest)](https://awsmate.readthedocs.io/en/latest/?badge=latest)
+The complete documentation is available at [ReadTheDocs](https://awsmate.readthedocs.io/ "Documentation - ReadTheDocs.io").
 
 ## Example application
 
 An example application is available to demonstrate the main features of this library. It is documented [in this chapter](https://awsmate.readthedocs.io/en/latest/example_application.html).
 
 ## Issues
 
 Should you encounter any bug or problem of any kind, please feel free to open an issue according to our [contribution guidelines](https://awsmate.readthedocs.io/en/latest/contributing.html).
 
-Tests status: ![tests status](https://github.com/shlublu/awsmate/actions/workflows/tests.yaml/badge.svg?branch=master)
-
 ## License
 
 This project is licensed under the EUROPEAN UNION PUBLIC LICENCE (EUPL) v. 1.2, which is compatible with the majority of open source licences.
 
 * [View all translations](https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12 "Translations of the EUPL-1.2")
 * [OSI Compatibility matrix](https://joinup.ec.europa.eu/collection/eupl/matrix-eupl-compatible-open-source-licences "Compatibility matrix of the EUPL-1.2")
```

