# Comparing `tmp/django-bootstrap5-23.1.tar.gz` & `tmp/django-bootstrap5-23.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-bootstrap5-23.1.tar", last modified: Sun Apr  2 09:24:45 2023, max compression
+gzip compressed data, was "django-bootstrap5-23.2.dev0.tar", last modified: Fri Apr 28 13:44:45 2023, max compression
```

## Comparing `django-bootstrap5-23.1.tar` & `django-bootstrap5-23.2.dev0.tar`

### file list

```diff
@@ -1,269 +1,95 @@
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-02 09:24:45.628373 django-bootstrap5-23.1/
--rw-r--r--   0 dylan      (501) staff       (20)      757 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/AUTHORS
--rw-r--r--   0 dylan      (501) staff       (20)     1533 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/LICENSE
--rw-r--r--   0 dylan      (501) staff       (20)      296 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/MANIFEST.in
--rw-r--r--   0 dylan      (501) staff       (20)     3478 2023-04-02 09:24:45.628453 django-bootstrap5-23.1/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)     2373 2022-08-06 06:57:52.000000 django-bootstrap5-23.1/README.md
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-02 09:24:45.571858 django-bootstrap5-23.1/docs/
--rw-r--r--   0 dylan      (501) staff       (20)       30 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/docs/changelog.rst
--rw-r--r--   0 dylan      (501) staff       (20)      973 2022-03-06 08:54:37.000000 django-bootstrap5-23.1/docs/conf.py
--rw-r--r--   0 dylan      (501) staff       (20)      577 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/docs/example_template.rst
--rw-r--r--   0 dylan      (501) staff       (20)     3276 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/docs/forms.rst
--rw-r--r--   0 dylan      (501) staff       (20)      249 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/docs/index.rst
--rw-r--r--   0 dylan      (501) staff       (20)      585 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/docs/installation.rst
--rw-r--r--   0 dylan      (501) staff       (20)       28 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/docs/migrate.rst
--rw-r--r--   0 dylan      (501) staff       (20)      665 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/docs/quickstart.rst
--rw-r--r--   0 dylan      (501) staff       (20)      103 2023-04-02 08:07:01.000000 django-bootstrap5-23.1/docs/requirements.txt
--rw-r--r--   0 dylan      (501) staff       (20)     3275 2022-10-14 14:58:03.000000 django-bootstrap5-23.1/docs/settings.rst
--rw-r--r--   0 dylan      (501) staff       (20)     1364 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/docs/templates.rst
--rw-r--r--   0 dylan      (501) staff       (20)     2217 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/docs/templatetags.rst
--rw-r--r--   0 dylan      (501) staff       (20)      799 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/docs/widgets.rst
--rwxr-xr-x   0 dylan      (501) staff       (20)      252 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/manage.py
--rw-r--r--   0 dylan      (501) staff       (20)      686 2022-03-26 14:32:39.000000 django-bootstrap5-23.1/pyproject.toml
--rw-r--r--   0 dylan      (501) staff       (20)     1156 2023-04-02 09:24:45.628810 django-bootstrap5-23.1/setup.cfg
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-02 09:24:45.567579 django-bootstrap5-23.1/src/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-02 09:24:45.574404 django-bootstrap5-23.1/src/django_bootstrap5/
--rw-r--r--   0 dylan      (501) staff       (20)       55 2023-04-02 09:15:15.000000 django-bootstrap5-23.1/src/django_bootstrap5/__init__.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-02 09:24:45.575552 django-bootstrap5-23.1/src/django_bootstrap5/__pycache__/
--rw-r--r--   0 dylan      (501) staff       (20)      413 2022-02-27 06:22:12.000000 django-bootstrap5-23.1/src/django_bootstrap5/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2351 2022-08-05 14:34:59.000000 django-bootstrap5-23.1/src/django_bootstrap5/components.py
--rw-r--r--   0 dylan      (501) staff       (20)     2693 2023-04-02 07:39:08.000000 django-bootstrap5-23.1/src/django_bootstrap5/core.py
--rw-r--r--   0 dylan      (501) staff       (20)      621 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/src/django_bootstrap5/css.py
--rw-r--r--   0 dylan      (501) staff       (20)     1482 2022-10-15 06:32:49.000000 django-bootstrap5-23.1/src/django_bootstrap5/forms.py
--rw-r--r--   0 dylan      (501) staff       (20)      870 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/src/django_bootstrap5/html.py
--rw-r--r--   0 dylan      (501) staff       (20)    21153 2022-11-22 12:41:26.000000 django-bootstrap5-23.1/src/django_bootstrap5/renderers.py
--rw-r--r--   0 dylan      (501) staff       (20)      901 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/src/django_bootstrap5/size.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-02 09:24:45.567776 django-bootstrap5-23.1/src/django_bootstrap5/templates/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-02 09:24:45.576624 django-bootstrap5-23.1/src/django_bootstrap5/templates/django_bootstrap5/
--rw-r--r--   0 dylan      (501) staff       (20)     1079 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/src/django_bootstrap5/templates/django_bootstrap5/bootstrap5.html
--rw-r--r--   0 dylan      (501) staff       (20)       95 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/src/django_bootstrap5/templates/django_bootstrap5/field_errors.html
--rw-r--r--   0 dylan      (501) staff       (20)       79 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/src/django_bootstrap5/templates/django_bootstrap5/field_help_text.html
--rw-r--r--   0 dylan      (501) staff       (20)      122 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/src/django_bootstrap5/templates/django_bootstrap5/form_errors.html
--rw-r--r--   0 dylan      (501) staff       (20)      206 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/src/django_bootstrap5/templates/django_bootstrap5/messages.html
--rw-r--r--   0 dylan      (501) staff       (20)     1762 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/src/django_bootstrap5/templates/django_bootstrap5/pagination.html
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-02 09:24:45.577213 django-bootstrap5-23.1/src/django_bootstrap5/templates/django_bootstrap5/widgets/
--rw-r--r--   0 dylan      (501) staff       (20)      895 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/src/django_bootstrap5/templates/django_bootstrap5/widgets/clearable_file_input.html
--rw-r--r--   0 dylan      (501) staff       (20)     1052 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select.html
--rw-r--r--   0 dylan      (501) staff       (20)      670 2022-10-15 06:09:49.000000 django-bootstrap5-23.1/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select_button_group.html
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-02 09:24:45.577693 django-bootstrap5-23.1/src/django_bootstrap5/templatetags/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/src/django_bootstrap5/templatetags/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)    19229 2023-04-02 08:04:04.000000 django-bootstrap5-23.1/src/django_bootstrap5/templatetags/django_bootstrap5.py
--rw-r--r--   0 dylan      (501) staff       (20)      467 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/src/django_bootstrap5/text.py
--rw-r--r--   0 dylan      (501) staff       (20)     1497 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/src/django_bootstrap5/utils.py
--rw-r--r--   0 dylan      (501) staff       (20)      745 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/src/django_bootstrap5/widgets.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-02 09:24:45.575394 django-bootstrap5-23.1/src/django_bootstrap5.egg-info/
--rw-r--r--   0 dylan      (501) staff       (20)     3478 2023-04-02 09:24:45.000000 django-bootstrap5-23.1/src/django_bootstrap5.egg-info/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)    11884 2023-04-02 09:24:45.000000 django-bootstrap5-23.1/src/django_bootstrap5.egg-info/SOURCES.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2023-04-02 09:24:45.000000 django-bootstrap5-23.1/src/django_bootstrap5.egg-info/dependency_links.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2021-12-12 13:27:59.000000 django-bootstrap5-23.1/src/django_bootstrap5.egg-info/not-zip-safe
--rw-r--r--   0 dylan      (501) staff       (20)       12 2023-04-02 09:24:45.000000 django-bootstrap5-23.1/src/django_bootstrap5.egg-info/requires.txt
--rw-r--r--   0 dylan      (501) staff       (20)       18 2023-04-02 09:24:45.000000 django-bootstrap5-23.1/src/django_bootstrap5.egg-info/top_level.txt
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-02 09:24:45.584391 django-bootstrap5-23.1/tests/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/__init__.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-02 09:24:45.624076 django-bootstrap5-23.1/tests/__pycache__/
--rw-r--r--   0 dylan      (501) staff       (20)      150 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      166 2023-03-31 09:33:20.000000 django-bootstrap5-23.1/tests/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      144 2021-12-29 05:53:46.000000 django-bootstrap5-23.1/tests/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      148 2021-12-29 05:54:12.000000 django-bootstrap5-23.1/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      148 2021-12-29 05:54:56.000000 django-bootstrap5-23.1/tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1197 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/base.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1626 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/base.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1177 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/base.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1193 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/base.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1193 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3585 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/image.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3869 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/image.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3569 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/image.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3579 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/image.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3579 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/image.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1982 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_alert.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2974 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_alert.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1962 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_alert.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1976 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_alert.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1996 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_alert.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2693 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_button.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     4389 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_button.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2635 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_button.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2665 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_button.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2685 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_button.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2229 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_css_and_js_tags.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3940 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_css_and_js_tags.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2236 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_css_and_js_tags.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2254 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_css_and_js_tags.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2320 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_css_and_js_tags.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3773 2023-03-31 09:32:41.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     6375 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3847 2023-03-31 09:29:17.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3743 2023-03-31 09:29:27.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3761 2023-03-31 09:31:49.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2839 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_datetime.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3976 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_datetime.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3316 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_datetime.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2929 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_datetime.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2929 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_datetime.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3357 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_checkbox.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     4504 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_checkbox.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3559 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_checkbox.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3425 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_checkbox.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3423 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_checkbox.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2077 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_color.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2930 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_color.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2361 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_color.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2151 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_color.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2151 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_color.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3322 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_file.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     4945 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_file.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3486 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_file.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3416 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_file.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3416 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_file.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2035 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_range.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2889 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_range.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2298 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_range.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2109 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_range.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2109 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_range.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     8815 2022-10-15 06:14:28.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_text.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)    12581 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_text.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     9106 2022-10-15 06:12:15.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_text.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     8791 2022-10-15 06:12:28.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_text.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     8803 2022-10-15 06:13:29.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_input_text.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2745 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_parameters.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3902 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_parameters.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2762 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_parameters.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2741 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_parameters.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2739 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_parameters.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3499 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_radio_select.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     4646 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_radio_select.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     4112 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_radio_select.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3571 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_radio_select.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3571 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_radio_select.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2242 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_select.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3053 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_select.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2316 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_select.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2316 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_select.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2316 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_select.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1631 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_textarea.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2242 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_textarea.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1657 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_textarea.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1665 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_textarea.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1665 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_textarea.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     6178 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_form.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)    10816 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_form.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     6376 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_form.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     6222 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_form.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     6242 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_form.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2283 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_formset.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3226 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_formset.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2267 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_formset.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2253 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_formset.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2273 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_formset.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1078 2023-03-31 09:32:42.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_label.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1610 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_label.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1054 2023-03-31 09:29:17.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_label.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1074 2023-03-31 09:29:27.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_label.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1074 2023-03-31 09:31:49.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_label.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2714 2022-08-05 14:41:59.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_messages.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     4727 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_messages.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2839 2022-08-05 14:39:33.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_messages.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2726 2022-08-05 14:39:49.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_messages.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2730 2022-08-05 14:40:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_messages.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     6482 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_pagination.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)    10889 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_pagination.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     6331 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_pagination.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     6388 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_pagination.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     6460 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_pagination.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2987 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_components.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     4119 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_components.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3049 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_components.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3033 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_components.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3033 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_components.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1375 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_css.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2113 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_css.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1365 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_css.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1371 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_css.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1371 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_css.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      804 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_html.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1319 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_html.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      788 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_html.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      800 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_html.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      800 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_html.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      801 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_settings.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1412 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_settings.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      761 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_settings.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      773 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_settings.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      793 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_settings.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1409 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_size.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     3016 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_size.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1360 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_size.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1357 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_size.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1397 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_size.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1389 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_templates.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2132 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_templates.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1455 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_templates.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1453 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_templates.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1453 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_templates.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      919 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_text.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1683 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_text.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      901 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_text.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      915 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_text.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      915 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_text.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1355 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_urls.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     2603 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_urls.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1317 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_urls.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1325 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_urls.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1345 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_urls.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      690 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/__pycache__/test_version.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      980 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/__pycache__/test_version.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      674 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/__pycache__/test_version.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      686 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/__pycache__/test_version.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      686 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/__pycache__/test_version.cpython-39.pyc
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-02 09:24:45.624562 django-bootstrap5-23.1/tests/app/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/app/__init__.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-02 09:24:45.628138 django-bootstrap5-23.1/tests/app/__pycache__/
--rw-r--r--   0 dylan      (501) staff       (20)      154 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/app/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      170 2023-03-31 09:33:20.000000 django-bootstrap5-23.1/tests/app/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      148 2021-12-29 05:53:46.000000 django-bootstrap5-23.1/tests/app/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      152 2021-12-29 05:54:12.000000 django-bootstrap5-23.1/tests/app/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      152 2021-12-29 05:54:56.000000 django-bootstrap5-23.1/tests/app/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1460 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/app/__pycache__/settings.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1568 2023-03-31 09:33:20.000000 django-bootstrap5-23.1/tests/app/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1472 2021-12-29 05:53:46.000000 django-bootstrap5-23.1/tests/app/__pycache__/settings.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1486 2021-12-29 05:54:12.000000 django-bootstrap5-23.1/tests/app/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1458 2021-12-29 05:54:56.000000 django-bootstrap5-23.1/tests/app/__pycache__/settings.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      164 2021-12-29 05:55:20.000000 django-bootstrap5-23.1/tests/app/__pycache__/urls.cpython-310.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      179 2023-03-31 09:33:21.000000 django-bootstrap5-23.1/tests/app/__pycache__/urls.cpython-311.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      158 2021-12-29 05:53:47.000000 django-bootstrap5-23.1/tests/app/__pycache__/urls.cpython-37.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      162 2021-12-29 05:54:13.000000 django-bootstrap5-23.1/tests/app/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 dylan      (501) staff       (20)      162 2021-12-29 05:54:57.000000 django-bootstrap5-23.1/tests/app/__pycache__/urls.cpython-39.pyc
--rw-r--r--   0 dylan      (501) staff       (20)     1703 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/app/settings.py
--rw-r--r--   0 dylan      (501) staff       (20)       17 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/app/urls.py
--rw-r--r--   0 dylan      (501) staff       (20)      836 2021-12-27 05:56:30.000000 django-bootstrap5-23.1/tests/base.py
--rw-r--r--   0 dylan      (501) staff       (20)     3439 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/image.py
--rw-r--r--   0 dylan      (501) staff       (20)     1595 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/test_bootstrap_alert.py
--rw-r--r--   0 dylan      (501) staff       (20)     2698 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/test_bootstrap_button.py
--rw-r--r--   0 dylan      (501) staff       (20)     2024 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/test_bootstrap_css_and_js_tags.py
--rw-r--r--   0 dylan      (501) staff       (20)     3065 2022-10-15 06:31:02.000000 django-bootstrap5-23.1/tests/test_bootstrap_field.py
--rw-r--r--   0 dylan      (501) staff       (20)     3343 2021-12-27 05:56:30.000000 django-bootstrap5-23.1/tests/test_bootstrap_field_datetime.py
--rw-r--r--   0 dylan      (501) staff       (20)     3521 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/test_bootstrap_field_input_checkbox.py
--rw-r--r--   0 dylan      (501) staff       (20)     2120 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/test_bootstrap_field_input_color.py
--rw-r--r--   0 dylan      (501) staff       (20)     3150 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/test_bootstrap_field_input_file.py
--rw-r--r--   0 dylan      (501) staff       (20)     2003 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/test_bootstrap_field_input_range.py
--rw-r--r--   0 dylan      (501) staff       (20)    12021 2022-10-14 15:03:53.000000 django-bootstrap5-23.1/tests/test_bootstrap_field_input_text.py
--rw-r--r--   0 dylan      (501) staff       (20)     3659 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/test_bootstrap_field_parameters.py
--rw-r--r--   0 dylan      (501) staff       (20)     4590 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/test_bootstrap_field_radio_select.py
--rw-r--r--   0 dylan      (501) staff       (20)     2240 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/test_bootstrap_field_select.py
--rw-r--r--   0 dylan      (501) staff       (20)     1340 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/test_bootstrap_field_textarea.py
--rw-r--r--   0 dylan      (501) staff       (20)     6094 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/test_bootstrap_form.py
--rw-r--r--   0 dylan      (501) staff       (20)     1634 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/test_bootstrap_formset.py
--rw-r--r--   0 dylan      (501) staff       (20)      869 2022-10-15 06:31:02.000000 django-bootstrap5-23.1/tests/test_bootstrap_label.py
--rw-r--r--   0 dylan      (501) staff       (20)     2934 2022-08-05 14:34:59.000000 django-bootstrap5-23.1/tests/test_bootstrap_messages.py
--rw-r--r--   0 dylan      (501) staff       (20)     6815 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/test_bootstrap_pagination.py
--rw-r--r--   0 dylan      (501) staff       (20)     2600 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/test_components.py
--rw-r--r--   0 dylan      (501) staff       (20)      839 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/test_css.py
--rw-r--r--   0 dylan      (501) staff       (20)      511 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/test_html.py
--rw-r--r--   0 dylan      (501) staff       (20)      515 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/test_settings.py
--rw-r--r--   0 dylan      (501) staff       (20)     1149 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/test_size.py
--rw-r--r--   0 dylan      (501) staff       (20)      852 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/test_templates.py
--rw-r--r--   0 dylan      (501) staff       (20)      556 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/test_text.py
--rw-r--r--   0 dylan      (501) staff       (20)     1258 2021-12-12 13:41:53.000000 django-bootstrap5-23.1/tests/test_urls.py
--rw-r--r--   0 dylan      (501) staff       (20)      315 2021-12-12 13:22:34.000000 django-bootstrap5-23.1/tests/test_version.py
--rw-r--r--   0 dylan      (501) staff       (20)     2434 2023-04-02 06:06:13.000000 django-bootstrap5-23.1/tox.ini
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 13:44:45.030165 django-bootstrap5-23.2.dev0/
+-rw-r--r--   0 dylan      (501) staff       (20)      757 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/AUTHORS
+-rw-r--r--   0 dylan      (501) staff       (20)     1533 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/LICENSE
+-rw-r--r--   0 dylan      (501) staff       (20)      281 2023-04-23 08:55:44.000000 django-bootstrap5-23.2.dev0/MANIFEST.in
+-rw-r--r--   0 dylan      (501) staff       (20)     3593 2023-04-28 13:44:45.030238 django-bootstrap5-23.2.dev0/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)     2483 2023-04-28 11:37:05.000000 django-bootstrap5-23.2.dev0/README.md
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 13:44:45.019418 django-bootstrap5-23.2.dev0/docs/
+-rw-r--r--   0 dylan      (501) staff       (20)       30 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/docs/changelog.rst
+-rw-r--r--   0 dylan      (501) staff       (20)     1023 2023-04-28 13:17:05.000000 django-bootstrap5-23.2.dev0/docs/conf.py
+-rw-r--r--   0 dylan      (501) staff       (20)      577 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/docs/example_template.rst
+-rw-r--r--   0 dylan      (501) staff       (20)     3276 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/docs/forms.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      249 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/docs/index.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      585 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/docs/installation.rst
+-rw-r--r--   0 dylan      (501) staff       (20)       28 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/docs/migrate.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      665 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/docs/quickstart.rst
+-rw-r--r--   0 dylan      (501) staff       (20)       62 2023-04-28 13:18:42.000000 django-bootstrap5-23.2.dev0/docs/requirements.txt
+-rw-r--r--   0 dylan      (501) staff       (20)     3275 2022-10-14 14:58:03.000000 django-bootstrap5-23.2.dev0/docs/settings.rst
+-rw-r--r--   0 dylan      (501) staff       (20)     1364 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/docs/templates.rst
+-rw-r--r--   0 dylan      (501) staff       (20)     2217 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/docs/templatetags.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      799 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/docs/widgets.rst
+-rwxr-xr-x   0 dylan      (501) staff       (20)      252 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/manage.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1376 2023-04-28 13:17:05.000000 django-bootstrap5-23.2.dev0/pyproject.toml
+-rw-r--r--   0 dylan      (501) staff       (20)     1129 2023-04-28 13:44:45.030502 django-bootstrap5-23.2.dev0/setup.cfg
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 13:44:45.015115 django-bootstrap5-23.2.dev0/src/
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 13:44:45.021272 django-bootstrap5-23.2.dev0/src/django_bootstrap5/
+-rw-r--r--   0 dylan      (501) staff       (20)       55 2023-04-28 13:44:39.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2351 2022-08-05 14:34:59.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/components.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2692 2023-04-23 08:55:44.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/core.py
+-rw-r--r--   0 dylan      (501) staff       (20)      621 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/css.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1482 2022-10-15 06:32:49.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/forms.py
+-rw-r--r--   0 dylan      (501) staff       (20)      870 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/html.py
+-rw-r--r--   0 dylan      (501) staff       (20)    21153 2022-11-22 12:41:26.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/renderers.py
+-rw-r--r--   0 dylan      (501) staff       (20)      901 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/size.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 13:44:45.015227 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 13:44:45.023075 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/
+-rw-r--r--   0 dylan      (501) staff       (20)     1079 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/bootstrap5.html
+-rw-r--r--   0 dylan      (501) staff       (20)       95 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/field_errors.html
+-rw-r--r--   0 dylan      (501) staff       (20)       79 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/field_help_text.html
+-rw-r--r--   0 dylan      (501) staff       (20)      122 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/form_errors.html
+-rw-r--r--   0 dylan      (501) staff       (20)      206 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/messages.html
+-rw-r--r--   0 dylan      (501) staff       (20)     1762 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/pagination.html
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 13:44:45.023568 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/widgets/
+-rw-r--r--   0 dylan      (501) staff       (20)      895 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/widgets/clearable_file_input.html
+-rw-r--r--   0 dylan      (501) staff       (20)     1052 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select.html
+-rw-r--r--   0 dylan      (501) staff       (20)      670 2022-10-15 06:09:49.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select_button_group.html
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 13:44:45.024008 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templatetags/
+-rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templatetags/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)    19229 2023-04-02 08:04:04.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templatetags/django_bootstrap5.py
+-rw-r--r--   0 dylan      (501) staff       (20)      467 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/text.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1497 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/utils.py
+-rw-r--r--   0 dylan      (501) staff       (20)      745 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/widgets.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 13:44:45.022189 django-bootstrap5-23.2.dev0/src/django_bootstrap5.egg-info/
+-rw-r--r--   0 dylan      (501) staff       (20)     3593 2023-04-28 13:44:45.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5.egg-info/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)     2693 2023-04-28 13:44:45.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2023-04-28 13:44:45.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2021-12-12 13:27:59.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5.egg-info/not-zip-safe
+-rw-r--r--   0 dylan      (501) staff       (20)       12 2023-04-28 13:44:45.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5.egg-info/requires.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       18 2023-04-28 13:44:45.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5.egg-info/top_level.txt
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 13:44:45.029483 django-bootstrap5-23.2.dev0/tests/
+-rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/__init__.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 13:44:45.029925 django-bootstrap5-23.2.dev0/tests/app/
+-rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/app/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1703 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/app/settings.py
+-rw-r--r--   0 dylan      (501) staff       (20)       17 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/app/urls.py
+-rw-r--r--   0 dylan      (501) staff       (20)      836 2021-12-27 05:56:30.000000 django-bootstrap5-23.2.dev0/tests/base.py
+-rw-r--r--   0 dylan      (501) staff       (20)     3439 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/image.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1595 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_alert.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2698 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_button.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2024 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_css_and_js_tags.py
+-rw-r--r--   0 dylan      (501) staff       (20)     3065 2022-10-15 06:31:02.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_field.py
+-rw-r--r--   0 dylan      (501) staff       (20)     3343 2021-12-27 05:56:30.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_datetime.py
+-rw-r--r--   0 dylan      (501) staff       (20)     3521 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_input_checkbox.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2120 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_input_color.py
+-rw-r--r--   0 dylan      (501) staff       (20)     3150 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_input_file.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2003 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_input_range.py
+-rw-r--r--   0 dylan      (501) staff       (20)    12018 2023-04-23 08:55:44.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_input_text.py
+-rw-r--r--   0 dylan      (501) staff       (20)     3657 2023-04-23 08:55:44.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_parameters.py
+-rw-r--r--   0 dylan      (501) staff       (20)     4590 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_radio_select.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2240 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_select.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1340 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_textarea.py
+-rw-r--r--   0 dylan      (501) staff       (20)     6094 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_form.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1634 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_formset.py
+-rw-r--r--   0 dylan      (501) staff       (20)      869 2022-10-15 06:31:02.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_label.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2934 2022-08-05 14:34:59.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_messages.py
+-rw-r--r--   0 dylan      (501) staff       (20)     6807 2023-04-25 10:31:45.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_pagination.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2600 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_components.py
+-rw-r--r--   0 dylan      (501) staff       (20)      839 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_css.py
+-rw-r--r--   0 dylan      (501) staff       (20)      511 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_html.py
+-rw-r--r--   0 dylan      (501) staff       (20)      515 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_settings.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1149 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_size.py
+-rw-r--r--   0 dylan      (501) staff       (20)      852 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_templates.py
+-rw-r--r--   0 dylan      (501) staff       (20)      556 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_text.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1257 2023-04-23 08:55:44.000000 django-bootstrap5-23.2.dev0/tests/test_urls.py
+-rw-r--r--   0 dylan      (501) staff       (20)      315 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_version.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2033 2023-04-28 13:20:24.000000 django-bootstrap5-23.2.dev0/tox.ini
```

### Comparing `django-bootstrap5-23.1/AUTHORS` & `django-bootstrap5-23.2.dev0/AUTHORS`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/LICENSE` & `django-bootstrap5-23.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/PKG-INFO` & `django-bootstrap5-23.2.dev0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: django-bootstrap5
-Version: 23.1
+Version: 23.2.dev0
 Summary: Bootstrap 5 for Django
 Home-page: https://github.com/zostera/django-bootstrap5
 Author: Dylan Verheul
 Author-email: dylan@dyve.net
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -43,15 +43,17 @@
 
 ## Status
 
 Ready for production. Issues and pull requests welcome, see [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## Requirements
 
-Python 3.7 or newer with Django 3.2 or newer.
+This package requires a combination of Python and Django that is currently supported.
+
+See "Supported Versions" on https://www.djangoproject.com/download/.
 
 ## Documentation
 
 The full documentation is at https://django-bootstrap5.readthedocs.io/
 
 ## Installation
```

