# Comparing `tmp/django-eventlog-1.1.tar.gz` & `tmp/django-eventlog-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-eventlog-1.1.tar", last modified: Fri May 11 11:47:19 2018, max compression
+gzip compressed data, was "django-eventlog-1.2.tar", last modified: Fri Apr 28 08:46:51 2023, max compression
```

## Comparing `django-eventlog-1.1.tar` & `django-eventlog-1.2.tar`

### file list

```diff
@@ -1,83 +1,64 @@
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-05-11 11:47:19.000000 django-eventlog-1.1/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-05-11 11:47:19.000000 django-eventlog-1.1/django_eventlog.egg-info/
--rw-r--r--   0 martin     (501) staff       (20)     3725 2018-05-11 11:47:19.000000 django-eventlog-1.1/django_eventlog.egg-info/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)     1990 2018-02-14 09:39:01.000000 django-eventlog-1.1/django_eventlog.egg-info/SOURCES.txt.py
--rw-r--r--   0 martin     (501) staff       (20)        1 2018-02-14 09:39:01.000000 django-eventlog-1.1/django_eventlog.egg-info/dependency_links.txt.py
--rw-r--r--   0 martin     (501) staff       (20)     1990 2018-05-11 11:47:19.000000 django-eventlog-1.1/django_eventlog.egg-info/SOURCES.txt
--rw-r--r--   0 martin     (501) staff       (20)       30 2018-05-11 11:47:19.000000 django-eventlog-1.1/django_eventlog.egg-info/requires.txt
--rw-r--r--   0 martin     (501) staff       (20)        9 2018-02-14 09:39:01.000000 django-eventlog-1.1/django_eventlog.egg-info/top_level.txt.py
--rw-r--r--   0 martin     (501) staff       (20)       30 2018-02-14 09:39:01.000000 django-eventlog-1.1/django_eventlog.egg-info/requires.txt.py
--rw-r--r--   0 martin     (501) staff       (20)        9 2018-05-11 11:47:19.000000 django-eventlog-1.1/django_eventlog.egg-info/top_level.txt
--rw-r--r--   0 martin     (501) staff       (20)        1 2018-05-11 11:47:19.000000 django-eventlog-1.1/django_eventlog.egg-info/dependency_links.txt
--rw-r--r--   0 martin     (501) staff       (20)     3725 2018-05-11 11:47:19.000000 django-eventlog-1.1/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)     1070 2018-02-09 15:46:57.000000 django-eventlog-1.1/LICENSE
--rw-r--r--   0 martin     (501) staff       (20)      229 2018-02-13 09:24:55.000000 django-eventlog-1.1/MANIFEST.in
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-05-11 11:47:19.000000 django-eventlog-1.1/docs/
--rw-r--r--   0 martin     (501) staff       (20)     1814 2018-02-13 11:26:26.000000 django-eventlog-1.1/docs/settings.rst
--rw-r--r--   0 martin     (501) staff       (20)     1669 2018-02-13 14:00:08.000000 django-eventlog-1.1/docs/index.rst
--rw-r--r--   0 martin     (501) staff       (20)      753 2018-02-13 11:37:35.000000 django-eventlog-1.1/docs/testing.rst
--rw-r--r--   0 martin     (501) staff       (20)      612 2018-01-12 17:45:27.000000 django-eventlog-1.1/docs/Makefile
--rw-r--r--   0 martin     (501) staff       (20)     5363 2018-02-13 11:34:07.000000 django-eventlog-1.1/docs/conf.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-05-11 11:47:19.000000 django-eventlog-1.1/docs/_static/
--rw-r--r--   0 martin     (501) staff       (20)   481688 2018-02-13 13:19:56.000000 django-eventlog-1.1/docs/_static/change_list.png
--rw-r--r--   0 martin     (501) staff       (20)   398751 2018-01-11 20:29:07.000000 django-eventlog-1.1/docs/_static/screenshot.png
--rw-r--r--   0 martin     (501) staff       (20)   367782 2018-02-13 13:51:54.000000 django-eventlog-1.1/docs/_static/change_form.png
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-05-11 11:47:19.000000 django-eventlog-1.1/docs/_build/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-05-11 11:47:19.000000 django-eventlog-1.1/docs/_build/html/
--rw-r--r--   0 martin     (501) staff       (20)    12102 2018-02-14 09:39:01.000000 django-eventlog-1.1/docs/_build/html/installation.html.py
--rw-r--r--   0 martin     (501) staff       (20)    10581 2018-02-14 09:39:01.000000 django-eventlog-1.1/docs/_build/html/usage.html.py
--rw-r--r--   0 martin     (501) staff       (20)     6365 2018-02-14 09:39:01.000000 django-eventlog-1.1/docs/_build/html/testing.html.py
--rw-r--r--   0 martin     (501) staff       (20)     4805 2018-02-14 09:39:01.000000 django-eventlog-1.1/docs/_build/html/search.html.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-05-11 11:47:19.000000 django-eventlog-1.1/docs/_build/html/_sources/
--rw-r--r--   0 martin     (501) staff       (20)     2373 2018-02-14 09:39:01.000000 django-eventlog-1.1/docs/_build/html/_sources/installation.rst.txt.py
--rw-r--r--   0 martin     (501) staff       (20)      738 2018-02-14 09:39:01.000000 django-eventlog-1.1/docs/_build/html/_sources/testing.rst.txt.py
--rw-r--r--   0 martin     (501) staff       (20)     1814 2018-02-14 09:39:01.000000 django-eventlog-1.1/docs/_build/html/_sources/settings.rst.txt.py
--rw-r--r--   0 martin     (501) staff       (20)     1465 2018-02-14 09:39:01.000000 django-eventlog-1.1/docs/_build/html/_sources/index.rst.txt.py
--rw-r--r--   0 martin     (501) staff       (20)     2109 2018-02-14 09:39:01.000000 django-eventlog-1.1/docs/_build/html/_sources/usage.rst.txt.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-05-11 11:47:19.000000 django-eventlog-1.1/docs/_build/html/_static/
--rw-r--r--   0 martin     (501) staff       (20)       90 2018-01-12 17:42:06.000000 django-eventlog-1.1/docs/_build/html/_static/plus.png
--rw-r--r--   0 martin     (501) staff       (20)      222 2018-01-12 17:42:06.000000 django-eventlog-1.1/docs/_build/html/_static/down-pressed.png
--rw-r--r--   0 martin     (501) staff       (20)      203 2018-01-12 17:42:06.000000 django-eventlog-1.1/docs/_build/html/_static/up.png
--rw-r--r--   0 martin     (501) staff       (20)      286 2018-01-12 17:42:06.000000 django-eventlog-1.1/docs/_build/html/_static/file.png
--rw-r--r--   0 martin     (501) staff       (20)      214 2018-01-12 17:42:06.000000 django-eventlog-1.1/docs/_build/html/_static/up-pressed.png
--rw-r--r--   0 martin     (501) staff       (20)      202 2018-01-12 17:42:06.000000 django-eventlog-1.1/docs/_build/html/_static/down.png
--rw-r--r--   0 martin     (501) staff       (20)   398751 2018-01-11 20:29:07.000000 django-eventlog-1.1/docs/_build/html/_static/screenshot.png
--rw-r--r--   0 martin     (501) staff       (20)       90 2018-01-12 17:42:06.000000 django-eventlog-1.1/docs/_build/html/_static/minus.png
--rw-r--r--   0 martin     (501) staff       (20)      641 2018-01-12 17:42:06.000000 django-eventlog-1.1/docs/_build/html/_static/comment.png
--rw-r--r--   0 martin     (501) staff       (20)      829 2018-01-12 17:42:06.000000 django-eventlog-1.1/docs/_build/html/_static/comment-close.png
--rw-r--r--   0 martin     (501) staff       (20)      756 2018-01-12 17:42:06.000000 django-eventlog-1.1/docs/_build/html/_static/comment-bright.png
--rw-r--r--   0 martin     (501) staff       (20)     4410 2018-02-14 09:39:01.000000 django-eventlog-1.1/docs/_build/html/genindex.html.py
--rw-r--r--   0 martin     (501) staff       (20)    10082 2018-02-14 09:39:01.000000 django-eventlog-1.1/docs/_build/html/settings.html.py
--rw-r--r--   0 martin     (501) staff       (20)     8325 2018-02-14 09:39:01.000000 django-eventlog-1.1/docs/_build/html/index.html.py
--rw-r--r--   0 martin     (501) staff       (20)     2376 2018-02-13 11:22:58.000000 django-eventlog-1.1/docs/installation.rst
--rw-r--r--   0 martin     (501) staff       (20)      253 2018-05-11 11:38:56.000000 django-eventlog-1.1/Pipfile
--rw-r--r--   0 martin     (501) staff       (20)     1028 2018-05-11 11:44:06.000000 django-eventlog-1.1/setup.py
--rw-r--r--   0 martin     (501) staff       (20)      772 2018-02-13 12:07:21.000000 django-eventlog-1.1/tox.ini
--rw-r--r--   0 martin     (501) staff       (20)       38 2018-05-11 11:47:19.000000 django-eventlog-1.1/setup.cfg
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-05-11 11:47:19.000000 django-eventlog-1.1/eventlog/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-05-11 11:47:19.000000 django-eventlog-1.1/eventlog/migrations/
--rw-r--r--   0 martin     (501) staff       (20)        0 2018-01-12 11:09:15.000000 django-eventlog-1.1/eventlog/migrations/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)     1063 2018-01-12 11:09:15.000000 django-eventlog-1.1/eventlog/migrations/0001_initial.py
--rw-r--r--   0 martin     (501) staff       (20)     2600 2018-02-13 13:42:13.000000 django-eventlog-1.1/eventlog/models.py
--rw-r--r--   0 martin     (501) staff       (20)     2479 2018-05-11 11:41:11.000000 django-eventlog-1.1/eventlog/events.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-05-11 11:47:19.000000 django-eventlog-1.1/eventlog/tests/
--rw-r--r--   0 martin     (501) staff       (20)     3869 2018-02-13 14:08:27.000000 django-eventlog-1.1/eventlog/tests/test_eventlog.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-05-11 11:47:19.000000 django-eventlog-1.1/eventlog/tests/testapp/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-05-11 11:47:19.000000 django-eventlog-1.1/eventlog/tests/testapp/migrations/
--rw-r--r--   0 martin     (501) staff       (20)        0 2018-01-11 19:02:03.000000 django-eventlog-1.1/eventlog/tests/testapp/migrations/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)        0 2018-01-11 19:02:03.000000 django-eventlog-1.1/eventlog/tests/testapp/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)     1701 2018-02-13 13:56:07.000000 django-eventlog-1.1/eventlog/tests/testapp/settings.py
--rw-r--r--   0 martin     (501) staff       (20)      287 2018-01-11 19:46:12.000000 django-eventlog-1.1/eventlog/tests/testapp/urls.py
--rw-r--r--   0 martin     (501) staff       (20)        0 2018-02-13 11:07:59.000000 django-eventlog-1.1/eventlog/tests/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)       84 2018-01-15 13:55:23.000000 django-eventlog-1.1/eventlog/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)     2419 2018-02-13 12:39:43.000000 django-eventlog-1.1/eventlog/apps.py
--rw-r--r--   0 martin     (501) staff       (20)     1485 2018-02-13 13:05:40.000000 django-eventlog-1.1/eventlog/admin.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-05-11 11:47:19.000000 django-eventlog-1.1/eventlog/templates/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-05-11 11:47:19.000000 django-eventlog-1.1/eventlog/templates/admin/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-05-11 11:47:19.000000 django-eventlog-1.1/eventlog/templates/admin/eventlog/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2018-05-11 11:47:19.000000 django-eventlog-1.1/eventlog/templates/admin/eventlog/event/
--rw-r--r--   0 martin     (501) staff       (20)      825 2018-02-13 12:44:49.000000 django-eventlog-1.1/eventlog/templates/admin/eventlog/event/change_list.html
--rw-r--r--   0 martin     (501) staff       (20)     1569 2018-02-13 14:04:46.000000 django-eventlog-1.1/eventlog/templates/admin/eventlog/event/change_form.html
--rw-r--r--   0 martin     (501) staff       (20)     1950 2018-05-11 11:38:59.000000 django-eventlog-1.1/README.rst
--rw-r--r--   0 martin     (501) staff       (20)      491 2018-05-11 11:43:41.000000 django-eventlog-1.1/CHANGELOG.rst
--rw-r--r--   0 martin     (501) staff       (20)    22221 2018-05-11 11:38:56.000000 django-eventlog-1.1/Pipfile.lock
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-28 08:46:51.770320 django-eventlog-1.2/
+-rw-r--r--   0 martin     (501) staff       (20)      590 2023-04-28 08:44:03.000000 django-eventlog-1.2/CHANGELOG.rst
+-rw-r--r--   0 martin     (501) staff       (20)     1070 2023-04-27 19:52:38.000000 django-eventlog-1.2/LICENSE
+-rw-r--r--   0 martin     (501) staff       (20)      229 2023-04-27 19:52:38.000000 django-eventlog-1.2/MANIFEST.in
+-rw-r--r--   0 martin     (501) staff       (20)     3645 2023-04-28 08:46:51.770438 django-eventlog-1.2/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)      465 2023-04-27 20:40:49.000000 django-eventlog-1.2/Pipfile
+-rw-r--r--   0 martin     (501) staff       (20)    30369 2023-04-27 20:42:14.000000 django-eventlog-1.2/Pipfile.lock
+-rw-r--r--   0 martin     (501) staff       (20)     2208 2023-04-28 08:45:57.000000 django-eventlog-1.2/README.rst
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-28 08:46:51.764076 django-eventlog-1.2/django_eventlog.egg-info/
+-rw-r--r--   0 martin     (501) staff       (20)     3645 2023-04-28 08:46:51.000000 django-eventlog-1.2/django_eventlog.egg-info/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)     1250 2023-04-28 08:46:51.000000 django-eventlog-1.2/django_eventlog.egg-info/SOURCES.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2023-04-28 08:46:51.000000 django-eventlog-1.2/django_eventlog.egg-info/dependency_links.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2023-04-27 19:57:33.000000 django-eventlog-1.2/django_eventlog.egg-info/not-zip-safe
+-rw-r--r--   0 martin     (501) staff       (20)       12 2023-04-28 08:46:51.000000 django-eventlog-1.2/django_eventlog.egg-info/requires.txt
+-rw-r--r--   0 martin     (501) staff       (20)        9 2023-04-28 08:46:51.000000 django-eventlog-1.2/django_eventlog.egg-info/top_level.txt
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-28 08:46:51.765184 django-eventlog-1.2/docs/
+-rw-r--r--   0 martin     (501) staff       (20)      612 2023-04-27 19:52:38.000000 django-eventlog-1.2/docs/Makefile
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-28 08:46:51.761085 django-eventlog-1.2/docs/_build/
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-28 08:46:51.761143 django-eventlog-1.2/docs/_build/html/
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-28 08:46:51.766664 django-eventlog-1.2/docs/_build/html/_static/
+-rw-r--r--   0 martin     (501) staff       (20)   367782 2023-04-27 19:52:38.000000 django-eventlog-1.2/docs/_build/html/_static/change_form.png
+-rw-r--r--   0 martin     (501) staff       (20)   481688 2023-04-27 19:52:38.000000 django-eventlog-1.2/docs/_build/html/_static/change_list.png
+-rw-r--r--   0 martin     (501) staff       (20)      286 2023-04-27 20:01:00.000000 django-eventlog-1.2/docs/_build/html/_static/file.png
+-rw-r--r--   0 martin     (501) staff       (20)       90 2023-04-27 20:01:00.000000 django-eventlog-1.2/docs/_build/html/_static/minus.png
+-rw-r--r--   0 martin     (501) staff       (20)       90 2023-04-27 20:01:00.000000 django-eventlog-1.2/docs/_build/html/_static/plus.png
+-rw-r--r--   0 martin     (501) staff       (20)   398751 2023-04-27 19:52:38.000000 django-eventlog-1.2/docs/_build/html/_static/screenshot.png
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-28 08:46:51.767972 django-eventlog-1.2/docs/_static/
+-rw-r--r--   0 martin     (501) staff       (20)   367782 2023-04-27 19:52:38.000000 django-eventlog-1.2/docs/_static/change_form.png
+-rw-r--r--   0 martin     (501) staff       (20)   481688 2023-04-27 19:52:38.000000 django-eventlog-1.2/docs/_static/change_list.png
+-rw-r--r--   0 martin     (501) staff       (20)   398751 2023-04-27 19:52:38.000000 django-eventlog-1.2/docs/_static/screenshot.png
+-rw-r--r--   0 martin     (501) staff       (20)       29 2023-04-27 19:52:38.000000 django-eventlog-1.2/docs/changelog.rst
+-rw-r--r--   0 martin     (501) staff       (20)     5363 2023-04-27 19:52:38.000000 django-eventlog-1.2/docs/conf.py
+-rw-r--r--   0 martin     (501) staff       (20)      127 2023-04-27 19:52:38.000000 django-eventlog-1.2/docs/index.rst
+-rw-r--r--   0 martin     (501) staff       (20)     2376 2023-04-27 19:52:38.000000 django-eventlog-1.2/docs/installation.rst
+-rw-r--r--   0 martin     (501) staff       (20)     1814 2023-04-27 19:52:38.000000 django-eventlog-1.2/docs/settings.rst
+-rw-r--r--   0 martin     (501) staff       (20)      753 2023-04-27 19:52:38.000000 django-eventlog-1.2/docs/testing.rst
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-28 08:46:51.768938 django-eventlog-1.2/eventlog/
+-rw-r--r--   0 martin     (501) staff       (20)       59 2023-04-27 20:28:24.000000 django-eventlog-1.2/eventlog/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     1435 2023-04-27 20:36:35.000000 django-eventlog-1.2/eventlog/admin.py
+-rw-r--r--   0 martin     (501) staff       (20)     2446 2023-04-27 20:36:35.000000 django-eventlog-1.2/eventlog/apps.py
+-rw-r--r--   0 martin     (501) staff       (20)     2539 2023-04-27 20:40:21.000000 django-eventlog-1.2/eventlog/events.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-28 08:46:51.769229 django-eventlog-1.2/eventlog/migrations/
+-rw-r--r--   0 martin     (501) staff       (20)     1399 2023-04-27 20:25:21.000000 django-eventlog-1.2/eventlog/migrations/0001_initial.py
+-rw-r--r--   0 martin     (501) staff       (20)        0 2023-04-27 19:52:38.000000 django-eventlog-1.2/eventlog/migrations/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     2618 2023-04-27 20:40:21.000000 django-eventlog-1.2/eventlog/models.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-28 08:46:51.761487 django-eventlog-1.2/eventlog/templates/
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-28 08:46:51.761540 django-eventlog-1.2/eventlog/templates/admin/
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-28 08:46:51.761591 django-eventlog-1.2/eventlog/templates/admin/eventlog/
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-28 08:46:51.769501 django-eventlog-1.2/eventlog/templates/admin/eventlog/event/
+-rw-r--r--   0 martin     (501) staff       (20)     1569 2023-04-27 19:52:38.000000 django-eventlog-1.2/eventlog/templates/admin/eventlog/event/change_form.html
+-rw-r--r--   0 martin     (501) staff       (20)      825 2023-04-27 19:52:38.000000 django-eventlog-1.2/eventlog/templates/admin/eventlog/event/change_list.html
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-28 08:46:51.769741 django-eventlog-1.2/eventlog/tests/
+-rw-r--r--   0 martin     (501) staff       (20)        0 2023-04-27 19:52:38.000000 django-eventlog-1.2/eventlog/tests/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     3797 2023-04-27 20:40:21.000000 django-eventlog-1.2/eventlog/tests/test_eventlog.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-28 08:46:51.770111 django-eventlog-1.2/eventlog/tests/testapp/
+-rw-r--r--   0 martin     (501) staff       (20)        0 2023-04-27 19:52:38.000000 django-eventlog-1.2/eventlog/tests/testapp/__init__.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-04-28 08:46:51.770229 django-eventlog-1.2/eventlog/tests/testapp/migrations/
+-rw-r--r--   0 martin     (501) staff       (20)        0 2023-04-27 19:52:38.000000 django-eventlog-1.2/eventlog/tests/testapp/migrations/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     1582 2023-04-27 20:36:35.000000 django-eventlog-1.2/eventlog/tests/testapp/settings.py
+-rw-r--r--   0 martin     (501) staff       (20)      294 2023-04-27 20:40:21.000000 django-eventlog-1.2/eventlog/tests/testapp/urls.py
+-rw-r--r--   0 martin     (501) staff       (20)     2295 2023-04-28 08:29:11.000000 django-eventlog-1.2/pyproject.toml
+-rw-r--r--   0 martin     (501) staff       (20)      916 2023-04-28 08:46:51.770723 django-eventlog-1.2/setup.cfg
+-rw-r--r--   0 martin     (501) staff       (20)       59 2023-04-27 19:52:38.000000 django-eventlog-1.2/setup.py
+-rw-r--r--   0 martin     (501) staff       (20)      628 2023-04-28 08:40:04.000000 django-eventlog-1.2/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-eventlog-1.1/django_eventlog.egg-info/PKG-INFO` & `django-eventlog-1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,97 +1,118 @@
 Metadata-Version: 2.1
 Name: django-eventlog
