# Comparing `tmp/django-axes-6.0.0b1.tar.gz` & `tmp/django-axes-6.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-axes-6.0.0b1.tar", last modified: Tue Apr 25 16:45:39 2023, max compression
+gzip compressed data, was "django-axes-6.0.0b2.tar", last modified: Fri Apr 28 11:25:29 2023, max compression
```

## Comparing `django-axes-6.0.0b1.tar` & `django-axes-6.0.0b2.tar`

### file list

```diff
@@ -1,131 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.261824 django-axes-6.0.0b1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.249824 django-axes-6.0.0b1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.249824 django-axes-6.0.0b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/.prospector.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    30870 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36037 2023-04-25 16:45:39.261824 django-axes-6.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.249824 django-axes-6.0.0b1/axes/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.253824 django-axes-6.0.0b1/axes/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/handlers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/handlers/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/handlers/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/handlers/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/handlers/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19557 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.245824 django-axes-6.0.0b1/axes/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.245824 django-axes-6.0.0b1/axes/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.253824 django-axes-6.0.0b1/axes/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.245824 django-axes-6.0.0b1/axes/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.253824 django-axes-6.0.0b1/axes/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.245824 django-axes-6.0.0b1/axes/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.253824 django-axes-6.0.0b1/axes/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.245824 django-axes-6.0.0b1/axes/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.253824 django-axes-6.0.0b1/axes/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.245824 django-axes-6.0.0b1/axes/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.253824 django-axes-6.0.0b1/axes/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.253824 django-axes-6.0.0b1/axes/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.253824 django-axes-6.0.0b1/axes/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/management/commands/axes_list_attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/management/commands/axes_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/management/commands/axes_reset_failure_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/management/commands/axes_reset_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/management/commands/axes_reset_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/management/commands/axes_reset_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.257824 django-axes-6.0.0b1/axes/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/migrations/0002_auto_20151217_2044.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/migrations/0003_auto_20160322_0929.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/migrations/0004_auto_20181024_1538.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/migrations/0005_remove_accessattempt_trusted.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/migrations/0006_remove_accesslog_trusted.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/migrations/0007_alter_accessattempt_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/migrations/0008_accessfailurelog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.257824 django-axes-6.0.0b1/django_axes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36037 2023-04-25 16:45:39.000000 django-axes-6.0.0b1/django_axes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-25 16:45:39.000000 django-axes-6.0.0b1/django_axes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:45:39.000000 django-axes-6.0.0b1/django_axes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:45:39.000000 django-axes-6.0.0b1/django_axes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-25 16:45:39.000000 django-axes-6.0.0b1/django_axes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-25 16:45:39.000000 django-axes-6.0.0b1/django_axes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.257824 django-axes-6.0.0b1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/10_changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/1_requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/2_installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/3_usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)    63212 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/4_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/5_customization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/6_integration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/7_architecture.rst
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/8_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/9_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.257824 django-axes-6.0.0b1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   133029 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/images/flow.png
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/requirements-qa.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 16:45:39.261824 django-axes-6.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.261824 django-axes-6.0.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_failures.py
--rw-r--r--   0 runner    (1001) docker     (123)    21076 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    31476 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    29839 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/urls_empty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.720070 django-axes-6.0.0b2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.700070 django-axes-6.0.0b2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.700070 django-axes-6.0.0b2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/.prospector.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    31470 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    35736 2023-04-28 11:25:29.720070 django-axes-6.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.700070 django-axes-6.0.0b2/axes/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.704070 django-axes-6.0.0b2/axes/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/handlers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/handlers/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/handlers/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/handlers/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/handlers/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20380 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.692070 django-axes-6.0.0b2/axes/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.692070 django-axes-6.0.0b2/axes/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.704070 django-axes-6.0.0b2/axes/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.692070 django-axes-6.0.0b2/axes/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.708070 django-axes-6.0.0b2/axes/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.692070 django-axes-6.0.0b2/axes/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.708070 django-axes-6.0.0b2/axes/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.692070 django-axes-6.0.0b2/axes/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.708070 django-axes-6.0.0b2/axes/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.692070 django-axes-6.0.0b2/axes/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.708070 django-axes-6.0.0b2/axes/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.708070 django-axes-6.0.0b2/axes/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.708070 django-axes-6.0.0b2/axes/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/management/commands/axes_list_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/management/commands/axes_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/management/commands/axes_reset_failure_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/management/commands/axes_reset_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/management/commands/axes_reset_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/management/commands/axes_reset_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.712070 django-axes-6.0.0b2/axes/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/migrations/0002_auto_20151217_2044.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/migrations/0003_auto_20160322_0929.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/migrations/0004_auto_20181024_1538.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/migrations/0005_remove_accessattempt_trusted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/migrations/0006_remove_accesslog_trusted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/migrations/0007_alter_accessattempt_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/migrations/0008_accessfailurelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.712070 django-axes-6.0.0b2/django_axes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    35736 2023-04-28 11:25:29.000000 django-axes-6.0.0b2/django_axes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-28 11:25:29.000000 django-axes-6.0.0b2/django_axes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:25:29.000000 django-axes-6.0.0b2/django_axes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:25:29.000000 django-axes-6.0.0b2/django_axes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-28 11:25:29.000000 django-axes-6.0.0b2/django_axes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-28 11:25:29.000000 django-axes-6.0.0b2/django_axes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.716070 django-axes-6.0.0b2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/10_changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/1_requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/2_installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/3_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    63233 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/4_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/5_customization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/6_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/7_architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/8_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/9_contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.716070 django-axes-6.0.0b2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   133029 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/images/flow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/requirements-qa.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 11:25:29.720070 django-axes-6.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.720070 django-axes-6.0.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_failures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21076 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31928 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29839 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/urls_empty.py
```

### Comparing `django-axes-6.0.0b1/.github/workflows/codeql.yml` & `django-axes-6.0.0b2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/.github/workflows/release.yml` & `django-axes-6.0.0b2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/.github/workflows/test.yml` & `django-axes-6.0.0b2/.github/workflows/test.yml`

 * *Files 4% similar despite different names*

```diff
@@ -9,43 +9,45 @@
   build:
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       max-parallel: 5
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11', 'pypy-3.8']
-        django-version: ['3.2', '4.0', '4.1']
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
+        django-version: ['3.2', '4.1', '4.2']
         include:
           # Tox configuration for QA environment
