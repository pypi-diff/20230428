# Comparing `tmp/kegstandcli-0.3.1.tar.gz` & `tmp/kegstandcli-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kegstandcli-0.3.1.tar", max compression
+gzip compressed data, was "kegstandcli-0.3.2.tar", max compression
```

## Comparing `kegstandcli-0.3.1.tar` & `kegstandcli-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1077 2023-04-23 18:42:25.686572 kegstandcli-0.3.1/LICENSE
--rw-r--r--   0        0        0     6568 2023-04-26 17:38:00.759465 kegstandcli-0.3.1/README.md
--rw-r--r--   0        0        0     1607 2023-04-27 22:50:56.415214 kegstandcli-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-03 20:22:59.696056 kegstandcli-0.3.1/src/kegstandcli/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 20:23:08.893322 kegstandcli-0.3.1/src/kegstandcli/cli/__init__.py
--rw-r--r--   0        0        0    16328 2023-04-12 22:03:29.066576 kegstandcli-0.3.1/src/kegstandcli/cli/__main__.py
--rw-r--r--   0        0        0     3158 2023-04-12 22:03:29.067785 kegstandcli-0.3.1/src/kegstandcli/cli/build.py
--rw-r--r--   0        0        0     1995 2023-04-23 18:42:31.185993 kegstandcli-0.3.1/src/kegstandcli/cli/config.py
--rw-r--r--   0        0        0      154 2023-04-12 22:03:29.068379 kegstandcli-0.3.1/src/kegstandcli/cli/default_lambda.py.tmpl
--rw-r--r--   0        0        0     1887 2023-04-12 22:03:29.068881 kegstandcli-0.3.1/src/kegstandcli/cli/deploy.py
--rw-r--r--   0        0        0     1179 2023-04-25 19:33:46.541089 kegstandcli-0.3.1/src/kegstandcli/cli/new.py
--rw-r--r--   0        0        0      985 2023-04-27 20:31:45.006926 kegstandcli-0.3.1/src/kegstandcli/cli/teardown.py
--rw-r--r--   0        0        0        0 2023-04-03 20:23:36.547617 kegstandcli-0.3.1/src/kegstandcli/infra/__init__.py
--rw-r--r--   0        0        0     2482 2023-04-26 17:37:46.125480 kegstandcli-0.3.1/src/kegstandcli/infra/app.py
--rw-r--r--   0        0        0      275 2023-04-27 20:31:57.718526 kegstandcli-0.3.1/src/kegstandcli/infra/cdk.json
--rw-r--r--   0        0        0        0 2023-04-03 20:23:50.899135 kegstandcli-0.3.1/src/kegstandcli/infra/stacks/__init__.py
--rw-r--r--   0        0        0     4193 2023-04-12 22:03:29.071990 kegstandcli-0.3.1/src/kegstandcli/infra/stacks/lambda_rest_api.py
--rw-r--r--   0        0        0     1491 2023-04-12 22:03:29.073183 kegstandcli-0.3.1/src/kegstandcli/utils.py
--rw-r--r--   0        0        0     7887 1970-01-01 00:00:00.000000 kegstandcli-0.3.1/setup.py
--rw-r--r--   0        0        0     7946 1970-01-01 00:00:00.000000 kegstandcli-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-23 18:42:25.686572 kegstandcli-0.3.2/LICENSE
+-rw-r--r--   0        0        0     6568 2023-04-26 17:38:00.759465 kegstandcli-0.3.2/README.md
+-rw-r--r--   0        0        0     1565 2023-04-27 23:16:18.840238 kegstandcli-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-03 20:22:59.696056 kegstandcli-0.3.2/src/kegstandcli/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-03 20:23:08.893322 kegstandcli-0.3.2/src/kegstandcli/cli/__init__.py
+-rw-r--r--   0        0        0    16328 2023-04-12 22:03:29.066576 kegstandcli-0.3.2/src/kegstandcli/cli/__main__.py
+-rw-r--r--   0        0        0     3158 2023-04-12 22:03:29.067785 kegstandcli-0.3.2/src/kegstandcli/cli/build.py
+-rw-r--r--   0        0        0     1995 2023-04-23 18:42:31.185993 kegstandcli-0.3.2/src/kegstandcli/cli/config.py
+-rw-r--r--   0        0        0      154 2023-04-12 22:03:29.068379 kegstandcli-0.3.2/src/kegstandcli/cli/default_lambda.py.tmpl
+-rw-r--r--   0        0        0     1887 2023-04-12 22:03:29.068881 kegstandcli-0.3.2/src/kegstandcli/cli/deploy.py
+-rw-r--r--   0        0        0     1179 2023-04-25 19:33:46.541089 kegstandcli-0.3.2/src/kegstandcli/cli/new.py
+-rw-r--r--   0        0        0      985 2023-04-27 20:31:45.006926 kegstandcli-0.3.2/src/kegstandcli/cli/teardown.py
+-rw-r--r--   0        0        0        0 2023-04-03 20:23:36.547617 kegstandcli-0.3.2/src/kegstandcli/infra/__init__.py
+-rw-r--r--   0        0        0     2482 2023-04-26 17:37:46.125480 kegstandcli-0.3.2/src/kegstandcli/infra/app.py
+-rw-r--r--   0        0        0      275 2023-04-27 20:31:57.718526 kegstandcli-0.3.2/src/kegstandcli/infra/cdk.json
+-rw-r--r--   0        0        0        0 2023-04-03 20:23:50.899135 kegstandcli-0.3.2/src/kegstandcli/infra/stacks/__init__.py
+-rw-r--r--   0        0        0     4193 2023-04-12 22:03:29.071990 kegstandcli-0.3.2/src/kegstandcli/infra/stacks/lambda_rest_api.py
+-rw-r--r--   0        0        0     1491 2023-04-12 22:03:29.073183 kegstandcli-0.3.2/src/kegstandcli/utils.py
+-rw-r--r--   0        0        0     7887 1970-01-01 00:00:00.000000 kegstandcli-0.3.2/setup.py
+-rw-r--r--   0        0        0     7946 1970-01-01 00:00:00.000000 kegstandcli-0.3.2/PKG-INFO
```

### Comparing `kegstandcli-0.3.1/LICENSE` & `kegstandcli-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.1/README.md` & `kegstandcli-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.1/pyproject.toml` & `kegstandcli-0.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kegstandcli"
-version = "0.3.1"
+version = "0.3.2"
 description = "The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS"
 authors = ["JensRoland <mail@jensroland.com>"]
 license = "MIT"
 repository = "https://github.com/jensroland/kegstand"
 homepage = "https://kegstand.dev"
 readme = "README.md"
 packages = [
@@ -40,12 +40,12 @@
 tomlkit = "^0.11.7"
 xxhash = "^3.2.0"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.2.3"
 pytest = "^7.3.0"
 pytest-subprocess = "^1.5.0"
-sentient-switchblade = {path = "../sentient-switchblade", develop = true}
+sentient-switchblade = "^0.1.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kegstandcli-0.3.1/src/kegstandcli/cli/__main__.py` & `kegstandcli-0.3.2/src/kegstandcli/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.1/src/kegstandcli/cli/build.py` & `kegstandcli-0.3.2/src/kegstandcli/cli/build.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.1/src/kegstandcli/cli/config.py` & `kegstandcli-0.3.2/src/kegstandcli/cli/config.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.1/src/kegstandcli/cli/deploy.py` & `kegstandcli-0.3.2/src/kegstandcli/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.1/src/kegstandcli/cli/new.py` & `kegstandcli-0.3.2/src/kegstandcli/cli/new.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.1/src/kegstandcli/cli/teardown.py` & `kegstandcli-0.3.2/src/kegstandcli/cli/teardown.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.1/src/kegstandcli/infra/app.py` & `kegstandcli-0.3.2/src/kegstandcli/infra/app.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.1/src/kegstandcli/infra/stacks/lambda_rest_api.py` & `kegstandcli-0.3.2/src/kegstandcli/infra/stacks/lambda_rest_api.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.1/src/kegstandcli/utils.py` & `kegstandcli-0.3.2/src/kegstandcli/utils.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.1/setup.py` & `kegstandcli-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'xxhash>=3.2.0,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['keg = kegstandcli.cli.__main__:kegstandcli']}
 
 setup_kwargs = {
     'name': 'kegstandcli',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': "The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS",
     'long_description': '<!-- markdownlint-disable first-line-h1 line-length no-inline-html -->\n<p align="center">\n  <a href="https://kegstand.dev/">\n    <img src="https://kegstand.dev/assets/kegstand-logotype.png" width="540px" alt="Kegstand logo" />\n  </a>\n</p>\n\n<h3 align="center">The Developer\'s Toolbelt For Accelerating <em>Mean Time To Party</em> on AWS</h3>\n<p align="center">created by <a href="https://jensroland.com/">Jens Roland</a> and fueled by a non-zero amount of alcohol</p>\n<p align="center"><a href="https://kegstand.dev/demo">Watch a 3-minute demo</a></p><!-- markdown-link-check-disable-line -->\n\n<br />\n\n## 🥂💃🕺 Welcome to the Party! 🥂💃🕺\n\nKegstand is a free and open-source framework for creating Python APIs and services. It allows you to rapidly build and deploy services on AWS. We all have better things to do than `print(json.dumps(event))` all day long, and Kegstand is here to help you get to the party &mdash; _and into Prod_ &mdash; a lot faster.\n\n**It provides:**\n\n- A CLI tool for creating and deploying your services.\n- A decorator based API abstracting away the boilerplate of Lambda, API Gateway, Cognito, and more.\n- The full power of CDK to define and deploy arbitrary AWS resources with your services.\n\n> _"Experience a streamlined cloud development process, enhanced productivity, and hit that "party" button sooner with Kegstand!"_ > **&mdash; GPT-4, official spokesbot for the Kegstand team**\n\nLearn more on the [Kegstand website](https://kegstand.dev/).\n\n## Prerequisites\n\n- [Python 3.8+](https://www.python.org/downloads/)\n- [Poetry](https://python-poetry.org/docs/#installation) (recommended)\n- An [AWS account](https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/)\n- The [CDK CLI configured on the local machine and initialized on the AWS account](https://docs.aws.amazon.com/cdk/latest/guide/getting_started.html)\n- The AWS CLI [configured with credentials](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html)\n- [Copier](https://copier.readthedocs.io/en/stable/#installation) project scaffolding tool (recommended)\n- [npx](https://docs.npmjs.com/cli/v9/commands/npx) for installing CLI tools (recommended)\n- A well-poured [Belgian style brown ale](https://www.grimbergen.com/)\n\n## Quick start\n\nTo create a service with Kegstand, you\'ll need a Python project with a few dependencies and a folder structure following the Kegstand convention.\n\nYou can create this in a few seconds, either with the Kegstand CLI or using [Copier](https://copier.readthedocs.io/en/stable/#installation).\n\n```shell\n# Using the Kegstand CLI\n> pipx install kegstandcli\n> keg new my-service\n\n# Using Copier\n> copier gh:JensRoland/kegstand-project-template my-service\n```\n\nEither method will create a new project folder called `my-service` containing:\n\n```shell\nmy-service\n├── .gitignore                        # Standard .gitignore file\n├── pyproject.toml                    # Project configuration\n└── src\n    └── api\n        └── resources\n            └── hello\n                └── any.py            # Logic for /hello/\n```\n\nKegstand projects are minimal by design, so a fresh project folder contains just those 3 files. Well, apart from a few empty `__init__.py` gatecrashers, but we can safely ignore those.\n\nTo install the dependencies for the new project:\n\n```shell\n> cd my-service\n> poetry install\n```\n\nFinally, to build and deploy the service to AWS:\n\n```shell\n> poetry run keg deploy\n```\n\nYou should now be able to access the API endpoint at `https://<api-id>.execute-api.<region>.amazonaws.com/prod/hello`.\n\n## Documentation\n\nFor further examples and more advanced usage, see the [official documentation](https://github.com/JensRoland/kegstand/blob/main/docs/index.md).\n\n## Roadmap\n\nHere are some notable changes, fixes and features that are planned for development:\n\n## 0.4.0\n\n- [ ] More content on [kegstand.dev](https://kegstand.dev)\n- [ ] Custom domain names\n- [ ] Maybe simplify the folder structure from `src/api/resources/<resource-name>/<method>.py` to `src/api/<resource-name>.py`\n\n### Pre-1.0.0\n\n- [ ] Specify event triggers for Lambda functions: S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc.\n- [ ] Pagination helper\n- [ ] [Record a screencast](https://asciinema.org/) for the README\n- [ ] Autogenerated docs using [MkDocs](https://www.mkdocs.org/)\n- [ ] GitHub Actions workflow for pushing docs to the website\n\n### 1.0.0\n\n- [ ] Intuitive and mostly automated API Versioning\n- [ ] Simple way to define/override core API/Lambda properties such as CPU/MEM, Python runtime version, warm pool (!), and concurrency\n- [ ] Deploy Lambda-only microservices with no API Gateway\n\n### Future\n\n- [ ] Configurable log level\n- [ ] Add AWS tags in the Kegstand config and they will be applied to the generated resources\n- [ ] Easily add [AWS Lambda Layers](https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html)\n- [ ] Add support for APIs using [FastAPI](https://fastapi.tiangolo.com/) with [Mangum](https://mangum.io/) instead of the default Kegstand API framework, and just provide deployment helpers for the API Gateway and Lambda\n- [ ] Improved output from deploy command; friendly post-deploy instructions for testing your API\n- [ ] Version bumper with [bump2version](https://pypi.org/project/bump2version/)\n- [ ] Include more goodies from [Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/2.11.0/) - tracing, metrics, etc.\n- [ ] Add support for APIs using pure [Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/2.11.0/) instead of the default Kegstand API framework, and just provide deployment helpers for the API Gateway and Lambda\n- [ ] Unit testing helpers (wrap moto and make it all a little more DRY and intuitive)\n- [ ] Secure endpoints which require re-authentication (and/or MFA) so a refreshed token isn’t enough (to, say, delete your account or change your credit card info)\n- [ ] Live Lambda development a la SST\n- [ ] Build and deploy gRPC endpoints (or similar alternative)\n- [ ] Build and deploy GraphQL endpoints\n- [ ] Build and deploy stream processors?\n- [ ] Option to teardown before deploying: `keg deploy --force-redeploy`\n- [ ] Use env vars to populate values in kegstand.toml\n- [ ] Merge Kegstand and Beth into one tool\n- [ ] CDK Pipelines\n- [ ] Support HTTP method-specific files (e.g. `get.py`, `post.py`, etc.)\n- [ ] Upgrade Copier once the [template-deleting bugfix](https://github.com/copier-org/copier/pull/1037) is released\n',
     'author': 'JensRoland',
     'author_email': 'mail@jensroland.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kegstand.dev',
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 'src'} packages = \ ['kegstandcli', 'kegstandcli.cli', 'kegstandcli.infra',
 'kegstandcli.infra.stacks'] package_data = \ {'': ['*']} install_requires = \
 ['aws-cdk-lib>=2.67.0,<3.0.0', 'aws-solutions-constructs-aws-apigateway-
 lambda>=2.36.0,<3.0.0', 'boto3>=1.17.113,<2.0.0', 'click>=8.0.3,<9.0.0',
 'constructs>=10.0.0,<11.0.0', 'copier>=6.2.0,<7.0.0', 'pyjwt>=2.1.0,<3.0.0',
 'tomlkit>=0.11.7,<0.12.0', 'xxhash>=3.2.0,<4.0.0'] entry_points = \
 {'console_scripts': ['keg = kegstandcli.cli.__main__:kegstandcli']}
-setup_kwargs = { 'name': 'kegstandcli', 'version': '0.3.1', 'description': "The
+setup_kwargs = { 'name': 'kegstandcli', 'version': '0.3.2', 'description': "The
 Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS",
 'long_description': '\n
                            \n \n_[Kegstand_logo]\n\n
 \n\n
 **** The Developer\'s Toolbelt For Accelerating Mean Time To Party on AWS ****
 \n
        created by Jens_Roland and fueled by a non-zero amount of alcohol
```

### Comparing `kegstandcli-0.3.1/PKG-INFO` & `kegstandcli-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kegstandcli
-Version: 0.3.1
+Version: 0.3.2
 Summary: The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS
 Home-page: https://kegstand.dev
 License: MIT
 Author: JensRoland
 Author-email: mail@jensroland.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kegstandcli Version: 0.3.1 Summary: The Developer's
+Metadata-Version: 2.1 Name: kegstandcli Version: 0.3.2 Summary: The Developer's
 Toolbelt For Accelerating Mean-Time-To-Party on AWS Home-page: https://
 kegstand.dev License: MIT Author: JensRoland Author-email: mail@jensroland.com
 Requires-Python: >=3.9,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