-Version: 1.1
+Version: 1.2
 Summary: django-eventlog stores event messages in a Django model.
-Home-page: https://github.com/bartTC/django-eventlog/
+Home-page: https://github.com/bartTC/django-eventlog
 Author: Martin Mahner
 Author-email: martin@mahner.org
-License: UNKNOWN
-Description: .. image:: https://travis-ci.org/bartTC/django-eventlog.svg?branch=master
-            :target: https://travis-ci.org/bartTC/django-eventlog
-        
-        .. image:: https://codecov.io/github/bartTC/django-eventlog/coverage.svg?branch=master
-            :target: https://codecov.io/github/bartTC/django-eventlog?branch=master
-        
-        Full documentation: https://docs.elephant.house/django-eventlog/
-        
-        ===============
-        django-eventlog
-        ===============
-        
-        django-eventlog is a very simple event logger you can use to track certain
-        actions in your code. Events are stored in a Django model and can be viewed
-        in the Django Admin.
-        
-        Usage Example::
-        
-            from eventlog import EventGroup
-        
-            e = EventGroup()                       # Start a new Event Group
-            e.info('About to send 1000 mails.',    # Trigger an Event
-                   initiator='Mailer Daemon')
-            try:
-                # ... sending 1000 mails
-                e.info('All emails sent!',         # Trigger an Event in the same group,
-                       initiator='Mailer Daemon')  # so they are combined in the admin.
-            except Exception:
-                e.error('There was an error sending the emails.',
-                        initiator='Mailer Daemon')
-        
-        
-        Events can be grouped in a "Event Group" and when hovering over one item
-        in the admin, all events of the same group are highlighted:
-        
-        .. image:: https://github.com/bartTC/django-eventlog/raw/master/docs/_static/change_list.png
-           :scale: 100 %
-        
-        The details view of an event will list all other events of this group so you
-        can track the progress:
-        
-        .. image:: https://github.com/bartTC/django-eventlog/raw/master/docs/_static/change_form.png
-           :scale: 100 %
-        
-        .. note::
-        
-          While looking similar, it's not intended to be a replacement for your
-          regular Python ``logging`` facility, rather an addition to it.
-        
-          django-eventlog stores it's data in a regular database model, so each log entry
-          will trigger a SQL Insert. Therefore you should be careful using it in high
-          performance and/or high volume environments.
-        
-        
-        =========
-        Changelog
-        =========
-        
-        1.1 (2018-05-11)
-        ================
-        
-        - Added ability to manually set a group id to make an EventGroup object
-          reusable through threads.
-        
-        1.0 (2018-02-13)
-        ================
-        
-        - Production ready 1.0 release.
-        - The details Admin view now displays all events of the group with an
-          annotated delay, so you can see the progress of the group.
-        
-        0.9 (2018-02-13)
-        ================
-        
-        - Initial release.
-        - Django 1.8 to 2.0 compatibility.
-        - Python 2.7 to 3.6 compatibility.
-        
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+License: MIT
+Keywords: django,logging,logger,events
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
-Provides-Extra: tests
+Requires-Python: >=3.8
+License-File: LICENSE
+
+.. image:: https://img.shields.io/pypi/v/django-eventlog.svg
+    :target: https://pypi.org/project/django-eventlog/
+
+.. image:: https://github.com/bartTC/django-eventlog/actions/workflows/push.yml/badge.svg
+    :target: https://github.com/bartTC/django-eventlog/actions/workflows/push.yml
+
+-----
+
+📖 **Full documentation: https://django-eventlog.readthedocs.io/**
+
+*Compatibility Matrix:*
+
+========= === === ==== ====
+Py/Dj     3.8 3.9 3.10 3.11
+========= === === ==== ====
+3.2 (LTS)  ✓   ✓   ✓    ✓
+4.0        ✓   ✓   ✓    ✓
+4.1        ✓   ✓   ✓    ✓
+4.2 (LTS)  ✓   ✓   ✓    ✓
+========= === === ==== ====
+
+django-eventlog
+===============
+
+django-eventlog is a very simple event logger you can use to track certain
+actions in your code. Events are stored in a Django model and can be viewed
+in the Django Admin.
+
+Usage Example::
+
+    from eventlog import EventGroup
+
+    e = EventGroup()                       # Start a new Event Group
+    e.info('About to send 1000 mails.',    # Trigger an Event
+           initiator='Mailer Daemon')
+    try:
+        # ... sending 1000 mails
+        e.info('All emails sent!',         # Trigger an Event in the same group,
+               initiator='Mailer Daemon')  # so they are combined in the admin.
+    except Exception:
+        e.error('There was an error sending the emails.',
+                initiator='Mailer Daemon')
+
+
+Events can be grouped in a "Event Group" and when hovering over one item
+in the admin, all events of the same group are highlighted:
+
+.. image:: https://github.com/bartTC/django-eventlog/raw/main/docs/_static/change_list.png
+   :scale: 100 %
+
+The details view of an event will list all other events of this group so you
+can track the progress:
+
+.. image:: https://github.com/bartTC/django-eventlog/raw/main/docs/_static/change_form.png
+   :scale: 100 %
+
+.. note::
+
+  While looking similar, it's not intended to be a replacement for your
+  regular Python ``logging`` facility, rather an addition to it.
+
+  django-eventlog stores it's data in a regular database model, so each log entry
+  will trigger a SQL Insert. Therefore you should be careful using it in high
+  performance and/or high volume environments.
+
+=========
+Changelog
+=========
+
+1.2 (2023-04-28)
+================
+
+- Python 3.7 to 3.11 compatibility
+- Django 3.2 to 4.2 support
+
+1.1 (2018-05-11)
+================
+
+- Added ability to manually set a group id to make an EventGroup object
+  reusable through threads.
+
+1.0 (2018-02-13)
+================
+
+- Production ready 1.0 release.
+- The details Admin view now displays all events of the group with an
+  annotated delay, so you can see the progress of the group.
+
+0.9 (2018-02-13)
+================
+
+- Initial release.
+- Django 1.8 to 2.0 compatibility.
+- Python 2.7 to 3.6 compatibility.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-eventlog-1.1/django_eventlog.egg-info/SOURCES.txt` & `django-eventlog-1.2/django_eventlog.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,36 @@
 CHANGELOG.rst
 LICENSE
 MANIFEST.in
 Pipfile
 Pipfile.lock
 README.rst