-          - python-version: '3.10'
+          - python-version: '3.11'
             django-version: 'qa'
           # Django main
-          - python-version: '3.10'
-            django-version: 'main'
-            experimental: true
           - python-version: '3.11'
             django-version: 'main'
             experimental: true
+          # PyPy 3.8
+          - python-version: 'pypy-3.8'
+            django-version: '3.2'
+            experimental: true
           - python-version: 'pypy-3.8'
             django-version: '4.1'
             experimental: true
+          - python-version: 'pypy-3.8'
+            django-version: '4.2'
+            experimental: true
         exclude:
-          # Exclude Python 3.7 for Django 4.0 and Django main
-          - python-version: '3.7'
-            django-version: '4.0'
+          # Exclude Python 3.7 for Django 4.x and Django main
           - python-version: '3.7'
             django-version: '4.1'
           - python-version: '3.7'
+            django-version: '4.2'
+          - python-version: '3.7'
             django-version: 'main'
           # Exclude Python 3.11 for Django 3.2 and Django 4.0
           - python-version: '3.11'
             django-version: '3.2'
-          - python-version: '3.11'
-            django-version: '4.0'
 
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
```

### Comparing `django-axes-6.0.0b1/CHANGES.rst` & `django-axes-6.0.0b2/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 
 Changes
 =======
 
 
+6.0.0b2 (2023-04-28)
+--------------------
+
+- Make ``django-ipware`` an optional dependency. Install it with e.g. ``pip install django-axes[ipware]`` package and extras specifier. [aleksihakli]
+- Deprecate and rename old configuration flags. Old flags will be removed in or after version ``6.1``. [aleksihakli]
+   * ``AXES_PROXY_ORDER`` is now ``AXES_IPWARE_PROXY_ORDER``, 
+   * ``AXES_PROXY_COUNT`` is now ``AXES_IPWARE_PROXY_COUNT``, 
+   * ``AXES_IPWARE_PROXY_TRUSTED_IPS`` is now ``AXES_PROXY_TRUSTED_IPS``, and 
+   * ``AXES_IPWARE_META_PRECEDENCE_ORDER`` is now ``AXES_META_PRECEDENCE_ORDER``. 
+
+
 6.0.0b1 (2023-04-25)
 --------------------
 
 - Set 429 as the default lockout response code. [hirotasoshu]
 
 
 5.41.1 (2023-04-16)
```

### Comparing `django-axes-6.0.0b1/CODE_OF_CONDUCT.md` & `django-axes-6.0.0b2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/LICENSE` & `django-axes-6.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/PKG-INFO` & `django-axes-6.0.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-axes
-Version: 6.0.0b1
+Version: 6.0.0b2
 Summary: Keep track of failed login attempts in Django-powered sites.
 Home-page: https://github.com/jazzband/django-axes
 Author: Josh VanderLinden, Philip Neustrom, Michael Blume, Alex Clark, Camilo Nova, Aleksi Hakli
 Author-email: security@jazzband.co
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.co
 License: MIT
