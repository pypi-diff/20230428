# Comparing `tmp/dd-import-1.0.8.tar.gz` & `tmp/dd-import-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dd-import-1.0.8.tar", last modified: Wed Jan  4 21:08:33 2023, max compression
+gzip compressed data, was "dd-import-1.0.9.tar", last modified: Thu Feb  2 11:29:41 2023, max compression
```

## Comparing `dd-import-1.0.8.tar` & `dd-import-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 stefanf   (1000) stefanf   (1000)        0 2023-01-04 21:08:32.995262 dd-import-1.0.8/
--rw-r--r--   0 stefanf   (1000) stefanf   (1000)     1476 2023-01-04 17:59:20.000000 dd-import-1.0.8/LICENSE.txt
--rw-r--r--   0 stefanf   (1000) stefanf   (1000)     8376 2023-01-04 21:08:32.995262 dd-import-1.0.8/PKG-INFO
--rw-r--r--   0 stefanf   (1000) stefanf   (1000)     7802 2023-01-04 20:52:48.000000 dd-import-1.0.8/README.md
-drwxr-xr-x   0 stefanf   (1000) stefanf   (1000)        0 2023-01-04 21:08:32.995262 dd-import-1.0.8/dd_import/
--rw-r--r--   0 stefanf   (1000) stefanf   (1000)        0 2023-01-04 17:59:20.000000 dd-import-1.0.8/dd_import/__init__.py
--rw-r--r--   0 stefanf   (1000) stefanf   (1000)    10587 2023-01-04 20:56:03.000000 dd-import-1.0.8/dd_import/dd_api.py
--rw-r--r--   0 stefanf   (1000) stefanf   (1000)      487 2023-01-04 17:59:20.000000 dd-import-1.0.8/dd_import/dd_import_languages.py
--rw-r--r--   0 stefanf   (1000) stefanf   (1000)      637 2023-01-04 17:59:20.000000 dd-import-1.0.8/dd_import/dd_reimport_findings.py
--rw-r--r--   0 stefanf   (1000) stefanf   (1000)     5138 2023-01-04 20:52:48.000000 dd-import-1.0.8/dd_import/environment.py
-drwxr-xr-x   0 stefanf   (1000) stefanf   (1000)        0 2023-01-04 21:08:32.995262 dd-import-1.0.8/dd_import.egg-info/
--rw-r--r--   0 stefanf   (1000) stefanf   (1000)     8376 2023-01-04 21:08:32.000000 dd-import-1.0.8/dd_import.egg-info/PKG-INFO
--rw-r--r--   0 stefanf   (1000) stefanf   (1000)      380 2023-01-04 21:08:32.000000 dd-import-1.0.8/dd_import.egg-info/SOURCES.txt
--rw-r--r--   0 stefanf   (1000) stefanf   (1000)        1 2023-01-04 21:08:32.000000 dd-import-1.0.8/dd_import.egg-info/dependency_links.txt
--rw-r--r--   0 stefanf   (1000) stefanf   (1000)      165 2023-01-04 21:08:32.000000 dd-import-1.0.8/dd_import.egg-info/entry_points.txt
--rw-r--r--   0 stefanf   (1000) stefanf   (1000)       17 2023-01-04 21:08:32.000000 dd-import-1.0.8/dd_import.egg-info/requires.txt
--rw-r--r--   0 stefanf   (1000) stefanf   (1000)       10 2023-01-04 21:08:32.000000 dd-import-1.0.8/dd_import.egg-info/top_level.txt
--rw-r--r--   0 stefanf   (1000) stefanf   (1000)      104 2023-01-04 17:59:20.000000 dd-import-1.0.8/pyproject.toml
--rw-r--r--   0 stefanf   (1000) stefanf   (1000)      951 2023-01-04 21:08:32.995262 dd-import-1.0.8/setup.cfg
+drwxr-xr-x   0 stefanf   (1000) stefanf   (1000)        0 2023-02-02 11:29:41.121962 dd-import-1.0.9/
+-rw-r--r--   0 stefanf   (1000) stefanf   (1000)     1476 2023-01-04 17:59:20.000000 dd-import-1.0.9/LICENSE.txt
+-rw-r--r--   0 stefanf   (1000) stefanf   (1000)     8691 2023-02-02 11:29:41.121962 dd-import-1.0.9/PKG-INFO
+-rw-r--r--   0 stefanf   (1000) stefanf   (1000)     8117 2023-02-02 11:23:28.000000 dd-import-1.0.9/README.md
+drwxr-xr-x   0 stefanf   (1000) stefanf   (1000)        0 2023-02-02 11:29:41.121962 dd-import-1.0.9/dd_import/
+-rw-r--r--   0 stefanf   (1000) stefanf   (1000)        0 2023-01-04 17:59:20.000000 dd-import-1.0.9/dd_import/__init__.py
+-rw-r--r--   0 stefanf   (1000) stefanf   (1000)    10620 2023-02-02 11:23:28.000000 dd-import-1.0.9/dd_import/dd_api.py
+-rw-r--r--   0 stefanf   (1000) stefanf   (1000)      487 2023-01-04 17:59:20.000000 dd-import-1.0.9/dd_import/dd_import_languages.py
+-rw-r--r--   0 stefanf   (1000) stefanf   (1000)      637 2023-01-04 17:59:20.000000 dd-import-1.0.9/dd_import/dd_reimport_findings.py
+-rw-r--r--   0 stefanf   (1000) stefanf   (1000)     5511 2023-02-02 11:23:28.000000 dd-import-1.0.9/dd_import/environment.py
+drwxr-xr-x   0 stefanf   (1000) stefanf   (1000)        0 2023-02-02 11:29:41.121962 dd-import-1.0.9/dd_import.egg-info/
+-rw-r--r--   0 stefanf   (1000) stefanf   (1000)     8691 2023-02-02 11:29:41.000000 dd-import-1.0.9/dd_import.egg-info/PKG-INFO
+-rw-r--r--   0 stefanf   (1000) stefanf   (1000)      380 2023-02-02 11:29:41.000000 dd-import-1.0.9/dd_import.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanf   (1000) stefanf   (1000)        1 2023-02-02 11:29:41.000000 dd-import-1.0.9/dd_import.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanf   (1000) stefanf   (1000)      165 2023-02-02 11:29:41.000000 dd-import-1.0.9/dd_import.egg-info/entry_points.txt
+-rw-r--r--   0 stefanf   (1000) stefanf   (1000)       17 2023-02-02 11:29:41.000000 dd-import-1.0.9/dd_import.egg-info/requires.txt
+-rw-r--r--   0 stefanf   (1000) stefanf   (1000)       10 2023-02-02 11:29:41.000000 dd-import-1.0.9/dd_import.egg-info/top_level.txt
+-rw-r--r--   0 stefanf   (1000) stefanf   (1000)      104 2023-01-04 17:59:20.000000 dd-import-1.0.9/pyproject.toml
+-rw-r--r--   0 stefanf   (1000) stefanf   (1000)      951 2023-02-02 11:29:41.121962 dd-import-1.0.9/setup.cfg
```

### Comparing `dd-import-1.0.8/LICENSE.txt` & `dd-import-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dd-import-1.0.8/PKG-INFO` & `dd-import-1.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: dd-import
-Version: 1.0.8
-Summary: A utility to (re-)import findings and language data into DefectDojo
-Home-page: https://github.com/MaibornWolff/dd-import
-Author: Stefan Fleckenstein
-Author-email: stefan.fleckenstein@maibornwolff.de
-Project-URL: Issue Tracker, https://github.com/MaibornWolff/dd-import/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # dd-import
 
 > A utility to (re-)import findings and language data into [DefectDojo](https://www.defectdojo.org/)
 
 Findings and languages can be imported into DefectDojo via an [API](https://defectdojo.github.io/django-DefectDojo/integrations/api-v2-docs/). To make automated build and deploy pipelines easier to implement, `dd-import` provides some convenience functions:
 
 - Products, engagements and tests will be created if they are not existing. This avoids manual preparation in DefectDojo or complicated steps within the pipeline.
@@ -33,24 +18,24 @@
 
 `dd-import` can be installed with pip. Only Python 3.8 and up is suported.
 
 ```bash
 pip install dd-import
 ```
 
-The command `dd-reimport-findings` re-imports findings into DefectDojo. Even though the name suggests otherwise, you do not need to do an initial import first. 
+The command `dd-reimport-findings` re-imports findings into DefectDojo. Even though the name suggests otherwise, you do not need to do an initial import first.
 
 The command `dd-import-languages` imports languages data that have been gathered with the tool [cloc](https://github.com/AlDanial/cloc), see [Languages and lines of code](https://defectdojo.github.io/django-DefectDojo/integrations/languages/) for more details.
 
 
 **Docker**
 
 Docker images can be found in https://hub.docker.com/r/maibornwolff/dd-import.
 
-A re-import of findings can be started with 
+A re-import of findings can be started with
 
 ```bash
 docker run --rm dd-import:latest dd-reimport-findings.sh
 ```
 
 Importing languages data can be started with
 
@@ -70,16 +55,18 @@
 | Parameter             | Re-import findings | Import languages | Remark |
 |-----------------------|:------------------:|:----------------:|--------|
 | DD_URL                | Mandatory          | Mandatory        | Base URL of the DefectDojo instance |
 | DD_API_KEY            | Mandatory          | Mandatory        | Shall be defined as a secret, eg. a protected variable in GitLab or an encrypted secret in GitHub |
 | DD_PRODUCT_TYPE_NAME  | Mandatory          | Mandatory        | A product type with this name must exist |
 | DD_PRODUCT_NAME       | Mandatory          | Mandatory        | If a product with this name does not exist, it will be created |
 | DD_ENGAGEMENT_NAME    | Mandatory          | -                | If an engagement with this name does not exist for the given product, it will be created |
+| DD_ENGAGEMENT_TARGET_START | Optional    | -                | Format: YYYY-MM-DD, default: `today`. The target start date for a newly created engagement. |
+| DD_ENGAGEMENT_TARGET_END | Optional    | -                | Format: YYYY-MM-DD, default: `2999-12-31`. The target start date for a newly created engagement. |
 | DD_TEST_NAME          | Mandatory          | -                | If a test with this name does not exist for the given engagement, it will be created |
-| DD_TEST_TYPE_NAME     | Mandatory          | -                | From DefectDojo's list of test types, eg. `Trivy Scan` | 
+| DD_TEST_TYPE_NAME     | Mandatory          | -                | From DefectDojo's list of test types, eg. `Trivy Scan` |
 | DD_FILE_NAME          | Optional           | Mandatory        | |
 | DD_ACTIVE             | Optional           | -                | Default: `true` |
 | DD_VERIFIED           | Optional           | -                | Default: `true` |
 | DD_MINIMUM_SEVERITY   | Optional           | -                | |
 | DD_GROUP_BY           | Optional           | -                | Group by file path, component name, component name + version |
 | DD_PUSH_TO_JIRA       | Optional           | -                | Default: `false` |
 | DD_CLOSE_OLD_FINDINGS | Optional           | -                | Default: `true` |
@@ -174,14 +161,14 @@
 
 Another example, showing how to use `dd-import` within a GitHub Action, can be found in [dd-import_example.yml](.github/workflows/dd-import_example.yml).
 
 ## Developer guide
 
 ### Testing
 
-`./bin/runUnitTests.sh` - Runs the unit tests and reports the test coverage. 
+`./bin/runUnitTests.sh` - Runs the unit tests and reports the test coverage.
 
 `./bin/runDockerUnitTests.sh` - First creates the docker image and then starts a docker container in which the unit tests are executed.
 
 ## License
 
 Licensed under the [3-Clause BSD License](LICENSE.txt)
```

### Comparing `dd-import-1.0.8/README.md` & `dd-import-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: dd-import
+Version: 1.0.9
+Summary: A utility to (re-)import findings and language data into DefectDojo
+Home-page: https://github.com/MaibornWolff/dd-import
+Author: Stefan Fleckenstein
+Author-email: stefan.fleckenstein@maibornwolff.de
+Project-URL: Issue Tracker, https://github.com/MaibornWolff/dd-import/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # dd-import
 
 > A utility to (re-)import findings and language data into [DefectDojo](https://www.defectdojo.org/)
 
 Findings and languages can be imported into DefectDojo via an [API](https://defectdojo.github.io/django-DefectDojo/integrations/api-v2-docs/). To make automated build and deploy pipelines easier to implement, `dd-import` provides some convenience functions:
 
 - Products, engagements and tests will be created if they are not existing. This avoids manual preparation in DefectDojo or complicated steps within the pipeline.
@@ -18,24 +33,24 @@
 
 `dd-import` can be installed with pip. Only Python 3.8 and up is suported.
 
 ```bash
 pip install dd-import
 ```
 
-The command `dd-reimport-findings` re-imports findings into DefectDojo. Even though the name suggests otherwise, you do not need to do an initial import first. 
+The command `dd-reimport-findings` re-imports findings into DefectDojo. Even though the name suggests otherwise, you do not need to do an initial import first.
 
 The command `dd-import-languages` imports languages data that have been gathered with the tool [cloc](https://github.com/AlDanial/cloc), see [Languages and lines of code](https://defectdojo.github.io/django-DefectDojo/integrations/languages/) for more details.
 
 
 **Docker**
 
 Docker images can be found in https://hub.docker.com/r/maibornwolff/dd-import.
 
-A re-import of findings can be started with 
+A re-import of findings can be started with
 
 ```bash
 docker run --rm dd-import:latest dd-reimport-findings.sh
 ```
 
 Importing languages data can be started with
 
@@ -55,16 +70,18 @@
 | Parameter             | Re-import findings | Import languages | Remark |
 |-----------------------|:------------------:|:----------------:|--------|
 | DD_URL                | Mandatory          | Mandatory        | Base URL of the DefectDojo instance |
 | DD_API_KEY            | Mandatory          | Mandatory        | Shall be defined as a secret, eg. a protected variable in GitLab or an encrypted secret in GitHub |
 | DD_PRODUCT_TYPE_NAME  | Mandatory          | Mandatory        | A product type with this name must exist |
 | DD_PRODUCT_NAME       | Mandatory          | Mandatory        | If a product with this name does not exist, it will be created |
 | DD_ENGAGEMENT_NAME    | Mandatory          | -                | If an engagement with this name does not exist for the given product, it will be created |
+| DD_ENGAGEMENT_TARGET_START | Optional    | -                | Format: YYYY-MM-DD, default: `today`. The target start date for a newly created engagement. |
+| DD_ENGAGEMENT_TARGET_END | Optional    | -                | Format: YYYY-MM-DD, default: `2999-12-31`. The target start date for a newly created engagement. |
 | DD_TEST_NAME          | Mandatory          | -                | If a test with this name does not exist for the given engagement, it will be created |
-| DD_TEST_TYPE_NAME     | Mandatory          | -                | From DefectDojo's list of test types, eg. `Trivy Scan` | 
+| DD_TEST_TYPE_NAME     | Mandatory          | -                | From DefectDojo's list of test types, eg. `Trivy Scan` |
 | DD_FILE_NAME          | Optional           | Mandatory        | |
 | DD_ACTIVE             | Optional           | -                | Default: `true` |
 | DD_VERIFIED           | Optional           | -                | Default: `true` |
 | DD_MINIMUM_SEVERITY   | Optional           | -                | |
 | DD_GROUP_BY           | Optional           | -                | Group by file path, component name, component name + version |
 | DD_PUSH_TO_JIRA       | Optional           | -                | Default: `false` |
 | DD_CLOSE_OLD_FINDINGS | Optional           | -                | Default: `true` |
@@ -159,14 +176,14 @@
 
 Another example, showing how to use `dd-import` within a GitHub Action, can be found in [dd-import_example.yml](.github/workflows/dd-import_example.yml).
 
 ## Developer guide
 
 ### Testing
 
-`./bin/runUnitTests.sh` - Runs the unit tests and reports the test coverage. 
+`./bin/runUnitTests.sh` - Runs the unit tests and reports the test coverage.
 
 `./bin/runDockerUnitTests.sh` - First creates the docker image and then starts a docker container in which the unit tests are executed.
 
 ## License
 
 Licensed under the [3-Clause BSD License](LICENSE.txt)
```

### Comparing `dd-import-1.0.8/dd_import/dd_api.py` & `dd-import-1.0.9/dd_import/dd_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,16 +96,16 @@
                 print('Engagement found,   id: ', engagement_id)
                 return engagement_id
         return self.new_engagement(product)
 
     def new_engagement(self, product):
         payload = {'name': self.environment.engagement_name,
                    'product': product,
-                   'target_start': datetime.date.today().isoformat(),
-                   'target_end': '2999-12-31',
+                   'target_start': self.environment.engagement_target_start,
+                   'target_end': self.environment.engagement_target_end,
                    'engagement_type': 'CI/CD',
                    'status': 'In Progress'}
         r = requests.post(self.engagement_url,
                           headers=self.headers,
                           data=json.dumps(payload),
                           verify=self.ssl_verification)
         r.raise_for_status()
```

### Comparing `dd-import-1.0.8/dd_import/dd_reimport_findings.py` & `dd-import-1.0.9/dd_import/dd_reimport_findings.py`

 * *Files identical despite different names*

### Comparing `dd-import-1.0.8/dd_import/environment.py` & `dd-import-1.0.9/dd_import/environment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+import datetime
 import os
 from distutils.util import strtobool
 
 
 class Environment:
 
     def __init__(self):
         self.url = os.getenv('DD_URL')
         self.api_key = os.getenv('DD_API_KEY')
         self.product_name = os.getenv('DD_PRODUCT_NAME')
         self.product_type_name = os.getenv('DD_PRODUCT_TYPE_NAME')
         self.engagement_name = os.getenv('DD_ENGAGEMENT_NAME')
+        self.engagement_target_start = os.getenv('DD_ENGAGEMENT_TARGET_START', datetime.date.today().isoformat())
+        self.engagement_target_end = os.getenv('DD_ENGAGEMENT_TARGET_END', '2999-12-31')
         self.test_name = os.getenv('DD_TEST_NAME')
         self.test_type_name = os.getenv('DD_TEST_TYPE_NAME')
         self.file_name = os.getenv('DD_FILE_NAME')
         self.active = os.getenv('DD_ACTIVE', 'True').lower() in ['true']
         self.verified = os.getenv('DD_VERIFIED', 'True').lower() in ['true']
         self.minimum_severity = os.getenv('DD_MINIMUM_SEVERITY', None)
         self.group_by = os.getenv('DD_GROUP_BY', None)
@@ -46,14 +49,16 @@
         if len(error_string) > 0:
             raise Exception(error_string)
 
         print('DD_URL:                       ', self.url)
         print('DD_PRODUCT_TYPE_NAME:         ', self.product_type_name)
         print('DD_PRODUCT_NAME:              ', self.product_name)
         print('DD_ENGAGEMENT_NAME:           ', self.engagement_name)
+        print('DD_ENGAGEMENT_TARGET_START:   ', self.engagement_target_start)
+        print('DD_ENGAGEMENT_TARGET_END:     ', self.engagement_target_end)
         print('DD_TEST_NAME:                 ', self.test_name)
         print('DD_TEST_TYPE_NAME:            ', self.test_type_name)
         print('DD_FILE_NAME:                 ', self.file_name)
         print('DD_ACTIVE:                    ', self.active)
         print('DD_VERIFIED:                  ', self.verified)
         print('DD_MINIMUM_SEVERITY:          ', self.minimum_severity)
         print('DD_GROUP_BY:                  ', self.group_by)
```

### Comparing `dd-import-1.0.8/dd_import.egg-info/PKG-INFO` & `dd-import-1.0.9/dd_import.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dd-import
-Version: 1.0.8
+Version: 1.0.9
 Summary: A utility to (re-)import findings and language data into DefectDojo
 Home-page: https://github.com/MaibornWolff/dd-import
 Author: Stefan Fleckenstein
 Author-email: stefan.fleckenstein@maibornwolff.de
 Project-URL: Issue Tracker, https://github.com/MaibornWolff/dd-import/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -33,24 +33,24 @@
 
 `dd-import` can be installed with pip. Only Python 3.8 and up is suported.
 
 ```bash
 pip install dd-import
 ```
 
-The command `dd-reimport-findings` re-imports findings into DefectDojo. Even though the name suggests otherwise, you do not need to do an initial import first. 
+The command `dd-reimport-findings` re-imports findings into DefectDojo. Even though the name suggests otherwise, you do not need to do an initial import first.
 
 The command `dd-import-languages` imports languages data that have been gathered with the tool [cloc](https://github.com/AlDanial/cloc), see [Languages and lines of code](https://defectdojo.github.io/django-DefectDojo/integrations/languages/) for more details.
 
 
 **Docker**
 
 Docker images can be found in https://hub.docker.com/r/maibornwolff/dd-import.
 
-A re-import of findings can be started with 
+A re-import of findings can be started with
 
 ```bash
 docker run --rm dd-import:latest dd-reimport-findings.sh
 ```
 
 Importing languages data can be started with
 
@@ -70,16 +70,18 @@
 | Parameter             | Re-import findings | Import languages | Remark |
 |-----------------------|:------------------:|:----------------:|--------|
 | DD_URL                | Mandatory          | Mandatory        | Base URL of the DefectDojo instance |
 | DD_API_KEY            | Mandatory          | Mandatory        | Shall be defined as a secret, eg. a protected variable in GitLab or an encrypted secret in GitHub |
 | DD_PRODUCT_TYPE_NAME  | Mandatory          | Mandatory        | A product type with this name must exist |
 | DD_PRODUCT_NAME       | Mandatory          | Mandatory        | If a product with this name does not exist, it will be created |
 | DD_ENGAGEMENT_NAME    | Mandatory          | -                | If an engagement with this name does not exist for the given product, it will be created |
+| DD_ENGAGEMENT_TARGET_START | Optional    | -                | Format: YYYY-MM-DD, default: `today`. The target start date for a newly created engagement. |
+| DD_ENGAGEMENT_TARGET_END | Optional    | -                | Format: YYYY-MM-DD, default: `2999-12-31`. The target start date for a newly created engagement. |
 | DD_TEST_NAME          | Mandatory          | -                | If a test with this name does not exist for the given engagement, it will be created |
-| DD_TEST_TYPE_NAME     | Mandatory          | -                | From DefectDojo's list of test types, eg. `Trivy Scan` | 
+| DD_TEST_TYPE_NAME     | Mandatory          | -                | From DefectDojo's list of test types, eg. `Trivy Scan` |
 | DD_FILE_NAME          | Optional           | Mandatory        | |
 | DD_ACTIVE             | Optional           | -                | Default: `true` |
 | DD_VERIFIED           | Optional           | -                | Default: `true` |
 | DD_MINIMUM_SEVERITY   | Optional           | -                | |
 | DD_GROUP_BY           | Optional           | -                | Group by file path, component name, component name + version |
 | DD_PUSH_TO_JIRA       | Optional           | -                | Default: `false` |
 | DD_CLOSE_OLD_FINDINGS | Optional           | -                | Default: `true` |
@@ -174,14 +176,14 @@
 
 Another example, showing how to use `dd-import` within a GitHub Action, can be found in [dd-import_example.yml](.github/workflows/dd-import_example.yml).
 
 ## Developer guide
 
 ### Testing
 
-`./bin/runUnitTests.sh` - Runs the unit tests and reports the test coverage. 
+`./bin/runUnitTests.sh` - Runs the unit tests and reports the test coverage.
 
 `./bin/runDockerUnitTests.sh` - First creates the docker image and then starts a docker container in which the unit tests are executed.
 
 ## License
 
 Licensed under the [3-Clause BSD License](LICENSE.txt)
```

### Comparing `dd-import-1.0.8/setup.cfg` & `dd-import-1.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dd-import
-version = 1.0.8
+version = 1.0.9
 author = Stefan Fleckenstein
 author_email = stefan.fleckenstein@maibornwolff.de
 description = A utility to (re-)import findings and language data into DefectDojo
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MaibornWolff/dd-import
 project_urls =
```