+pyproject.toml
+setup.cfg
 setup.py
 tox.ini
 django_eventlog.egg-info/PKG-INFO
 django_eventlog.egg-info/SOURCES.txt
-django_eventlog.egg-info/SOURCES.txt.py
 django_eventlog.egg-info/dependency_links.txt
-django_eventlog.egg-info/dependency_links.txt.py
+django_eventlog.egg-info/not-zip-safe
 django_eventlog.egg-info/requires.txt
-django_eventlog.egg-info/requires.txt.py
 django_eventlog.egg-info/top_level.txt
-django_eventlog.egg-info/top_level.txt.py
 docs/Makefile
+docs/changelog.rst
 docs/conf.py
 docs/index.rst
 docs/installation.rst
 docs/settings.rst
 docs/testing.rst
-docs/_build/html/genindex.html.py
-docs/_build/html/index.html.py
-docs/_build/html/installation.html.py
-docs/_build/html/search.html.py
-docs/_build/html/settings.html.py
-docs/_build/html/testing.html.py
-docs/_build/html/usage.html.py
-docs/_build/html/_sources/index.rst.txt.py
-docs/_build/html/_sources/installation.rst.txt.py
-docs/_build/html/_sources/settings.rst.txt.py
-docs/_build/html/_sources/testing.rst.txt.py
-docs/_build/html/_sources/usage.rst.txt.py
-docs/_build/html/_static/comment-bright.png
-docs/_build/html/_static/comment-close.png
-docs/_build/html/_static/comment.png
-docs/_build/html/_static/down-pressed.png
-docs/_build/html/_static/down.png
+docs/_build/html/_static/change_form.png
+docs/_build/html/_static/change_list.png
 docs/_build/html/_static/file.png
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/plus.png
 docs/_build/html/_static/screenshot.png