@@ -32,14 +32,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: Log Analysis
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Logging
 Requires-Python: >=3.7
+Provides-Extra: ipware
 License-File: LICENSE
 
 
 django-axes
 ===========
 
 .. image:: https://jazzband.co/static/img/badge.svg
@@ -113,45 +114,33 @@
 ------
 
 If you have questions or have trouble using the app please file a bug report at:
 
 https://github.com/jazzband/django-axes/issues
 
 
-Contributions
--------------
+Contributing
+------------
 
-All contributions are welcome!
+See `CONTRIBUTING <CONTRIBUTING.rst>`__.
 
-It is best to separate proposed changes and PRs into small, distinct patches
-by type so that they can be merged faster into upstream and released quicker.
 
-One way to organize contributions would be to separate PRs for e.g.
+Changes
+=======
 
-* bugfixes,
-* new features,
-* code and design improvements,
-* documentation improvements, or
-* tooling and CI improvements.
-
-Merging contributions requires passing the checks configured
-with the CI. This includes running tests and linters successfully
-on the currently officially supported Python and Django versions.
-
-The test automation is run automatically with GitHub Actions, but you can
-run it locally with the ``tox`` command before pushing commits.
-
-Please note that this is a `Jazzband <https://jazzband.co>`_ project.
-By contributing you agree to abide by the
-`Contributor Code of Conduct <https://jazzband.co/about/conduct>`_
-and follow the `guidelines <https://jazzband.co/about/guidelines>`_.
 
+6.0.0b2 (2023-04-28)
+--------------------
 
-Changes
-=======
+- Make ``django-ipware`` an optional dependency. Install it with e.g. ``pip install django-axes[ipware]`` package and extras specifier. [aleksihakli]
+- Deprecate and rename old configuration flags. Old flags will be removed in or after version ``6.1``. [aleksihakli]
+   * ``AXES_PROXY_ORDER`` is now ``AXES_IPWARE_PROXY_ORDER``, 
+   * ``AXES_PROXY_COUNT`` is now ``AXES_IPWARE_PROXY_COUNT``, 
+   * ``AXES_IPWARE_PROXY_TRUSTED_IPS`` is now ``AXES_PROXY_TRUSTED_IPS``, and 
+   * ``AXES_IPWARE_META_PRECEDENCE_ORDER`` is now ``AXES_META_PRECEDENCE_ORDER``. 
 
 
 6.0.0b1 (2023-04-25)
 --------------------
 
 - Set 429 as the default lockout response code. [hirotasoshu]
