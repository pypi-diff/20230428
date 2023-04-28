# Comparing `tmp/django-jalali-date-1.0.1.tar.gz` & `tmp/django-jalali-date-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-jalali-date-1.0.1.tar", last modified: Mon Dec 13 19:25:55 2021, max compression
+gzip compressed data, was "django-jalali-date-1.0.2.tar", last modified: Fri Apr 28 19:03:29 2023, max compression
```

## Comparing `django-jalali-date-1.0.1.tar` & `django-jalali-date-1.0.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 19:25:55.935231 django-jalali-date-1.0.1/
--rwxrwxrwx   0 root         (0) root         (0)       99 2019-06-20 10:43:45.000000 django-jalali-date-1.0.1/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)     7653 2021-12-13 19:25:55.935558 django-jalali-date-1.0.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5448 2021-10-22 11:44:52.000000 django-jalali-date-1.0.1/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 19:25:55.905500 django-jalali-date-1.0.1/django_jalali_date.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     7653 2021-12-13 19:25:55.000000 django-jalali-date-1.0.1/django_jalali_date.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2226 2021-12-13 19:25:55.000000 django-jalali-date-1.0.1/django_jalali_date.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2021-12-13 19:25:55.000000 django-jalali-date-1.0.1/django_jalali_date.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2019-06-23 18:27:50.000000 django-jalali-date-1.0.1/django_jalali_date.egg-info/not-zip-safe
--rwxrwxrwx   0 root         (0) root         (0)       17 2021-12-13 19:25:55.000000 django-jalali-date-1.0.1/django_jalali_date.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       12 2021-12-13 19:25:55.000000 django-jalali-date-1.0.1/django_jalali_date.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 19:25:55.908577 django-jalali-date-1.0.1/jalali_date/
--rwxrwxrwx   0 root         (0) root         (0)      523 2019-06-20 10:43:45.000000 django-jalali-date-1.0.1/jalali_date/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1644 2019-12-20 13:00:49.000000 django-jalali-date-1.0.1/jalali_date/admin.py
--rwxrwxrwx   0 root         (0) root         (0)     1930 2019-06-20 10:43:45.000000 django-jalali-date-1.0.1/jalali_date/fields.py
--rwxrwxrwx   0 root         (0) root         (0)     1237 2020-04-02 18:05:29.000000 django-jalali-date-1.0.1/jalali_date/settings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 19:25:55.897967 django-jalali-date-1.0.1/jalali_date/static/
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 19:25:55.898851 django-jalali-date-1.0.1/jalali_date/static/admin/
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 19:25:55.909394 django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/
--rwxrwxrwx   0 root         (0) root         (0)     9386 2019-06-20 10:43:45.000000 django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/default.htm
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 19:25:55.918027 django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/
--rwxrwxrwx   0 root         (0) root         (0)    45960 2019-06-20 10:43:45.000000 django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.all.js
--rwxrwxrwx   0 root         (0) root         (0)     3991 2019-06-20 10:43:45.000000 django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.js
--rwxrwxrwx   0 root         (0) root         (0)    93107 2019-06-20 10:43:45.000000 django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.js
--rwxrwxrwx   0 root         (0) root         (0)   140036 2019-06-20 10:43:45.000000 django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.map
--rwxrwxrwx   0 root         (0) root         (0)     8198 2019-06-20 10:43:45.000000 django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.core.js
--rwxrwxrwx   0 root         (0) root         (0)     4296 2020-02-09 19:52:55.000000 django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc-fa.js
--rwxrwxrwx   0 root         (0) root         (0)    77969 2019-06-20 10:43:45.000000 django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc.js
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 19:25:55.898515 django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 19:25:55.919510 django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 19:25:55.924181 django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/
--rwxrwxrwx   0 root         (0) root         (0)     6992 2019-06-20 10:43:45.000000 django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_444444_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)     6988 2019-06-20 10:43:45.000000 django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_555555_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)     4549 2019-06-20 10:43:45.000000 django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777620_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)     6999 2019-06-20 10:43:45.000000 django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777777_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)     4549 2019-06-20 10:43:45.000000 django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_cc0000_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)     6299 2019-06-20 10:43:45.000000 django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_ffffff_256x240.png
--rwxrwxrwx   0 root         (0) root         (0)    19200 2019-06-20 10:43:45.000000 django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.min.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 19:25:55.929858 django-jalali-date-1.0.1/jalali_date/static/admin/js/
--rwxrwxrwx   0 root         (0) root         (0)   254855 2021-06-04 16:08:38.000000 django-jalali-date-1.0.1/jalali_date/static/admin/js/django_jalali..js
--rwxrwxrwx   0 root         (0) root         (0)   139534 2021-06-04 16:08:38.000000 django-jalali-date-1.0.1/jalali_date/static/admin/js/django_jalali.min.js
--rwxrwxrwx   0 root         (0) root         (0)      306 2021-06-04 16:07:42.000000 django-jalali-date-1.0.1/jalali_date/static/admin/js/main.js
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 19:25:55.899128 django-jalali-date-1.0.1/jalali_date/templates/
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 19:25:55.930569 django-jalali-date-1.0.1/jalali_date/templates/admin/
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 19:25:55.931800 django-jalali-date-1.0.1/jalali_date/templates/admin/edit_inline/
--rwxrwxrwx   0 root         (0) root         (0)     2365 2019-12-20 13:00:49.000000 django-jalali-date-1.0.1/jalali_date/templates/admin/edit_inline/jalali_stacked.html
--rwxrwxrwx   0 root         (0) root         (0)     4301 2019-12-20 13:00:49.000000 django-jalali-date-1.0.1/jalali_date/templates/admin/edit_inline/jalali_tabular.html
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 19:25:55.932563 django-jalali-date-1.0.1/jalali_date/templates/admin/includes/
--rwxrwxrwx   0 root         (0) root         (0)     1878 2019-12-20 13:00:49.000000 django-jalali-date-1.0.1/jalali_date/templates/admin/includes/jalali_fieldset.html
--rwxrwxrwx   0 root         (0) root         (0)      191 2019-06-20 10:43:45.000000 django-jalali-date-1.0.1/jalali_date/templates/admin/jalali_change_form.html
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 19:25:55.933303 django-jalali-date-1.0.1/jalali_date/templates/admin/widgets/
--rwxrwxrwx   0 root         (0) root         (0)      234 2020-02-07 19:35:37.000000 django-jalali-date-1.0.1/jalali_date/templates/admin/widgets/jalali_split_datetime.html
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-12-13 19:25:55.934667 django-jalali-date-1.0.1/jalali_date/templatetags/
--rwxrwxrwx   0 root         (0) root         (0)        0 2019-06-20 10:43:45.000000 django-jalali-date-1.0.1/jalali_date/templatetags/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2002 2019-12-20 13:00:49.000000 django-jalali-date-1.0.1/jalali_date/templatetags/jalali_tags.py
--rwxrwxrwx   0 root         (0) root         (0)     2055 2021-12-13 19:19:21.000000 django-jalali-date-1.0.1/jalali_date/widgets.py
--rwxrwxrwx   0 root         (0) root         (0)       76 2021-12-13 19:25:55.936274 django-jalali-date-1.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1335 2021-12-13 19:19:21.000000 django-jalali-date-1.0.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 19:03:29.829271 django-jalali-date-1.0.2/
+-rwxrwxrwx   0 root         (0) root         (0)       99 2019-06-20 10:43:45.000000 django-jalali-date-1.0.2/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     7938 2023-04-28 19:03:29.829616 django-jalali-date-1.0.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5661 2023-04-28 18:51:14.000000 django-jalali-date-1.0.2/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 19:03:29.791366 django-jalali-date-1.0.2/django_jalali_date.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     7938 2023-04-28 19:03:29.000000 django-jalali-date-1.0.2/django_jalali_date.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2226 2023-04-28 19:03:29.000000 django-jalali-date-1.0.2/django_jalali_date.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-28 19:03:29.000000 django-jalali-date-1.0.2/django_jalali_date.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2019-06-23 18:27:50.000000 django-jalali-date-1.0.2/django_jalali_date.egg-info/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)       17 2023-04-28 19:03:29.000000 django-jalali-date-1.0.2/django_jalali_date.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       12 2023-04-28 19:03:29.000000 django-jalali-date-1.0.2/django_jalali_date.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 19:03:29.797535 django-jalali-date-1.0.2/jalali_date/
+-rwxrwxrwx   0 root         (0) root         (0)      523 2019-06-20 10:43:45.000000 django-jalali-date-1.0.2/jalali_date/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1644 2019-12-20 13:00:49.000000 django-jalali-date-1.0.2/jalali_date/admin.py
+-rwxrwxrwx   0 root         (0) root         (0)     1930 2019-06-20 10:43:45.000000 django-jalali-date-1.0.2/jalali_date/fields.py
+-rwxrwxrwx   0 root         (0) root         (0)     1237 2020-04-02 18:05:29.000000 django-jalali-date-1.0.2/jalali_date/settings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 19:03:29.771999 django-jalali-date-1.0.2/jalali_date/static/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 19:03:29.773171 django-jalali-date-1.0.2/jalali_date/static/admin/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 19:03:29.798496 django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/
+-rwxrwxrwx   0 root         (0) root         (0)     9386 2019-06-20 10:43:45.000000 django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/default.htm
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 19:03:29.813496 django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)    45960 2019-06-20 10:43:45.000000 django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.all.js
+-rwxrwxrwx   0 root         (0) root         (0)     3991 2019-06-20 10:43:45.000000 django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.js
+-rwxrwxrwx   0 root         (0) root         (0)    93107 2019-06-20 10:43:45.000000 django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.js
+-rwxrwxrwx   0 root         (0) root         (0)   140036 2019-06-20 10:43:45.000000 django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.map
+-rwxrwxrwx   0 root         (0) root         (0)     8198 2019-06-20 10:43:45.000000 django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.core.js
+-rwxrwxrwx   0 root         (0) root         (0)     4296 2020-02-09 19:52:55.000000 django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc-fa.js
+-rwxrwxrwx   0 root         (0) root         (0)    77969 2019-06-20 10:43:45.000000 django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc.js
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 19:03:29.772764 django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 19:03:29.814947 django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 19:03:29.819040 django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/
+-rwxrwxrwx   0 root         (0) root         (0)     6992 2019-06-20 10:43:45.000000 django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_444444_256x240.png
+-rwxrwxrwx   0 root         (0) root         (0)     6988 2019-06-20 10:43:45.000000 django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_555555_256x240.png
+-rwxrwxrwx   0 root         (0) root         (0)     4549 2019-06-20 10:43:45.000000 django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777620_256x240.png
+-rwxrwxrwx   0 root         (0) root         (0)     6999 2019-06-20 10:43:45.000000 django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777777_256x240.png
+-rwxrwxrwx   0 root         (0) root         (0)     4549 2019-06-20 10:43:45.000000 django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_cc0000_256x240.png
+-rwxrwxrwx   0 root         (0) root         (0)     6299 2019-06-20 10:43:45.000000 django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_ffffff_256x240.png
+-rwxrwxrwx   0 root         (0) root         (0)    19200 2019-06-20 10:43:45.000000 django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.min.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 19:03:29.824787 django-jalali-date-1.0.2/jalali_date/static/admin/js/
+-rwxrwxrwx   0 root         (0) root         (0)   254855 2021-06-04 16:08:38.000000 django-jalali-date-1.0.2/jalali_date/static/admin/js/django_jalali..js
+-rwxrwxrwx   0 root         (0) root         (0)   139534 2021-06-04 16:08:38.000000 django-jalali-date-1.0.2/jalali_date/static/admin/js/django_jalali.min.js
+-rwxrwxrwx   0 root         (0) root         (0)      306 2021-06-04 16:07:42.000000 django-jalali-date-1.0.2/jalali_date/static/admin/js/main.js
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 19:03:29.773500 django-jalali-date-1.0.2/jalali_date/templates/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 19:03:29.825449 django-jalali-date-1.0.2/jalali_date/templates/admin/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 19:03:29.826590 django-jalali-date-1.0.2/jalali_date/templates/admin/edit_inline/
+-rwxrwxrwx   0 root         (0) root         (0)     2365 2019-12-20 13:00:49.000000 django-jalali-date-1.0.2/jalali_date/templates/admin/edit_inline/jalali_stacked.html
+-rwxrwxrwx   0 root         (0) root         (0)     4301 2019-12-20 13:00:49.000000 django-jalali-date-1.0.2/jalali_date/templates/admin/edit_inline/jalali_tabular.html
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 19:03:29.827148 django-jalali-date-1.0.2/jalali_date/templates/admin/includes/
+-rwxrwxrwx   0 root         (0) root         (0)     2232 2023-04-14 20:45:36.000000 django-jalali-date-1.0.2/jalali_date/templates/admin/includes/jalali_fieldset.html
+-rwxrwxrwx   0 root         (0) root         (0)      191 2019-06-20 10:43:45.000000 django-jalali-date-1.0.2/jalali_date/templates/admin/jalali_change_form.html
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 19:03:29.827771 django-jalali-date-1.0.2/jalali_date/templates/admin/widgets/
+-rwxrwxrwx   0 root         (0) root         (0)      234 2020-02-07 19:35:37.000000 django-jalali-date-1.0.2/jalali_date/templates/admin/widgets/jalali_split_datetime.html
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 19:03:29.828724 django-jalali-date-1.0.2/jalali_date/templatetags/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2019-06-20 10:43:45.000000 django-jalali-date-1.0.2/jalali_date/templatetags/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2002 2019-12-20 13:00:49.000000 django-jalali-date-1.0.2/jalali_date/templatetags/jalali_tags.py
+-rwxrwxrwx   0 root         (0) root         (0)     2055 2021-12-13 19:19:21.000000 django-jalali-date-1.0.2/jalali_date/widgets.py
+-rwxrwxrwx   0 root         (0) root         (0)       76 2023-04-28 19:03:29.830547 django-jalali-date-1.0.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1335 2023-04-28 18:57:46.000000 django-jalali-date-1.0.2/setup.py
```

### Comparing `django-jalali-date-1.0.1/PKG-INFO` & `django-jalali-date-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jalali-date
-Version: 1.0.1
+Version: 1.0.2
 Summary: Jalali Date support for user interface. Easy conversion of DateTimeFiled to JalaliDateTimeField within the admin site, views, forms and templates.
 Home-page: http://github.com/a-roomana/django-jalali-date
 Author: Arman Roomana
 Author-email: roomana.arman@gmail.com
 License: MIT
 Download-URL: https://pypi.python.org/pypi/django-jalali-date/
 Description: 