-docs/_build/html/_static/up-pressed.png
-docs/_build/html/_static/up.png
 docs/_static/change_form.png
 docs/_static/change_list.png
 docs/_static/screenshot.png
 eventlog/__init__.py
 eventlog/admin.py
 eventlog/apps.py
 eventlog/events.py
```

### Comparing `django-eventlog-1.1/PKG-INFO` & `django-eventlog-1.2/django_eventlog.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,97 +1,118 @@
 Metadata-Version: 2.1
 Name: django-eventlog
-Version: 1.1
+Version: 1.2
 Summary: django-eventlog stores event messages in a Django model.
-Home-page: https://github.com/bartTC/django-eventlog/
+Home-page: https://github.com/bartTC/django-eventlog
 Author: Martin Mahner
 Author-email: martin@mahner.org
-License: UNKNOWN
-Description: .. image:: https://travis-ci.org/bartTC/django-eventlog.svg?branch=master
-            :target: https://travis-ci.org/bartTC/django-eventlog
-        
-        .. image:: https://codecov.io/github/bartTC/django-eventlog/coverage.svg?branch=master
-            :target: https://codecov.io/github/bartTC/django-eventlog?branch=master
-        
-        Full documentation: https://docs.elephant.house/django-eventlog/
-        
-        ===============
-        django-eventlog
-        ===============
-        
-        django-eventlog is a very simple event logger you can use to track certain
-        actions in your code. Events are stored in a Django model and can be viewed
-        in the Django Admin.
-        
-        Usage Example::
-        
-            from eventlog import EventGroup
-        
-            e = EventGroup()                       # Start a new Event Group
-            e.info('About to send 1000 mails.',    # Trigger an Event
-                   initiator='Mailer Daemon')
-            try:
-                # ... sending 1000 mails
-                e.info('All emails sent!',         # Trigger an Event in the same group,
-                       initiator='Mailer Daemon')  # so they are combined in the admin.
-            except Exception:
-                e.error('There was an error sending the emails.',
-                        initiator='Mailer Daemon')
-        
-        
-        Events can be grouped in a "Event Group" and when hovering over one item
-        in the admin, all events of the same group are highlighted:
-        
-        .. image:: https://github.com/bartTC/django-eventlog/raw/master/docs/_static/change_list.png
-           :scale: 100 %
-        
-        The details view of an event will list all other events of this group so you
-        can track the progress:
-        
-        .. image:: https://github.com/bartTC/django-eventlog/raw/master/docs/_static/change_form.png
-           :scale: 100 %
-        
-        .. note::
-        
-          While looking similar, it's not intended to be a replacement for your
-          regular Python ``logging`` facility, rather an addition to it.
-        
-          django-eventlog stores it's data in a regular database model, so each log entry
-          will trigger a SQL Insert. Therefore you should be careful using it in high
-          performance and/or high volume environments.
-        
-        
-        =========
-        Changelog
-        =========
-        
-        1.1 (2018-05-11)
-        ================
-        
-        - Added ability to manually set a group id to make an EventGroup object
-          reusable through threads.
-        
-        1.0 (2018-02-13)
-        ================
-        
-        - Production ready 1.0 release.
-        - The details Admin view now displays all events of the group with an
-          annotated delay, so you can see the progress of the group.
-        
-        0.9 (2018-02-13)
-        ================
-        
-        - Initial release.
-        - Django 1.8 to 2.0 compatibility.
-        - Python 2.7 to 3.6 compatibility.
-        
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+License: MIT
+Keywords: django,logging,logger,events
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
-Provides-Extra: tests
+Requires-Python: >=3.8
+License-File: LICENSE
+
+.. image:: https://img.shields.io/pypi/v/django-eventlog.svg
+    :target: https://pypi.org/project/django-eventlog/
+
+.. image:: https://github.com/bartTC/django-eventlog/actions/workflows/push.yml/badge.svg
+    :target: https://github.com/bartTC/django-eventlog/actions/workflows/push.yml
+
+-----
+
+📖 **Full documentation: https://django-eventlog.readthedocs.io/**
+
+*Compatibility Matrix:*
+
+========= === === ==== ====
+Py/Dj     3.8 3.9 3.10 3.11
+========= === === ==== ====
+3.2 (LTS)  ✓   ✓   ✓    ✓
+4.0        ✓   ✓   ✓    ✓
+4.1        ✓   ✓   ✓    ✓
+4.2 (LTS)  ✓   ✓   ✓    ✓
+========= === === ==== ====
+
+django-eventlog
+===============
+
+django-eventlog is a very simple event logger you can use to track certain
+actions in your code. Events are stored in a Django model and can be viewed
+in the Django Admin.
+
+Usage Example::
+
+    from eventlog import EventGroup
+
+    e = EventGroup()                       # Start a new Event Group
+    e.info('About to send 1000 mails.',    # Trigger an Event
+           initiator='Mailer Daemon')
+    try:
+        # ... sending 1000 mails
+        e.info('All emails sent!',         # Trigger an Event in the same group,
+               initiator='Mailer Daemon')  # so they are combined in the admin.
+    except Exception:
+        e.error('There was an error sending the emails.',
+                initiator='Mailer Daemon')
+
+
+Events can be grouped in a "Event Group" and when hovering over one item
+in the admin, all events of the same group are highlighted:
+
+.. image:: https://github.com/bartTC/django-eventlog/raw/main/docs/_static/change_list.png
+   :scale: 100 %
+
+The details view of an event will list all other events of this group so you
+can track the progress:
+
+.. image:: https://github.com/bartTC/django-eventlog/raw/main/docs/_static/change_form.png
+   :scale: 100 %
+
+.. note::
+
+  While looking similar, it's not intended to be a replacement for your
+  regular Python ``logging`` facility, rather an addition to it.
+
+  django-eventlog stores it's data in a regular database model, so each log entry
+  will trigger a SQL Insert. Therefore you should be careful using it in high
+  performance and/or high volume environments.
+
+=========
+Changelog
+=========
+
+1.2 (2023-04-28)
+================
+
+- Python 3.7 to 3.11 compatibility
+- Django 3.2 to 4.2 support
+
+1.1 (2018-05-11)
+================
+
+- Added ability to manually set a group id to make an EventGroup object
+  reusable through threads.
+
+1.0 (2018-02-13)
+================
+
+- Production ready 1.0 release.
+- The details Admin view now displays all events of the group with an
+  annotated delay, so you can see the progress of the group.
+
+0.9 (2018-02-13)
+================
+
+- Initial release.
+- Django 1.8 to 2.0 compatibility.
+- Python 2.7 to 3.6 compatibility.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-eventlog-1.1/LICENSE` & `django-eventlog-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-eventlog-1.1/docs/settings.rst` & `django-eventlog-1.2/docs/settings.rst`

 * *Files identical despite different names*

### Comparing `django-eventlog-1.1/docs/index.rst` & `django-eventlog-1.2/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,30 @@
-.. _index:
+.. image:: https://img.shields.io/pypi/v/django-eventlog.svg
+    :target: https://pypi.org/project/django-eventlog/
 
