# Comparing `tmp/payla_utils-0.2.8.tar.gz` & `tmp/payla_utils-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payla_utils-0.2.8.tar", max compression
+gzip compressed data, was "payla_utils-0.2.9.tar", max compression
```

## Comparing `payla_utils-0.2.8.tar` & `payla_utils-0.2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     5917 2022-12-15 09:48:34.541602 payla_utils-0.2.8/README-public-pypi.md
--rw-r--r--   0        0        0      151 2022-12-15 09:48:34.541602 payla_utils-0.2.8/payla_utils/__init__.py
--rw-r--r--   0        0        0       81 2022-12-15 09:48:34.541602 payla_utils-0.2.8/payla_utils/access/__init__.py
--rw-r--r--   0        0        0      786 2022-12-15 09:48:34.541602 payla_utils-0.2.8/payla_utils/access/decorators.py
--rw-r--r--   0        0        0      148 2022-12-15 09:48:34.541602 payla_utils-0.2.8/payla_utils/apps.py
--rw-r--r--   0        0        0      201 2022-12-15 09:48:34.541602 payla_utils-0.2.8/payla_utils/logging/__init__.py
--rw-r--r--   0        0        0     3447 2022-12-15 09:48:34.541602 payla_utils-0.2.8/payla_utils/logging/default_configuration.py
--rw-r--r--   0        0        0      840 2022-12-15 09:48:34.541602 payla_utils-0.2.8/payla_utils/logging/logformatter.py
--rw-r--r--   0        0        0     4509 2022-12-15 09:48:34.541602 payla_utils-0.2.8/payla_utils/logging/logger.py
--rw-r--r--   0        0        0     2016 2022-12-15 09:48:34.541602 payla_utils-0.2.8/payla_utils/logging/middlewares.py
--rw-r--r--   0        0        0      581 2022-12-15 09:48:34.541602 payla_utils-0.2.8/payla_utils/logging/sentry_logger.py
--rw-r--r--   0        0        0        0 2022-12-15 09:48:34.541602 payla_utils-0.2.8/payla_utils/management/__init__.py
--rw-r--r--   0        0        0        0 2022-12-15 09:48:34.542603 payla_utils-0.2.8/payla_utils/management/commands/__init__.py
--rw-r--r--   0        0        0     2788 2022-12-15 09:48:34.542603 payla_utils-0.2.8/payla_utils/management/commands/init_environment.py
--rw-r--r--   0        0        0      105 2022-12-15 09:48:34.542603 payla_utils-0.2.8/payla_utils/models/__init__.py
--rw-r--r--   0        0        0     1119 2022-12-15 09:48:34.542603 payla_utils-0.2.8/payla_utils/models/base.py
--rw-r--r--   0        0        0    10325 2022-12-15 09:48:34.542603 payla_utils-0.2.8/payla_utils/settings.py
--rw-r--r--   0        0        0     1558 2022-12-15 09:48:34.542603 payla_utils-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     7135 1970-01-01 00:00:00.000000 payla_utils-0.2.8/setup.py
--rw-r--r--   0        0        0     6998 1970-01-01 00:00:00.000000 payla_utils-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     5917 2022-12-21 08:29:52.704095 payla_utils-0.2.9/README-public-pypi.md
+-rw-r--r--   0        0        0      151 2022-12-21 08:29:52.704095 payla_utils-0.2.9/payla_utils/__init__.py
+-rw-r--r--   0        0        0       81 2022-12-21 08:29:52.704095 payla_utils-0.2.9/payla_utils/access/__init__.py
+-rw-r--r--   0        0        0      786 2022-12-21 08:29:52.704095 payla_utils-0.2.9/payla_utils/access/decorators.py
+-rw-r--r--   0        0        0      148 2022-12-21 08:29:52.704095 payla_utils-0.2.9/payla_utils/apps.py
+-rw-r--r--   0        0        0      201 2022-12-21 08:29:52.704095 payla_utils-0.2.9/payla_utils/logging/__init__.py
+-rw-r--r--   0        0        0     3447 2022-12-21 08:29:52.704095 payla_utils-0.2.9/payla_utils/logging/default_configuration.py
+-rw-r--r--   0        0        0      840 2022-12-21 08:29:52.704095 payla_utils-0.2.9/payla_utils/logging/logformatter.py
+-rw-r--r--   0        0        0     4509 2022-12-21 08:29:52.704095 payla_utils-0.2.9/payla_utils/logging/logger.py
+-rw-r--r--   0        0        0     2016 2022-12-21 08:29:52.704095 payla_utils-0.2.9/payla_utils/logging/middlewares.py
+-rw-r--r--   0        0        0      581 2022-12-21 08:29:52.704095 payla_utils-0.2.9/payla_utils/logging/sentry_logger.py
+-rw-r--r--   0        0        0        0 2022-12-21 08:29:52.704095 payla_utils-0.2.9/payla_utils/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-21 08:29:52.704095 payla_utils-0.2.9/payla_utils/management/commands/__init__.py
+-rw-r--r--   0        0        0     2788 2022-12-21 08:29:52.704095 payla_utils-0.2.9/payla_utils/management/commands/init_environment.py
+-rw-r--r--   0        0        0      105 2022-12-21 08:29:52.704095 payla_utils-0.2.9/payla_utils/models/__init__.py
+-rw-r--r--   0        0        0     1906 2022-12-21 08:29:52.704095 payla_utils-0.2.9/payla_utils/models/base.py
+-rw-r--r--   0        0        0    10325 2022-12-21 08:29:52.704095 payla_utils-0.2.9/payla_utils/settings.py
+-rw-r--r--   0        0        0     1558 2022-12-21 08:29:52.705095 payla_utils-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     7135 1970-01-01 00:00:00.000000 payla_utils-0.2.9/setup.py
+-rw-r--r--   0        0        0     6998 1970-01-01 00:00:00.000000 payla_utils-0.2.9/PKG-INFO
```

### Comparing `payla_utils-0.2.8/README-public-pypi.md` & `payla_utils-0.2.9/README-public-pypi.md`

 * *Files identical despite different names*

### Comparing `payla_utils-0.2.8/payla_utils/access/decorators.py` & `payla_utils-0.2.9/payla_utils/access/decorators.py`

 * *Files identical despite different names*

### Comparing `payla_utils-0.2.8/payla_utils/logging/default_configuration.py` & `payla_utils-0.2.9/payla_utils/logging/default_configuration.py`

 * *Files identical despite different names*

### Comparing `payla_utils-0.2.8/payla_utils/logging/logformatter.py` & `payla_utils-0.2.9/payla_utils/logging/logformatter.py`

 * *Files identical despite different names*

### Comparing `payla_utils-0.2.8/payla_utils/logging/logger.py` & `payla_utils-0.2.9/payla_utils/logging/logger.py`

 * *Files identical despite different names*

### Comparing `payla_utils-0.2.8/payla_utils/logging/middlewares.py` & `payla_utils-0.2.9/payla_utils/logging/middlewares.py`

 * *Files identical despite different names*

### Comparing `payla_utils-0.2.8/payla_utils/logging/sentry_logger.py` & `payla_utils-0.2.9/payla_utils/logging/sentry_logger.py`

 * *Files identical despite different names*

### Comparing `payla_utils-0.2.8/payla_utils/management/commands/init_environment.py` & `payla_utils-0.2.9/payla_utils/management/commands/init_environment.py`

 * *Files identical despite different names*

### Comparing `payla_utils-0.2.8/payla_utils/models/base.py` & `payla_utils-0.2.9/payla_utils/models/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,47 @@
+from __future__ import annotations
+
 from typing import Any
 
 from django.db import models