@@ -25,14 +25,15 @@
         ## Version Compatibility
         #### Python
         - python 3.8 and below is  compatible with 0.3.2 and below
         - python 3.X and above is compatible with 1.0.0 and above
         
         #### Django
         I tested the latest version on some Django versions on python 3.8
+        - django == 4.2
         - django == 3.2.8
         - django == 2.2.24
         
         I think it will work properly on other versions as well.
         
         If you plan to use it in Django 1.X, install version 0.3.2
         
@@ -41,30 +42,30 @@
         ## Install
         
             pip install django-jalali-date   
         
         
         ## Usage
         
-        **settings.py**
+        #### settings.py
         
         - don't forget to make sure you've also added `jalali_date` to your `INSTALLED_APPS`.
         - any global settings for a Django Jalali Date are kept in a single configuration dictionary named `JALALI_DATE_DEFAULTS`
           - you can change the default display of dates by override `Strftime`
           - you can use your own date picker by override `Static` 
         ```python
         INSTALLED_APPS = [
         	'django_apps',
         	
         	'jalali_date',
         	
         	'my_apps',
         ]
         
-        # default settings
+        # default settings (optional)
         JALALI_DATE_DEFAULTS = {
            'Strftime': {
                 'date': '%y/%m/%d',
                 'datetime': '%H:%M:%S _ %y/%m/%d',
             },
             'Static': {
                 'js': [
@@ -82,22 +83,31 @@
                         'admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.min.css',
                     ]
                 }
             },
         }
         ```
         