-===============
-django-eventlog
-===============
+.. image:: https://github.com/bartTC/django-eventlog/actions/workflows/push.yml/badge.svg
+    :target: https://github.com/bartTC/django-eventlog/actions/workflows/push.yml
 
-.. toctree::
-   :maxdepth: 1
+-----
 
-   installation
-   settings
-   testing
+📖 **Full documentation: https://django-eventlog.readthedocs.io/**
+
+*Compatibility Matrix:*
+
+========= === === ==== ====
+Py/Dj     3.8 3.9 3.10 3.11
+========= === === ==== ====
+3.2 (LTS)  ✓   ✓   ✓    ✓
+4.0        ✓   ✓   ✓    ✓
+4.1        ✓   ✓   ✓    ✓
+4.2 (LTS)  ✓   ✓   ✓    ✓
+========= === === ==== ====
+
+django-eventlog
+===============
 
 django-eventlog is a very simple event logger you can use to track certain
 actions in your code. Events are stored in a Django model and can be viewed
 in the Django Admin.
 
 Usage Example::
 
@@ -30,21 +41,21 @@
         e.error('There was an error sending the emails.',
                 initiator='Mailer Daemon')
 
 
 Events can be grouped in a "Event Group" and when hovering over one item
 in the admin, all events of the same group are highlighted:
 