### Comparing `django-bootstrap5-23.1/README.md` & `django-bootstrap5-23.2.dev0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 
 ## Status
 
 Ready for production. Issues and pull requests welcome, see [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## Requirements
 
-Python 3.7 or newer with Django 3.2 or newer.
+This package requires a combination of Python and Django that is currently supported.
+
+See "Supported Versions" on https://www.djangoproject.com/download/.
 
 ## Documentation
 
 The full documentation is at https://django-bootstrap5.readthedocs.io/
 
 ## Installation
```

### Comparing `django-bootstrap5-23.1/docs/example_template.rst` & `django-bootstrap5-23.2.dev0/docs/example_template.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/docs/forms.rst` & `django-bootstrap5-23.2.dev0/docs/forms.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/docs/installation.rst` & `django-bootstrap5-23.2.dev0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/docs/quickstart.rst` & `django-bootstrap5-23.2.dev0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/docs/settings.rst` & `django-bootstrap5-23.2.dev0/docs/settings.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/docs/templates.rst` & `django-bootstrap5-23.2.dev0/docs/templates.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/docs/templatetags.rst` & `django-bootstrap5-23.2.dev0/docs/templatetags.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/docs/widgets.rst` & `django-bootstrap5-23.2.dev0/docs/widgets.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/setup.cfg` & `django-bootstrap5-23.2.dev0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [metadata]
 name = django-bootstrap5
-version = attr:django_bootstrap5.__version__
+version = 23.2dev
 description = Bootstrap 5 for Django
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/zostera/django-bootstrap5
 author = Dylan Verheul
 author_email = dylan@dyve.net
 license = BSD-3-Clause
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 3.2
-	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
```

### Comparing `django-bootstrap5-23.1/src/django_bootstrap5/components.py` & `django-bootstrap5-23.2.dev0/src/django_bootstrap5/components.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/src/django_bootstrap5/core.py` & `django-bootstrap5-23.2.dev0/src/django_bootstrap5/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 
     Lookup order is:
 
     1. Django settings
     2. `django-bootstrap5` defaults
     3. Given default value
     """
-
     bootstrap5_settings = getattr(settings, "BOOTSTRAP5", {})
     return bootstrap5_settings.get(name, BOOTSTRAP5_DEFAULTS.get(name, default))
 
 
 def javascript_url():
     """Return the full url to the Bootstrap JavaScript file."""
     return get_bootstrap_setting("javascript_url")
```

### Comparing `django-bootstrap5-23.1/src/django_bootstrap5/css.py` & `django-bootstrap5-23.2.dev0/src/django_bootstrap5/css.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/src/django_bootstrap5/forms.py` & `django-bootstrap5-23.2.dev0/src/django_bootstrap5/forms.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/src/django_bootstrap5/html.py` & `django-bootstrap5-23.2.dev0/src/django_bootstrap5/html.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/src/django_bootstrap5/renderers.py` & `django-bootstrap5-23.2.dev0/src/django_bootstrap5/renderers.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/src/django_bootstrap5/size.py` & `django-bootstrap5-23.2.dev0/src/django_bootstrap5/size.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/src/django_bootstrap5/templates/django_bootstrap5/bootstrap5.html` & `django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/bootstrap5.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/src/django_bootstrap5/templates/django_bootstrap5/pagination.html` & `django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/pagination.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/src/django_bootstrap5/templates/django_bootstrap5/widgets/clearable_file_input.html` & `django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/widgets/clearable_file_input.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select.html` & `django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select_button_group.html` & `django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select_button_group.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/src/django_bootstrap5/templatetags/django_bootstrap5.py` & `django-bootstrap5-23.2.dev0/src/django_bootstrap5/templatetags/django_bootstrap5.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/src/django_bootstrap5/utils.py` & `django-bootstrap5-23.2.dev0/src/django_bootstrap5/utils.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/src/django_bootstrap5/widgets.py` & `django-bootstrap5-23.2.dev0/src/django_bootstrap5/widgets.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/src/django_bootstrap5.egg-info/PKG-INFO` & `django-bootstrap5-23.2.dev0/src/django_bootstrap5.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: django-bootstrap5
-Version: 23.1
+Version: 23.2.dev0
 Summary: Bootstrap 5 for Django
 Home-page: https://github.com/zostera/django-bootstrap5
 Author: Dylan Verheul
 Author-email: dylan@dyve.net
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -43,15 +43,17 @@
 
 ## Status
 
 Ready for production. Issues and pull requests welcome, see [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## Requirements
 
-Python 3.7 or newer with Django 3.2 or newer.
+This package requires a combination of Python and Django that is currently supported.
+
+See "Supported Versions" on https://www.djangoproject.com/download/.
 
 ## Documentation
 
 The full documentation is at https://django-bootstrap5.readthedocs.io/
 
 ## Installation
```

### Comparing `django-bootstrap5-23.1/tests/__pycache__/image.cpython-310.pyc` & `django-bootstrap5-23.2.dev0/tests/image.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,225 +1,215 @@
-00000000: 6f0d 0d0a 0000 0000 9af7 b561 6f0d 0000  o..........ao...
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
-00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6404  ..d.d.l.m.Z...d.
-00000050: a005 a100 5a06 6405 6406 8400 5a07 6401  ....Z.d.d...Z.d.
-00000060: 5300 2907 e900 0000 004e 2901 da07 4279  S.)......N)...By
-00000070: 7465 7349 4f29 01da 1449 6e4d 656d 6f72  tesIO)...InMemor
-00000080: 7955 706c 6f61 6465 6446 696c 6561 b40b  yUploadedFilea..
-00000090: 0000 0a69 5642 4f52 7730 4b47 676f 4141  ...iVBORw0KGgoAA
-000000a0: 4141 4e53 5568 4555 6741 4141 4241 4141  AANSUhEUgAAABAAA
-000000b0: 4141 5143 4159 4141 4141 6638 2f39 6841  AAQCAYAAAAf8/9hA
-000000c0: 4141 4142 6d4a 4c52 3051 412f 7744 2f41  AAABmJLR0QA/wD/A
-000000d0: 502b 6776 6165 5441 4141 4143 5842 490a  P+gvaeTAAAACXBI.
-000000e0: 5758 4d41 4141 4249 4141 4141 5341 4247  WXMAAABIAAAASABG
-000000f0: 7957 732b 4141 4141 4358 5a77 5157 6341  yWs+AAAACXZwQWcA
-00000100: 4141 4151 4141 4141 4541 4263 7871 3344  AAAQAAAAEABcxq3D
-00000110: 4141 4142 6645 6c45 5156 5134 7935 3254  AAABfElEQVQ4y52T
-00000120: 7655 7543 5552 5447 6635 5a67 0a39 676f  vUuCURTGf5Zg.9go
-00000130: 5239 4156 6c55 5a4a 394b 5552 7555 6b68  R9AVlUZJ9KURuUkh
-00000140: 4955 4550 5155 4975 6252 4674 494a 546b  IUEPQUIubRFtIJTk
-00000150: 304e 546b 5546 6667 6e74 4155 7430 6542  0NTkUFfgntAUt0eB
-00000160: 5351 7752 4b52 4653 5942 5946 6c31 4741  SQwRKRFSYBYFl1GA
-00000170: 7439 3031 6555 5975 770a 5154 4c4d 3179  t901eUYuw.QTLM1y
-00000180: 4c50 6473 2f7a 5044 2f75 5059 6572 6559  LPds/zPD/uPYereY
-00000190: 6a48 6377 442b 7451 332b 5579 732b 4c77  jHcwD+tQ3+Uys+Lw
-000001a0: 4361 6833 6738 3531 6c61 2f6c 6634 7177  Cah3g851la/lf4qw
-000001b0: 4b62 3631 536e 337a 3557 4655 5770 4348  Kb61Sn3z5WFUWpCH
-000001c0: 422b 4755 4762 0a53 4352 4970 564b 7142  B+GUGb.SCRIpVKqB
-000001d0: 6b6d 5341 4d72 7173 5669 4d71 6e49 6977  kmSAMrqsViMqnIiw
-000001e0: 4c78 3748 4f2f 552b 362b 3330 4759 7961  Lx7HO/U+6+30GYya
-000001f0: 5658 4250 3175 4872 6655 4157 7657 4d57  VXBP1uHrfUAWvWMW
-00000200: 6946 342b 716f 4f55 4a4c 4a6b 7562 5963  iF4+qoOUJLJkubYc
-00000210: 4473 320a 5330 3368 764f 4453 4537 3536  Ds2.S03hvODSE756
-00000220: 3465 6b35 572b 4b74 2b74 6c6f 6139 6178  4ek5W+Kt+tloa9ax
-00000230: 3676 344f 5a2b 2b6a 5a4f 2b6a 624d 2b70  6v4OZ++jZO+jbM+p
-00000240: 4437 6f45 3448 4d31 6c58 3176 594e 476f  D7oE4HM1lX1vYNGo
-00000250: 4468 4379 514d 6943 4761 6352 6d30 5666  DhCyQMiCGacRm0Vf
-00000260: 0a45 4d2b 7569 7564 6a6b 6536 5963 526f  .EM+uiudjke6YcRo
-00000270: 4c66 6945 4c4e 4232 6458 546b 4161 3038  LfiELNB2dXTkAa08
-00000280: 4c50 6c63 5432 6670 4a41 4d78 575a 3148  LPlcT2fpJAMxWZ1H
-00000290: 344e 6e4b 4954 7577 4434 4e6c 3652 4d67  4NnKITuwD4Nl6RMg
-000002a0: 4341 4531 4459 3350 7579 7951 5a0a 4a4c  CAE1DY3PuyyQZ.JL
-000002b0: 724e 765a 684d 4a67 436d 4a77 5942 3241  rNvZhMJgCmJwYB2A
-000002c0: 3165 4148 4153 4469 466b 5155 7235 586e  1eAHASDiFkQUr5Xn
-000002d0: 3052 6f4a 4c53 4467 375a 4342 3066 5652  0RoJLSDg7ZCB0fVR
-000002e0: 5132 392f 546d 5031 4e66 2f30 4246 674c  Q29/TmP1Nf/0BFgL
-000002f0: 3264 5148 344c 4e39 6452 0a37 434d 4f61  2dQH4LN9dR.7CMOa
-00000300: 6958 446e 3646 6179 5942 3978 4d48 6554  iXDn6FayYB9xMHeT
-00000310: 6743 7a31 636b 6e64 2b57 4333 5667 546f  gCz1cknd+WC3VgTo
-00000320: 7255 4141 4141 6c64 4556 5964 474e 795a  rUAAAAldEVYdGNyZ
-00000330: 5746 305a 5331 6b59 5852 6c41 4449 774d  WF0ZS1kYXRlADIwM
-00000340: 5441 744d 5449 740a 4d6a 5a55 4d54 5136  TAtMTIt.MjZUMTQ6
-00000350: 4e44 6b36 4d6a 4572 4d44 6b36 4d44 4148  NDk6MjErMDk6MDAH
-00000360: 4842 4231 4141 4141 4a58 5246 5748 5274  HBB1AAAAJXRFWHRt
-00000370: 6232 5270 5a6e 6b74 5a47 4630 5a51 4179  b2RpZnktZGF0ZQAy
-00000380: 4d44 4577 4c54 4579 4c54 4932 5644 4530  MDEwLTEyLTI2VDE0
-00000390: 4f6a 5135 0a4f 6a49 784b 7a41 354f 6a41  OjQ5.OjIxKzA5OjA
-000003a0: 7757 4b31 6d51 5141 4141 4142 4a52 5535  wWK1mQQAAAABJRU5
-000003b0: 4572 6b4a 6767 6f6c 5154 6b63 4e43 686f  ErkJggolQTkcNCho
-000003c0: 4b41 4141 4144 556c 4952 4649 4141 4141  KAAAADUlIRFIAAAA
-000003d0: 5141 4141 4145 4167 4741 4141 4148 2f50  QAAAAEAgGAAAAH/P
-000003e0: 2f0a 5951 4141 4141 5a69 5330 6445 4150  /.YQAAAAZiS0dEAP
-000003f0: 3841 2f77 442f 6f4c 326e 6b77 4141 4141  8A/wD/oL2nkwAAAA
-00000400: 6c77 5346 6c7a 4141 4141 5341 4141 4145  lwSFlzAAAASAAAAE
-00000410: 6741 5273 6c72 5067 4141 4141 6c32 6345  gARslrPgAAAAl2cE
-00000420: 466e 4141 4141 4541 4141 4142 4141 0a58  FnAAAAEAAAABAA.X
-00000430: 4d61 7477 7741 4141 6864 4a52 4546 554f  MatwwAAAhdJREFUO
-00000440: 4d75 566b 3831 4c56 4645 5978 6e2f 337a  MuVk81LVFEYxn/3z
-00000450: 6f63 6671 5665 6255 6243 7954 4c79 5952  ocfqVebUbCyTLyYR
-00000460: 5977 4430 6365 6d43 4952 7955 5654 6f4c  YwD0cemCIRyUVToL
-00000470: 6c6f 4552 5546 4262 5970 6f0a 4537 5749  loERUFBbYpo.E7WI
-00000480: 4676 3054 4c61 5036 4332 5931 376f 5957  Fv0TLaP6C2Y17oYW
-00000490: 5751 7852 4d77 6f35 4f55 706c 6b52 2f58  WQxRMwo5OUplkR/X
-000004a0: 4f65 664d 7557 384c 4e59 795a 4c42 3934  OefMuW8LNYyZLB94
-000004b0: 654f 4535 4c37 397a 7a6e 7334 6a6f 6849  eOE5L79zzns4johI
-000004c0: 5070 2f6e 2b59 7458 0a66 506e 366a 6171  Pp/n+YtX.fPn6jaq
-000004d0: 3162 4b61 4936 354c 5933 7348 6f68 584f  1bKaI65LY3sHohXO
-000004e0: 6b30 326d 634e 784d 5438 766a 4a55 3554  k02mcNxMT8vjJU5T
-000004f0: 5762 4555 4e38 5469 3362 6c34 6e30 744c  WbEUN8Ti3bl4n0tL
-00000500: 572f 7142 636e 6957 306c 7442 6178 4672  W/qBcniW0ltBaxFr
-00000510: 7357 6c33 500a 3749 5a38 5064 4e61 3832  sWl3P.7IZ8PdNa82
-00000520: 6d36 5250 5444 7879 4c47 6d4c 7137 4a44  m6RPTDxyLGmLq7JD
-00000530: 7561 7156 5143 6c6c 6271 6e36 4934 4f55  uaqVQCllbqn6I4OU
-00000540: 5530 434a 594a 7737 426d 4d52 364c 6350  U0CJYJw7BmMR6LcP
-00000550: 7679 5552 624c 4752 3439 712f 3731 4b6c  vyURbLGR49q/71Kl
-00000560: 476a 0a64 5633 416c 6245 6842 6e6f 6733  Gj.dV3AlbEhBnog3
-00000570: 6d6f 3565 3854 7963 727a 2b63 4b50 616d  mo5e8Tycrz+cKPam
-00000580: 4272 4169 554f 646e 442f 5a68 6c46 7a69  BrAiUOdnD/ZhlFzi
-00000590: 4b70 7737 5253 384c 5672 7930 3149 4463  Kpw7RS8LVry01IDc
-000005a0: 4933 5762 4852 5875 384f 6453 3532 340a  I3WbHRXu8OdS524.
-000005b0: 7067 7836 426c 6b4a 454b 5734 5078 7253  pgx6BlkJEKW4PxrS
-000005c0: 4650 327a 3132 694e 7131 5546 7254 5661  FP2z12iNq1UFrTVa
-000005d0: 6178 444e 7736 7674 7444 584d 672f 324f  axDNw6vttDXMg/2O
-000005e0: 3241 5843 3555 556b 574b 4937 7673 4464  2AXC5UUkWKI7vsDd
-000005f0: 4d2b 5a33 5839 5773 3274 5847 0a59 4c54  M+Z3X9Ws2tXG.YLT
-00000600: 4361 4d57 4e4d 5938 4466 5245 4146 7063  CaMWNMY8DfREAFpc
-00000610: 556b 7a50 4331 4a7a 4c38 6b4b 4147 4d33  UkzPC1JzL8kKAGM3
-00000620: 7876 6f44 442b 3175 4a56 582b 696c 4549  xvoDD+1uJVX+ilEI
-00000630: 7074 5470 4543 5550 3850 5845 4742 2f72  ptTpECUP8PXEGB/r
-00000640: 497a 772f 694e 5058 6a0a 6465 316a 4d4c  Izw/iNPXj.de1jML
-00000650: 3058 6179 336c 3651 4b66 5a79 6577 5039  0Xay3l6QKfZyewP9
-00000660: 3578 3864 6872 3772 3048 7053 6f41 4f44  5x8dhr7r0HpSoAOD
-00000670: 7437 646b 746f 5130 5345 7073 5a47 656e  t7dktoQ0SEpsZGen
-00000680: 7437 3866 312b 664e 2f48 392f 7378 786c  t78f1+fN/H9/sxxl
-00000690: 416f 4643 6b55 0a43 7851 4b52 5571 6c45  AoFCkU.CxQKRUqlE
-000006a0: 6b70 7058 4e64 6442 5854 7632 4358 7274  kppXNddBXTv2CXrt
-000006b0: 482f 4a6f 6659 566f 716e 5551 624c 5a38  H/JofYVoqnUQbLZ8
-000006c0: 662f 2b41 3835 6146 5741 6f6c 594a 634c  f/+A85aFWAolYJcL
-000006d0: 6965 6535 306b 7346 7475 536d 3765 3153  iee50ksFtuSm7e1S
-000006e0: 4361 540a 4555 5245 6372 6d63 6e42 345a  CaT.EUREcrmcnB4Z
-000006f0: 6b57 5179 4b5a 376e 6265 7045 4969 4844  kWQyKZ7nbepEIiHD
-00000700: 7738 4f53 7a57 5a46 524f 5158 3650 705a  w8OSzWZFROQX6PpZ
-00000710: 4678 4174 5338 4941 4141 416c 6445 5659  FxAtS8IAAAAldEVY
-00000720: 6447 4e79 5a57 4630 5a53 316b 5958 526c  dGNyZWF0ZS1kYXRl
-00000730: 0a41 4449 774d 5441 744d 5449 744d 6a5a  .ADIwMTAtMTItMjZ
-00000740: 554d 5451 364e 446b 364d 6a45 724d 446b  UMTQ6NDk6MjErMDk
-00000750: 364d 4441 4848 4242 3141 4141 414a 5852  6MDAHHBB1AAAAJXR
-00000760: 4657 4852 7462 3252 705a 6e6b 745a 4746  FWHRtb2RpZnktZGF
-00000770: 305a 5141 794d 4445 774c 5445 790a 4c54  0ZQAyMDEwLTEy.LT
-00000780: 4932 5644 4530 4f6a 5135 4f6a 4978 4b7a  I2VDE0OjQ5OjIxKz
-00000790: 4135 4f6a 4177 574b 316d 5151 4141 4141  A5OjAwWK1mQQAAAA
-000007a0: 424a 5255 3545 726b 4a67 676f 6c51 546b  BJRU5ErkJggolQTk
-000007b0: 634e 4368 6f4b 4141 4141 4455 6c49 5246  cNChoKAAAADUlIRF
-000007c0: 4941 4141 4151 4141 4141 0a45 4167 4741  IAAAAQAAAA.EAgGA
-000007d0: 4141 4148 2f50 2f59 5141 4141 415a 6953  AAAH/P/YQAAAAZiS
-000007e0: 3064 4541 5038 412f 7744 2f6f 4c32 6e6b  0dEAP8A/wD/oL2nk
-000007f0: 7741 4141 416c 7753 466c 7a41 4141 4153  wAAAAlwSFlzAAAAS
-00000800: 4141 4141 4567 4152 736c 7250 6741 4141  AAAAEgARslrPgAAA
-00000810: 416c 3263 4546 6e0a 4141 4141 4541 4141  Al2cEFn.AAAAEAAA
-00000820: 4142 4141 584d 6174 7777 4141 416f 394a  ABAAXMatwwAAAo9J
-00000830: 5245 4655 4f4d 754e 6b73 3172 5647 6355  REFUOMuNks1rVGcU
-00000840: 786e 2f76 652b 396b 5575 4f64 6649 7a61  xn/ve+9kUuOdfIza
-00000850: 6d4e 4845 4d4b 3352 5649 4c51 5141 7543  mNHEMK3RVILQQAuC
-00000860: 5755 526f 0a72 5341 7462 7356 3230 542f  WURo.rSAtbsV20T/
-00000870: 4550 364f 3746 7478 6b6b 5957 514b 4b37  EP6O7FtxkkYWQKK7
-00000880: 4634 4b62 3143 3679 6f53 5672 4e64 4449  F4Kb1C6yoSVrNdDI
-00000890: 6d31 5954 4d6a 4450 3376 6663 3970 3475  m1YTMjDP3vfc9p4u
-000008a0: 625a 4559 6f70 5163 6544 6877 4f44 3839  bZEYopQceDhwOD89
-000008b0: 7a0a 7a6d 4f38 392f 7277 3053 4e75 3362  z.zmO89/rw0SNu3b
-000008c0: 3544 3561 3871 3367 7637 5a58 6137 646b  5D5a8q3gv7ZXa7dk
-000008d0: 5932 7349 774d 6638 7733 5833 2f46 3950  Y2sIwMf8w3X3/F9P
-000008e0: 546e 684c 2f2b 396f 4366 6637 6e42 6571  TnhL/+9oCff7nBeq
-000008f0: 3247 4d59 622f 5535 7362 6d31 5458 0a61  2GMYb/U5sbm1TX.a
-00000900: 3854 4f45 5177 4d48 6271 2b76 4c4b 4b71  8TOEQwMHbq+vLKKq
-00000910: 7149 6969 4168 2b72 3374 4276 4b42 6473  qIiiAh+r3tBvKBds
-00000920: 3732 6465 7231 4f74 566f 6c66 5037 3842  72der1OtVolfP78B
-00000930: 576d 6164 6d6e 4e56 4b67 7149 3063 4f6b  WmadmnNVKgqI0cOk
-00000940: 6952 744e 7263 395a 7439 480a 7839 664b  iRtNrc9Zt9H.x9fK
-00000950: 3669 7068 732f 6b65 5666 6c41 6f71 7053  6iphs/keVflAoqpS
-00000960: 484f 7a6a 682b 386d 614c 3539 796b 3833  HOzjh+8maL59yk83
-00000970: 577a 5261 3847 384f 777a 5278 6948 5149  WzRa8G8OwzRxiHQI
-00000980: 464f 6a4a 4258 7737 4f38 6230 7156 3530  FOjJBXw7O8b0qV50
-00000990: 4b32 4831 7457 662b 0a72 6943 6948 5262  K2H1tWf+.riCiHRb
-000009a0: 4e46 4955 7563 5967 6f5a 752f 5971 6c7a  NFIUucYgoZu/Yqlz
-000009b0: 3434 6969 587a 6833 4570 4a75 4530 754c  44iiXzh3EpJuE0uL
-000009c0: 4b6c 3537 6c4e 632f 3933 7756 6a4f 7959  Kl57lNc/93wVjOyY
-000009d0: 7941 7065 6775 7770 456c 544f 6639 4848  yApeguwpElTOf9HH
-000009e0: 3159 6b53 550a 6530 4f37 3263 432f 6231  1YkSU.e0O72cC/b1
-000009f0: 444d 4b39 2f50 4750 3563 3937 7a61 5547  DMK9/PGP5c97zaUG
-00000a00: 7758 6730 3163 6a48 4d78 6352 777a 3043  wXg01cjHMxcRwz0C
-00000a10: 6638 6550 6b41 4a34 3755 3065 5276 534c  f8ePkAJ47U0eRvSL
-00000a20: 6568 7459 4d30 3670 772b 314f 5461 755a  ehtYM06pw+1OTauZ
-00000a30: 6a65 0a77 4247 376d 4354 4a45 4471 5833  je.wBG7mCTJEDqX3
-00000a40: 6543 6a76 4f58 7178 5147 6d54 7758 556d  eCjvOXqxQGmTwXUm
-00000a50: 776c 786d 6d64 7270 772b 7a30 7962 6948  wlxmmdrpw+z0ybiH
-00000a60: 586e 6259 7161 7376 4467 6263 4750 4a45  XnbYqasvDgbcGPJE
-00000a70: 7676 7348 4b46 7a44 7039 3654 677a 330a  vvsHKFzDp96Tgz3.
-00000a80: 6376 6a77 4d4d 2f65 6673 6142 775a 5030  cvjwMM/efsaBwZP0
-00000a90: 4433 394b 6162 4b45 7067 6e62 4733 2f77  D39KabKEpgnbG3/w
-00000aa0: 7276 6155 3570 736e 4844 2f36 6d4d 4638  rvaU5psnHD/6mMF8
-00000ab0: 6a63 7157 7752 6777 7057 4f6a 4b69 4c6b  jcqWwRgwpWOjKiLk
-00000ac0: 516b 4f68 7635 2b78 7354 4c6c 0a63 706e  QkOhv5+xsTLl.cpn
-00000ad0: 5230 574f 5553 6956 4568 4c56 4b68 6258  R0WOUSiVEhLVKhbX
-00000ae0: 5861 3778 6358 7148 7961 6f56 366f 3048  Xa7xcXqHyaoV6o0H
-00000af0: 7164 314d 7855 6a71 7537 5859 4c4d 466b  qd1MxUjqu7XYLMFk
-00000b00: 614e 5874 5859 4330 392b 5235 5577 626b  aNXtXYC09+R5Uwbk
-00000b10: 5945 6356 6169 7a46 6d0a 502f 4c57 4773  YEcVaizFm.P/LWGs
-00000b20: 4c4a 7964 4d73 3356 7643 576b 5033 677a  LJydMs3VvCWkP3gz
-00000b30: 784b 374f 4b75 3742 6c38 312f 7445 684b  xK7OKu7Bl81/tEhK
-00000b40: 6d70 4b56 6859 574e 434a 6951 6b4e 676c  mpKVhYWNCJiQkNgl
-00000b50: 4444 4d4b 6468 4c70 6631 2f30 4151 6844  DDMKdhLpf1/0AQhD
-00000b60: 6f2b 5071 357a 0a63 334e 4b6d 7161 3675  o+Pq5z.c3NKmqa6u
-00000b70: 4c69 6f73 374d 5874 4667 7361 6852 4647  Lios7MXtFgsahRFG
-00000b80: 6855 4b48 5553 374b 4251 3069 6949 6447  hUKHUS7KBQ0iiIdG
-00000b90: 6872 5338 2b64 6e64 4835 2b58 704d 6b30  hrS8+dndH5+XpMk0
-00000ba0: 5838 414d 5456 782f 696e 7055 3463 4141  X8AMTVx/inpU4cAA
-00000bb0: 4141 6c0a 6445 5659 6447 4e79 5a57 4630  AAl.dEVYdGNyZWF0
-00000bc0: 5a53 316b 5958 526c 4144 4977 4d54 4174  ZS1kYXRlADIwMTAt
-00000bd0: 4d54 4974 4d6a 5a55 4d54 5136 4e44 6b36  MTItMjZUMTQ6NDk6
-00000be0: 4d6a 4572 4d44 6b36 4d44 4148 4842 4231  MjErMDk6MDAHHBB1
-00000bf0: 4141 4141 4a58 5246 5748 5274 6232 5270  AAAAJXRFWHRtb2Rp
-00000c00: 0a5a 6e6b 745a 4746 305a 5141 794d 4445  .ZnktZGF0ZQAyMDE
-00000c10: 774c 5445 794c 5449 3256 4445 304f 6a51  wLTEyLTI2VDE0OjQ
-00000c20: 354f 6a49 784b 7a41 354f 6a41 7757 4b31  5OjIxKzA5OjAwWK1
-00000c30: 6d51 5141 4141 4142 4a52 5535 4572 6b4a  mQQAAAABJRU5ErkJ
-00000c40: 6767 673d 3d0a 6300 0000 0000 0000 0000  ggg==.c.........
-00000c50: 0000 0000 0000 0008 0000 0043 0000 0073  ...........C...s
-00000c60: 2200 0000 7400 7401 7402 a003 7404 a101  "...t.t.t...t...
-00000c70: 8301 6401 6402 6403 7405 7404 8301 6404  ..d.d.d.t.t...d.
-00000c80: 6405 8d06 5300 2906 4eda 0874 656d 7066  d...S.).N..tempf
-00000c90: 696c 657a 0c74 656d 7066 696c 652e 706e  ilez.tempfile.pn
-00000ca0: 677a 0969 6d61 6765 2f70 6e67 7a05 7574  gz.image/pngz.ut
-00000cb0: 662d 3829 05da 0a66 6965 6c64 5f6e 616d  f-8)...field_nam
-00000cc0: 65da 046e 616d 65da 0c63 6f6e 7465 6e74  e..name..content
-00000cd0: 5f74 7970 65da 0473 697a 65da 0763 6861  _type..size..cha
-00000ce0: 7273 6574 2906 7203 0000 0072 0200 0000  rset).r....r....
-00000cf0: da06 6261 7365 3634 da09 6236 3464 6563  ..base64..b64dec
-00000d00: 6f64 65da 0a54 4553 545f 494d 4147 45da  ode..TEST_IMAGE.
-00000d10: 036c 656e a900 720e 0000 0072 0e00 0000  .len..r....r....
-00000d20: fa36 2f55 7365 7273 2f64 796c 616e 2f50  .6/Users/dylan/P
-00000d30: 726f 6a65 6374 732f 646a 616e 676f 2d62  rojects/django-b
-00000d40: 6f6f 7473 7472 6170 352f 7465 7374 732f  ootstrap5/tests/
-00000d50: 696d 6167 652e 7079 da0e 6765 745f 7465  image.py..get_te
-00000d60: 7374 5f69 6d61 6765 3300 0000 7310 0000  st_image3...s...
-00000d70: 0002 010c 0102 0102 0102 0106 0102 0106  ................
-00000d80: fa72 1000 0000 2908 720a 0000 00da 0269  .r....).r......i
-00000d90: 6f72 0200 0000 da1e 646a 616e 676f 2e63  or......django.c
-00000da0: 6f72 652e 6669 6c65 732e 7570 6c6f 6164  ore.files.upload
-00000db0: 6564 6669 6c65 7203 0000 00da 0573 7472  edfiler......str
-00000dc0: 6970 720c 0000 0072 1000 0000 720e 0000  ipr....r....r...
-00000dd0: 0072 0e00 0000 720e 0000 0072 0f00 0000  .r....r....r....
-00000de0: da08 3c6d 6f64 756c 653e 0100 0000 730e  ..<module>....s.
-00000df0: 0000 0008 000c 010c 0202 0404 2802 d80c  ............(...
-00000e00: 2b                                       +
+00000000: 696d 706f 7274 2062 6173 6536 340a 6672  import base64.fr
+00000010: 6f6d 2069 6f20 696d 706f 7274 2042 7974  om io import Byt
+00000020: 6573 494f 0a0a 6672 6f6d 2064 6a61 6e67  esIO..from djang
+00000030: 6f2e 636f 7265 2e66 696c 6573 2e75 706c  o.core.files.upl
+00000040: 6f61 6465 6466 696c 6520 696d 706f 7274  oadedfile import
+00000050: 2049 6e4d 656d 6f72 7955 706c 6f61 6465   InMemoryUploade
+00000060: 6446 696c 650a 0a23 2053 6f75 7263 653a  dFile..# Source:
+00000070: 2068 7474 7073 3a2f 2f67 6973 742e 6769   https://gist.gi
+00000080: 7468 7562 2e63 6f6d 2f64 7269 6c6c 6269  thub.com/drillbi
+00000090: 7473 2f35 3433 3236 3939 0a0a 5445 5354  ts/5432699..TEST
+000000a0: 5f49 4d41 4745 203d 2022 2222 0a69 5642  _IMAGE = """.iVB
+000000b0: 4f52 7730 4b47 676f 4141 4141 4e53 5568  ORw0KGgoAAAANSUh
+000000c0: 4555 6741 4141 4241 4141 4141 5143 4159  EUgAAABAAAAAQCAY
+000000d0: 4141 4141 6638 2f39 6841 4141 4142 6d4a  AAAAf8/9hAAAABmJ
+000000e0: 4c52 3051 412f 7744 2f41 502b 6776 6165  LR0QA/wD/AP+gvae
+000000f0: 5441 4141 4143 5842 490a 5758 4d41 4141  TAAAACXBI.WXMAAA
+00000100: 4249 4141 4141 5341 4247 7957 732b 4141  BIAAAASABGyWs+AA
+00000110: 4141 4358 5a77 5157 6341 4141 4151 4141  AACXZwQWcAAAAQAA
+00000120: 4141 4541 4263 7871 3344 4141 4142 6645  AAEABcxq3DAAABfE
+00000130: 6c45 5156 5134 7935 3254 7655 7543 5552  lEQVQ4y52TvUuCUR
+00000140: 5447 6635 5a67 0a39 676f 5239 4156 6c55  TGf5Zg.9goR9AVlU
+00000150: 5a4a 394b 5552 7555 6b68 4955 4550 5155  ZJ9KURuUkhIUEPQU
+00000160: 4975 6252 4674 494a 546b 304e 546b 5546  IubRFtIJTk0NTkUF
+00000170: 6667 6e74 4155 7430 6542 5351 7752 4b52  fgntAUt0eBSQwRKR
+00000180: 4653 5942 5946 6c31 4741 7439 3031 6555  FSYBYFl1GAt901eU
+00000190: 5975 770a 5154 4c4d 3179 4c50 6473 2f7a  Yuw.QTLM1yLPds/z
+000001a0: 5044 2f75 5059 6572 6559 6a48 6377 442b  PD/uPYereYjHcwD+
+000001b0: 7451 332b 5579 732b 4c77 4361 6833 6738  tQ3+Uys+LwCah3g8
+000001c0: 3531 6c61 2f6c 6634 7177 4b62 3631 536e  51la/lf4qwKb61Sn
+000001d0: 337a 3557 4655 5770 4348 422b 4755 4762  3z5WFUWpCHB+GUGb
+000001e0: 0a53 4352 4970 564b 7142 6b6d 5341 4d72  .SCRIpVKqBkmSAMr
+000001f0: 7173 5669 4d71 6e49 6977 4c78 3748 4f2f  qsViMqnIiwLx7HO/
+00000200: 552b 362b 3330 4759 7961 5658 4250 3175  U+6+30GYyaVXBP1u
+00000210: 4872 6655 4157 7657 4d57 6946 342b 716f  HrfUAWvWMWiF4+qo
+00000220: 4f55 4a4c 4a6b 7562 5963 4473 320a 5330  OUJLJkubYcDs2.S0
+00000230: 3368 764f 4453 4537 3536 3465 6b35 572b  3hvODSE7564ek5W+
+00000240: 4b74 2b74 6c6f 6139 6178 3676 344f 5a2b  Kt+tloa9ax6v4OZ+
+00000250: 2b6a 5a4f 2b6a 624d 2b70 4437 6f45 3448  +jZO+jbM+pD7oE4H
+00000260: 4d31 6c58 3176 594e 476f 4468 4379 514d  M1lX1vYNGoDhCyQM
+00000270: 6943 4761 6352 6d30 5666 0a45 4d2b 7569  iCGacRm0Vf.EM+ui
+00000280: 7564 6a6b 6536 5963 526f 4c66 6945 4c4e  udjke6YcRoLfiELN
+00000290: 4232 6458 546b 4161 3038 4c50 6c63 5432  B2dXTkAa08LPlcT2
+000002a0: 6670 4a41 4d78 575a 3148 344e 6e4b 4954  fpJAMxWZ1H4NnKIT
+000002b0: 7577 4434 4e6c 3652 4d67 4341 4531 4459  uwD4Nl6RMgCAE1DY
+000002c0: 3350 7579 7951 5a0a 4a4c 724e 765a 684d  3PuyyQZ.JLrNvZhM
+000002d0: 4a67 436d 4a77 5942 3241 3165 4148 4153  JgCmJwYB2A1eAHAS
+000002e0: 4469 466b 5155 7235 586e 3052 6f4a 4c53  DiFkQUr5Xn0RoJLS
+000002f0: 4467 375a 4342 3066 5652 5132 392f 546d  Dg7ZCB0fVRQ29/Tm
+00000300: 5031 4e66 2f30 4246 674c 3264 5148 344c  P1Nf/0BFgL2dQH4L
+00000310: 4e39 6452 0a37 434d 4f61 6958 446e 3646  N9dR.7CMOaiXDn6F
+00000320: 6179 5942 3978 4d48 6554 6743 7a31 636b  ayYB9xMHeTgCz1ck
+00000330: 6e64 2b57 4333 5667 546f 7255 4141 4141  nd+WC3VgTorUAAAA
+00000340: 6c64 4556 5964 474e 795a 5746 305a 5331  ldEVYdGNyZWF0ZS1
+00000350: 6b59 5852 6c41 4449 774d 5441 744d 5449  kYXRlADIwMTAtMTI
+00000360: 740a 4d6a 5a55 4d54 5136 4e44 6b36 4d6a  t.MjZUMTQ6NDk6Mj
+00000370: 4572 4d44 6b36 4d44 4148 4842 4231 4141  ErMDk6MDAHHBB1AA
+00000380: 4141 4a58 5246 5748 5274 6232 5270 5a6e  AAJXRFWHRtb2RpZn
+00000390: 6b74 5a47 4630 5a51 4179 4d44 4577 4c54  ktZGF0ZQAyMDEwLT
+000003a0: 4579 4c54 4932 5644 4530 4f6a 5135 0a4f  EyLTI2VDE0OjQ5.O
+000003b0: 6a49 784b 7a41 354f 6a41 7757 4b31 6d51  jIxKzA5OjAwWK1mQ
+000003c0: 5141 4141 4142 4a52 5535 4572 6b4a 6767  QAAAABJRU5ErkJgg
+000003d0: 6f6c 5154 6b63 4e43 686f 4b41 4141 4144  olQTkcNChoKAAAAD
+000003e0: 556c 4952 4649 4141 4141 5141 4141 4145  UlIRFIAAAAQAAAAE
+000003f0: 4167 4741 4141 4148 2f50 2f0a 5951 4141  AgGAAAAH/P/.YQAA
+00000400: 4141 5a69 5330 6445 4150 3841 2f77 442f  AAZiS0dEAP8A/wD/
+00000410: 6f4c 326e 6b77 4141 4141 6c77 5346 6c7a  oL2nkwAAAAlwSFlz
+00000420: 4141 4141 5341 4141 4145 6741 5273 6c72  AAAASAAAAEgARslr
+00000430: 5067 4141 4141 6c32 6345 466e 4141 4141  PgAAAAl2cEFnAAAA
+00000440: 4541 4141 4142 4141 0a58 4d61 7477 7741  EAAAABAA.XMatwwA
+00000450: 4141 6864 4a52 4546 554f 4d75 566b 3831  AAhdJREFUOMuVk81
+00000460: 4c56 4645 5978 6e2f 337a 6f63 6671 5665  LVFEYxn/3zocfqVe
+00000470: 6255 6243 7954 4c79 5952 5977 4430 6365  bUbCyTLyYRYwD0ce
+00000480: 6d43 4952 7955 5654 6f4c 6c6f 4552 5546  mCIRyUVToLloERUF
+00000490: 4262 5970 6f0a 4537 5749 4676 3054 4c61  BbYpo.E7WIFv0TLa
+000004a0: 5036 4332 5931 376f 5957 5751 7852 4d77  P6C2Y17oYWWQxRMw
+000004b0: 6f35 4f55 706c 6b52 2f58 4f65 664d 7557  o5OUplkR/XOefMuW
+000004c0: 384c 4e59 795a 4c42 3934 654f 4535 4c37  8LNYyZLB94eOE5L7
+000004d0: 397a 7a6e 7334 6a6f 6849 5070 2f6e 2b59  9zzns4johIPp/n+Y
+000004e0: 7458 0a66 506e 366a 6171 3162 4b61 4936  tX.fPn6jaq1bKaI6
+000004f0: 354c 5933 7348 6f68 584f 6b30 326d 634e  5LY3sHohXOk02mcN
+00000500: 784d 5438 766a 4a55 3554 5762 4555 4e38  xMT8vjJU5TWbEUN8
+00000510: 5469 3362 6c34 6e30 744c 572f 7142 636e  Ti3bl4n0tLW/qBcn
+00000520: 6957 306c 7442 6178 4672 7357 6c33 500a  iW0ltBaxFrsWl3P.
+00000530: 3749 5a38 5064 4e61 3832 6d36 5250 5444  7IZ8PdNa82m6RPTD
+00000540: 7879 4c47 6d4c 7137 4a44 7561 7156 5143  xyLGmLq7JDuaqVQC
+00000550: 6c6c 6271 6e36 4934 4f55 5530 434a 594a  llbqn6I4OUU0CJYJ
+00000560: 7737 426d 4d52 364c 6350 7679 5552 624c  w7BmMR6LcPvyURbL
+00000570: 4752 3439 712f 3731 4b6c 476a 0a64 5633  GR49q/71KlGj.dV3
+00000580: 416c 6245 6842 6e6f 6733 6d6f 3565 3854  AlbEhBnog3mo5e8T
+00000590: 7963 727a 2b63 4b50 616d 4272 4169 554f  ycrz+cKPamBrAiUO
+000005a0: 646e 442f 5a68 6c46 7a69 4b70 7737 5253  dnD/ZhlFziKpw7RS
+000005b0: 384c 5672 7930 3149 4463 4933 5762 4852  8LVry01IDcI3WbHR
+000005c0: 5875 384f 6453 3532 340a 7067 7836 426c  Xu8OdS524.pgx6Bl
+000005d0: 6b4a 454b 5734 5078 7253 4650 327a 3132  kJEKW4PxrSFP2z12
+000005e0: 694e 7131 5546 7254 5661 6178 444e 7736  iNq1UFrTVaaxDNw6
+000005f0: 7674 7444 584d 672f 324f 3241 5843 3555  vttDXMg/2O2AXC5U
+00000600: 556b 574b 4937 7673 4464 4d2b 5a33 5839  UkWKI7vsDdM+Z3X9
+00000610: 5773 3274 5847 0a59 4c54 4361 4d57 4e4d  Ws2tXG.YLTCaMWNM
+00000620: 5938 4466 5245 4146 7063 556b 7a50 4331  Y8DfREAFpcUkzPC1
+00000630: 4a7a 4c38 6b4b 4147 4d33 7876 6f44 442b  JzL8kKAGM3xvoDD+
+00000640: 3175 4a56 582b 696c 4549 7074 5470 4543  1uJVX+ilEIptTpEC
+00000650: 5550 3850 5845 4742 2f72 497a 772f 694e  UP8PXEGB/rIzw/iN
+00000660: 5058 6a0a 6465 316a 4d4c 3058 6179 336c  PXj.de1jML0Xay3l
+00000670: 3651 4b66 5a79 6577 5039 3578 3864 6872  6QKfZyewP95x8dhr
+00000680: 3772 3048 7053 6f41 4f44 7437 646b 746f  7r0HpSoAODt7dkto
+00000690: 5130 5345 7073 5a47 656e 7437 3866 312b  Q0SEpsZGent78f1+
+000006a0: 664e 2f48 392f 7378 786c 416f 4643 6b55  fN/H9/sxxlAoFCkU
+000006b0: 0a43 7851 4b52 5571 6c45 6b70 7058 4e64  .CxQKRUqlEkppXNd
+000006c0: 6442 5854 7632 4358 7274 482f 4a6f 6659  dBXTv2CXrtH/JofY
+000006d0: 566f 716e 5551 624c 5a38 662f 2b41 3835  VoqnUQbLZ8f/+A85
+000006e0: 6146 5741 6f6c 594a 634c 6965 6535 306b  aFWAolYJcLiee50k
+000006f0: 7346 7475 536d 3765 3153 4361 540a 4555  sFtuSm7e1SCaT.EU
+00000700: 5245 6372 6d63 6e42 345a 6b57 5179 4b5a  REcrmcnB4ZkWQyKZ
+00000710: 376e 6265 7045 4969 4844 7738 4f53 7a57  7nbepEIiHDw8OSzW
+00000720: 5a46 524f 5158 3650 705a 4678 4174 5338  ZFROQX6PpZFxAtS8
+00000730: 4941 4141 416c 6445 5659 6447 4e79 5a57  IAAAAldEVYdGNyZW
+00000740: 4630 5a53 316b 5958 526c 0a41 4449 774d  F0ZS1kYXRl.ADIwM
+00000750: 5441 744d 5449 744d 6a5a 554d 5451 364e  TAtMTItMjZUMTQ6N
+00000760: 446b 364d 6a45 724d 446b 364d 4441 4848  Dk6MjErMDk6MDAHH
+00000770: 4242 3141 4141 414a 5852 4657 4852 7462  BB1AAAAJXRFWHRtb
+00000780: 3252 705a 6e6b 745a 4746 305a 5141 794d  2RpZnktZGF0ZQAyM
+00000790: 4445 774c 5445 790a 4c54 4932 5644 4530  DEwLTEy.LTI2VDE0
+000007a0: 4f6a 5135 4f6a 4978 4b7a 4135 4f6a 4177  OjQ5OjIxKzA5OjAw
+000007b0: 574b 316d 5151 4141 4141 424a 5255 3545  WK1mQQAAAABJRU5E
+000007c0: 726b 4a67 676f 6c51 546b 634e 4368 6f4b  rkJggolQTkcNChoK
+000007d0: 4141 4141 4455 6c49 5246 4941 4141 4151  AAAADUlIRFIAAAAQ
+000007e0: 4141 4141 0a45 4167 4741 4141 4148 2f50  AAAA.EAgGAAAAH/P
+000007f0: 2f59 5141 4141 415a 6953 3064 4541 5038  /YQAAAAZiS0dEAP8
+00000800: 412f 7744 2f6f 4c32 6e6b 7741 4141 416c  A/wD/oL2nkwAAAAl
+00000810: 7753 466c 7a41 4141 4153 4141 4141 4567  wSFlzAAAASAAAAEg
+00000820: 4152 736c 7250 6741 4141 416c 3263 4546  ARslrPgAAAAl2cEF
+00000830: 6e0a 4141 4141 4541 4141 4142 4141 584d  n.AAAAEAAAABAAXM
+00000840: 6174 7777 4141 416f 394a 5245 4655 4f4d  atwwAAAo9JREFUOM
+00000850: 754e 6b73 3172 5647 6355 786e 2f76 652b  uNks1rVGcUxn/ve+
+00000860: 396b 5575 4f64 6649 7a61 6d4e 4845 4d4b  9kUuOdfIzamNHEMK
+00000870: 3352 5649 4c51 5141 7543 5755 526f 0a72  3RVILQQAuCWURo.r
+00000880: 5341 7462 7356 3230 542f 4550 364f 3746  SAtbsV20T/EP6O7F
+00000890: 7478 6b6b 5957 514b 4b37 4634 4b62 3143  txkkYWQKK7F4Kb1C
+000008a0: 3679 6f53 5672 4e64 4449 6d31 5954 4d6a  6yoSVrNdDIm1YTMj
+000008b0: 4450 3376 6663 3970 3475 625a 4559 6f70  DP3vfc9p4ubZEYop
+000008c0: 5163 6544 6877 4f44 3839 7a0a 7a6d 4f38  QceDhwOD89z.zmO8
+000008d0: 392f 7277 3053 4e75 3362 3544 3561 3871  9/rw0SNu3b5D5a8q
+000008e0: 3367 7637 5a58 6137 646b 5932 7349 774d  3gv7ZXa7dkY2sIwM
+000008f0: 6638 7733 5833 2f46 3950 546e 684c 2f2b  f8w3X3/F9PTnhL/+
+00000900: 396f 4366 6637 6e42 6571 3247 4d59 622f  9oCff7nBeq2GMYb/
+00000910: 5535 7362 6d31 5458 0a61 3854 4f45 5177  U5sbm1TX.a8TOEQw
+00000920: 4d48 6271 2b76 4c4b 4b71 7149 6969 4168  MHbq+vLKKqqIiiAh
+00000930: 2b72 3374 4276 4b42 6473 3732 6465 7231  +r3tBvKBds72der1
+00000940: 4f74 566f 6c66 5037 3842 576d 6164 6d6e  OtVolfP78BWmadmn
+00000950: 4e56 4b67 7149 3063 4f6b 6952 744e 7263  NVKgqI0cOkiRtNrc
+00000960: 395a 7439 480a 7839 664b 3669 7068 732f  9Zt9H.x9fK6iphs/
+00000970: 6b65 5666 6c41 6f71 7053 484f 7a6a 682b  keVflAoqpSHOzjh+
+00000980: 386d 614c 3539 796b 3833 577a 5261 3847  8maL59yk83WzRa8G
+00000990: 384f 777a 5278 6948 5149 464f 6a4a 4258  8OwzRxiHQIFOjJBX
+000009a0: 7737 4f38 6230 7156 3530 4b32 4831 7457  w7O8b0qV50K2H1tW
+000009b0: 662b 0a72 6943 6948 5262 4e46 4955 7563  f+.riCiHRbNFIUuc
+000009c0: 5967 6f5a 752f 5971 6c7a 3434 6969 587a  YgoZu/Yqlz44iiXz
+000009d0: 6833 4570 4a75 4530 754c 4b6c 3537 6c4e  h3EpJuE0uLKl57lN
+000009e0: 632f 3933 7756 6a4f 7959 7941 7065 6775  c/93wVjOyYyApegu
+000009f0: 7770 456c 544f 6639 4848 3159 6b53 550a  wpElTOf9HH1YkSU.
+00000a00: 6530 4f37 3263 432f 6231 444d 4b39 2f50  e0O72cC/b1DMK9/P
+00000a10: 4750 3563 3937 7a61 5547 7758 6730 3163  GP5c97zaUGwXg01c
+00000a20: 6a48 4d78 6352 777a 3043 6638 6550 6b41  jHMxcRwz0Cf8ePkA
+00000a30: 4a34 3755 3065 5276 534c 6568 7459 4d30  J47U0eRvSLehtYM0
+00000a40: 3670 772b 314f 5461 755a 6a65 0a77 4247  6pw+1OTauZje.wBG
+00000a50: 376d 4354 4a45 4471 5833 6543 6a76 4f58  7mCTJEDqX3eCjvOX
+00000a60: 7178 5147 6d54 7758 556d 776c 786d 6d64  qxQGmTwXUmwlxmmd
+00000a70: 7270 772b 7a30 7962 6948 586e 6259 7161  rpw+z0ybiHXnbYqa
+00000a80: 7376 4467 6263 4750 4a45 7676 7348 4b46  svDgbcGPJEvvsHKF
+00000a90: 7a44 7039 3654 677a 330a 6376 6a77 4d4d  zDp96Tgz3.cvjwMM
+00000aa0: 2f65 6673 6142 775a 5030 4433 394b 6162  /efsaBwZP0D39Kab
+00000ab0: 4b45 7067 6e62 4733 2f77 7276 6155 3570  KEpgnbG3/wrvaU5p
+00000ac0: 736e 4844 2f36 6d4d 4638 6a63 7157 7752  snHD/6mMF8jcqWwR
+00000ad0: 6777 7057 4f6a 4b69 4c6b 516b 4f68 7635  gwpWOjKiLkQkOhv5
+00000ae0: 2b78 7354 4c6c 0a63 706e 5230 574f 5553  +xsTLl.cpnR0WOUS
+00000af0: 6956 4568 4c56 4b68 6258 5861 3778 6358  iVEhLVKhbXXa7xcX
+00000b00: 7148 7961 6f56 366f 3048 7164 314d 7855  qHyaoV6o0Hqd1MxU
+00000b10: 6a71 7537 5859 4c4d 466b 614e 5874 5859  jqu7XYLMFkaNXtXY
+00000b20: 4330 392b 5235 5577 626b 5945 6356 6169  C09+R5UwbkYEcVai
+00000b30: 7a46 6d0a 502f 4c57 4773 4c4a 7964 4d73  zFm.P/LWGsLJydMs
+00000b40: 3356 7643 576b 5033 677a 784b 374f 4b75  3VvCWkP3gzxK7OKu
+00000b50: 3742 6c38 312f 7445 684b 6d70 4b56 6859  7Bl81/tEhKmpKVhY
+00000b60: 574e 434a 6951 6b4e 676c 4444 4d4b 6468  WNCJiQkNglDDMKdh
+00000b70: 4c70 6631 2f30 4151 6844 6f2b 5071 357a  Lpf1/0AQhDo+Pq5z
+00000b80: 0a63 334e 4b6d 7161 3675 4c69 6f73 374d  .c3NKmqa6uLios7M
+00000b90: 5874 4667 7361 6852 4647 6855 4b48 5553  XtFgsahRFGhUKHUS
+00000ba0: 374b 4251 3069 6949 6447 6872 5338 2b64  7KBQ0iiIdGhrS8+d
+00000bb0: 6e64 4835 2b58 704d 6b30 5838 414d 5456  ndH5+XpMk0X8AMTV
+00000bc0: 782f 696e 7055 3463 4141 4141 6c0a 6445  x/inpU4cAAAAl.dE
+00000bd0: 5659 6447 4e79 5a57 4630 5a53 316b 5958  VYdGNyZWF0ZS1kYX
+00000be0: 526c 4144 4977 4d54 4174 4d54 4974 4d6a  RlADIwMTAtMTItMj
+00000bf0: 5a55 4d54 5136 4e44 6b36 4d6a 4572 4d44  ZUMTQ6NDk6MjErMD
+00000c00: 6b36 4d44 4148 4842 4231 4141 4141 4a58  k6MDAHHBB1AAAAJX
+00000c10: 5246 5748 5274 6232 5270 0a5a 6e6b 745a  RFWHRtb2Rp.ZnktZ
+00000c20: 4746 305a 5141 794d 4445 774c 5445 794c  GF0ZQAyMDEwLTEyL
+00000c30: 5449 3256 4445 304f 6a51 354f 6a49 784b  TI2VDE0OjQ5OjIxK
+00000c40: 7a41 354f 6a41 7757 4b31 6d51 5141 4141  zA5OjAwWK1mQQAAA
+00000c50: 4142 4a52 5535 4572 6b4a 6767 673d 3d0a  ABJRU5ErkJggg==.
+00000c60: 2222 222e 7374 7269 7028 290a 0a0a 6465  """.strip()...de
+00000c70: 6620 6765 745f 7465 7374 5f69 6d61 6765  f get_test_image
+00000c80: 2829 3a0a 2020 2020 7265 7475 726e 2049  ():.    return I
+00000c90: 6e4d 656d 6f72 7955 706c 6f61 6465 6446  nMemoryUploadedF
+00000ca0: 696c 6528 0a20 2020 2020 2020 2042 7974  ile(.        Byt
+00000cb0: 6573 494f 2862 6173 6536 342e 6236 3464  esIO(base64.b64d
+00000cc0: 6563 6f64 6528 5445 5354 5f49 4d41 4745  ecode(TEST_IMAGE
+00000cd0: 2929 2c0a 2020 2020 2020 2020 6669 656c  )),.        fiel
+00000ce0: 645f 6e61 6d65 3d22 7465 6d70 6669 6c65  d_name="tempfile
+00000cf0: 222c 0a20 2020 2020 2020 206e 616d 653d  ",.        name=
+00000d00: 2274 656d 7066 696c 652e 706e 6722 2c0a  "tempfile.png",.
+00000d10: 2020 2020 2020 2020 636f 6e74 656e 745f          content_
+00000d20: 7479 7065 3d22 696d 6167 652f 706e 6722  type="image/png"
+00000d30: 2c0a 2020 2020 2020 2020 7369 7a65 3d6c  ,.        size=l
+00000d40: 656e 2854 4553 545f 494d 4147 4529 2c0a  en(TEST_IMAGE),.
+00000d50: 2020 2020 2020 2020 6368 6172 7365 743d          charset=
+00000d60: 2275 7466 2d38 222c 0a20 2020 2029 0a    "utf-8",.    ).
```

### Comparing `django-bootstrap5-23.1/tests/__pycache__/test_bootstrap_field_datetime.cpython-37.pyc` & `django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_datetime.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,208 +1,209 @@
-00000000: 420d 0d0a 0000 0000 8e55 c961 0f0d 0000  B........U.a....
-00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
-00000020: 0040 0000 0073 4e00 0000 6400 6401 6c00  .@...sN...d.d.l.
-00000030: 6d01 5a01 0100 6400 6402 6c02 6d03 5a03  m.Z...d.d.l.m.Z.
-00000040: 0100 6400 6403 6c04 6d05 5a05 6d06 5a06  ..d.d.l.m.Z.m.Z.
-00000050: 0100 4700 6404 6405 8400 6405 6501 6a07  ..G.d.d...d.e.j.
-00000060: 8303 5a08 4700 6406 6407 8400 6407 6506  ..Z.G.d.d...d.e.
-00000070: 8303 5a09 6408 5300 2909 e900 0000 0029  ..Z.d.S.)......)
-00000080: 01da 0566 6f72 6d73 2901 da12 4164 6d69  ...forms)...Admi
-00000090: 6e53 706c 6974 4461 7465 5469 6d65 2902  nSplitDateTime).
-000000a0: da0e 444a 414e 474f 5f56 4552 5349 4f4e  ..DJANGO_VERSION
-000000b0: da11 426f 6f74 7374 7261 7054 6573 7443  ..BootstrapTestC
-000000c0: 6173 6563 0000 0000 0000 0000 0000 0000  asec............
-000000d0: 0300 0000 4000 0000 731a 0000 0065 005a  ....@...s....e.Z
-000000e0: 0164 005a 0265 036a 0465 0583 0064 018d  .d.Z.e.j.e...d..
-000000f0: 015a 0664 0253 0029 03da 1044 6174 6554  .Z.d.S.)...DateT
-00000100: 696d 6554 6573 7446 6f72 6d29 01da 0677  imeTestForm)...w
-00000110: 6964 6765 744e 2907 da08 5f5f 6e61 6d65  idgetN)...__name
-00000120: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00000130: 5f5f 7175 616c 6e61 6d65 5f5f 7202 0000  __qualname__r...
-00000140: 00da 1253 706c 6974 4461 7465 5469 6d65  ...SplitDateTime
-00000150: 4669 656c 6472 0300 0000 da04 7465 7374  Fieldr......test
-00000160: a900 720d 0000 0072 0d00 0000 fa4e 2f55  ..r....r.....N/U
-00000170: 7365 7273 2f64 796c 616e 2f50 726f 6a65  sers/dylan/Proje
-00000180: 6374 732f 646a 616e 676f 2d62 6f6f 7473  cts/django-boots
-00000190: 7472 6170 352f 7465 7374 732f 7465 7374  trap5/tests/test
-000001a0: 5f62 6f6f 7473 7472 6170 5f66 6965 6c64  _bootstrap_field
-000001b0: 5f64 6174 6574 696d 652e 7079 7206 0000  _datetime.pyr...
-000001c0: 0007 0000 0073 0200 0000 0801 7206 0000  .....s......r...
-000001d0: 0063 0000 0000 0000 0000 0000 0000 0200  .c..............
-000001e0: 0000 4000 0000 732c 0000 0065 005a 0164  ..@...s,...e.Z.d
-000001f0: 005a 0264 0164 0284 005a 0364 0364 0484  .Z.d.d...Z.d.d..
-00000200: 005a 0464 0564 0684 005a 0564 0764 0884  .Z.d.d...Z.d.d..
-00000210: 005a 0664 0953 0029 0ada 1044 6174 6554  .Z.d.S.)...DateT
-00000220: 696d 6554 6573 7443 6173 6563 0200 0000  imeTestCasec....
-00000230: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-00000240: 7318 0000 0074 0064 016b 0572 147c 01a0  s....t.d.k.r.|..
-00000250: 0164 0264 03a1 027d 017c 0153 0029 047a  .d.d...}.|.S.).z
-00000260: 3752 6574 7572 6e20 6578 7065 6374 6564  7Return expected
-00000270: 2048 544d 4c20 6669 7865 6420 666f 7220   HTML fixed for 
-00000280: 446a 616e 676f 2034 2e31 2069 6620 6e65  Django 4.1 if ne
-00000290: 6365 7373 6172 792e 7a03 342e 317a 1020  cessary.z.4.1z. 
-000002a0: 666f 723d 2269 645f 7465 7374 5f30 22da  for="id_test_0".
-000002b0: 0029 0272 0400 0000 da07 7265 706c 6163  .).r......replac
-000002c0: 6529 02da 0473 656c 66da 0468 746d 6c72  e)...self..htmlr
-000002d0: 0d00 0000 720d 0000 0072 0e00 0000 da0c  ....r....r......
-000002e0: 6669 785f 646a 616e 676f 3431 0c00 0000  fix_django41....
-000002f0: 7306 0000 0000 0208 010c 017a 1d44 6174  s..........z.Dat
-00000300: 6554 696d 6554 6573 7443 6173 652e 6669  eTimeTestCase.fi
-00000310: 785f 646a 616e 676f 3431 6301 0000 0000  x_django41c.....
-00000320: 0000 0002 0000 0006 0000 0043 0000 0073  ...........C...s
-00000330: 2a00 0000 6401 7d01 7c00 a000 7c00 6a01  *...d.}.|...|.j.
-00000340: 6402 6403 7402 8300 6901 6404 8d02 7c00  d.d.t...i.d...|.
-00000350: a003 7c01 a101 a102 0100 6405 5300 2906  ..|.......d.S.).
-00000360: 7a2a 5465 7374 2066 6965 6c64 2077 6974  z*Test field wit
-00000370: 6820 4164 6d69 6e53 706c 6974 4461 7465  h AdminSplitDate
-00000380: 5469 6d65 2077 6964 6765 742e 6177 0100  Time widget.aw..
-00000390: 003c 6469 7620 636c 6173 733d 2264 6a61  .<div class="dja
-000003a0: 6e67 6f5f 626f 6f74 7374 7261 7035 2d72  ngo_bootstrap5-r
-000003b0: 6571 206d 622d 3322 3e3c 6c61 6265 6c20  eq mb-3"><label 
-000003c0: 636c 6173 733d 2266 6f72 6d2d 6c61 6265  class="form-labe
-000003d0: 6c22 2066 6f72 3d22 6964 5f74 6573 745f  l" for="id_test_
-000003e0: 3022 3e54 6573 743c 2f6c 6162 656c 3e3c  0">Test</label><
-000003f0: 7020 636c 6173 733d 2264 6174 6574 696d  p class="datetim
-00000400: 6522 3e44 6174 653a 203c 696e 7075 7420  e">Date: <input 
-00000410: 7479 7065 3d22 7465 7874 2220 6e61 6d65  type="text" name
-00000420: 3d22 7465 7374 5f30 2220 636c 6173 733d  ="test_0" class=
-00000430: 2266 6f72 6d2d 636f 6e74 726f 6c20 7644  "form-control vD
-00000440: 6174 6546 6965 6c64 2220 7369 7a65 3d22  ateField" size="
-00000450: 3130 2220 706c 6163 6568 6f6c 6465 723d  10" placeholder=
-00000460: 2254 6573 7422 2072 6571 7569 7265 6420  "Test" required 
-00000470: 6964 3d22 6964 5f74 6573 745f 3022 3e3c  id="id_test_0"><
-00000480: 6272 3e54 696d 653a 203c 696e 7075 7420  br>Time: <input 
-00000490: 7479 7065 3d22 7465 7874 2220 6e61 6d65  type="text" name
-000004a0: 3d22 7465 7374 5f31 2220 636c 6173 733d  ="test_1" class=
-000004b0: 2266 6f72 6d2d 636f 6e74 726f 6c20 7654  "form-control vT
-000004c0: 696d 6546 6965 6c64 2220 7369 7a65 3d22  imeField" size="
-000004d0: 3822 2070 6c61 6365 686f 6c64 6572 3d22  8" placeholder="
-000004e0: 5465 7374 2220 7265 7175 6972 6564 2069  Test" required i
-000004f0: 643d 2269 645f 7465 7374 5f31 223e 3c2f  d="id_test_1"></
-00000500: 703e 3c2f 6469 763e 7a1f 7b25 2062 6f6f  p></div>z.{% boo
-00000510: 7473 7472 6170 5f66 6965 6c64 2066 6f72  tstrap_field for
-00000520: 6d2e 7465 7374 2025 7dda 0466 6f72 6d29  m.test %}..form)
-00000530: 01da 0763 6f6e 7465 7874 4e29 04da 0f61  ...contextN)...a
-00000540: 7373 6572 7448 544d 4c45 7175 616c da06  ssertHTMLEqual..
-00000550: 7265 6e64 6572 7206 0000 0072 1400 0000  renderr....r....
-00000560: 2902 7212 0000 00da 0d65 7870 6563 7465  ).r......expecte
-00000570: 645f 6874 6d6c 720d 0000 0072 0d00 0000  d_htmlr....r....
-00000580: 720e 0000 00da 2574 6573 745f 696e 7075  r.....%test_inpu
-00000590: 745f 7479 7065 5f61 646d 696e 5f73 706c  t_type_admin_spl
-000005a0: 6974 5f64 6174 655f 7469 6d65 1200 0000  it_date_time....
-000005b0: 7308 0000 0000 0304 0d04 0112 017a 3644  s............z6D
-000005c0: 6174 6554 696d 6554 6573 7443 6173 652e  ateTimeTestCase.
-000005d0: 7465 7374 5f69 6e70 7574 5f74 7970 655f  test_input_type_
-000005e0: 6164 6d69 6e5f 7370 6c69 745f 6461 7465  admin_split_date
-000005f0: 5f74 696d 6563 0100 0000 0000 0000 0200  _timec..........
-00000600: 0000 0600 0000 4300 0000 732a 0000 0064  ......C...s*...d
-00000610: 017d 017c 00a0 007c 006a 0164 0264 0374  .}.|...|.j.d.d.t
-00000620: 0283 0069 0164 048d 027c 00a0 037c 01a1  ...i.d...|...|..
-00000630: 01a1 0201 0064 0553 0029 067a 4154 6573  .....d.S.).zATes
-00000640: 7420 6669 656c 6420 7769 7468 2041 646d  t field with Adm
-00000650: 696e 5370 6c69 7444 6174 6554 696d 6520  inSplitDateTime 
-00000660: 7769 6467 6574 2077 6974 6820 6c61 796f  widget with layo
-00000670: 7574 2068 6f72 697a 6f6e 7461 6c2e 61a5  ut horizontal.a.
-00000680: 0100 003c 6469 7620 636c 6173 733d 2264  ...<div class="d
-00000690: 6a61 6e67 6f5f 626f 6f74 7374 7261 7035  jango_bootstrap5
-000006a0: 2d72 6571 2072 6f77 206d 622d 3322 3e3c  -req row mb-3"><
-000006b0: 6c61 6265 6c20 636c 6173 733d 2263 6f6c  label class="col
-000006c0: 2d66 6f72 6d2d 6c61 6265 6c20 636f 6c2d  -form-label col-
-000006d0: 736d 2d32 2220 666f 723d 2269 645f 7465  sm-2" for="id_te
-000006e0: 7374 5f30 223e 5465 7374 3c2f 6c61 6265  st_0">Test</labe
-000006f0: 6c3e 3c64 6976 2063 6c61 7373 3d22 636f  l><div class="co
-00000700: 6c2d 736d 2d31 3022 3e3c 7020 636c 6173  l-sm-10"><p clas
-00000710: 733d 2264 6174 6574 696d 6522 3e44 6174  s="datetime">Dat
-00000720: 653a 203c 696e 7075 7420 7479 7065 3d22  e: <input type="
-00000730: 7465 7874 2220 6e61 6d65 3d22 7465 7374  text" name="test
-00000740: 5f30 2220 636c 6173 733d 2266 6f72 6d2d  _0" class="form-
-00000750: 636f 6e74 726f 6c20 7644 6174 6546 6965  control vDateFie
-00000760: 6c64 2220 7369 7a65 3d22 3130 2220 706c  ld" size="10" pl
+00000000: 6672 6f6d 2064 6a61 6e67 6f20 696d 706f  from django impo
+00000010: 7274 2066 6f72 6d73 0a66 726f 6d20 646a  rt forms.from dj
+00000020: 616e 676f 2e63 6f6e 7472 6962 2e61 646d  ango.contrib.adm
+00000030: 696e 2e77 6964 6765 7473 2069 6d70 6f72  in.widgets impor
+00000040: 7420 4164 6d69 6e53 706c 6974 4461 7465  t AdminSplitDate
+00000050: 5469 6d65 0a0a 6672 6f6d 2074 6573 7473  Time..from tests
+00000060: 2e62 6173 6520 696d 706f 7274 2044 4a41  .base import DJA
+00000070: 4e47 4f5f 5645 5253 494f 4e2c 2042 6f6f  NGO_VERSION, Boo
+00000080: 7473 7472 6170 5465 7374 4361 7365 0a0a  tstrapTestCase..
+00000090: 0a63 6c61 7373 2044 6174 6554 696d 6554  .class DateTimeT
+000000a0: 6573 7446 6f72 6d28 666f 726d 732e 466f  estForm(forms.Fo
+000000b0: 726d 293a 0a20 2020 2074 6573 7420 3d20  rm):.    test = 
+000000c0: 666f 726d 732e 5370 6c69 7444 6174 6554  forms.SplitDateT
+000000d0: 696d 6546 6965 6c64 2877 6964 6765 743d  imeField(widget=
+000000e0: 4164 6d69 6e53 706c 6974 4461 7465 5469  AdminSplitDateTi
+000000f0: 6d65 2829 290a 0a0a 636c 6173 7320 4461  me())...class Da
+00000100: 7465 5469 6d65 5465 7374 4361 7365 2842  teTimeTestCase(B
+00000110: 6f6f 7473 7472 6170 5465 7374 4361 7365  ootstrapTestCase
+00000120: 293a 0a20 2020 2064 6566 2066 6978 5f64  ):.    def fix_d
+00000130: 6a61 6e67 6f34 3128 7365 6c66 2c20 6874  jango41(self, ht
+00000140: 6d6c 293a 0a20 2020 2020 2020 2022 2222  ml):.        """
+00000150: 5265 7475 726e 2065 7870 6563 7465 6420  Return expected 
+00000160: 4854 4d4c 2066 6978 6564 2066 6f72 2044  HTML fixed for D
+00000170: 6a61 6e67 6f20 342e 3120 6966 206e 6563  jango 4.1 if nec
+00000180: 6573 7361 7279 2e22 2222 0a20 2020 2020  essary.""".     
+00000190: 2020 2069 6620 444a 414e 474f 5f56 4552     if DJANGO_VER
+000001a0: 5349 4f4e 203e 3d20 2234 2e31 223a 0a20  SION >= "4.1":. 
+000001b0: 2020 2020 2020 2020 2020 2068 746d 6c20             html 
+000001c0: 3d20 6874 6d6c 2e72 6570 6c61 6365 2827  = html.replace('
+000001d0: 2066 6f72 3d22 6964 5f74 6573 745f 3022   for="id_test_0"
+000001e0: 272c 2022 2229 0a20 2020 2020 2020 2072  ', "").        r
+000001f0: 6574 7572 6e20 6874 6d6c 0a0a 2020 2020  eturn html..    
+00000200: 6465 6620 7465 7374 5f69 6e70 7574 5f74  def test_input_t
+00000210: 7970 655f 6164 6d69 6e5f 7370 6c69 745f  ype_admin_split_
+00000220: 6461 7465 5f74 696d 6528 7365 6c66 293a  date_time(self):
+00000230: 0a20 2020 2020 2020 2022 2222 5465 7374  .        """Test
+00000240: 2066 6965 6c64 2077 6974 6820 4164 6d69   field with Admi
+00000250: 6e53 706c 6974 4461 7465 5469 6d65 2077  nSplitDateTime w
+00000260: 6964 6765 742e 2222 220a 2020 2020 2020  idget.""".      
+00000270: 2020 6578 7065 6374 6564 5f68 746d 6c20    expected_html 
+00000280: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+00000290: 273c 6469 7620 636c 6173 733d 2264 6a61  '<div class="dja
+000002a0: 6e67 6f5f 626f 6f74 7374 7261 7035 2d72  ngo_bootstrap5-r
+000002b0: 6571 206d 622d 3322 3e27 0a20 2020 2020  eq mb-3">'.     
+000002c0: 2020 2020 2020 2027 3c6c 6162 656c 2063         '<label c
+000002d0: 6c61 7373 3d22 666f 726d 2d6c 6162 656c  lass="form-label
+000002e0: 2220 666f 723d 2269 645f 7465 7374 5f30  " for="id_test_0
+000002f0: 223e 5465 7374 3c2f 6c61 6265 6c3e 270a  ">Test</label>'.
+00000300: 2020 2020 2020 2020 2020 2020 273c 7020              '<p 
+00000310: 636c 6173 733d 2264 6174 6574 696d 6522  class="datetime"
+00000320: 3e27 0a20 2020 2020 2020 2020 2020 2022  >'.            "
+00000330: 4461 7465 3a20 220a 2020 2020 2020 2020  Date: ".        
+00000340: 2020 2020 273c 696e 7075 7420 7479 7065      '<input type
+00000350: 3d22 7465 7874 2220 6e61 6d65 3d22 7465  ="text" name="te
+00000360: 7374 5f30 2220 636c 6173 733d 2266 6f72  st_0" class="for
+00000370: 6d2d 636f 6e74 726f 6c20 7644 6174 6546  m-control vDateF
+00000380: 6965 6c64 2220 7369 7a65 3d22 3130 2227  ield" size="10"'
+00000390: 0a20 2020 2020 2020 2020 2020 2027 2070  .            ' p
+000003a0: 6c61 6365 686f 6c64 6572 3d22 5465 7374  laceholder="Test
+000003b0: 2220 7265 7175 6972 6564 2069 643d 2269  " required id="i
+000003c0: 645f 7465 7374 5f30 223e 270a 2020 2020  d_test_0">'.    
+000003d0: 2020 2020 2020 2020 223c 6272 3e22 0a20          "<br>". 
+000003e0: 2020 2020 2020 2020 2020 2022 5469 6d65             "Time
+000003f0: 3a20 220a 2020 2020 2020 2020 2020 2020  : ".            
+00000400: 273c 696e 7075 7420 7479 7065 3d22 7465  '<input type="te
+00000410: 7874 2220 6e61 6d65 3d22 7465 7374 5f31  xt" name="test_1
+00000420: 2220 636c 6173 733d 2266 6f72 6d2d 636f  " class="form-co
+00000430: 6e74 726f 6c20 7654 696d 6546 6965 6c64  ntrol vTimeField
+00000440: 2220 7369 7a65 3d22 3822 270a 2020 2020  " size="8"'.    
+00000450: 2020 2020 2020 2020 2720 706c 6163 6568          ' placeh
+00000460: 6f6c 6465 723d 2254 6573 7422 2072 6571  older="Test" req
+00000470: 7569 7265 6420 6964 3d22 6964 5f74 6573  uired id="id_tes
+00000480: 745f 3122 3e27 0a20 2020 2020 2020 2020  t_1">'.         
+00000490: 2020 2022 3c2f 703e 220a 2020 2020 2020     "</p>".      
+000004a0: 2020 2020 2020 223c 2f64 6976 3e22 0a20        "</div>". 
+000004b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000004c0: 2073 656c 662e 6173 7365 7274 4854 4d4c   self.assertHTML
+000004d0: 4571 7561 6c28 0a20 2020 2020 2020 2020  Equal(.         
+000004e0: 2020 2073 656c 662e 7265 6e64 6572 2822     self.render("
+000004f0: 7b25 2062 6f6f 7473 7472 6170 5f66 6965  {% bootstrap_fie
+00000500: 6c64 2066 6f72 6d2e 7465 7374 2025 7d22  ld form.test %}"
+00000510: 2c20 636f 6e74 6578 743d 7b22 666f 726d  , context={"form
+00000520: 223a 2044 6174 6554 696d 6554 6573 7446  ": DateTimeTestF
+00000530: 6f72 6d28 297d 292c 0a20 2020 2020 2020  orm()}),.       
+00000540: 2020 2020 2073 656c 662e 6669 785f 646a       self.fix_dj
+00000550: 616e 676f 3431 2865 7870 6563 7465 645f  ango41(expected_
+00000560: 6874 6d6c 292c 0a20 2020 2020 2020 2029  html),.        )
+00000570: 0a0a 2020 2020 6465 6620 7465 7374 5f69  ..    def test_i
+00000580: 6e70 7574 5f74 7970 655f 6164 6d69 6e5f  nput_type_admin_
+00000590: 7370 6c69 745f 6461 7465 5f74 696d 655f  split_date_time_
+000005a0: 686f 7269 7a6f 6e74 616c 2873 656c 6629  horizontal(self)
+000005b0: 3a0a 2020 2020 2020 2020 2222 2254 6573  :.        """Tes
+000005c0: 7420 6669 656c 6420 7769 7468 2041 646d  t field with Adm
+000005d0: 696e 5370 6c69 7444 6174 6554 696d 6520  inSplitDateTime 
+000005e0: 7769 6467 6574 2077 6974 6820 6c61 796f  widget with layo
+000005f0: 7574 2068 6f72 697a 6f6e 7461 6c2e 2222  ut horizontal.""
+00000600: 220a 2020 2020 2020 2020 6578 7065 6374  ".        expect
+00000610: 6564 5f68 746d 6c20 3d20 280a 2020 2020  ed_html = (.    
+00000620: 2020 2020 2020 2020 273c 6469 7620 636c          '<div cl
+00000630: 6173 733d 2264 6a61 6e67 6f5f 626f 6f74  ass="django_boot
+00000640: 7374 7261 7035 2d72 6571 2072 6f77 206d  strap5-req row m
+00000650: 622d 3322 3e27 0a20 2020 2020 2020 2020  b-3">'.         
+00000660: 2020 2027 3c6c 6162 656c 2063 6c61 7373     '<label class
+00000670: 3d22 636f 6c2d 666f 726d 2d6c 6162 656c  ="col-form-label
+00000680: 2063 6f6c 2d73 6d2d 3222 2066 6f72 3d22   col-sm-2" for="
+00000690: 6964 5f74 6573 745f 3022 3e54 6573 743c  id_test_0">Test<
+000006a0: 2f6c 6162 656c 3e27 0a20 2020 2020 2020  /label>'.       
+000006b0: 2020 2020 2027 3c64 6976 2063 6c61 7373       '<div class
+000006c0: 3d22 636f 6c2d 736d 2d31 3022 3e27 0a20  ="col-sm-10">'. 
+000006d0: 2020 2020 2020 2020 2020 2027 3c70 2063             '<p c
+000006e0: 6c61 7373 3d22 6461 7465 7469 6d65 223e  lass="datetime">
+000006f0: 270a 2020 2020 2020 2020 2020 2020 2244  '.            "D
+00000700: 6174 653a 2022 0a20 2020 2020 2020 2020  ate: ".         
+00000710: 2020 2027 3c69 6e70 7574 2074 7970 653d     '<input type=
+00000720: 2274 6578 7422 206e 616d 653d 2274 6573  "text" name="tes
+00000730: 745f 3022 2063 6c61 7373 3d22 666f 726d  t_0" class="form
+00000740: 2d63 6f6e 7472 6f6c 2076 4461 7465 4669  -control vDateFi
+00000750: 656c 6422 2073 697a 653d 2231 3022 270a  eld" size="10"'.
+00000760: 2020 2020 2020 2020 2020 2020 2720 706c              ' pl
 00000770: 6163 6568 6f6c 6465 723d 2254 6573 7422  aceholder="Test"
 00000780: 2072 6571 7569 7265 6420 6964 3d22 6964   required id="id
-00000790: 5f74 6573 745f 3022 3e3c 6272 3e54 696d  _test_0"><br>Tim
-000007a0: 653a 203c 696e 7075 7420 7479 7065 3d22  e: <input type="
-000007b0: 7465 7874 2220 6e61 6d65 3d22 7465 7374  text" name="test
-000007c0: 5f31 2220 636c 6173 733d 2266 6f72 6d2d  _1" class="form-
-000007d0: 636f 6e74 726f 6c20 7654 696d 6546 6965  control vTimeFie
-000007e0: 6c64 2220 7369 7a65 3d22 3822 2070 6c61  ld" size="8" pla
-000007f0: 6365 686f 6c64 6572 3d22 5465 7374 2220  ceholder="Test" 
-00000800: 7265 7175 6972 6564 2069 643d 2269 645f  required id="id_
-00000810: 7465 7374 5f31 223e 3c2f 703e 3c2f 6469  test_1"></p></di
-00000820: 763e 3c2f 6469 763e 7a33 7b25 2062 6f6f  v></div>z3{% boo
-00000830: 7473 7472 6170 5f66 6965 6c64 2066 6f72  tstrap_field for
-00000840: 6d2e 7465 7374 206c 6179 6f75 743d 2268  m.test layout="h
-00000850: 6f72 697a 6f6e 7461 6c22 2025 7d72 1500  orizontal" %}r..
-00000860: 0000 2901 7216 0000 004e 2904 7217 0000  ..).r....N).r...
-00000870: 0072 1800 0000 7206 0000 0072 1400 0000  .r....r....r....
-00000880: 2902 7212 0000 0072 1900 0000 720d 0000  ).r....r....r...
-00000890: 0072 0d00 0000 720e 0000 00da 3074 6573  .r....r.....0tes
-000008a0: 745f 696e 7075 745f 7479 7065 5f61 646d  t_input_type_adm
-000008b0: 696e 5f73 706c 6974 5f64 6174 655f 7469  in_split_date_ti
-000008c0: 6d65 5f68 6f72 697a 6f6e 7461 6c27 0000  me_horizontal'..
-000008d0: 0073 0800 0000 0003 040f 0401 1201 7a41  .s............zA
-000008e0: 4461 7465 5469 6d65 5465 7374 4361 7365  DateTimeTestCase
-000008f0: 2e74 6573 745f 696e 7075 745f 7479 7065  .test_input_type
-00000900: 5f61 646d 696e 5f73 706c 6974 5f64 6174  _admin_split_dat
-00000910: 655f 7469 6d65 5f68 6f72 697a 6f6e 7461  e_time_horizonta
-00000920: 6c63 0100 0000 0000 0000 0200 0000 0600  lc..............
-00000930: 0000 4300 0000 732a 0000 0064 017d 017c  ..C...s*...d.}.|
-00000940: 00a0 007c 006a 0164 0264 0374 0283 0069  ...|.j.d.d.t...i
-00000950: 0164 048d 027c 00a0 037c 01a1 01a1 0201  .d...|...|......
-00000960: 0064 0553 0029 067a 3f54 6573 7420 6669  .d.S.).z?Test fi
-00000970: 656c 6420 7769 7468 2041 646d 696e 5370  eld with AdminSp
-00000980: 6c69 7444 6174 6554 696d 6520 7769 6467  litDateTime widg
-00000990: 6574 2077 6974 6820 6c61 796f 7574 2066  et with layout f
-000009a0: 6c6f 6174 696e 672e 6177 0100 003c 6469  loating.aw...<di
-000009b0: 7620 636c 6173 733d 2264 6a61 6e67 6f5f  v class="django_
-000009c0: 626f 6f74 7374 7261 7035 2d72 6571 206d  bootstrap5-req m
-000009d0: 622d 3322 3e3c 6c61 6265 6c20 636c 6173  b-3"><label clas
-000009e0: 733d 2266 6f72 6d2d 6c61 6265 6c22 2066  s="form-label" f
-000009f0: 6f72 3d22 6964 5f74 6573 745f 3022 3e54  or="id_test_0">T
-00000a00: 6573 743c 2f6c 6162 656c 3e3c 7020 636c  est</label><p cl
-00000a10: 6173 733d 2264 6174 6574 696d 6522 3e44  ass="datetime">D
-00000a20: 6174 653a 203c 696e 7075 7420 7479 7065  ate: <input type
-00000a30: 3d22 7465 7874 2220 6e61 6d65 3d22 7465  ="text" name="te
-00000a40: 7374 5f30 2220 636c 6173 733d 2266 6f72  st_0" class="for
-00000a50: 6d2d 636f 6e74 726f 6c20 7644 6174 6546  m-control vDateF
-00000a60: 6965 6c64 2220 7369 7a65 3d22 3130 2220  ield" size="10" 
-00000a70: 706c 6163 6568 6f6c 6465 723d 2254 6573  placeholder="Tes
-00000a80: 7422 2072 6571 7569 7265 6420 6964 3d22  t" required id="
-00000a90: 6964 5f74 6573 745f 3022 3e3c 6272 3e54  id_test_0"><br>T
-00000aa0: 696d 653a 203c 696e 7075 7420 7479 7065  ime: <input type
-00000ab0: 3d22 7465 7874 2220 6e61 6d65 3d22 7465  ="text" name="te
-00000ac0: 7374 5f31 2220 636c 6173 733d 2266 6f72  st_1" class="for
-00000ad0: 6d2d 636f 6e74 726f 6c20 7654 696d 6546  m-control vTimeF
-00000ae0: 6965 6c64 2220 7369 7a65 3d22 3822 2070  ield" size="8" p
-00000af0: 6c61 6365 686f 6c64 6572 3d22 5465 7374  laceholder="Test
-00000b00: 2220 7265 7175 6972 6564 2069 643d 2269  " required id="i
-00000b10: 645f 7465 7374 5f31 223e 3c2f 703e 3c2f  d_test_1"></p></
-00000b20: 6469 763e 7a31 7b25 2062 6f6f 7473 7472  div>z1{% bootstr
-00000b30: 6170 5f66 6965 6c64 2066 6f72 6d2e 7465  ap_field form.te
-00000b40: 7374 206c 6179 6f75 743d 2266 6c6f 6174  st layout="float
-00000b50: 696e 6722 2025 7d72 1500 0000 2901 7216  ing" %}r....).r.
-00000b60: 0000 004e 2904 7217 0000 0072 1800 0000  ...N).r....r....
-00000b70: 7206 0000 0072 1400 0000 2902 7212 0000  r....r....).r...
-00000b80: 0072 1900 0000 720d 0000 0072 0d00 0000  .r....r....r....
-00000b90: 720e 0000 00da 2e74 6573 745f 696e 7075  r......test_inpu
-00000ba0: 745f 7479 7065 5f61 646d 696e 5f73 706c  t_type_admin_spl
-00000bb0: 6974 5f64 6174 655f 7469 6d65 5f66 6c6f  it_date_time_flo
-00000bc0: 6174 696e 673e 0000 0073 0800 0000 0003  ating>...s......
-00000bd0: 040d 0401 1201 7a3f 4461 7465 5469 6d65  ......z?DateTime
-00000be0: 5465 7374 4361 7365 2e74 6573 745f 696e  TestCase.test_in
-00000bf0: 7075 745f 7479 7065 5f61 646d 696e 5f73  put_type_admin_s
-00000c00: 706c 6974 5f64 6174 655f 7469 6d65 5f66  plit_date_time_f
-00000c10: 6c6f 6174 696e 674e 2907 7208 0000 0072  loatingN).r....r
-00000c20: 0900 0000 720a 0000 0072 1400 0000 721a  ....r....r....r.
-00000c30: 0000 0072 1b00 0000 721c 0000 0072 0d00  ...r....r....r..
-00000c40: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
-00000c50: 0072 0f00 0000 0b00 0000 7308 0000 0008  .r........s.....
-00000c60: 0108 0608 1508 1772 0f00 0000 4e29 0ada  .......r....N)..
-00000c70: 0664 6a61 6e67 6f72 0200 0000 5a1c 646a  .djangor....Z.dj
-00000c80: 616e 676f 2e63 6f6e 7472 6962 2e61 646d  ango.contrib.adm
-00000c90: 696e 2e77 6964 6765 7473 7203 0000 005a  in.widgetsr....Z
-00000ca0: 0a74 6573 7473 2e62 6173 6572 0400 0000  .tests.baser....
-00000cb0: 7205 0000 00da 0446 6f72 6d72 0600 0000  r......Formr....
-00000cc0: 720f 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
-00000cd0: 0d00 0000 720e 0000 00da 083c 6d6f 6475  ....r......<modu
-00000ce0: 6c65 3e01 0000 0073 0800 0000 0c01 0c02  le>....s........
-00000cf0: 1003 1204                                ....
+00000790: 5f74 6573 745f 3022 3e27 0a20 2020 2020  _test_0">'.     
+000007a0: 2020 2020 2020 2022 3c62 723e 220a 2020         "<br>".  
+000007b0: 2020 2020 2020 2020 2020 2254 696d 653a            "Time:
+000007c0: 2022 0a20 2020 2020 2020 2020 2020 2027   ".            '
+000007d0: 3c69 6e70 7574 2074 7970 653d 2274 6578  <input type="tex
+000007e0: 7422 206e 616d 653d 2274 6573 745f 3122  t" name="test_1"
+000007f0: 2063 6c61 7373 3d22 666f 726d 2d63 6f6e   class="form-con
+00000800: 7472 6f6c 2076 5469 6d65 4669 656c 6422  trol vTimeField"
+00000810: 2073 697a 653d 2238 2227 0a20 2020 2020   size="8"'.     
+00000820: 2020 2020 2020 2027 2070 6c61 6365 686f         ' placeho
+00000830: 6c64 6572 3d22 5465 7374 2220 7265 7175  lder="Test" requ
+00000840: 6972 6564 2069 643d 2269 645f 7465 7374  ired id="id_test
+00000850: 5f31 223e 270a 2020 2020 2020 2020 2020  _1">'.          
+00000860: 2020 223c 2f70 3e22 0a20 2020 2020 2020    "</p>".       
+00000870: 2020 2020 2022 3c2f 6469 763e 220a 2020       "</div>".  
+00000880: 2020 2020 2020 2020 2020 223c 2f64 6976            "</div
+00000890: 3e22 0a20 2020 2020 2020 2029 0a20 2020  >".        ).   
+000008a0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000008b0: 4854 4d4c 4571 7561 6c28 0a20 2020 2020  HTMLEqual(.     
+000008c0: 2020 2020 2020 2073 656c 662e 7265 6e64         self.rend
+000008d0: 6572 2827 7b25 2062 6f6f 7473 7472 6170  er('{% bootstrap
+000008e0: 5f66 6965 6c64 2066 6f72 6d2e 7465 7374  _field form.test
+000008f0: 206c 6179 6f75 743d 2268 6f72 697a 6f6e   layout="horizon
+00000900: 7461 6c22 2025 7d27 2c20 636f 6e74 6578  tal" %}', contex
+00000910: 743d 7b22 666f 726d 223a 2044 6174 6554  t={"form": DateT
+00000920: 696d 6554 6573 7446 6f72 6d28 297d 292c  imeTestForm()}),
+00000930: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00000940: 662e 6669 785f 646a 616e 676f 3431 2865  f.fix_django41(e
+00000950: 7870 6563 7465 645f 6874 6d6c 292c 0a20  xpected_html),. 
+00000960: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+00000970: 6620 7465 7374 5f69 6e70 7574 5f74 7970  f test_input_typ
+00000980: 655f 6164 6d69 6e5f 7370 6c69 745f 6461  e_admin_split_da
+00000990: 7465 5f74 696d 655f 666c 6f61 7469 6e67  te_time_floating
+000009a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000009b0: 2222 2254 6573 7420 6669 656c 6420 7769  """Test field wi
+000009c0: 7468 2041 646d 696e 5370 6c69 7444 6174  th AdminSplitDat
+000009d0: 6554 696d 6520 7769 6467 6574 2077 6974  eTime widget wit
+000009e0: 6820 6c61 796f 7574 2066 6c6f 6174 696e  h layout floatin
+000009f0: 672e 2222 220a 2020 2020 2020 2020 6578  g.""".        ex
+00000a00: 7065 6374 6564 5f68 746d 6c20 3d20 280a  pected_html = (.
+00000a10: 2020 2020 2020 2020 2020 2020 273c 6469              '<di
+00000a20: 7620 636c 6173 733d 2264 6a61 6e67 6f5f  v class="django_
+00000a30: 626f 6f74 7374 7261 7035 2d72 6571 206d  bootstrap5-req m
+00000a40: 622d 3322 3e27 0a20 2020 2020 2020 2020  b-3">'.         
+00000a50: 2020 2027 3c6c 6162 656c 2063 6c61 7373     '<label class
+00000a60: 3d22 666f 726d 2d6c 6162 656c 2220 666f  ="form-label" fo
+00000a70: 723d 2269 645f 7465 7374 5f30 223e 5465  r="id_test_0">Te
+00000a80: 7374 3c2f 6c61 6265 6c3e 270a 2020 2020  st</label>'.    
+00000a90: 2020 2020 2020 2020 273c 7020 636c 6173          '<p clas
+00000aa0: 733d 2264 6174 6574 696d 6522 3e27 0a20  s="datetime">'. 
+00000ab0: 2020 2020 2020 2020 2020 2022 4461 7465             "Date
+00000ac0: 3a20 220a 2020 2020 2020 2020 2020 2020  : ".            
+00000ad0: 273c 696e 7075 7420 7479 7065 3d22 7465  '<input type="te
+00000ae0: 7874 2220 6e61 6d65 3d22 7465 7374 5f30  xt" name="test_0
+00000af0: 2220 636c 6173 733d 2266 6f72 6d2d 636f  " class="form-co
+00000b00: 6e74 726f 6c20 7644 6174 6546 6965 6c64  ntrol vDateField
+00000b10: 2220 7369 7a65 3d22 3130 2227 0a20 2020  " size="10"'.   
+00000b20: 2020 2020 2020 2020 2027 2070 6c61 6365           ' place
+00000b30: 686f 6c64 6572 3d22 5465 7374 2220 7265  holder="Test" re
+00000b40: 7175 6972 6564 2069 643d 2269 645f 7465  quired id="id_te
+00000b50: 7374 5f30 223e 270a 2020 2020 2020 2020  st_0">'.        
+00000b60: 2020 2020 223c 6272 3e22 0a20 2020 2020      "<br>".     
+00000b70: 2020 2020 2020 2022 5469 6d65 3a20 220a         "Time: ".
+00000b80: 2020 2020 2020 2020 2020 2020 273c 696e              '<in
+00000b90: 7075 7420 7479 7065 3d22 7465 7874 2220  put type="text" 
+00000ba0: 6e61 6d65 3d22 7465 7374 5f31 2220 636c  name="test_1" cl
+00000bb0: 6173 733d 2266 6f72 6d2d 636f 6e74 726f  ass="form-contro
+00000bc0: 6c20 7654 696d 6546 6965 6c64 2220 7369  l vTimeField" si
+00000bd0: 7a65 3d22 3822 270a 2020 2020 2020 2020  ze="8"'.        
+00000be0: 2020 2020 2720 706c 6163 6568 6f6c 6465      ' placeholde
+00000bf0: 723d 2254 6573 7422 2072 6571 7569 7265  r="Test" require
+00000c00: 6420 6964 3d22 6964 5f74 6573 745f 3122  d id="id_test_1"
+00000c10: 3e27 0a20 2020 2020 2020 2020 2020 2022  >'.            "
+00000c20: 3c2f 703e 220a 2020 2020 2020 2020 2020  </p>".          
+00000c30: 2020 223c 2f64 6976 3e22 0a20 2020 2020    "</div>".     
+00000c40: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
+00000c50: 662e 6173 7365 7274 4854 4d4c 4571 7561  f.assertHTMLEqua
+00000c60: 6c28 0a20 2020 2020 2020 2020 2020 2073  l(.            s
+00000c70: 656c 662e 7265 6e64 6572 2827 7b25 2062  elf.render('{% b
+00000c80: 6f6f 7473 7472 6170 5f66 6965 6c64 2066  ootstrap_field f
+00000c90: 6f72 6d2e 7465 7374 206c 6179 6f75 743d  orm.test layout=
+00000ca0: 2266 6c6f 6174 696e 6722 2025 7d27 2c20  "floating" %}', 
+00000cb0: 636f 6e74 6578 743d 7b22 666f 726d 223a  context={"form":
+00000cc0: 2044 6174 6554 696d 6554 6573 7446 6f72   DateTimeTestFor
+00000cd0: 6d28 297d 292c 0a20 2020 2020 2020 2020  m()}),.         
+00000ce0: 2020 2073 656c 662e 6669 785f 646a 616e     self.fix_djan
+00000cf0: 676f 3431 2865 7870 6563 7465 645f 6874  go41(expected_ht
+00000d00: 6d6c 292c 0a20 2020 2020 2020 2029 0a    ml),.        ).
```

### Comparing `django-bootstrap5-23.1/tests/app/settings.py` & `django-bootstrap5-23.2.dev0/tests/app/settings.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/tests/base.py` & `django-bootstrap5-23.2.dev0/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/tests/test_bootstrap_alert.py` & `django-bootstrap5-23.2.dev0/tests/test_bootstrap_alert.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/tests/test_bootstrap_button.py` & `django-bootstrap5-23.2.dev0/tests/test_bootstrap_button.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/tests/test_bootstrap_css_and_js_tags.py` & `django-bootstrap5-23.2.dev0/tests/test_bootstrap_css_and_js_tags.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/tests/test_bootstrap_field.py` & `django-bootstrap5-23.2.dev0/tests/test_bootstrap_field.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/tests/test_bootstrap_field_input_checkbox.py` & `django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_input_checkbox.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/tests/test_bootstrap_field_input_color.py` & `django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_input_color.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/tests/test_bootstrap_field_input_file.py` & `django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_input_file.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/tests/test_bootstrap_field_input_range.py` & `django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_input_range.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/tests/test_bootstrap_field_input_text.py` & `django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_input_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 
 class InputTypeTextTestCase(BootstrapTestCase):
     """Test for TextInput widgets that only differ in `input_type`."""
 
     def test_input_type_text(self):
         """Test field with default CharField widget."""
-
         form = CharFieldTestForm()
 
         self.assertHTMLEqual(
             self.render("{% bootstrap_field form.test %}", context={"form": form}),
             (
                 '<div class="django_bootstrap5-req mb-3">'
                 '<label for="id_test" class="form-label">Test</label>'
@@ -41,15 +40,14 @@
                 '<div class="invalid-feedback">This field is required.</div>'
                 "</div>"
             ),
         )
 
     def test_input_type_text_more(self):
         """Test field with default CharField widget."""
-
         form = CharFieldTestForm()
 
         self.assertHTMLEqual(
             self.render('{% bootstrap_field form.test addon_before="foo" %}', context={"form": form}),
             (
                 '<div class="django_bootstrap5-req mb-3">'
                 '<label for="id_test" class="form-label">Test</label>'
@@ -159,15 +157,14 @@
                 '<label for="id_test" class="form-label">Test</label>'
                 "</div>"
             ),
         )
 
     def test_input_validation_failure(self):
         """Test field with default CharField widget and min-length requirement to trigger validation errors."""
-
         form = CharFieldRequiredTestForm(data={"test": ""})
         self.assertFalse(form.is_valid())
 
         self.assertHTMLEqual(
             self.render('{% bootstrap_field form.test addon_before="foo" %}', context={"form": form}),
             (
                 '<div class="django_bootstrap5-err django_bootstrap5-req mb-3">'
```

### Comparing `django-bootstrap5-23.1/tests/test_bootstrap_field_parameters.py` & `django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 
 class BootstrapFieldParameterTestCase(BootstrapTestCase):
     """Test `bootstrap_field` parameters`."""
 
     def test_wrapper_class(self):
         """Test field with default CharField widget."""
-
         form = CharFieldTestForm()
 
         self.assertHTMLEqual(
             self.render("{% bootstrap_field form.test %}", context={"form": form}),
             (
                 '<div class="django_bootstrap5-req mb-3">'
                 '<label for="id_test" class="form-label">Test</label>'
@@ -53,15 +52,14 @@
                 '<input class="form-control" id="id_test" name="test" placeholder="Test" required type="text">'
                 "</div>"
             ),
         )
 
     def test_inline_wrapper_class(self):
         """Test field with default CharField widget."""
-
         form = CharFieldTestForm()
 
         self.assertHTMLEqual(
             self.render("{% bootstrap_field form.test layout='inline' %}", context={"form": form}),
             (
                 '<div class="col-12 django_bootstrap5-req">'
                 '<label class="visually-hidden" for="id_test">Test</label>'
```

### Comparing `django-bootstrap5-23.1/tests/test_bootstrap_field_radio_select.py` & `django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_radio_select.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/tests/test_bootstrap_field_select.py` & `django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_select.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/tests/test_bootstrap_field_textarea.py` & `django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_textarea.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/tests/test_bootstrap_form.py` & `django-bootstrap5-23.2.dev0/tests/test_bootstrap_form.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/tests/test_bootstrap_formset.py` & `django-bootstrap5-23.2.dev0/tests/test_bootstrap_formset.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/tests/test_bootstrap_label.py` & `django-bootstrap5-23.2.dev0/tests/test_bootstrap_label.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/tests/test_bootstrap_messages.py` & `django-bootstrap5-23.2.dev0/tests/test_bootstrap_messages.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/tests/test_bootstrap_pagination.py` & `django-bootstrap5-23.2.dev0/tests/test_bootstrap_pagination.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     def test_url_replace_param(self):
         self.assertEqual(url_replace_param("/foo/bar?baz=foo", "baz", "yohoo"), "/foo/bar?baz=yohoo")
         self.assertEqual(url_replace_param("/foo/bar?baz=foo", "baz", None), "/foo/bar")
         self.assertEqual(url_replace_param("/foo/bar#id", "baz", "foo"), "/foo/bar?baz=foo#id")
 
     def bootstrap_pagination(self, page, extra=""):
-        """Helper to test bootstrap_pagination tag."""
+        """Render bootstrap_pagination tag."""
         return self.render(f"{{% bootstrap_pagination page {extra} %}}", {"page": page})
 
     def test_paginator(self):
         html = self.bootstrap_pagination(self.paginator.page(2), extra='url="/projects/?foo=bar"')
         self.assertHTMLEqual(
             html,
             (
```

### Comparing `django-bootstrap5-23.1/tests/test_components.py` & `django-bootstrap5-23.2.dev0/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/tests/test_css.py` & `django-bootstrap5-23.2.dev0/tests/test_css.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/tests/test_settings.py` & `django-bootstrap5-23.2.dev0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/tests/test_size.py` & `django-bootstrap5-23.2.dev0/tests/test_size.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/tests/test_templates.py` & `django-bootstrap5-23.2.dev0/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/tests/test_text.py` & `django-bootstrap5-23.2.dev0/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.1/tests/test_urls.py` & `django-bootstrap5-23.2.dev0/tests/test_urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 from django_bootstrap5.core import get_bootstrap_setting
 
 
 class UrlValidityTestCase(TestCase):
     def test_get_bootstrap_setting(self):
         """Tests that it's possible to pull the URLs listed in the settings, and the hashes match."""
-
         logger = logging.getLogger(__name__)
 
         jsurl = get_bootstrap_setting("javascript_url")
         cssurl = get_bootstrap_setting("css_url")
 
         for link in (jsurl, cssurl):
             req = urllib.request.Request(url=link.get("url"), method="GET")
```

