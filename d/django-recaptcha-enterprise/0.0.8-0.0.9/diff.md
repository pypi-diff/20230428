# Comparing `tmp/django-recaptcha-enterprise-0.0.8.tar.gz` & `tmp/django-recaptcha-enterprise-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-recaptcha-enterprise-0.0.8.tar", last modified: Fri Jan 27 19:53:19 2023, max compression
+gzip compressed data, was "django-recaptcha-enterprise-0.0.9.tar", last modified: Fri Jan 27 20:45:03 2023, max compression
```

## Comparing `django-recaptcha-enterprise-0.0.8.tar` & `django-recaptcha-enterprise-0.0.9.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.551864 django-recaptcha-enterprise-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-01-27 19:53:19.551864 django-recaptcha-enterprise-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.547865 django-recaptcha-enterprise-0.0.8/captcha/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.547865 django-recaptcha-enterprise-0.0.8/captcha/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.547865 django-recaptcha-enterprise-0.0.8/captcha/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.547865 django-recaptcha-enterprise-0.0.8/captcha/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.547865 django-recaptcha-enterprise-0.0.8/captcha/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.547865 django-recaptcha-enterprise-0.0.8/captcha/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.547865 django-recaptcha-enterprise-0.0.8/captcha/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.547865 django-recaptcha-enterprise-0.0.8/captcha/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.547865 django-recaptcha-enterprise-0.0.8/captcha/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.551864 django-recaptcha-enterprise-0.0.8/captcha/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.547865 django-recaptcha-enterprise-0.0.8/captcha/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.551864 django-recaptcha-enterprise-0.0.8/captcha/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.547865 django-recaptcha-enterprise-0.0.8/captcha/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.551864 django-recaptcha-enterprise-0.0.8/captcha/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.547865 django-recaptcha-enterprise-0.0.8/captcha/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.551864 django-recaptcha-enterprise-0.0.8/captcha/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.547865 django-recaptcha-enterprise-0.0.8/captcha/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.551864 django-recaptcha-enterprise-0.0.8/captcha/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.547865 django-recaptcha-enterprise-0.0.8/captcha/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.551864 django-recaptcha-enterprise-0.0.8/captcha/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.547865 django-recaptcha-enterprise-0.0.8/captcha/locale/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.551864 django-recaptcha-enterprise-0.0.8/captcha/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/locale/zh_TW/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.547865 django-recaptcha-enterprise-0.0.8/captcha/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.551864 django-recaptcha-enterprise-0.0.8/captcha/templates/captcha/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.551864 django-recaptcha-enterprise-0.0.8/captcha/templates/captcha/includes/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/templates/captcha/includes/js_v2_checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/templates/captcha/includes/js_v2_invisible.html
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/templates/captcha/includes/js_v3.html
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/templates/captcha/widget_v2_checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/templates/captcha/widget_v2_invisible.html
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/templates/captcha/widget_v3.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.551864 django-recaptcha-enterprise-0.0.8/captcha/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.551864 django-recaptcha-enterprise-0.0.8/captcha/tests/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/tests/requirements/py27.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.551864 django-recaptcha-enterprise-0.0.8/captcha/tests/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/tests/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/tests/settings/coveralls_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/captcha/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 19:53:19.551864 django-recaptcha-enterprise-0.0.8/django_recaptcha_enterprise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-01-27 19:53:19.000000 django-recaptcha-enterprise-0.0.8/django_recaptcha_enterprise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-01-27 19:53:19.000000 django-recaptcha-enterprise-0.0.8/django_recaptcha_enterprise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 19:53:19.000000 django-recaptcha-enterprise-0.0.8/django_recaptcha_enterprise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-27 19:53:19.000000 django-recaptcha-enterprise-0.0.8/django_recaptcha_enterprise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-27 19:53:19.000000 django-recaptcha-enterprise-0.0.8/django_recaptcha_enterprise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-27 19:53:19.551864 django-recaptcha-enterprise-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-01-27 19:53:09.000000 django-recaptcha-enterprise-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.667306 django-recaptcha-enterprise-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-01-27 20:45:03.667306 django-recaptcha-enterprise-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.667306 django-recaptcha-enterprise-0.0.9/captcha/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.663306 django-recaptcha-enterprise-0.0.9/captcha/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.663306 django-recaptcha-enterprise-0.0.9/captcha/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.667306 django-recaptcha-enterprise-0.0.9/captcha/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.663306 django-recaptcha-enterprise-0.0.9/captcha/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.667306 django-recaptcha-enterprise-0.0.9/captcha/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.663306 django-recaptcha-enterprise-0.0.9/captcha/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.667306 django-recaptcha-enterprise-0.0.9/captcha/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.663306 django-recaptcha-enterprise-0.0.9/captcha/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.667306 django-recaptcha-enterprise-0.0.9/captcha/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.663306 django-recaptcha-enterprise-0.0.9/captcha/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.667306 django-recaptcha-enterprise-0.0.9/captcha/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.663306 django-recaptcha-enterprise-0.0.9/captcha/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.667306 django-recaptcha-enterprise-0.0.9/captcha/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.663306 django-recaptcha-enterprise-0.0.9/captcha/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.667306 django-recaptcha-enterprise-0.0.9/captcha/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.663306 django-recaptcha-enterprise-0.0.9/captcha/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.667306 django-recaptcha-enterprise-0.0.9/captcha/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.663306 django-recaptcha-enterprise-0.0.9/captcha/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.667306 django-recaptcha-enterprise-0.0.9/captcha/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.663306 django-recaptcha-enterprise-0.0.9/captcha/locale/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.667306 django-recaptcha-enterprise-0.0.9/captcha/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/locale/zh_TW/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.663306 django-recaptcha-enterprise-0.0.9/captcha/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.667306 django-recaptcha-enterprise-0.0.9/captcha/templates/captcha/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.667306 django-recaptcha-enterprise-0.0.9/captcha/templates/captcha/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/templates/captcha/includes/js_v2_checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/templates/captcha/includes/js_v2_invisible.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/templates/captcha/includes/js_v3.html
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/templates/captcha/widget_v2_checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/templates/captcha/widget_v2_invisible.html
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/templates/captcha/widget_v3.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.667306 django-recaptcha-enterprise-0.0.9/captcha/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.667306 django-recaptcha-enterprise-0.0.9/captcha/tests/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/tests/requirements/py27.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.667306 django-recaptcha-enterprise-0.0.9/captcha/tests/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/tests/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/tests/settings/coveralls_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/captcha/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:45:03.667306 django-recaptcha-enterprise-0.0.9/django_recaptcha_enterprise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-01-27 20:45:03.000000 django-recaptcha-enterprise-0.0.9/django_recaptcha_enterprise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-01-27 20:45:03.000000 django-recaptcha-enterprise-0.0.9/django_recaptcha_enterprise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 20:45:03.000000 django-recaptcha-enterprise-0.0.9/django_recaptcha_enterprise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-27 20:45:03.000000 django-recaptcha-enterprise-0.0.9/django_recaptcha_enterprise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-27 20:45:03.000000 django-recaptcha-enterprise-0.0.9/django_recaptcha_enterprise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-27 20:45:03.667306 django-recaptcha-enterprise-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-01-27 20:44:55.000000 django-recaptcha-enterprise-0.0.9/setup.py
```

### Comparing `django-recaptcha-enterprise-0.0.8/PKG-INFO` & `django-recaptcha-enterprise-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: django-recaptcha-enterprise
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Django app to utilise full capabilities of reCaptcha enterprise.
 Home-page: https://github.com/rapidbounce/django-recaptcha-enterprise
 Author: Panagiotis Skarlas
 Author-email: devs@rapidbounce.co
 License: MIT License
+Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.9
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
@@ -30,7 +31,8 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
 
 A Django app to utilise full capabilities of reCaptcha enterprise.
+
```

### Comparing `django-recaptcha-enterprise-0.0.8/captcha/__init__.py` & `django-recaptcha-enterprise-0.0.9/captcha/__init__.py`

 * *Files identical despite different names*

### Comparing `django-recaptcha-enterprise-0.0.8/captcha/checks.py` & `django-recaptcha-enterprise-0.0.9/captcha/checks.py`

 * *Files identical despite different names*

### Comparing `django-recaptcha-enterprise-0.0.8/captcha/client.py` & `django-recaptcha-enterprise-0.0.9/captcha/client.py`

 * *Files identical despite different names*

### Comparing `django-recaptcha-enterprise-0.0.8/captcha/fields.py` & `django-recaptcha-enterprise-0.0.9/captcha/fields.py`

 * *Files identical despite different names*

### Comparing `django-recaptcha-enterprise-0.0.8/captcha/locale/el/LC_MESSAGES/django.po` & `django-recaptcha-enterprise-0.0.9/captcha/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-recaptcha-enterprise-0.0.8/captcha/locale/en/LC_MESSAGES/django.po` & `django-recaptcha-enterprise-0.0.9/captcha/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-recaptcha-enterprise-0.0.8/captcha/locale/es/LC_MESSAGES/django.po` & `django-recaptcha-enterprise-0.0.9/captcha/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-recaptcha-enterprise-0.0.8/captcha/locale/fr/LC_MESSAGES/django.po` & `django-recaptcha-enterprise-0.0.9/captcha/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-recaptcha-enterprise-0.0.8/captcha/locale/nl/LC_MESSAGES/django.po` & `django-recaptcha-enterprise-0.0.9/captcha/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-recaptcha-enterprise-0.0.8/captcha/locale/pl/LC_MESSAGES/django.po` & `django-recaptcha-enterprise-0.0.9/captcha/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-recaptcha-enterprise-0.0.8/captcha/locale/pt_BR/LC_MESSAGES/django.po` & `django-recaptcha-enterprise-0.0.9/captcha/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-recaptcha-enterprise-0.0.8/captcha/locale/ru/LC_MESSAGES/django.po` & `django-recaptcha-enterprise-0.0.9/captcha/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-recaptcha-enterprise-0.0.8/captcha/locale/zh_CN/LC_MESSAGES/django.po` & `django-recaptcha-enterprise-0.0.9/captcha/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-recaptcha-enterprise-0.0.8/captcha/locale/zh_TW/LC_MESSAGES/django.po` & `django-recaptcha-enterprise-0.0.9/captcha/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-recaptcha-enterprise-0.0.8/captcha/templates/captcha/includes/js_v2_checkbox.html` & `django-recaptcha-enterprise-0.0.9/captcha/templates/captcha/includes/js_v2_checkbox.html`

 * *Files identical despite different names*

### Comparing `django-recaptcha-enterprise-0.0.8/captcha/templates/captcha/includes/js_v2_invisible.html` & `django-recaptcha-enterprise-0.0.9/captcha/templates/captcha/includes/js_v2_invisible.html`

 * *Files identical despite different names*

### Comparing `django-recaptcha-enterprise-0.0.8/captcha/templates/captcha/includes/js_v3.html` & `django-recaptcha-enterprise-0.0.9/captcha/templates/captcha/includes/js_v3.html`

 * *Files identical despite different names*

### Comparing `django-recaptcha-enterprise-0.0.8/captcha/tests/test_client.py` & `django-recaptcha-enterprise-0.0.9/captcha/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `django-recaptcha-enterprise-0.0.8/captcha/tests/test_fields.py` & `django-recaptcha-enterprise-0.0.9/captcha/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-recaptcha-enterprise-0.0.8/captcha/tests/tests.py` & `django-recaptcha-enterprise-0.0.9/captcha/tests/tests.py`

 * *Files identical despite different names*