-.. image:: https://github.com/bartTC/django-eventlog/raw/master/docs/_static/change_list.png
+.. image:: https://github.com/bartTC/django-eventlog/raw/main/docs/_static/change_list.png
    :scale: 100 %
 
 The details view of an event will list all other events of this group so you
 can track the progress:
 
-.. image:: https://github.com/bartTC/django-eventlog/raw/master/docs/_static/change_form.png
+.. image:: https://github.com/bartTC/django-eventlog/raw/main/docs/_static/change_form.png
    :scale: 100 %
 
 .. note::
 
   While looking similar, it's not intended to be a replacement for your
   regular Python ``logging`` facility, rather an addition to it.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-eventlog-1.1/docs/testing.rst` & `django-eventlog-1.2/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `django-eventlog-1.1/docs/Makefile` & `django-eventlog-1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-eventlog-1.1/docs/conf.py` & `django-eventlog-1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-eventlog-1.1/docs/_static/change_list.png` & `django-eventlog-1.2/docs/_build/html/_static/change_list.png`

 * *Files identical despite different names*

### Comparing `django-eventlog-1.1/docs/_static/screenshot.png` & `django-eventlog-1.2/docs/_build/html/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `django-eventlog-1.1/docs/_static/change_form.png` & `django-eventlog-1.2/docs/_build/html/_static/change_form.png`

 * *Files identical despite different names*

### Comparing `django-eventlog-1.1/docs/_build/html/_static/screenshot.png` & `django-eventlog-1.2/docs/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `django-eventlog-1.1/docs/installation.rst` & `django-eventlog-1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django-eventlog-1.1/eventlog/migrations/0001_initial.py` & `django-eventlog-1.2/eventlog/migrations/0001_initial.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,44 @@
 # Generated by Django 2.0.1 on 2018-01-12 05:09
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
-    dependencies = [
-    ]
+    dependencies = []
 
     operations = [
         migrations.CreateModel(
-            name='Event',
+            name="Event",
             fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('type', models.CharField(max_length=50, verbose_name='Event Type')),
-                ('group', models.UUIDField(verbose_name='Event Group')),
-                ('timestamp', models.DateTimeField(auto_now_add=True, verbose_name='Timestamp')),
-                ('message', models.CharField(max_length=500, verbose_name='Message')),
-                ('initiator', models.CharField(blank=True, max_length=500, null=True, verbose_name='Initiator')),
+                (
+                    "id",
+                    models.AutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                ("type", models.CharField(max_length=50, verbose_name="Event Type")),
+                ("group", models.UUIDField(verbose_name="Event Group")),
+                (
+                    "timestamp",
+                    models.DateTimeField(auto_now_add=True, verbose_name="Timestamp"),
+                ),
+                ("message", models.CharField(max_length=500, verbose_name="Message")),
+                (
+                    "initiator",
+                    models.CharField(
+                        blank=True, max_length=500, null=True, verbose_name="Initiator"
+                    ),
+                ),
             ],
             options={
-                'verbose_name': 'Event Log',
-                'verbose_name_plural': 'Event Logs',
-                'ordering': ('-timestamp',),
+                "verbose_name": "Event Log",
+                "verbose_name_plural": "Event Logs",
+                "ordering": ("-timestamp",),
             },
         ),
     ]
```

### Comparing `django-eventlog-1.1/eventlog/models.py` & `django-eventlog-1.2/eventlog/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 from datetime import datetime, timedelta
 from logging import getLogger
-import re
 
 from django.apps import apps
 from django.db import models
 from django.utils.safestring import mark_safe
-from django.utils.translation import ugettext_lazy as _, ugettext_lazy
+from django.utils.translation import gettext_lazy as _
 
 logger = getLogger(__file__)
-config = apps.get_app_config('eventlog')
+config = apps.get_app_config("eventlog")
 
 
 class EventLogManager(models.Manager):
     def purge(self, days=30):
         """
         Delete all events older than <days> days.
         """
-        return self.filter(
-            timestamp__gt=datetime.now() - timedelta(days=days)
-        ).delete()
+        return self.filter(timestamp__gt=datetime.now() - timedelta(days=days)).delete()
 
 
 class Event(models.Model):
     """
     Event log model.
     """
-    type = models.CharField(_('Event Type'), max_length=50)
-    group = models.UUIDField(_('Event Group'))
-    timestamp = models.DateTimeField(_('Timestamp'), auto_now_add=True)
-    message = models.CharField(_('Message'), max_length=500)
-    initiator = models.CharField(_('Initiator'), max_length=500, blank=True, null=True)
+
+    type = models.CharField(_("Event Type"), max_length=50)
+    group = models.UUIDField(_("Event Group"))
+    timestamp = models.DateTimeField(_("Timestamp"), auto_now_add=True)
+    message = models.CharField(_("Message"), max_length=500)
+    initiator = models.CharField(_("Initiator"), max_length=500, blank=True, null=True)
 
     objects = EventLogManager()
 
     class Meta:
-        ordering = ('-timestamp',)
-        verbose_name = _('Event Log')
-        verbose_name_plural = _('Event Logs')
+        ordering = ("-timestamp",)
+        verbose_name = _("Event Log")
+        verbose_name_plural = _("Event Logs")
 
     def __str__(self):
-        return '{group} - {type} - {message}...'.format(
+        return "{group} - {type} - {message}...".format(
             group=self.group_label,
             type=self.type,
-            message=self.message[:40])
+            message=self.message[:40],
+        )
 
     @property
     def group_label(self):
         return self.group.hex[-6:]
 
     @property
     def type_label(self):
         event_types = config.get_event_types()
         label = event_types.get(self.type, None)
+
         if not label:
             return self.type.capitalize()