+from django.utils.timezone import now
 from django.utils.translation import gettext_lazy as _
 
 
 class PaylaQuerySet(models.QuerySet):
     """
     This custom QuerySet with get_or_none method
     """
 
-    def get_or_none(self, *args: Any, **kwargs: Any):
+    def get_or_none(self, *args: Any, **kwargs: Any) -> PaylaModel | None:
+        """
+        Use this instead of Queryset.get to either get an object if it exists or
+        None if it doesn't. This is a shortcut to avoid having to catch DoesNotExist
+        exceptions.
+
+        Returns:
+            PaylaModel | None: Either the model if it exists or None if it doesn't.
+        """
         try:
             return self.get(*args, **kwargs)
         except self.model.DoesNotExist:
             return None
 
+    def update(self, *args, **kwargs) -> int:
+        """
+        Override Queryset.update to make sure that modified_at is also updated when
+        performing multi-row updates.
+
+        Returns:
+            int: number of rows updated
+        """
+        if 'modified_at' not in kwargs:
+            kwargs['modified_at'] = now()
+        return super().update(*args, **kwargs)
+
 
 class PaylaModel(models.Model):
     created_at = models.DateTimeField(verbose_name=_('Created At'), auto_now_add=True)
     modified_at = models.DateTimeField(verbose_name=_('Last modified'), auto_now=True)
 
     objects = PaylaQuerySet.as_manager()