-        **views.py**
+        (Optional) If you want the names of the dates to be displayed in Farsi, please add the following command to the settings.
+        
+        ```python
+        LANGUAGE_CODE = 'fa'
+        
+        import locale
+        locale.setlocale(locale.LC_ALL, "fa_IR.UTF-8")
+        ```
+        
+        #### views.py
         ```python
         from jalali_date import datetime2jalali, date2jalali
         
         def my_view(request):
         	jalali_join = datetime2jalali(request.user.date_joined).strftime('%y/%m/%d _ %H:%M:%S')
         ```
-        **forms.py**
+        #### forms.py
         ```python
         from django import forms
         from jalali_date.fields import JalaliDateField, SplitJalaliDateTimeField
         from jalali_date.widgets import AdminJalaliDateWidget, AdminSplitJalaliDateTime
         
         
         class TestForm(forms.ModelForm):
@@ -114,15 +124,16 @@
                 # you can added a "class" to this field for use your datepicker!
                 # self.fields['date'].widget.attrs.update({'class': 'jalali_date-date'})
         
                 self.fields['date_time'] = SplitJalaliDateTimeField(label=_('date time'), 
                     widget=AdminSplitJalaliDateTime # required, for decompress DatetimeField to JalaliDateField and JalaliTimeField
                 )
         ```