### Comparing `django-recaptcha-enterprise-0.0.8/captcha/widgets.py` & `django-recaptcha-enterprise-0.0.9/captcha/widgets.py`

 * *Files identical despite different names*

### Comparing `django-recaptcha-enterprise-0.0.8/django_recaptcha_enterprise.egg-info/PKG-INFO` & `django-recaptcha-enterprise-0.0.9/django_recaptcha_enterprise.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: django-recaptcha-enterprise
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Django app to utilise full capabilities of reCaptcha enterprise.
 Home-page: https://github.com/rapidbounce/django-recaptcha-enterprise
 Author: Panagiotis Skarlas
 Author-email: devs@rapidbounce.co
 License: MIT License
+Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.9
 Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
@@ -30,7 +31,8 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
 
 A Django app to utilise full capabilities of reCaptcha enterprise.
+
```

### Comparing `django-recaptcha-enterprise-0.0.8/django_recaptcha_enterprise.egg-info/SOURCES.txt` & `django-recaptcha-enterprise-0.0.9/django_recaptcha_enterprise.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 captcha/__init__.py
 captcha/_compat.py
 captcha/apps.py
 captcha/checks.py
 captcha/client.py
 captcha/constants.py
```

### Comparing `django-recaptcha-enterprise-0.0.8/setup.py` & `django-recaptcha-enterprise-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 install_requirements = [
     "django>=1.0",
 ]
 
 setup(
     name='django-recaptcha-enterprise',
-    version='0.0.8',
+    version='0.0.9',
     packages=find_packages(),
     install_requires=install_requirements,
     include_package_data=True,
     license='MIT License',
     description=short_description,
     long_description=short_description,
     long_description_content_type="text/markdown",
```