```

### Comparing `payla_utils-0.2.8/payla_utils/settings.py` & `payla_utils-0.2.9/payla_utils/settings.py`

 * *Files identical despite different names*

### Comparing `payla_utils-0.2.8/pyproject.toml` & `payla_utils-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "payla-utils"
-version = "0.2.8"
+version = "0.2.9"
 description = "payla_utils python package"
 authors = [
     "Payla Services <tools@payla.de>",
 ]
 readme = "README-public-pypi.md"
 keywords = [
     "payla_utils",
```

### Comparing `payla_utils-0.2.8/setup.py` & `payla_utils-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'python-json-logger>=2.0.0,<3.0.0',
  'sentry-sdk>=1.0',
  'structlog-sentry>=2.0.0,<3.0.0',
  'structlog>=22.3.0,<23.0.0']
 
 setup_kwargs = {
     'name': 'payla-utils',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'payla_utils python package',
     'long_description': '# payla_utils python package\n\n## Features\n\n### Structlog config\n\n#### Example, structlog configuration, django\nin django settings.py\n\n    from payla_utils.logging import LoggingConfigurator\n\n    LoggingConfigurator(\n        \'testapp\',\n        log_level=\'INFO\',\n        own_apps=settings.OWN_APPS,\n        setup_logging_dict=True,\n    ).configure_structlog(formatter=\'plain_console\')\n\n\n#### Example, structlog configuration, passing extra loggers names\nin django settings.py\n\n    from payla_utils.logging import LoggingConfigurator\n\n    LoggingConfigurator(\n        \'testapp\',\n        log_level=\'INFO\',\n        own_apps=settings.OWN_APPS,\n        setup_logging_dict=True,\n    ).configure_structlog(formatter=\'plain_console\', extra_loggers_name=[\'mylogger1\', \'mylogger2\'])\n\n\n#### If you want to use structlog in django celery\n\nin celery.py\n\n    from django.conf import settings\n    from payla_utils.logging import LoggingConfigurator\n\n    @signals.setup_logging.connect\n    def receiver_setup_logging(\n        loglevel, logfile, format, colorize, **kwargs\n    ):  # pragma: no cover\n\n        LoggingConfigurator(\n            \'testapp\',\n            log_level=\'INFO\',\n            own_apps=settings.OWN_APPS,\n            setup_logging_dict=True,\n        ).configure_structlog(formatter=\'plain_console\')\n\n#### If you want to use structlog with Sentry\n\nYou will have to set `PaylaLoggingIntegration` in sentry sdk setup\n\n```python\nsentry_sdk.init(\n    # take sentry DSN from environment or add a default value here:\n    dsn=env.str(\'SENTRY_DSN\'),\n    integrations=[DjangoIntegration(), CeleryIntegration(), PaylaLoggingIntegration()],\n    auto_session_tracking=False,\n    traces_sample_rate=0.01,\n    send_default_pii=True,\n    attach_stacktrace=True,\n    request_bodies=\'medium\',\n    release=PROJECT_VERSION,\n    environment=ENVIRONMENT,\n)\n```\n\n### If you want to use a structlog, not Django based project\n\n    from payla_utils.logging import LoggingConfigurator\n\n    LoggingConfigurator(\n        \'testapp\',\n        log_level=\'INFO\',\n        own_apps=[],\n        setup_logging_dict=True,\n    ).configure_structlog(formatter=\'plain_console\')\n\n\n#### How to use generic structured logger:\n\n    logger = structlog.get_logger(__name__)\n    logger.warning("Here is your message", key_1="value_1", key_2="value_2", key_n="value_n")\n\n\n#### Using request middleware to inject request_id and/or trace_id:\n\nThis middleware will inject reqest_id and/or trace_id to all logs producer during a request/response cycle.\n\n    MIDDLEWARE += [\'payla_utils.logging.middlewares.RequestMiddleware\']\n\n- Pass your custom request id header via the PAYLA_UTILS settings: `REQUEST_ID_HEADER`, defaults to `X-Request-ID`\n- Enable tracing (Only supports opentelemetry) via `configure_structlog(tracing_enabled=True)`\n\n[See configuration section](#Configuration-and-settings)\n\n### Why structured logger\n\n- By default, the logging frameworks outputs the traces in plain text and tools like EFK stack or Grafana Loki can’t fully process these traces.\n- Therefore, if we “structure” or send the traces in JSON format directly, all the tools can benefit of.\n- As a developer, it would be nice to be able to filter all logs by a certain customer or transaction.\n- The goal of structured logging is to solve these sorts of problems and allow additional analytics.\n\n\n- When you log something, remember that the actual consumer is the machine Grafana Loki (EFK stack), not only humans.\n- Our generic logger comes with some default context structure, but as you can see, you can introduce new keys.\n- We use structlog as wraper on standard logging library, you can check for more details [structlog](https://www.structlog.org/en/stable/).\n\n\n## Access decorator\n\nTo prohibit access to only internal IPs for a specific view it\'s possible to use the `only_internal_access` decorator.\n\nSERVER_IP is required to be set on payla_utils settings.\n\n[See configuration section](#Configuration-and-settings)\n\nExample usage\n\n```python\n@only_internal_access\ndef test_view(request):\n    return HttpResponse(\'OK\')\n```\nOr inline\n\n```python\npath(\'test/\', only_internal_access(test_view), name="test-view"),\n```\n\n## Management command to init environment\n\nThis management command will init environment based on the current env (local.dev, dev, stage, playground and prod)\n\n- load fixtures on the first run (when the DB is empty)\n- setup custom theme for admin_interface\n- create user when not in prod if `LOCAL_DJANGO_ADMIN_PASSWORD` is set\n\nAPP_NAME and ENVIRONMENT settings are required. [See configuration section](#Configuration-and-settings)\n\n## Configuration and settings\n\nSettings for Payla Utils are all namespaced in the PAYLA_UTILS setting.\nFor example your project\'s `settings.py` file might look like this:\n\n```python\nPAYLA_UTILS = {\n    \'APP_NAME\': \'My App\',\n    # Used for json logging\n    \'MICROSERVICE_NAME: \'myapp\',\n    # dev, stage, prod ...\n    \'ENVIRONMENT\': ENVIRONMENT,\n    \'INITIAL_FIXTURES\': [\n        os.path.join(BASE_DIR, \'testapp\', \'fixtures\', \'users.json\'),\n    ],\n    \'SERVER_IP\': \'192.168.1.4\',\n    \'REQUEST_ID_HEADER\': \'X-Request-ID\',\n    \'RUN_EXTRA_COMMANDS\': [\'loadinitialusers\', \'setup_something\'],\n    \'LOCAL_DJANGO_ADMIN_PASSWORD\': os.environ.get(\'LOCAL_DJANGO_ADMIN_PASSWORD\', \'admin\'),\n    # Only in case you need to change the defaults\n    \'ENV_THEMES\': {\n        \'local.dev\': {\n            ...\n        },\n        \'dev\': {\n            ...\n        },\n        \'stage\': {\n            ...\n        },\n        \'playground\': {\n            ...\n        },\n        \'prod\': {\n            ...\n        },\n    }\n}\n```\n\n## Payla Generic model\n\n### Usage\n\n    from payla_utils.models import PaylaModel\n\n    class MyModel(PaylaModel):\n        ...\n\nThis model will add the following fields:\n\n- `created_at` - datetime\n- `modified_at` - datetime\n\nIt has also a QuerySet that will add the following methods:\n\n- `get_or_none` - returns the object or None\n',
     'author': 'Payla Services',
     'author_email': 'tools@payla.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `payla_utils-0.2.8/PKG-INFO` & `payla_utils-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payla-utils
-Version: 0.2.8
+Version: 0.2.9
 Summary: payla_utils python package
 License: MIT
 Keywords: payla_utils
 Author: Payla Services
 Author-email: tools@payla.de
 Requires-Python: >=3.9,<4
 Classifier: Development Status :: 2 - Pre-Alpha
```