+        # fmt: off
         s = '<span class="eventType" style="{color} {bgcolor}">{label}</span>'.format(
-            color='color: {0};'.format(label['color']) if label.get('color', None) else '',
-            bgcolor='background-color: {0};'.format(label['bgcolor']) if label.get('bgcolor', None) else '',
-            label=label['label'])
+            color="color: {};".format(label["color"]) if label.get("color", None) else "",
+            bgcolor="background-color: {};".format(label["bgcolor"]) if label.get("bgcolor", None) else "",
+            label=label["label"],
+        )
+        # fmt: on
         return mark_safe(s)
 
     def get_all_group_events(self):
         """
         Get all events which are in the same Event group as this event.
         """
-        qs = Event.objects.filter(group=self.group).order_by('timestamp')
+        qs = Event.objects.filter(group=self.group).order_by("timestamp")
         # Annotate the delay between events
         last = None
         for e in qs:
             if last:
                 delay = int((e.timestamp - last.timestamp).total_seconds())
                 delay_minutes, delayseconds = divmod(delay, 60)
-                e.timestamp_delay = ugettext_lazy('{min}m {sec}s').format(
-                    min=delay_minutes, sec=delayseconds
+                e.timestamp_delay = _("{min}m {sec}s").format(
+                    min=delay_minutes,
+                    sec=delayseconds,
                 )
             last = e
         return qs
```

### Comparing `django-eventlog-1.1/eventlog/events.py` & `django-eventlog-1.2/eventlog/events.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 from uuid import uuid4
 
 from django.apps import apps
 from django.core.mail import send_mail as django_send_mail
 from django.utils.html import linebreaks
 
+
 def generate_group_id():
     return uuid4().hex
 
-class EventGroup(object):
+
+class EventGroup:
     """
     Enterprise Event Object Factory.
     """
+
     group_id = None
     event_types = None
     send_mail = None
 
     def __init__(self, send_mail=None, group_id=None):
-        self.config = apps.get_app_config('eventlog')
+        self.config = apps.get_app_config("eventlog")
         self.group_id = group_id or generate_group_id()
         self.event_types = self.config.get_event_types()
         self.send_mail = send_mail
 
     def __getattr__(self, attr):
-        if attr in self.event_types.keys():
+        if attr in self.event_types:
+
             def f(*args, **kwargs):
                 return self._log_event(attr, *args, **kwargs)
+
             f.__name__ = attr
             return f
-        raise AttributeError('Event type "{}" does not exist'.format(attr))
+        raise AttributeError(f'Event type "{attr}" does not exist')
 
     def _log_event(self, type, message, initiator=None, send_mail=None):
         """
         Log a new event entry.
         """
-        EventModel = apps.get_model('eventlog', 'Event')
+        EventModel = apps.get_model("eventlog", "Event")
         event_object = EventModel.objects.create(
-            type=type, group=self.group_id, message=message, initiator=initiator)
+            type=type,
+            group=self.group_id,
+            message=message,
+            initiator=initiator,
+        )
 
         # Mail this event per email. Either if this method has it enabled,
         # or if its globally enabled for the EventGroup.
         mail = send_mail or self.send_mail
         if mail:
             self._send_mail(mail, event_object)
 
@@ -47,25 +56,27 @@
         """
         Send a simple HTML email to the recipient defined in :email:.
         """
         type_label = self.event_types.get(event_object.type, None)
         if not type_label:
             return event_object.type.capitalize()
         context = {
-            'type': type_label,
-            'message': event_object.message,
-            'initiator': event_object.initiator,
-            'date': event_object.timestamp
+            "type": type_label,
+            "message": event_object.message,
+            "initiator": event_object.initiator,
+            "date": event_object.timestamp,
         }
         subject = self.config.email_subject_template.format(**context)
         text_message = self.config.email_template.format(**context)
-        html_message = '<html><body>{html}</body></html>'.format(
-            html=linebreaks(text_message))
+        html_message = "<html><body>{html}</body></html>".format(
+            html=linebreaks(text_message),
+        )
 
         django_send_mail(
             subject=subject,
             message=text_message,
             html_message=html_message,
             recipient_list=[email],
             from_email=self.config.email_from,
-            fail_silently=self.config.email_fail_silently
+            fail_silently=self.config.email_fail_silently,
         )
+        return None
```

### Comparing `django-eventlog-1.1/eventlog/tests/test_eventlog.py` & `django-eventlog-1.2/eventlog/tests/test_eventlog.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,114 +1,119 @@
 from uuid import uuid4
 
 from django.core import mail
 from django.test import TestCase
-
-try:
-    from django.urls import reverse
-except ImportError:
-    from django.core.urlresolvers import reverse
+from django.urls import reverse
 
 
 class EventLogTestCase(TestCase):
     def test_simple_log(self):
         """Simple log item."""
         from eventlog import EventGroup
         from eventlog.models import Event
+
         e = EventGroup()
-        e.info('Hello World')
+        e.info("Hello World")
         self.assertEqual(Event.objects.count(), 1)
 
     def test_multi_log(self):
         """Multiple log items."""
         from eventlog import EventGroup
         from eventlog.models import Event
+
         e = EventGroup()
-        e.info('Hello World')
-        e.error('Hello World')
-        e.warning('Hello World')
-        e.critical('Hello World')
+        e.info("Hello World")
+        e.error("Hello World")
+        e.warning("Hello World")
+        e.critical("Hello World")
         self.assertEqual(Event.objects.count(), 4)
 
     def test_invalid_type(self):
         """Calling an invalid type will raise an error."""
         from eventlog import EventGroup
+
         e = EventGroup()
         with self.assertRaises(AttributeError):
-            e.doesnotexist('Hello World')
+            e.doesnotexist("Hello World")
 
     def test_mail_per_event(self):
         """Send one mail per event."""
         from eventlog import EventGroup
         from eventlog.models import Event
+
         e = EventGroup()
-        e.info('Hello World', send_mail='user@example.com')
-        e.error('Hello World')
-        e.warning('Hello World')
-        e.critical('Hello World', send_mail='user@example.com')
+        e.info("Hello World", send_mail="user@example.com")
+        e.error("Hello World")
+        e.warning("Hello World")
+        e.critical("Hello World", send_mail="user@example.com")
         self.assertEqual(Event.objects.count(), 4)
         self.assertEqual(len(mail.outbox), 2)
 
     def test_mail_per_group(self):
         """Send one mail per event."""
         from eventlog import EventGroup
         from eventlog.models import Event
-        e = EventGroup(send_mail='user@example.com')
-        e.info('Hello World')
-        e.error('Hello World')
-        e.warning('Hello World')
-        e.critical('Hello World') # Explicitly disabled
+
+        e = EventGroup(send_mail="user@example.com")
+        e.info("Hello World")
+        e.error("Hello World")
+        e.warning("Hello World")
+        e.critical("Hello World")  # Explicitly disabled
         self.assertEqual(Event.objects.count(), 4)
         self.assertEqual(len(mail.outbox), 4)
 
     def test_admin_changelist(self):
         """Admin Changelist is OK"""
+        from django.contrib.auth.models import User
+
         from eventlog import EventGroup
         from eventlog.models import Event
-        from django.contrib.auth.models import User
 
         # Regular Event
         e = EventGroup()
-        e.info('Hello World')
-        e.info('Hello World 2')
-        e.error('Hello World 3')
-        e.warning('Hello World 4')
+        e.info("Hello World")
+        e.info("Hello World 2")
+        e.error("Hello World 3")
+        e.warning("Hello World 4")
 
         # Legacy Event (Created and in database, but its type no longer valid)
         Event.objects.create(
-            type='Legacy Event',
+            type="Legacy Event",
             group=uuid4().hex,
-            message='This is some info.',
-            initiator='Test Runner'
+            message="This is some info.",
+            initiator="Test Runner",
         )
 