-        **template.html**
+        
+        #### template.html
         ```html    
         {% load jalali_tags %}
         
         <p>{{ request.user.date_joined|to_jalali:'%y/%m/%d _ %H:%M:%S' }}</p>
         
         <form method="post">{% csrf_token %}
             {{ form.as_p }}
@@ -135,15 +146,15 @@
         		<script src="{% static 'admin/js/django_jalali.min.js' %}"></script>
         	<!-- OR -->
         	<!-- loading by form (if used AdminJalaliDateWidget) -->
         		{{ form.media }}
         ```
         ![example-template-form](http://bayanbox.ir/view/4091856023129600494/photo-2019-04-06-11-11-03-min.jpg)
         
-        **admin.py**
+        #### admin.py
         ```python
         from django.contrib import admin
         from jalali_date import datetime2jalali, date2jalali
         from jalali_date.admin import ModelAdminJalaliMixin, StackedInlineJalaliMixin, TabularInlineJalaliMixin	
             
         class MyInlines1(TabularInlineJalaliMixin, admin.TabularInline):
         	model = SecendModel
@@ -160,19 +171,17 @@
         	raw_id_fields = ('some_fields', )
         	readonly_fields = ('some_fields', 'date_field',)
         	# you can override formfield, for example:
         	formfield_overrides = {
         	    JSONField: {'widget': JSONEditor},
         	}
         	
+        	@admin.display(description='تاریخ ایجاد', ordering='created')
         	def get_created_jalali(self, obj):
-        		return datetime2jalali(obj.created).strftime('%y/%m/%d _ %H:%M:%S')
-        	
-        	get_created_jalali.short_description = 'تاریخ ایجاد'
-        	get_created_jalali.admin_order_field = 'created'
+        		return datetime2jalali(obj.created).strftime('%a, %d %b %Y %H:%M:%S')
         ```
         ![example-admin](http://bayanbox.ir/view/2877111068605695571/Screenshot-from-2016-07-26-01-37-07.png)
         
 Keywords: django jalali date
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-jalali-date-1.0.1/README.md` & `django-jalali-date-1.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 ## Version Compatibility
 #### Python
 - python 3.8 and below is  compatible with 0.3.2 and below
 - python 3.X and above is compatible with 1.0.0 and above
 
 #### Django
 I tested the latest version on some Django versions on python 3.8
+- django == 4.2
 - django == 3.2.8
 - django == 2.2.24
 
 I think it will work properly on other versions as well.
 
 If you plan to use it in Django 1.X, install version 0.3.2
 
@@ -32,30 +33,30 @@
 ## Install
 
     pip install django-jalali-date   
 
 
 ## Usage
 
-**settings.py**
+#### settings.py
 
 - don't forget to make sure you've also added `jalali_date` to your `INSTALLED_APPS`.
 - any global settings for a Django Jalali Date are kept in a single configuration dictionary named `JALALI_DATE_DEFAULTS`
   - you can change the default display of dates by override `Strftime`
   - you can use your own date picker by override `Static` 
 ```python
 INSTALLED_APPS = [
 	'django_apps',
 	
 	'jalali_date',
 	
 	'my_apps',
 ]
 
-# default settings
+# default settings (optional)
 JALALI_DATE_DEFAULTS = {
    'Strftime': {
         'date': '%y/%m/%d',
         'datetime': '%H:%M:%S _ %y/%m/%d',
     },
     'Static': {
         'js': [
@@ -73,22 +74,31 @@
                 'admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.min.css',
             ]
         }
     },
 }
 ```
 
-**views.py**
+(Optional) If you want the names of the dates to be displayed in Farsi, please add the following command to the settings.
+
+```python
+LANGUAGE_CODE = 'fa'
+
+import locale
+locale.setlocale(locale.LC_ALL, "fa_IR.UTF-8")
+```
+
+#### views.py
 ```python
 from jalali_date import datetime2jalali, date2jalali
 
 def my_view(request):
 	jalali_join = datetime2jalali(request.user.date_joined).strftime('%y/%m/%d _ %H:%M:%S')
 ```
-**forms.py**
+#### forms.py
 ```python
 from django import forms
 from jalali_date.fields import JalaliDateField, SplitJalaliDateTimeField
 from jalali_date.widgets import AdminJalaliDateWidget, AdminSplitJalaliDateTime
 
 
 class TestForm(forms.ModelForm):
@@ -105,15 +115,16 @@
         # you can added a "class" to this field for use your datepicker!
         # self.fields['date'].widget.attrs.update({'class': 'jalali_date-date'})
 
         self.fields['date_time'] = SplitJalaliDateTimeField(label=_('date time'), 
             widget=AdminSplitJalaliDateTime # required, for decompress DatetimeField to JalaliDateField and JalaliTimeField
         )
 ```
-**template.html**
+
+#### template.html
 ```html    
 {% load jalali_tags %}
 
 <p>{{ request.user.date_joined|to_jalali:'%y/%m/%d _ %H:%M:%S' }}</p>
 
 <form method="post">{% csrf_token %}
     {{ form.as_p }}
@@ -126,15 +137,15 @@
 		<script src="{% static 'admin/js/django_jalali.min.js' %}"></script>
 	<!-- OR -->
 	<!-- loading by form (if used AdminJalaliDateWidget) -->
 		{{ form.media }}
 ```
 ![example-template-form](http://bayanbox.ir/view/4091856023129600494/photo-2019-04-06-11-11-03-min.jpg)
 
-**admin.py**
+#### admin.py
 ```python
 from django.contrib import admin
 from jalali_date import datetime2jalali, date2jalali
 from jalali_date.admin import ModelAdminJalaliMixin, StackedInlineJalaliMixin, TabularInlineJalaliMixin	
     
 class MyInlines1(TabularInlineJalaliMixin, admin.TabularInline):
 	model = SecendModel
@@ -151,14 +162,12 @@
 	raw_id_fields = ('some_fields', )
 	readonly_fields = ('some_fields', 'date_field',)
 	# you can override formfield, for example:
 	formfield_overrides = {
 	    JSONField: {'widget': JSONEditor},
 	}
 	
+	@admin.display(description='تاریخ ایجاد', ordering='created')
 	def get_created_jalali(self, obj):
-		return datetime2jalali(obj.created).strftime('%y/%m/%d _ %H:%M:%S')
-	
-	get_created_jalali.short_description = 'تاریخ ایجاد'
-	get_created_jalali.admin_order_field = 'created'
+		return datetime2jalali(obj.created).strftime('%a, %d %b %Y %H:%M:%S')
 ```
 ![example-admin](http://bayanbox.ir/view/2877111068605695571/Screenshot-from-2016-07-26-01-37-07.png)
```

### Comparing `django-jalali-date-1.0.1/django_jalali_date.egg-info/PKG-INFO` & `django-jalali-date-1.0.2/django_jalali_date.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jalali-date
-Version: 1.0.1
+Version: 1.0.2
 Summary: Jalali Date support for user interface. Easy conversion of DateTimeFiled to JalaliDateTimeField within the admin site, views, forms and templates.
 Home-page: http://github.com/a-roomana/django-jalali-date
 Author: Arman Roomana
 Author-email: roomana.arman@gmail.com
 License: MIT
 Download-URL: https://pypi.python.org/pypi/django-jalali-date/
 Description: 
@@ -25,14 +25,15 @@
         ## Version Compatibility
         #### Python
         - python 3.8 and below is  compatible with 0.3.2 and below
         - python 3.X and above is compatible with 1.0.0 and above
         
         #### Django
         I tested the latest version on some Django versions on python 3.8
+        - django == 4.2
         - django == 3.2.8
         - django == 2.2.24
         
         I think it will work properly on other versions as well.
         
         If you plan to use it in Django 1.X, install version 0.3.2
         
@@ -41,30 +42,30 @@
         ## Install
         
             pip install django-jalali-date   
         
         
         ## Usage
         
-        **settings.py**
+        #### settings.py
         
         - don't forget to make sure you've also added `jalali_date` to your `INSTALLED_APPS`.
         - any global settings for a Django Jalali Date are kept in a single configuration dictionary named `JALALI_DATE_DEFAULTS`
           - you can change the default display of dates by override `Strftime`
           - you can use your own date picker by override `Static` 
         ```python
         INSTALLED_APPS = [
         	'django_apps',
         	
         	'jalali_date',
         	
         	'my_apps',
         ]
         
-        # default settings
+        # default settings (optional)
         JALALI_DATE_DEFAULTS = {
            'Strftime': {
                 'date': '%y/%m/%d',
                 'datetime': '%H:%M:%S _ %y/%m/%d',
             },
             'Static': {
                 'js': [
@@ -82,22 +83,31 @@
                         'admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.min.css',
                     ]
                 }
             },
         }
         ```
         
-        **views.py**
+        (Optional) If you want the names of the dates to be displayed in Farsi, please add the following command to the settings.
+        
+        ```python
+        LANGUAGE_CODE = 'fa'
+        
+        import locale
+        locale.setlocale(locale.LC_ALL, "fa_IR.UTF-8")
+        ```
+        
+        #### views.py
         ```python
         from jalali_date import datetime2jalali, date2jalali
         
         def my_view(request):
         	jalali_join = datetime2jalali(request.user.date_joined).strftime('%y/%m/%d _ %H:%M:%S')
         ```
-        **forms.py**
+        #### forms.py
         ```python
         from django import forms
         from jalali_date.fields import JalaliDateField, SplitJalaliDateTimeField
         from jalali_date.widgets import AdminJalaliDateWidget, AdminSplitJalaliDateTime
         
         
         class TestForm(forms.ModelForm):
@@ -114,15 +124,16 @@
                 # you can added a "class" to this field for use your datepicker!
                 # self.fields['date'].widget.attrs.update({'class': 'jalali_date-date'})
         
                 self.fields['date_time'] = SplitJalaliDateTimeField(label=_('date time'), 
                     widget=AdminSplitJalaliDateTime # required, for decompress DatetimeField to JalaliDateField and JalaliTimeField
                 )
         ```
-        **template.html**
+        
+        #### template.html
         ```html    
         {% load jalali_tags %}
         
         <p>{{ request.user.date_joined|to_jalali:'%y/%m/%d _ %H:%M:%S' }}</p>
         
         <form method="post">{% csrf_token %}
             {{ form.as_p }}
@@ -135,15 +146,15 @@
         		<script src="{% static 'admin/js/django_jalali.min.js' %}"></script>
         	<!-- OR -->
         	<!-- loading by form (if used AdminJalaliDateWidget) -->
         		{{ form.media }}
         ```
         ![example-template-form](http://bayanbox.ir/view/4091856023129600494/photo-2019-04-06-11-11-03-min.jpg)
         
-        **admin.py**
+        #### admin.py
         ```python
         from django.contrib import admin
         from jalali_date import datetime2jalali, date2jalali
         from jalali_date.admin import ModelAdminJalaliMixin, StackedInlineJalaliMixin, TabularInlineJalaliMixin	
             
         class MyInlines1(TabularInlineJalaliMixin, admin.TabularInline):
         	model = SecendModel
@@ -160,19 +171,17 @@
         	raw_id_fields = ('some_fields', )
         	readonly_fields = ('some_fields', 'date_field',)
         	# you can override formfield, for example:
         	formfield_overrides = {
         	    JSONField: {'widget': JSONEditor},
         	}
         	
+        	@admin.display(description='تاریخ ایجاد', ordering='created')
         	def get_created_jalali(self, obj):
-        		return datetime2jalali(obj.created).strftime('%y/%m/%d _ %H:%M:%S')
-        	
-        	get_created_jalali.short_description = 'تاریخ ایجاد'
-        	get_created_jalali.admin_order_field = 'created'
+        		return datetime2jalali(obj.created).strftime('%a, %d %b %Y %H:%M:%S')
         ```
         ![example-admin](http://bayanbox.ir/view/2877111068605695571/Screenshot-from-2016-07-26-01-37-07.png)
         
 Keywords: django jalali date
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-jalali-date-1.0.1/django_jalali_date.egg-info/SOURCES.txt` & `django-jalali-date-1.0.2/django_jalali_date.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/__init__.py` & `django-jalali-date-1.0.2/jalali_date/__init__.py`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/admin.py` & `django-jalali-date-1.0.2/jalali_date/admin.py`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/fields.py` & `django-jalali-date-1.0.2/jalali_date/fields.py`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/settings.py` & `django-jalali-date-1.0.2/jalali_date/settings.py`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/default.htm` & `django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/default.htm`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.all.js` & `django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.all.js`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.js` & `django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.js`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.js` & `django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.js`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.map` & `django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.map`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.core.js` & `django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.core.js`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc-fa.js` & `django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc-fa.js`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc.js` & `django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc.js`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_444444_256x240.png` & `django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_555555_256x240.png` & `django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777620_256x240.png` & `django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777777_256x240.png` & `django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_cc0000_256x240.png` & `django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_ffffff_256x240.png` & `django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.min.css` & `django-jalali-date-1.0.2/jalali_date/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/static/admin/js/django_jalali..js` & `django-jalali-date-1.0.2/jalali_date/static/admin/js/django_jalali..js`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/static/admin/js/django_jalali.min.js` & `django-jalali-date-1.0.2/jalali_date/static/admin/js/django_jalali.min.js`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/templates/admin/edit_inline/jalali_stacked.html` & `django-jalali-date-1.0.2/jalali_date/templates/admin/edit_inline/jalali_stacked.html`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/templates/admin/edit_inline/jalali_tabular.html` & `django-jalali-date-1.0.2/jalali_date/templates/admin/edit_inline/jalali_tabular.html`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/templates/admin/includes/jalali_fieldset.html` & `django-jalali-date-1.0.2/jalali_date/templates/admin/includes/jalali_fieldset.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 {% load jalali_tags %}
 <fieldset class="module aligned {{ fieldset.classes }}">
     {% if fieldset.name %}<h2>{{ fieldset.name }}</h2>{% endif %}
     {% if fieldset.description %}
         <div class="description">{{ fieldset.description|safe }}</div>
     {% endif %}
     {% for line in fieldset %}
-        <div class="form-row{% if line.fields|length_is:'1' and line.errors %} errors{% endif %}{% if not line.has_visible_field %} hidden{% endif %}{% for field in line %}{% if field.field.name %} field-{{ field.field.name }}{% endif %}{% endfor %}">
-            {% if line.fields|length_is:'1' %}{{ line.errors }}{% endif %}
+        <div class="form-row{% if line.fields|length == 1 and line.errors %} errors{% endif %}{% if not line.has_visible_field %} hidden{% endif %}{% for field in line %}{% if field.field.name %} field-{{ field.field.name }}{% endif %}{% endfor %}">
+            {% if line.fields|length == 1 %}{{ line.errors }}{% else %}<div class="flex-container form-multiline">{% endif %}
             {% for field in line %}
-                <div{% if not line.fields|length_is:'1' %} class="fieldBox field-box{% if field.field.name %} field-{{ field.field.name }}{% endif %}{% if not field.is_readonly and field.errors %} errors{% endif %}{% if field.field.is_hidden %} hidden{% endif %}"{% elif field.is_checkbox %} class="checkbox-row"{% endif %}>
-                    {% if not line.fields|length_is:'1' and not field.is_readonly %}{{ field.errors }}{% endif %}
-                    {% if field.is_checkbox %}
-                        {{ field.field }}{{ field.label_tag }}
-                    {% else %}
-                        {{ field.label_tag }}
-                        {% if field.is_readonly %}
-                            <div class="readonly">{% with field|jalali_admin_safe_readonly as f %}{{ f.contents }}{% endwith %}</div>
+                <div>
+                    {% if not line.fields|length == 1 and not field.is_readonly %}{{ field.errors }}{% endif %}
+                    <div class="flex-container{% if not line.fields|length == 1 %} fieldBox{% if field.field.name %} field-{{ field.field.name }}{% endif %}{% if not field.is_readonly and field.errors %} errors{% endif %}{% if field.field.is_hidden %} hidden{% endif %}{% elif field.is_checkbox %} checkbox-row{% endif %}">
+                        {% if field.is_checkbox %}
+                            {{ field.field }}{{ field.label_tag }}
                         {% else %}
-                            {{ field.field }}
+                            {{ field.label_tag }}
+                            {% if field.is_readonly %}
+                                <div class="readonly">{% with field|jalali_admin_safe_readonly as f %}{{ f.contents }}{% endwith %}</div>
+                            {% else %}
+                                {{ field.field }}
+                            {% endif %}
                         {% endif %}
-                    {% endif %}
+                    </div>
                     {% if field.field.help_text %}
-                        <div class="help">{{ field.field.help_text|safe }}</div>
+                        <div class="help"{% if field.field.id_for_label %} id="{{ field.field.id_for_label }}_helptext"{% endif %}>
+                            <div>{{ field.field.help_text|safe }}</div>
+                        </div>
                     {% endif %}
                 </div>
             {% endfor %}
+            {% if not line.fields|length == 1 %}</div>{% endif %}
         </div>
     {% endfor %}
 </fieldset>
-
```

### Comparing `django-jalali-date-1.0.1/jalali_date/templatetags/jalali_tags.py` & `django-jalali-date-1.0.2/jalali_date/templatetags/jalali_tags.py`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/jalali_date/widgets.py` & `django-jalali-date-1.0.2/jalali_date/widgets.py`

 * *Files identical despite different names*

### Comparing `django-jalali-date-1.0.1/setup.py` & `django-jalali-date-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def read_me(filename):
     return codecs.open(filename, encoding='utf-8').read()
 
 
 setup(
     name='django-jalali-date',
-    version='1.0.1',
+    version='1.0.2',
     python_requires='>=3',
     packages=find_packages(),
     include_package_data=True,
     description=(
         'Jalali Date support for user interface. Easy conversion of DateTimeFiled to JalaliDateTimeField within the admin site, views, forms and templates.'
     ),
     url='http://github.com/a-roomana/django-jalali-date',
```