```

### Comparing `django-axes-6.0.0b1/axes/admin.py` & `django-axes-6.0.0b2/axes/admin.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/apps.py` & `django-axes-6.0.0b2/axes/apps.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/attempts.py` & `django-axes-6.0.0b2/axes/attempts.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/backends.py` & `django-axes-6.0.0b2/axes/backends.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/checks.py` & `django-axes-6.0.0b2/axes/checks.py`

 * *Files 8% similar despite different names*

```diff
@@ -118,14 +118,20 @@
 @register(Tags.compatibility)
 def axes_deprecation_check(app_configs, **kwargs):  # pylint: disable=unused-argument
     warnings = []
 
     deprecated_settings = [
         "AXES_DISABLE_SUCCESS_ACCESS_LOG",
         "AXES_LOGGER",
+        # AXES_PROXY_ and AXES_META_ parameters were updated to more explicit
+        # AXES_IPWARE_PROXY_ and AXES_IPWARE_META_ prefixes in version 6.x
+        "AXES_PROXY_ORDER",
+        "AXES_PROXY_COUNT",
+        "AXES_PROXY_TRUSTED_IPS",
+        "AXES_META_PRECEDENCE_ORDER",
     ]
 
     for deprecated_setting in deprecated_settings:
         try:
             getattr(settings, deprecated_setting)
             warnings.append(
                 Warning(
```

### Comparing `django-axes-6.0.0b1/axes/conf.py` & `django-axes-6.0.0b2/axes/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,32 +104,14 @@
     settings,
     "AXES_PERMALOCK_MESSAGE",
     _(
         "Account locked: too many login attempts. Contact an admin to unlock your account."
     ),
 )
 
-# if your deployment is using reverse proxies, set this value to 'left-most' or 'right-most' per your configuration
-settings.AXES_PROXY_ORDER = getattr(settings, "AXES_PROXY_ORDER", "left-most")
-
-# if your deployment is using reverse proxies, set this value to the number of proxies in front of Django
-settings.AXES_PROXY_COUNT = getattr(settings, "AXES_PROXY_COUNT", None)
-
-# if your deployment is using reverse proxies, set to your trusted proxy IP addresses prefixes if needed
-settings.AXES_PROXY_TRUSTED_IPS = getattr(settings, "AXES_PROXY_TRUSTED_IPS", None)
-
-# set to the names of request.META attributes that should be checked for the IP address of the client
-# if your deployment is using reverse proxies, ensure that the header attributes are securely set by the proxy
-# ensure that the client can not spoof the headers by setting them and sending them through the proxy
-settings.AXES_META_PRECEDENCE_ORDER = getattr(
-    settings,
-    "AXES_META_PRECEDENCE_ORDER",
-    getattr(settings, "IPWARE_META_PRECEDENCE_ORDER", ("REMOTE_ADDR",)),
-)
-
 # set CORS allowed origins when calling authentication over ajax
 settings.AXES_ALLOWED_CORS_ORIGINS = getattr(settings, "AXES_ALLOWED_CORS_ORIGINS", "*")
 
 # set the list of sensitive parameters to cleanse from get/post data before logging
 settings.AXES_SENSITIVE_PARAMETERS = getattr(
     settings,
     "AXES_SENSITIVE_PARAMETERS",
@@ -143,7 +125,48 @@
 # set the HTTP response code given by too many requests
 settings.AXES_HTTP_RESPONSE_CODE = getattr(settings, "AXES_HTTP_RESPONSE_CODE", 429)
 
 # If True, a failed login attempt during lockout will reset the cool off period
 settings.AXES_RESET_COOL_OFF_ON_FAILURE_DURING_LOCKOUT = getattr(
     settings, "AXES_RESET_COOL_OFF_ON_FAILURE_DURING_LOCKOUT", True
 )
+
+
+###
+# django-ipware settings for client IP address calculation and proxy detection
+# there are old AXES_PROXY_ and AXES_META_ legacy keys present for backwards compatibility
+# see https://github.com/un33k/django-ipware for further details
+###
+
+# if your deployment is using reverse proxies, set this value to 'left-most' or 'right-most' per your configuration
+settings.AXES_IPWARE_PROXY_ORDER = getattr(
+    settings,
+    "AXES_IPWARE_PROXY_ORDER",
+    getattr(settings, "AXES_PROXY_ORDER", "left-most"),
+)
+
+# if your deployment is using reverse proxies, set this value to the number of proxies in front of Django
+settings.AXES_IPWARE_PROXY_COUNT = getattr(
+    settings,
+    "AXES_IPWARE_PROXY_COUNT",
+    getattr(settings, "AXES_PROXY_COUNT", None),
+)
+
+# if your deployment is using reverse proxies, set to your trusted proxy IP addresses prefixes if needed
+settings.AXES_IPWARE_PROXY_TRUSTED_IPS = getattr(
+    settings,
+    "AXES_IPWARE_PROXY_TRUSTED_IPS",
+    getattr(settings, "AXES_PROXY_TRUSTED_IPS", None),
+)
+
+# set to the names of request.META attributes that should be checked for the IP address of the client
+# if your deployment is using reverse proxies, ensure that the header attributes are securely set by the proxy
+# ensure that the client can not spoof the headers by setting them and sending them through the proxy
+settings.AXES_IPWARE_META_PRECEDENCE_ORDER = getattr(
+    settings,
+    "AXES_IPWARE_META_PRECEDENCE_ORDER",
+    getattr(
+        settings,
+        "AXES_META_PRECEDENCE_ORDER",
+        getattr(settings, "IPWARE_META_PRECEDENCE_ORDER", ("REMOTE_ADDR",)),
+    ),
+)
```

### Comparing `django-axes-6.0.0b1/axes/decorators.py` & `django-axes-6.0.0b2/axes/decorators.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/handlers/base.py` & `django-axes-6.0.0b2/axes/handlers/base.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/handlers/cache.py` & `django-axes-6.0.0b2/axes/handlers/cache.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/handlers/database.py` & `django-axes-6.0.0b2/axes/handlers/database.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/handlers/dummy.py` & `django-axes-6.0.0b2/axes/handlers/dummy.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/handlers/proxy.py` & `django-axes-6.0.0b2/axes/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/handlers/test.py` & `django-axes-6.0.0b2/axes/handlers/test.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/helpers.py` & `django-axes-6.0.0b2/axes/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from datetime import timedelta
 from hashlib import sha256
 from logging import getLogger
 from string import Template
 from typing import Callable, Optional, Type, Union
 from urllib.parse import urlencode
 
-import ipware.ip
 from django.core.cache import BaseCache, caches
 from django.http import HttpRequest, HttpResponse, JsonResponse, QueryDict
 from django.shortcuts import redirect, render
 from django.utils.module_loading import import_string
 
 from axes.conf import settings
 from axes.models import AccessBase
 
 log = getLogger(__name__)
 
+try:
+    import ipware.ip
+
+    IPWARE_INSTALLED = True
+except ImportError:
+    IPWARE_INSTALLED = False
+
 
 def get_cache() -> BaseCache:
     """
     Get the cache instance Axes is configured to use with ``settings.AXES_CACHE`` and use ``'default'`` if not set.
     """
 
     return caches[getattr(settings, "AXES_CACHE", "default")]
@@ -144,48 +150,63 @@
         "Using parameter request.POST to get username with key settings.AXES_USERNAME_FORM_FIELD"
     )
 
     request_data = getattr(request, "data", request.POST)
     return request_data.get(settings.AXES_USERNAME_FORM_FIELD, None)
 
 
-def get_client_ip_address(request: HttpRequest) -> str:
+def get_client_ip_address(
+    request: HttpRequest,
+    use_ipware: Optional[bool] = None,
+) -> Optional[str]:
     """
     Get client IP address as configured by the user.
 
     The order of preference for address resolution is as follows:
 
     1. If configured, use ``AXES_CLIENT_IP_CALLABLE``, and supply ``request`` as argument
-    2. Use django-ipware package (parameters can be configured in the Axes package)
+    2. If available, use django-ipware package (parameters can be configured in the Axes package)
+    3. Use ``request.META.get('REMOTE_ADDR', None)`` as a fallback
 
     :param request: incoming Django ``HttpRequest`` or similar object from authentication backend or other source
     """
 
     if settings.AXES_CLIENT_IP_CALLABLE:
-        log.debug("Using settings.AXES_CLIENT_IP_CALLABLE to get username")
+        log.debug("Using settings.AXES_CLIENT_IP_CALLABLE to get client IP address")
 
         if callable(settings.AXES_CLIENT_IP_CALLABLE):
             return settings.AXES_CLIENT_IP_CALLABLE(  # pylint: disable=not-callable
                 request
             )
         if isinstance(settings.AXES_CLIENT_IP_CALLABLE, str):
             return import_string(settings.AXES_CLIENT_IP_CALLABLE)(request)
         raise TypeError(
             "settings.AXES_CLIENT_IP_CALLABLE needs to be a string, callable, or None."
         )
 
-    client_ip_address, _ = ipware.ip.get_client_ip(
-        request,
-        proxy_order=settings.AXES_PROXY_ORDER,
-        proxy_count=settings.AXES_PROXY_COUNT,
-        proxy_trusted_ips=settings.AXES_PROXY_TRUSTED_IPS,
-        request_header_order=settings.AXES_META_PRECEDENCE_ORDER,
-    )
+    # Resolve using django-ipware from a configuration flag that can be set to False to explicitly disable
+    # this is added to both enable or disable the branch when ipware is installed in the test environment
+    if use_ipware is None:
+        use_ipware = IPWARE_INSTALLED
+    if use_ipware:
+        log.debug("Using django-ipware to get client IP address")
+
+        client_ip_address, _ = ipware.ip.get_client_ip(
+            request,
+            proxy_order=settings.AXES_IPWARE_PROXY_ORDER,
+            proxy_count=settings.AXES_IPWARE_PROXY_COUNT,
+            proxy_trusted_ips=settings.AXES_IPWARE_PROXY_TRUSTED_IPS,
+            request_header_order=settings.AXES_IPWARE_META_PRECEDENCE_ORDER,
+        )
+        return client_ip_address
 
-    return client_ip_address
+    log.debug(
+        "Using request.META.get('REMOTE_ADDR', None) fallback method to get client IP address"
+    )
+    return request.META.get("REMOTE_ADDR", None)
 
 
 def get_client_user_agent(request: HttpRequest) -> str:
     return request.META.get("HTTP_USER_AGENT", "<unknown>")[:255]
 
 
 def get_client_path_info(request: HttpRequest) -> str:
```

### Comparing `django-axes-6.0.0b1/axes/locale/ar/LC_MESSAGES/django.mo` & `django-axes-6.0.0b2/axes/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/locale/ar/LC_MESSAGES/django.po` & `django-axes-6.0.0b2/axes/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/locale/de/LC_MESSAGES/django.mo` & `django-axes-6.0.0b2/axes/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/locale/de/LC_MESSAGES/django.po` & `django-axes-6.0.0b2/axes/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/locale/pl/LC_MESSAGES/django.mo` & `django-axes-6.0.0b2/axes/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/locale/pl/LC_MESSAGES/django.po` & `django-axes-6.0.0b2/axes/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/locale/ru/LC_MESSAGES/django.mo` & `django-axes-6.0.0b2/axes/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/locale/ru/LC_MESSAGES/django.po` & `django-axes-6.0.0b2/axes/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/locale/tr/LC_MESSAGES/django.mo` & `django-axes-6.0.0b2/axes/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/locale/tr/LC_MESSAGES/django.po` & `django-axes-6.0.0b2/axes/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/management/commands/axes_reset_failure_logs.py` & `django-axes-6.0.0b2/axes/management/commands/axes_reset_failure_logs.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/management/commands/axes_reset_ip.py` & `django-axes-6.0.0b2/axes/management/commands/axes_reset_ip.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/management/commands/axes_reset_logs.py` & `django-axes-6.0.0b2/axes/management/commands/axes_reset_logs.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/management/commands/axes_reset_username.py` & `django-axes-6.0.0b2/axes/management/commands/axes_reset_username.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/middleware.py` & `django-axes-6.0.0b2/axes/middleware.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/migrations/0001_initial.py` & `django-axes-6.0.0b2/axes/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/migrations/0002_auto_20151217_2044.py` & `django-axes-6.0.0b2/axes/migrations/0002_auto_20151217_2044.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/migrations/0003_auto_20160322_0929.py` & `django-axes-6.0.0b2/axes/migrations/0003_auto_20160322_0929.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/migrations/0004_auto_20181024_1538.py` & `django-axes-6.0.0b2/axes/migrations/0004_auto_20181024_1538.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/migrations/0007_alter_accessattempt_unique_together.py` & `django-axes-6.0.0b2/axes/migrations/0007_alter_accessattempt_unique_together.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/migrations/0008_accessfailurelog.py` & `django-axes-6.0.0b2/axes/migrations/0008_accessfailurelog.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/models.py` & `django-axes-6.0.0b2/axes/models.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/signals.py` & `django-axes-6.0.0b2/axes/signals.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/axes/utils.py` & `django-axes-6.0.0b2/axes/utils.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/django_axes.egg-info/PKG-INFO` & `django-axes-6.0.0b2/django_axes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-axes
-Version: 6.0.0b1
+Version: 6.0.0b2
 Summary: Keep track of failed login attempts in Django-powered sites.
 Home-page: https://github.com/jazzband/django-axes
 Author: Josh VanderLinden, Philip Neustrom, Michael Blume, Alex Clark, Camilo Nova, Aleksi Hakli
 Author-email: security@jazzband.co
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.co
 License: MIT
@@ -32,14 +32,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: Log Analysis
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Logging
 Requires-Python: >=3.7
+Provides-Extra: ipware
 License-File: LICENSE
 
 
 django-axes
 ===========
 
 .. image:: https://jazzband.co/static/img/badge.svg
@@ -113,45 +114,33 @@
 ------
 
 If you have questions or have trouble using the app please file a bug report at:
 
 https://github.com/jazzband/django-axes/issues
 
 
-Contributions
--------------
+Contributing
+------------
 
-All contributions are welcome!
+See `CONTRIBUTING <CONTRIBUTING.rst>`__.
 
-It is best to separate proposed changes and PRs into small, distinct patches
-by type so that they can be merged faster into upstream and released quicker.
 
-One way to organize contributions would be to separate PRs for e.g.
+Changes
+=======
 
-* bugfixes,
-* new features,
-* code and design improvements,
-* documentation improvements, or
-* tooling and CI improvements.
-
-Merging contributions requires passing the checks configured
-with the CI. This includes running tests and linters successfully
-on the currently officially supported Python and Django versions.
-
-The test automation is run automatically with GitHub Actions, but you can
-run it locally with the ``tox`` command before pushing commits.
-
-Please note that this is a `Jazzband <https://jazzband.co>`_ project.
-By contributing you agree to abide by the
-`Contributor Code of Conduct <https://jazzband.co/about/conduct>`_
-and follow the `guidelines <https://jazzband.co/about/guidelines>`_.
 
+6.0.0b2 (2023-04-28)
+--------------------
 
-Changes
-=======
+- Make ``django-ipware`` an optional dependency. Install it with e.g. ``pip install django-axes[ipware]`` package and extras specifier. [aleksihakli]
+- Deprecate and rename old configuration flags. Old flags will be removed in or after version ``6.1``. [aleksihakli]
+   * ``AXES_PROXY_ORDER`` is now ``AXES_IPWARE_PROXY_ORDER``, 
+   * ``AXES_PROXY_COUNT`` is now ``AXES_IPWARE_PROXY_COUNT``, 
+   * ``AXES_IPWARE_PROXY_TRUSTED_IPS`` is now ``AXES_PROXY_TRUSTED_IPS``, and 
+   * ``AXES_IPWARE_META_PRECEDENCE_ORDER`` is now ``AXES_META_PRECEDENCE_ORDER``. 
 
 
 6.0.0b1 (2023-04-25)
 --------------------
 
 - Set 429 as the default lockout response code. [hirotasoshu]
```

### Comparing `django-axes-6.0.0b1/django_axes.egg-info/SOURCES.txt` & `django-axes-6.0.0b2/django_axes.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .gitignore
 .pre-commit-config.yaml
 .prospector.yaml
 CHANGES.rst
 CODE_OF_CONDUCT.md
+CONTRIBUTING.rst
 LICENSE
 README.rst
 codecov.yml
 manage.py
 mypy.ini
 pyproject.toml
 requirements-qa.txt
@@ -76,15 +77,15 @@
 docs/2_installation.rst
 docs/3_usage.rst
 docs/4_configuration.rst
 docs/5_customization.rst
 docs/6_integration.rst
 docs/7_architecture.rst
 docs/8_reference.rst
-docs/9_development.rst
+docs/9_contributing.rst
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/images/flow.png
 tests/__init__.py
 tests/base.py
 tests/settings.py
```

### Comparing `django-axes-6.0.0b1/docs/1_requirements.rst` & `django-axes-6.0.0b2/docs/1_requirements.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/docs/2_installation.rst` & `django-axes-6.0.0b2/docs/2_installation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 .. _installation:
 
 Installation
 ============
 
 Axes is easy to install from the PyPI package::
 
-    $ pip install django-axes
+    $ pip install django-axes[ipware]  # use django-ipware for resolving client IP addresses OR
+    $ pip install django-axes          # implement and configure custom AXES_CLIENT_IP_CALLABLE
 
 After installing the package, the project settings need to be configured.
 
 **1.** Add ``axes`` to your ``INSTALLED_APPS``::
 
     INSTALLED_APPS = [
         'django.contrib.admin',
```

### Comparing `django-axes-6.0.0b1/docs/3_usage.rst` & `django-axes-6.0.0b2/docs/3_usage.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/docs/4_configuration.rst` & `django-axes-6.0.0b2/docs/4_configuration.rst`

 * *Files 0% similar despite different names*

```diff
@@ -99,26 +99,26 @@
 
 Axes makes use of ``django-ipware`` package to detect the IP address of the client
 and uses some conservative configuration parameters by default for security.
 
 If you are using reverse proxies, you will need to configure one or more of the
 following settings to suit your set up to correctly resolve client IP addresses:
 
-* ``AXES_PROXY_COUNT``: The number of reverse proxies in front of Django as an integer. Default: ``None``
-* ``AXES_META_PRECEDENCE_ORDER``: The names of ``request.META`` attributes as a tuple of strings
+* ``AXES_IPWARE_PROXY_COUNT``: The number of reverse proxies in front of Django as an integer. Default: ``None``
+* ``AXES_IPWARE_META_PRECEDENCE_ORDER``: The names of ``request.META`` attributes as a tuple of strings
   to check to get the client IP address. Check the Django documentation for header naming conventions.
   Default: ``IPWARE_META_PRECEDENCE_ORDER`` setting if set, else ``('REMOTE_ADDR', )``
 
 .. note::
    For reverse proxies or e.g. Heroku, you might also want to fetch IP addresses from a HTTP header such as ``X-Forwarded-For``. To configure this, you can fetch IPs through the ``HTTP_X_FORWARDED_FOR`` key from the ``request.META`` property which contains all the HTTP headers in Django:
 
    .. code-block:: python
 
       # refer to the Django request and response objects documentation
-      AXES_META_PRECEDENCE_ORDER = [
+      AXES_IPWARE_META_PRECEDENCE_ORDER = [
           'HTTP_X_FORWARDED_FOR',
           'REMOTE_ADDR',
       ]
 
    Please note that proxies have different behaviours with the HTTP headers. Make sure that your proxy either strips the incoming value or otherwise makes sure of the validity of the header that is used because **any header values used in application configuration must be secure and trusted**. Otherwise the client can spoof IP addresses by just setting the header in their request and circumvent the IP address monitoring. Normal proxy server behaviours include overriding and appending the header value depending on the platform. Different platforms and gateway services utilize different headers, please refer to your deployment target documentation for up-to-date information on correct configuration.
```

### Comparing `django-axes-6.0.0b1/docs/5_customization.rst` & `django-axes-6.0.0b2/docs/5_customization.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/docs/6_integration.rst` & `django-axes-6.0.0b2/docs/6_integration.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/docs/7_architecture.rst` & `django-axes-6.0.0b2/docs/7_architecture.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/docs/Makefile` & `django-axes-6.0.0b2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/docs/conf.py` & `django-axes-6.0.0b2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/docs/images/flow.png` & `django-axes-6.0.0b2/docs/images/flow.png`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/pyproject.toml` & `django-axes-6.0.0b2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -7,57 +7,57 @@
 DJANGO_SETTINGS_MODULE = "tests.settings"
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
     py{37,38,39,310,py38}-dj32
-    py{38,39,310,py38}-dj40
     py{38,39,310,311,py38}-dj41
-    py{310,311,py38}-djmain
-    py310-djqa
+    py{38,39,310,311,py38}-dj42
+    py311-djmain
+    py311-djqa
 
 [gh-actions]
 python =
     3.7: py37
     3.8: py38
     3.9: py39
     3.10: py310
     3.11: py311
     pypy-3.8: pypy38
 
 [gh-actions:env]
 DJANGO =
     3.2: dj32
-    4.0: dj40
     4.1: dj41
+    4.2: dj42
     main: djmain
     qa: djqa
 
 # Normal test environment runs pytest which orchestrates other tools
 [testenv]
 deps =
     -r requirements-test.txt
     dj32: django>=3.2,<3.3
-    dj40: django>=4.0,<4.1
     dj41: django>=4.1,<4.2
+    dj42: django>=4.1,<4.2
     djmain: https://github.com/django/django/archive/main.tar.gz
 usedevelop = true
 commands = pytest
 setenv =
     PYTHONDONTWRITEBYTECODE=1
 # Django development version is allowed to fail the test matrix
 ignore_outcome =
     djmain: True
-    pypy38-dj41: True
+    pypy38: True
 ignore_errors =
     djmain: True
-    pypy38-dj41: True
+    pypy38: True
 
 # QA runs type checks, linting, and code formatting checks
-[testenv:py310-djqa]
+[testenv:py311-djqa]
 deps = -r requirements-qa.txt
 commands =
     mypy axes
     prospector
     black -t py38 --check --diff axes
 """
```

### Comparing `django-axes-6.0.0b1/setup.py` & `django-axes-6.0.0b2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,18 @@
         "Tracker": "https://github.com/jazzband/django-axes/issues",
     },
     license="MIT",
     package_dir={"axes": "axes"},
     use_scm_version=True,
     setup_requires=["setuptools_scm"],
     python_requires=">=3.7",
-    install_requires=["django>=3.2", "django-ipware>=3", "setuptools"],
+    install_requires=["django>=3.2", "setuptools"],
+    extras_require={
+        "ipware": "django-ipware>=3",
+    },
     include_package_data=True,
     packages=find_packages(exclude=["tests"]),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Environment :: Plugins",
         "Framework :: Django",
```

### Comparing `django-axes-6.0.0b1/tests/base.py` & `django-axes-6.0.0b2/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/tests/settings.py` & `django-axes-6.0.0b2/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/tests/test_admin.py` & `django-axes-6.0.0b2/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/tests/test_attempts.py` & `django-axes-6.0.0b2/tests/test_attempts.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/tests/test_backends.py` & `django-axes-6.0.0b2/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/tests/test_checks.py` & `django-axes-6.0.0b2/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/tests/test_decorators.py` & `django-axes-6.0.0b2/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/tests/test_failures.py` & `django-axes-6.0.0b2/tests/test_failures.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/tests/test_handlers.py` & `django-axes-6.0.0b2/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/tests/test_helpers.py` & `django-axes-6.0.0b2/tests/test_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -610,14 +610,24 @@
     @override_settings(
         AXES_CLIENT_IP_CALLABLE=lambda request, extra: None
     )  # pragma: no cover
     def test_get_client_ip_address_invalid_callable_too_many_arguments(self):
         with self.assertRaises(TypeError):
             get_client_ip_address(HttpRequest())
 
+    def test_get_client_ip_address_with_ipware(self):
+        request = HttpRequest()
+        request.META["REMOTE_ADDR"] = "127.0.0.2"
+        self.assertEqual(get_client_ip_address(request, use_ipware=True), "127.0.0.2")
+
+    def test_get_client_ip_address_without_ipware(self):
+        request = HttpRequest()
+        request.META["REMOTE_ADDR"] = "127.0.0.3"
+        self.assertEqual(get_client_ip_address(request, use_ipware=False), "127.0.0.3")
+
 
 class IPWhitelistTestCase(AxesTestCase):
     def setUp(self):
         self.request = HttpRequest()
         self.request.method = "POST"
         self.request.META["REMOTE_ADDR"] = "127.0.0.1"
         self.request.axes_ip_address = "127.0.0.1"
```

### Comparing `django-axes-6.0.0b1/tests/test_logging.py` & `django-axes-6.0.0b2/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/tests/test_login.py` & `django-axes-6.0.0b2/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/tests/test_management.py` & `django-axes-6.0.0b2/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/tests/test_middleware.py` & `django-axes-6.0.0b2/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b1/tests/test_models.py` & `django-axes-6.0.0b2/tests/test_models.py`

 * *Files identical despite different names*