-        User.objects.create_superuser('jon', 'jon@example.com', 'foobar')
-        self.client.login(username='jon', password='foobar')
+        User.objects.create_superuser("jon", "jon@example.com", "foobar")
+        self.client.login(username="jon", password="foobar")
 
-        changelist_url = reverse('admin:{0}_{1}_changelist'.format('eventlog', 'event'))
+        changelist_url = reverse("admin:{}_{}_changelist".format("eventlog", "event"))
         response = self.client.get(changelist_url)
 
         self.assertEqual(response.status_code, 200)
-        self.assertContains(response, 'Hello World')
+        self.assertContains(response, "Hello World")
 
     def test_admin_changeform(self):
         """Admin Changeform is OK"""
+        from django.contrib.auth.models import User
+
         from eventlog import EventGroup
         from eventlog.models import Event
-        from django.contrib.auth.models import User
 
         e = EventGroup()
-        e.info('Hello World')
-        e.info('Hello World 2')
-        e.error('Hello World 3')
-        e.warning('Hello World 4')
+        e.info("Hello World")
+        e.info("Hello World 2")
+        e.error("Hello World 3")
+        e.warning("Hello World 4")
 
         obj = Event.objects.first()
-        User.objects.create_superuser('jon', 'jon@example.com', 'foobar')
-        self.client.login(username='jon', password='foobar')
+        User.objects.create_superuser("jon", "jon@example.com", "foobar")
+        self.client.login(username="jon", password="foobar")
 
-        changelist_url = reverse('admin:{0}_{1}_change'.format('eventlog', 'event'),
-                                 args=(obj.pk,))
+        changelist_url = reverse(
+            "admin:{}_{}_change".format("eventlog", "event"),
+            args=(obj.pk,),
+        )
         response = self.client.get(changelist_url)
 
         self.assertEqual(response.status_code, 200)
-        self.assertContains(response, 'Hello World')
+        self.assertContains(response, "Hello World")
```

### Comparing `django-eventlog-1.1/eventlog/apps.py` & `django-eventlog-1.2/eventlog/apps.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django.apps import AppConfig
 from django.conf import settings
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 
 class EventLogConfig(AppConfig):
-    name = 'eventlog'
-    verbose_name = 'EventLog'
+    name = "eventlog"
+    verbose_name = "EventLog"
 
     # List of event types to be used in events. A list of dictionaries
     # in the format::
     #
     #     {
     #         'name': 'info',      # The method name.
     #         'label': _('Info'),  # Human readable label
@@ -19,37 +19,38 @@
     #
     # Method names must be lowercase and only contain strings, numbers and
     # underscores, but must not start with either a number or underscore.
     # The max length is 50 characters.
     #
     # This is OK:  yolo, hello_world, jerry123
     # This is NOK: _yolo, 1pineappleplease,
+    # fmt: off
     event_types = {
-        'info': {
-            'label': _('Info'),
-            'color': None,
-            'bgcolor': None,
+        "info": {
+            "label": _("Info"),
+            "color": None,
+            "bgcolor": None,
         },
-        'warning': {
-            'label': _('Warning'),
-            'color': None,
-            'bgcolor': None,
+        "warning": {
+            "label": _("Warning"),
+            "color": None,
+            "bgcolor": None,
         },
-        'error': {
-            'label': _('Error'),
-            'color': 'red',
-            'bgcolor': None,
+        "error": {
+            "label": _("Error"),
+            "color": "red",
+            "bgcolor": None,
         },
-        'critical': {
-            'label': _('Critical'),
-            'color': 'white',
-            'bgcolor': 'red',
+        "critical": {
+            "label": _("Critical"),
+            "color": "white",
+            "bgcolor": "red",
         },
     }
-
+    # fmt: on
 
     # -- Email Notification Settings
 
     # Fail silently if the email server does not exist or respond
     email_fail_silently = False
 
     # From email address used when sending notifications
@@ -58,16 +59,16 @@
     # Email subject and text body templates. This needs to be a standard
     # Python string. You may use 'new style' format variables here.
     #
     # {type}      Event type, such as "Info" or "Warning".
     # {date}      The date and time the event was triggered.
     # {message}   The message sent with the event.
     # {initiator} The initiator string (optional)
-    email_subject_template = _('Event Log: {type}')
-    email_template = _('The Event was {type} on {date}\n\n{message}\n\n-- {initiator}')
+    email_subject_template = _("Event Log: {type}")
+    email_template = _("The Event was {type} on {date}\n\n{message}\n\n-- {initiator}")
 
     def get_event_types(self):
         """
         All code calls this method and not `self.event_types`, so you can
         programmatically create event types, if required..
         """
         return self.event_types
```

### Comparing `django-eventlog-1.1/eventlog/admin.py` & `django-eventlog-1.2/eventlog/admin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 from django.apps import apps
 from django.contrib import admin
 from django.template.defaultfilters import timesince_filter
-from django.utils.safestring import mark_safe
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from eventlog.models import Event
 
-config = apps.get_app_config('eventlog')
+config = apps.get_app_config("eventlog")
 
 
 class EventAdmin(admin.ModelAdmin):
     """
     Event Admin.
     """
-    list_display = ('relative_timestamp', 'group_label', 'type_display',
-                    'message', 'initiator')
-    search_fields = ('group', 'message', 'initiator')
-    list_filter = ('type', 'timestamp')
-    change_list_template = 'admin/eventlog/event/change_list.html'
-    change_form_template = 'admin/eventlog/event/change_form.html'
+
+    list_display = (
+        "relative_timestamp",
+        "group_label",
+        "type_display",
+        "message",
+        "initiator",
+    )
+    search_fields = ("group", "message", "initiator")
+    list_filter = ("type", "timestamp")
+    change_list_template = "admin/eventlog/event/change_list.html"
+    change_form_template = "admin/eventlog/event/change_form.html"
 
     def __init__(self, *args, **kwargs):
-        super(EventAdmin, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.event_types = config.get_event_types()
 
+    @admin.display(description="Time")
     def relative_timestamp(self, obj):
-        return _('{time} ago').format(time=timesince_filter(obj.timestamp))
-    relative_timestamp.short_description = 'Time'
+        return _("{time} ago").format(time=timesince_filter(obj.timestamp))
 
+    @admin.display(description="Type")
     def type_display(self, obj):
         return obj.type_label
-    type_display.short_description = 'Type'
 
     def get_readonly_fields(self, request, obj=None):
         """All fields are readonly. It's pure logging."""
         return [i.name for i in obj._meta.get_fields()]
 
     def has_add_permission(self, request):
         """Nobody can add events manually. Only programatically."""
         return False
 
+
 admin.site.register(Event, EventAdmin)
```

### Comparing `django-eventlog-1.1/eventlog/templates/admin/eventlog/event/change_list.html` & `django-eventlog-1.2/eventlog/templates/admin/eventlog/event/change_list.html`

 * *Files identical despite different names*

### Comparing `django-eventlog-1.1/eventlog/templates/admin/eventlog/event/change_form.html` & `django-eventlog-1.2/eventlog/templates/admin/eventlog/event/change_form.html`

 * *Files identical despite different names*

