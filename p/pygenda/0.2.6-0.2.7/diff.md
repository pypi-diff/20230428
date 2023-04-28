# Comparing `tmp/pygenda-0.2.6.tar.gz` & `tmp/pygenda-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygenda-0.2.6.tar", last modified: Thu Mar 16 08:06:44 2023, max compression
+gzip compressed data, was "pygenda-0.2.7.tar", last modified: Fri Apr 28 10:30:07 2023, max compression
```

## Comparing `pygenda-0.2.6.tar` & `pygenda-0.2.7.tar`

### file list

```diff
@@ -1,79 +1,83 @@
-drwx------   0 matt      (1000) users      (100)        0 2023-03-16 08:06:44.305012 pygenda-0.2.6/
--rw-------   0 matt      (1000) users      (100)    35149 2022-01-30 22:37:16.000000 pygenda-0.2.6/COPYING
--rw-------   0 matt      (1000) users      (100)     1019 2023-03-16 08:06:44.305012 pygenda-0.2.6/PKG-INFO
--rw-------   0 matt      (1000) users      (100)     5881 2022-11-19 09:35:07.000000 pygenda-0.2.6/README.md
-drwx------   0 matt      (1000) users      (100)        0 2023-03-16 08:06:44.293012 pygenda-0.2.6/csrc/
--rw-------   0 matt      (1000) users      (100)      773 2022-01-30 22:37:16.000000 pygenda-0.2.6/csrc/Makefile
--rw-------   0 matt      (1000) users      (100)     3027 2022-05-10 09:35:33.000000 pygenda-0.2.6/csrc/pygenda_clipboard.c
-drwx------   0 matt      (1000) users      (100)        0 2023-03-16 08:06:44.294012 pygenda-0.2.6/docs/
--rw-------   0 matt      (1000) users      (100)     3429 2023-03-15 23:28:59.000000 pygenda-0.2.6/docs/CalDAV.md
--rw-------   0 matt      (1000) users      (100)     3559 2023-03-15 16:57:28.000000 pygenda-0.2.6/docs/Development.md
--rw-------   0 matt      (1000) users      (100)     2475 2023-03-15 16:57:28.000000 pygenda-0.2.6/docs/Usage.md
-drwx------   0 matt      (1000) users      (100)        0 2023-03-16 08:06:44.295012 pygenda-0.2.6/docs/config-examples/
--rw-------   0 matt      (1000) users      (100)      497 2022-01-30 22:37:16.000000 pygenda-0.2.6/docs/config-examples/README.md
--rw-------   0 matt      (1000) users      (100)     2532 2022-11-16 18:46:21.000000 pygenda-0.2.6/docs/config-examples/backgrounds.css
--rw-------   0 matt      (1000) users      (100)     6205 2023-03-15 16:57:28.000000 pygenda-0.2.6/docs/config-examples/darkmode.css
--rw-------   0 matt      (1000) users      (100)     4687 2023-03-15 16:57:28.000000 pygenda-0.2.6/docs/config-examples/defaults.ini
--rw-------   0 matt      (1000) users      (100)     2148 2023-03-15 16:57:28.000000 pygenda-0.2.6/docs/config-examples/gemini.css
--rw-------   0 matt      (1000) users      (100)       41 2022-01-30 22:37:16.000000 pygenda-0.2.6/docs/config-examples/gemini.ini
--rw-------   0 matt      (1000) users      (100)      342 2022-04-27 21:43:12.000000 pygenda-0.2.6/docs/config-examples/pygenda.desktop
--rw-------   0 matt      (1000) users      (100)    10166 2023-03-15 23:28:59.000000 pygenda-0.2.6/docs/known_issues.md
-drwx------   0 matt      (1000) users      (100)        0 2023-03-16 08:06:44.299012 pygenda-0.2.6/pygenda/
--rwx------   0 matt      (1000) users      (100)      823 2023-03-15 16:57:28.000000 pygenda-0.2.6/pygenda/__main__.py
-drwx------   0 matt      (1000) users      (100)        0 2023-03-16 08:06:44.302012 pygenda-0.2.6/pygenda/css/
--rw-------   0 matt      (1000) users      (100)      288 2022-01-30 22:37:16.000000 pygenda-0.2.6/pygenda/css/disc+loop+star.svg
--rw-------   0 matt      (1000) users      (100)      215 2022-01-30 22:37:16.000000 pygenda-0.2.6/pygenda/css/disc+loop.svg
--rw-------   0 matt      (1000) users      (100)      208 2022-01-30 22:37:16.000000 pygenda-0.2.6/pygenda/css/disc+star.svg
--rw-------   0 matt      (1000) users      (100)      135 2022-01-30 22:37:16.000000 pygenda-0.2.6/pygenda/css/disc.svg
--rw-------   0 matt      (1000) users      (100)      223 2022-01-30 22:37:16.000000 pygenda-0.2.6/pygenda/css/loop+star.svg
--rw-------   0 matt      (1000) users      (100)      150 2022-01-30 22:37:16.000000 pygenda-0.2.6/pygenda/css/loop.svg
--rw-------   0 matt      (1000) users      (100)    14421 2023-03-15 16:57:28.000000 pygenda-0.2.6/pygenda/css/pygenda.css
--rw-------   0 matt      (1000) users      (100)      150 2022-01-30 22:37:16.000000 pygenda-0.2.6/pygenda/css/star.svg
-drwx------   0 matt      (1000) users      (100)        0 2023-03-16 08:06:44.303012 pygenda-0.2.6/pygenda/glade/
--rw-------   0 matt      (1000) users      (100)    44415 2023-03-15 23:28:59.000000 pygenda-0.2.6/pygenda/glade/dialog_event.glade
--rw-------   0 matt      (1000) users      (100)     5150 2023-03-15 16:57:28.000000 pygenda-0.2.6/pygenda/glade/dialog_find.glade
--rw-------   0 matt      (1000) users      (100)     7963 2023-03-15 16:57:28.000000 pygenda-0.2.6/pygenda/glade/dialog_todo.glade
--rw-------   0 matt      (1000) users      (100)    28251 2023-03-15 16:57:28.000000 pygenda-0.2.6/pygenda/glade/main.glade
--rw-------   0 matt      (1000) users      (100)     3892 2023-03-15 16:57:28.000000 pygenda-0.2.6/pygenda/glade/view_week.glade
--rw-------   0 matt      (1000) users      (100)     5701 2023-03-15 16:57:28.000000 pygenda-0.2.6/pygenda/glade/view_year.glade
-drwx------   0 matt      (1000) users      (100)        0 2023-03-16 08:06:44.292012 pygenda-0.2.6/pygenda/locale/
-drwx------   0 matt      (1000) users      (100)        0 2023-03-16 08:06:44.292012 pygenda-0.2.6/pygenda/locale/en_US/
-drwx------   0 matt      (1000) users      (100)        0 2023-03-16 08:06:44.303012 pygenda-0.2.6/pygenda/locale/en_US/LC_MESSAGES/
--rw-------   0 matt      (1000) users      (100)      433 2023-03-15 23:28:59.000000 pygenda-0.2.6/pygenda/locale/en_US/LC_MESSAGES/pygenda.mo
--rw-------   0 matt      (1000) users      (100)     1289 2023-03-15 23:28:59.000000 pygenda-0.2.6/pygenda/locale/en_US/LC_MESSAGES/pygenda.po
-drwx------   0 matt      (1000) users      (100)        0 2023-03-16 08:06:44.292012 pygenda-0.2.6/pygenda/locale/fr/
-drwx------   0 matt      (1000) users      (100)        0 2023-03-16 08:06:44.303012 pygenda-0.2.6/pygenda/locale/fr/LC_MESSAGES/
--rw-------   0 matt      (1000) users      (100)     8276 2023-03-15 23:28:59.000000 pygenda-0.2.6/pygenda/locale/fr/LC_MESSAGES/pygenda.mo
--rw-------   0 matt      (1000) users      (100)    14177 2023-03-15 23:28:59.000000 pygenda-0.2.6/pygenda/locale/fr/LC_MESSAGES/pygenda.po
--rw-------   0 matt      (1000) users      (100)     1104 2023-03-15 16:57:28.000000 pygenda-0.2.6/pygenda/mypy.ini
--rw-------   0 matt      (1000) users      (100)    58256 2023-03-15 16:57:28.000000 pygenda-0.2.6/pygenda/pygenda_calendar.py
--rw-------   0 matt      (1000) users      (100)     5450 2022-05-10 09:37:11.000000 pygenda-0.2.6/pygenda/pygenda_config.py
--rw-------   0 matt      (1000) users      (100)     9869 2023-03-15 23:28:59.000000 pygenda-0.2.6/pygenda/pygenda_dialog_entryprops.py
--rw-------   0 matt      (1000) users      (100)    62580 2023-03-15 23:28:59.000000 pygenda-0.2.6/pygenda/pygenda_dialog_event.py
--rw-------   0 matt      (1000) users      (100)     3538 2023-03-15 16:57:28.000000 pygenda-0.2.6/pygenda/pygenda_dialog_find.py
--rw-------   0 matt      (1000) users      (100)     5377 2023-03-15 16:57:28.000000 pygenda-0.2.6/pygenda/pygenda_dialog_todo.py
--rw-------   0 matt      (1000) users      (100)     4146 2023-03-15 16:57:28.000000 pygenda-0.2.6/pygenda/pygenda_entryinfo.py
--rw-------   0 matt      (1000) users      (100)    39811 2023-03-15 23:28:59.000000 pygenda-0.2.6/pygenda/pygenda_gui.py
--rw-------   0 matt      (1000) users      (100)    10419 2023-03-15 16:57:28.000000 pygenda-0.2.6/pygenda/pygenda_util.py
--rw-------   0 matt      (1000) users      (100)      300 2023-03-15 23:29:29.000000 pygenda-0.2.6/pygenda/pygenda_version.py
--rw-------   0 matt      (1000) users      (100)    14282 2023-03-15 16:57:28.000000 pygenda-0.2.6/pygenda/pygenda_view.py
--rw-------   0 matt      (1000) users      (100)    21017 2023-03-15 16:57:28.000000 pygenda-0.2.6/pygenda/pygenda_view_todo.py
--rw-------   0 matt      (1000) users      (100)    19429 2023-03-15 16:57:28.000000 pygenda-0.2.6/pygenda/pygenda_view_week.py
--rw-------   0 matt      (1000) users      (100)    27129 2023-03-15 16:57:28.000000 pygenda-0.2.6/pygenda/pygenda_view_year.py
--rw-------   0 matt      (1000) users      (100)    21975 2022-10-05 17:00:54.000000 pygenda-0.2.6/pygenda/pygenda_widgets.py
-drwx------   0 matt      (1000) users      (100)        0 2023-03-16 08:06:44.300012 pygenda-0.2.6/pygenda.egg-info/
--rw-------   0 matt      (1000) users      (100)     1019 2023-03-16 08:06:44.000000 pygenda-0.2.6/pygenda.egg-info/PKG-INFO
--rw-------   0 matt      (1000) users      (100)     2125 2023-03-16 08:06:44.000000 pygenda-0.2.6/pygenda.egg-info/SOURCES.txt
--rw-------   0 matt      (1000) users      (100)        1 2023-03-16 08:06:44.000000 pygenda-0.2.6/pygenda.egg-info/dependency_links.txt
--rw-------   0 matt      (1000) users      (100)       44 2023-03-16 08:06:44.000000 pygenda-0.2.6/pygenda.egg-info/requires.txt
--rw-------   0 matt      (1000) users      (100)        8 2023-03-16 08:06:44.000000 pygenda-0.2.6/pygenda.egg-info/top_level.txt
--rw-------   0 matt      (1000) users      (100)       38 2023-03-16 08:06:44.306012 pygenda-0.2.6/setup.cfg
--rwx------   0 matt      (1000) users      (100)     3749 2023-03-15 16:57:28.000000 pygenda-0.2.6/setup.py
-drwx------   0 matt      (1000) users      (100)        0 2023-03-16 08:06:44.304012 pygenda-0.2.6/test/
--rwx------   0 matt      (1000) users      (100)    15117 2023-03-15 16:57:28.000000 pygenda-0.2.6/test/maketest_example.py
--rwx------   0 matt      (1000) users      (100)     1274 2022-11-11 22:25:45.000000 pygenda-0.2.6/test/maketest_large.py
--rw-------   0 matt      (1000) users      (100)       83 2022-01-30 22:37:16.000000 pygenda-0.2.6/test/test00_empty.ics
--rw-------   0 matt      (1000) users      (100)     1500 2023-03-15 16:57:28.000000 pygenda-0.2.6/test/test01_small.ics
--rw-------   0 matt      (1000) users      (100)    12965 2023-01-29 22:35:48.000000 pygenda-0.2.6/test/test02_repeats.ics
--rw-------   0 matt      (1000) users      (100)     1241 2022-05-28 15:39:16.000000 pygenda-0.2.6/test/test03_errors.ics
--rwx------   0 matt      (1000) users      (100)   107588 2023-03-15 10:31:37.000000 pygenda-0.2.6/test/test_repeats.py
+drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.421058 pygenda-0.2.7/
+-rw-------   0 matt      (1000) users      (100)    35149 2022-01-30 22:37:16.000000 pygenda-0.2.7/COPYING
+-rw-------   0 matt      (1000) users      (100)     1015 2023-04-28 10:30:07.420058 pygenda-0.2.7/PKG-INFO
+-rw-------   0 matt      (1000) users      (100)     6283 2023-04-28 10:14:02.000000 pygenda-0.2.7/README.md
+drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.407058 pygenda-0.2.7/csrc/
+-rw-------   0 matt      (1000) users      (100)      773 2022-01-30 22:37:16.000000 pygenda-0.2.7/csrc/Makefile
+-rw-------   0 matt      (1000) users      (100)     3027 2023-03-31 11:03:09.000000 pygenda-0.2.7/csrc/pygenda_clipboard.c
+drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.408058 pygenda-0.2.7/docs/
+-rw-------   0 matt      (1000) users      (100)     3429 2023-03-31 11:03:09.000000 pygenda-0.2.7/docs/CalDAV.md
+-rw-------   0 matt      (1000) users      (100)     3559 2023-04-23 17:43:29.000000 pygenda-0.2.7/docs/Development.md
+-rw-------   0 matt      (1000) users      (100)     3066 2023-04-28 10:14:02.000000 pygenda-0.2.7/docs/Usage.md
+drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.409058 pygenda-0.2.7/docs/config-examples/
+-rw-------   0 matt      (1000) users      (100)      497 2022-01-30 22:37:16.000000 pygenda-0.2.7/docs/config-examples/README.md
+-rw-------   0 matt      (1000) users      (100)     2532 2023-03-31 11:03:09.000000 pygenda-0.2.7/docs/config-examples/backgrounds.css
+-rw-------   0 matt      (1000) users      (100)     6205 2023-03-31 11:03:09.000000 pygenda-0.2.7/docs/config-examples/darkmode.css
+-rw-------   0 matt      (1000) users      (100)     6023 2023-04-28 10:14:02.000000 pygenda-0.2.7/docs/config-examples/defaults.ini
+-rw-------   0 matt      (1000) users      (100)     3459 2023-04-28 10:14:02.000000 pygenda-0.2.7/docs/config-examples/gemini.css
+-rw-------   0 matt      (1000) users      (100)       41 2022-01-30 22:37:16.000000 pygenda-0.2.7/docs/config-examples/gemini.ini
+-rw-------   0 matt      (1000) users      (100)      342 2023-03-31 11:03:09.000000 pygenda-0.2.7/docs/config-examples/pygenda.desktop
+-rw-------   0 matt      (1000) users      (100)    10433 2023-04-28 10:14:02.000000 pygenda-0.2.7/docs/known_issues.md
+drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.410058 pygenda-0.2.7/docs/screenshots/
+-rw-------   0 matt      (1000) users      (100)    17045 2023-04-16 11:30:10.000000 pygenda-0.2.7/docs/screenshots/todo_view.png
+-rw-------   0 matt      (1000) users      (100)    16198 2023-04-16 11:30:10.000000 pygenda-0.2.7/docs/screenshots/week_view.png
+-rw-------   0 matt      (1000) users      (100)    23745 2023-04-16 11:30:10.000000 pygenda-0.2.7/docs/screenshots/year_view.png
+drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.413058 pygenda-0.2.7/pygenda/
+-rwx------   0 matt      (1000) users      (100)      823 2023-03-31 11:03:09.000000 pygenda-0.2.7/pygenda/__main__.py
+drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.415058 pygenda-0.2.7/pygenda/css/
+-rw-------   0 matt      (1000) users      (100)      288 2022-01-30 22:37:16.000000 pygenda-0.2.7/pygenda/css/disc+loop+star.svg
+-rw-------   0 matt      (1000) users      (100)      215 2022-01-30 22:37:16.000000 pygenda-0.2.7/pygenda/css/disc+loop.svg
+-rw-------   0 matt      (1000) users      (100)      208 2022-01-30 22:37:16.000000 pygenda-0.2.7/pygenda/css/disc+star.svg
+-rw-------   0 matt      (1000) users      (100)      135 2022-01-30 22:37:16.000000 pygenda-0.2.7/pygenda/css/disc.svg
+-rw-------   0 matt      (1000) users      (100)      223 2022-01-30 22:37:16.000000 pygenda-0.2.7/pygenda/css/loop+star.svg
+-rw-------   0 matt      (1000) users      (100)      150 2022-01-30 22:37:16.000000 pygenda-0.2.7/pygenda/css/loop.svg
+-rw-------   0 matt      (1000) users      (100)    15656 2023-04-28 10:14:02.000000 pygenda-0.2.7/pygenda/css/pygenda.css
+-rw-------   0 matt      (1000) users      (100)      150 2022-01-30 22:37:16.000000 pygenda-0.2.7/pygenda/css/star.svg
+drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.417058 pygenda-0.2.7/pygenda/glade/
+-rw-------   0 matt      (1000) users      (100)    44996 2023-04-09 10:20:50.000000 pygenda-0.2.7/pygenda/glade/dialog_event.glade
+-rw-------   0 matt      (1000) users      (100)     5150 2023-03-31 11:03:09.000000 pygenda-0.2.7/pygenda/glade/dialog_find.glade
+-rw-------   0 matt      (1000) users      (100)     7963 2023-03-31 11:03:09.000000 pygenda-0.2.7/pygenda/glade/dialog_todo.glade
+-rw-------   0 matt      (1000) users      (100)    27159 2023-04-23 17:32:42.000000 pygenda-0.2.7/pygenda/glade/main.glade
+-rw-------   0 matt      (1000) users      (100)     3892 2023-03-31 11:03:09.000000 pygenda-0.2.7/pygenda/glade/view_week.glade
+-rw-------   0 matt      (1000) users      (100)     5931 2023-04-09 10:20:50.000000 pygenda-0.2.7/pygenda/glade/view_year.glade
+drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.405058 pygenda-0.2.7/pygenda/locale/
+drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.405058 pygenda-0.2.7/pygenda/locale/en_US/
+drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.417058 pygenda-0.2.7/pygenda/locale/en_US/LC_MESSAGES/
+-rw-------   0 matt      (1000) users      (100)      433 2023-04-28 10:14:02.000000 pygenda-0.2.7/pygenda/locale/en_US/LC_MESSAGES/pygenda.mo
+-rw-------   0 matt      (1000) users      (100)     1290 2023-04-28 10:14:02.000000 pygenda-0.2.7/pygenda/locale/en_US/LC_MESSAGES/pygenda.po
+drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.405058 pygenda-0.2.7/pygenda/locale/fr/
+drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.417058 pygenda-0.2.7/pygenda/locale/fr/LC_MESSAGES/
+-rw-------   0 matt      (1000) users      (100)     8312 2023-04-28 10:14:02.000000 pygenda-0.2.7/pygenda/locale/fr/LC_MESSAGES/pygenda.mo
+-rw-------   0 matt      (1000) users      (100)    14232 2023-04-28 10:14:02.000000 pygenda-0.2.7/pygenda/locale/fr/LC_MESSAGES/pygenda.po
+-rw-------   0 matt      (1000) users      (100)     1104 2023-04-25 20:33:58.000000 pygenda-0.2.7/pygenda/mypy.ini
+-rw-------   0 matt      (1000) users      (100)    58256 2023-04-23 17:43:29.000000 pygenda-0.2.7/pygenda/pygenda_calendar.py
+-rw-------   0 matt      (1000) users      (100)     5450 2023-03-31 11:03:09.000000 pygenda-0.2.7/pygenda/pygenda_config.py
+-rw-------   0 matt      (1000) users      (100)     9869 2023-03-31 11:03:09.000000 pygenda-0.2.7/pygenda/pygenda_dialog_entryprops.py
+-rw-------   0 matt      (1000) users      (100)    62921 2023-04-09 10:20:50.000000 pygenda-0.2.7/pygenda/pygenda_dialog_event.py
+-rw-------   0 matt      (1000) users      (100)     3538 2023-03-31 11:03:09.000000 pygenda-0.2.7/pygenda/pygenda_dialog_find.py
+-rw-------   0 matt      (1000) users      (100)     5377 2023-03-31 11:03:09.000000 pygenda-0.2.7/pygenda/pygenda_dialog_todo.py
+-rw-------   0 matt      (1000) users      (100)     4146 2023-03-31 11:03:09.000000 pygenda-0.2.7/pygenda/pygenda_entryinfo.py
+-rw-------   0 matt      (1000) users      (100)    42037 2023-04-28 10:14:02.000000 pygenda-0.2.7/pygenda/pygenda_gui.py
+-rw-------   0 matt      (1000) users      (100)    10419 2023-03-31 11:03:09.000000 pygenda-0.2.7/pygenda/pygenda_util.py
+-rw-------   0 matt      (1000) users      (100)      300 2023-04-28 10:14:24.000000 pygenda-0.2.7/pygenda/pygenda_version.py
+-rw-------   0 matt      (1000) users      (100)    15418 2023-04-09 10:20:50.000000 pygenda-0.2.7/pygenda/pygenda_view.py
+-rw-------   0 matt      (1000) users      (100)    26915 2023-04-28 10:14:02.000000 pygenda-0.2.7/pygenda/pygenda_view_todo.py
+-rw-------   0 matt      (1000) users      (100)    21063 2023-04-23 17:43:29.000000 pygenda-0.2.7/pygenda/pygenda_view_week.py
+-rw-------   0 matt      (1000) users      (100)    27377 2023-04-09 10:20:50.000000 pygenda-0.2.7/pygenda/pygenda_view_year.py
+-rw-------   0 matt      (1000) users      (100)    22142 2023-04-09 10:20:50.000000 pygenda-0.2.7/pygenda/pygenda_widgets.py
+drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.413058 pygenda-0.2.7/pygenda.egg-info/
+-rw-------   0 matt      (1000) users      (100)     1015 2023-04-28 10:30:07.000000 pygenda-0.2.7/pygenda.egg-info/PKG-INFO
+-rw-------   0 matt      (1000) users      (100)     2218 2023-04-28 10:30:07.000000 pygenda-0.2.7/pygenda.egg-info/SOURCES.txt
+-rw-------   0 matt      (1000) users      (100)        1 2023-04-28 10:30:07.000000 pygenda-0.2.7/pygenda.egg-info/dependency_links.txt
+-rw-------   0 matt      (1000) users      (100)       44 2023-04-28 10:30:07.000000 pygenda-0.2.7/pygenda.egg-info/requires.txt
+-rw-------   0 matt      (1000) users      (100)        8 2023-04-28 10:30:07.000000 pygenda-0.2.7/pygenda.egg-info/top_level.txt
+-rw-------   0 matt      (1000) users      (100)       38 2023-04-28 10:30:07.421058 pygenda-0.2.7/setup.cfg
+-rwx------   0 matt      (1000) users      (100)     3745 2023-04-28 10:14:02.000000 pygenda-0.2.7/setup.py
+drwx------   0 matt      (1000) users      (100)        0 2023-04-28 10:30:07.418058 pygenda-0.2.7/test/
+-rwx------   0 matt      (1000) users      (100)    15117 2023-03-31 11:03:09.000000 pygenda-0.2.7/test/maketest_example.py
+-rwx------   0 matt      (1000) users      (100)     1274 2023-03-31 11:03:09.000000 pygenda-0.2.7/test/maketest_large.py
+-rw-------   0 matt      (1000) users      (100)       83 2022-01-30 22:37:16.000000 pygenda-0.2.7/test/test00_empty.ics
+-rw-------   0 matt      (1000) users      (100)     1500 2023-03-31 11:03:09.000000 pygenda-0.2.7/test/test01_small.ics
+-rw-------   0 matt      (1000) users      (100)    12965 2023-03-31 11:03:09.000000 pygenda-0.2.7/test/test02_repeats.ics
+-rw-------   0 matt      (1000) users      (100)     1241 2023-03-31 11:03:09.000000 pygenda-0.2.7/test/test03_errors.ics
+-rwx------   0 matt      (1000) users      (100)   107588 2023-04-23 17:43:29.000000 pygenda-0.2.7/test/test_repeats.py
```

### Comparing `pygenda-0.2.6/COPYING` & `pygenda-0.2.7/COPYING`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/PKG-INFO` & `pygenda-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pygenda
-Version: 0.2.6
+Version: 0.2.7
 Summary: An agenda application inspired by Agenda programs on Psion PDAs.
 Home-page: https://github.com/semiprime/pygenda
 Author: Matthew Lewis
 Author-email: pygenda@semiprime.com
 License: GPLv3 only
 Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Handhelds/PDA's
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Office/Business :: Scheduling
 Requires-Python: >=3.5
```

### Comparing `pygenda-0.2.6/README.md` & `pygenda-0.2.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,46 @@
 Pygenda
 =======
 Pygenda is a calendar/agenda application written in Python3/GTK3 and
 designed for "PDA" devices such as Planet Computers' Gemini. The user
 interface is inspired by the Agenda programs on the Psion Series 3 and
 Series 5 range of PDAs.
 
-**WARNING: This is in-development code, released as a preview for
-developers. The software is provided as-is, with no guarantees. You
-should back up any data or files used by Pygenda (e.g. iCal files
-or data stored on calendar servers).**
+**WARNING: This is in-development code, released for testing/feedback and
+as a preview for developers. The software is provided as-is, with no
+guarantees. You should back up any files or data used by Pygenda (e.g. iCal
+files or data stored on calendar servers).**
 
 There are currently **lots of missing/incomplete features** as well as
 **bugs**. For a list of known issues, see: [known_issues.md](docs/known_issues.md).
-If you find any new bugs (or have any feature requests), please send
-them to: pygenda@semiprime.com.
+If you find any new bugs, please send them to: pygenda@semiprime.com.
 
 *However*, it currently has Week, Year and Todo Views that are functional
 enough that the author is now using Pygenda as his main agenda, so
 maybe other people will also find it useful. Feedback is welcome at
-pygenda@semiprime.com - suggestions, questions about how to get something
+pygenda@semiprime.com – suggestions, questions about how to get something
 working, or just to say that you tried it out.
 
-Video (from March 2021): https://www.youtube.com/watch?v=QjHcgeRudMo
+Video and screenshots
+---------------------
+Video: https://www.youtube.com/watch?v=uvQqFmlZ6nM (v0.2.7, April 2023)
+
+Screenshots from a PC running Xfce and rescaled – your results may vary.
+
+Week View:
+
+![Screenshot – Week View](docs/screenshots/week_view.png?raw=true)
+
+Year View:
+
+![Screenshot – Year View](docs/screenshots/year_view.png?raw=true)
+
+Todo View:
+
+![Screenshot – Todo View](docs/screenshots/todo_view.png?raw=true)
 
 Source code
 -----------
 Source is available at: https://github.com/semiprime/pygenda
 
 License (GPL3)
 --------------
@@ -41,27 +56,28 @@
 You should have received a copy of the GNU General Public License along
 with Pygenda (see COPYING file). If not, see <https://www.gnu.org/licenses/>.
 
 Run/install
 -----------
 (See note about dependencies below.)
 
-To run without installing, cd to the root pygenda directory, and do:
+To run without installing, cd to the root directory of the project (containing
+this readme), and run:
 
 	python3 -m pygenda
 
 Better/recommended: install the Python module with (for example)...
 
 	./setup.py install --user
 
 (You can uninstall the module with `pip3 uninstall pygenda`.)
 
 NOTE: Gemian (Debian port for Gemini PDA) doesn't install the Python module
 dependencies. The reason for this appears to be old pip/setuptools on Gemian.
-I recommend installing these dependencies manually - see "Dependencies" below.
+I recommend installing these dependencies manually – see "Dependencies" below.
 
 Then you can now run Pygenda from anywhere with:
 
 	python3 -m pygenda
 
 There are a few command-line options, which you can view using:
 
@@ -129,15 +145,15 @@
 LXQt panel, edit the `~/.config/lxqt/panel.conf` file and add a line
 in the [quicklaunch] section (& restart LXQt).
 
 Usage
 -----
 See: [Usage.md](docs/Usage.md)
 
-Calendar data storage - a CalDAV server is recommended
+Calendar data storage – a CalDAV server is recommended
 ------------------------------------------------------
 Calendar data can be stored as an ICS file, or via a CalDAV server.
 The ICS file is the default, because it works without configuration,
 but a CalDAV server is recommended for real use.
 
 For CalDAV configuration, see: [CalDAV.md](docs/CalDAV.md)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pygenda-0.2.6/csrc/Makefile` & `pygenda-0.2.7/csrc/Makefile`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/csrc/pygenda_clipboard.c` & `pygenda-0.2.7/csrc/pygenda_clipboard.c`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/docs/CalDAV.md` & `pygenda-0.2.7/docs/CalDAV.md`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/docs/Development.md` & `pygenda-0.2.7/docs/Development.md`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/docs/Usage.md` & `pygenda-0.2.7/docs/Usage.md`

 * *Files 14% similar despite different names*

```diff
@@ -19,14 +19,25 @@
   increased with + or >, and decreased with - or <.
 
 * The Escape key toggles between the most recent two views.
 
 * In Week and Year views, the space key toggles between Today and
   wherever the cursor was last.
 
+* Plus and minus keys will zoom in/out (no need for ctrl). The motivation
+  for this is that on handheld devices, +/- might be require more than one
+  key on their own, so adding another key would make zooming awkward.
+  If you wish, you can disable this by setting the global/plus_minus_zoom
+  config setting to False (ctrl+plus/minus will work in either case).
+
+* The Zoom soft-button zooms in; shift+Zoom or ctrl+Zoom zooms out.
+
+* You can set the number of zoom levels and the default with the zoom_levels
+  and default_zoom config options. You can set the font sizes with custom CSS.
+
 * If you want the Tab key to move within elements in date/time/duration
   widgets then set the global/tab_elts_datetime config option to True.
 
 * Pressing y/m/d keys in date widget moves the cursor to year/month/day
   fields respectively. Similarly, pressing h/m keys in time or duration
   widget moves to hour/minute fields. (These shortcut keys are localised,
   for example in French they are a/m/j/h/m.)
@@ -36,15 +47,15 @@
   purple circle for other repeating events, and a yellow disc for other
   events.
 
 * Hint: To convert To-dos into Events, or vice-versa, cut & paste them.
 
 * Setting alarms is currently under development and testing is welcome.
   (Note: sounding/displaying/sending alarms will be the job of a
-  different program - an alarm server. Pygenda does not, and will not,
+  different program - an alarm handler. Pygenda does not, and will not,
   activate the alarms. There is a warning in the UI about this because
   it's important that you understand that you need to do some setup or
   alarms will not be activated. You can get rid of the warning by
   changing the appropriate config setting to False.)
   Keys: +/>/-/< - move alarm time of the selected alarm forward/back;
   N - new alarm; Delete - delete selected alarm; A/D/E - change action
   of selected alarm to Audio/Display/Email. For email alarms, you will
```

### Comparing `pygenda-0.2.6/docs/config-examples/backgrounds.css` & `pygenda-0.2.7/docs/config-examples/backgrounds.css`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/docs/config-examples/darkmode.css` & `pygenda-0.2.7/docs/config-examples/darkmode.css`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/docs/config-examples/defaults.ini` & `pygenda-0.2.7/docs/config-examples/defaults.ini`

 * *Files 18% similar despite different names*

```diff
@@ -57,14 +57,19 @@
 #       Default: 0 (Monday)
 
 # tab_elts_datetime = Boolean
 #       This indicates if pressing tab moves between elements in
 #       date/time entry widgets.
 #       Default: False
 
+# plus_minus_zoom = Boolean
+#       If True, pressing plus or minus keys (without ctrl) will zoom
+#       (ctrl with plus/minus keys will always zoom).
+#       Default: True
+
 
 [startup]
 # maximize = Boolean
 #       Default: False
 
 # fullscreen = Boolean
 #       Default: False
@@ -90,37 +95,62 @@
 #       time *before* event that alarm activates.
 #       Default: 15m
 
 # default_alarm_emailaddr = string
 #       When user creates an alarm with Action 'Email', use this value
 #       as the email address. If this is None, then (for the moment)
 #       new email alarms can't be set.
-#		Default: None
+#       Default: None
 
 
 [week_view]
 # pageleft_datepos = 'left' or 'right'
 #       Default: 'left'
 
 # pageright_datepos = 'left' or 'right'
 #       Default: 'right'
 
+# show_ongoing_event = 'every_day' or 'first_day'
+#       Default: 'first_day'
+#       Whether ongoing events should be shown only on their start day
+#       or on every day that they span.
+#       Note: WORK IN PROGRESS! Currently only works within starting week.
+
 # show_event_location = 'always' or 'never'
 #       Default: 'always'
 #       The plan is to have further options in the future, e.g.
 #       'first-day' => only show on the first day of multi-day event,
 #       'start-of-week' => on first day and also on first day of week.
 
+# zoom_levels = integer>0
+#       Default: 5
+#       The number of zoom levels in Week View. The font sizes for
+#       each zoom level are set using CSS - see pygenda/css/pygenda.css
+#       or gemini.css in this directory for examples.
+
+# default_zoom = integer>=0 and <zoom_levels
+#       Default: 1
+#       The Week View zoom level when Pygenda is started.
+
 
 [year_view]
 # show_event_location = 'always' or 'never'
 #       Default: 'always'
 #       The plan is to have further options in the future, e.g.
 #       'first-day' => only show on the first day of multi-day event.
 
+# zoom_levels = integer>0
+#       Default: 5
+#       The number of zoom levels in Year View.
+#       (See zoom_levels for Week View above.)
+
+# default_zoom = integer>=0 and <zoom_levels
+#       Default: 2
+#       The Year View zoom level when Pygenda is started.
+
 
 [todo_view]
 # list0_title = string
 #       Default: 'To-do' (or localized equivalent)
 #       The displayed name of the to-do list.
 
 # listN_title = string (where N is an integer>0)
@@ -133,7 +163,16 @@
 #       Default: undefined for N>=0
 #       These are used to filter to-do items according to categories.
 #       Typically a filter will be the name of a possible category.
 #       Undefined (the default) means that all to-do items are shown
 #       (so the default behaviour is for a to-do list to show all items).
 #       A special value 'UNCATEGORIZED' will show only to-do items with
 #       no categories.
+
+# zoom_levels = integer>0
+#       Default: 5
+#       The number of zoom levels in Todo View.
+#       (See zoom_levels for Week View above.)
+
+# default_zoom = integer>=0 and <zoom_levels
+#       Default: 2
+#       The Todo View zoom level when Pygenda is started.
```

### Comparing `pygenda-0.2.6/docs/known_issues.md` & `pygenda-0.2.7/docs/known_issues.md`

 * *Files 5% similar despite different names*

```diff
@@ -39,18 +39,17 @@
   that are not part of the repeat run, and they are saved without
   problem, and not highlighted in UI as problematic in any way;
   dates can be added that are not visible because box doesn't scroll
   to newly added date; events can be made invisible (thus uneditable)
   by making all occurrences exceptions; keyboard navigation in menu
   is not intuitive.
 
-* Multi-day events (i.e. that span multiple days) only displayed on
-  first day. (Need to set a config, e.g. "next_day_crossover" for week
-  view, year view.  If time goes beyond that, then also show in next
-  day.)
+* Multi-day events (i.e. ones that span multiple days) only displayed
+  on first day. (In progress - started on Week View.) (Future: config
+  option "next_day_crossover" to determine if an even crosses over.)
 
 * Cutting repeating events is not implemented. (Not sure how to do UI -
   probably need to bring up a dialog "Cut just this occurrence, or all
   repeats?". That then raises question about behaviour when copying
   repeating events, where currently just one occurrence is copied. See
   also deleting repeated events - currently all repeats are deleted.)
 
@@ -67,30 +66,27 @@
 
 * Only one calendar source can be used at a time. (Maybe allow multiple
   CalDAV calendars, each with own style element, so can be coloured
   differently by CSS. No support for multiple .ics files?)
 
 Medium
 ------
-* No "Zoom" function (is this even needed with a decent modern display?)
+* How to handle setting the status of a repeating event? (E.g., a
+  reasonable use-case would be to cancel just one occurrence of a
+  repeating event. How is this done with ical?)
 
 * Need InfoPrints (a.k.a. toast notifications) for some situations
 
-* Todo View navigation needs refining: left/right can make cursor jump
-  up and down
-
 * Todo items cannot be shown in Week or Year views
 
 * When deleting a repeated event, all are deleted. Should offer option
   of deleting this one (better, also offer delete all from, all before...)
 
 * No goto next/previous entry (for those without endless appointments)
 
-* No file manipulation: open, save-as, new file (what's the use case?)
-
 * No time-zone support (should at least be part of time widget)
   (Options: "Travels with me" (default), zone xxx (list local first))
 
 * No GUI for configuration settings/preferences
 
 * Only French & English translations are provided (and the French needs
   checking by a native speaker).
@@ -172,14 +168,18 @@
 
 Minor
 -----
 (Note: minor bugs can still be irritating!)
 
 * After creating/editing a repeating event, cursor not always on that event
 
+* Todo View navigation refinements: left/right can sometimes make the cursor
+  move to an unexpected entry (need to find a better algorithm); if there
+  is a border/margin/padding, up/down navigation not obviously at start/end.
+
 * Would be nice to be able to edit dates with a calendar interface
   (Like pressing tab in S5)
 
 * Week view: no touchscreen way to go forward/back a week (use swipe??)
 
 * Ctrl+Left-Shift+X/C/V/N don't work on Gemini (UI eats keypress?)
   Workaround: Use Right-Shift.
@@ -211,14 +211,17 @@
 * If the first event edited after starting Pygenda has multiple exception
   dates, then it makes room for these in the Event dialog Repeats tab.
   This means that the Event dialog is made wide, and stays that way
   until Pygenda is restarted.
 
 * Year View: Pixel missing in grid lines at top-left corner
 
+* If Todo View is initial view, the vertical separator is not shown until
+  there is a redraw.
+
 * On Gemini, shows "no access" icons in instead of "minus" icons (e.g. in
   spin buttons of Event dialog) - Gemian bug?
 
 * Year view is slow to redraw on Gemini, so get black rectangles when
   e.g. closing dialogs.
 
 * Startup spinner is a bit glitchy (visible for large calendars).
```

### Comparing `pygenda-0.2.6/pygenda/__main__.py` & `pygenda-0.2.7/pygenda/__main__.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/pygenda/css/pygenda.css` & `pygenda-0.2.7/pygenda/css/pygenda.css`

 * *Files 8% similar despite different names*

```diff
@@ -53,19 +53,35 @@
 
 #weekview_labelmonth {
 	font-family:'DejaVu Sans Condensed';
 	font-size:12pt;
 	font-weight:bold;
 }
 
+.zoom3 #weekview_labelmonth {
+	font-size:13pt;
+}
+
+.zoom4 #weekview_labelmonth {
+	font-size:14pt;
+}
+
 #weekview_labelweek {
 	font-family:'DejaVu Sans';
 	font-size:9pt;
 }
 
+.zoom3 #weekview_labelweek {
+	font-size:9.5pt;
+}
+
+.zoom4 #weekview_labelweek {
+	font-size:10pt;
+}
+
 #weekview_fold {
 	min-width:12px;
 	background-color:transparent;
 	background-image:linear-gradient(90deg, rgba(255,255,255,0) 0%, rgba(136,136,136,0.8) 35%, rgba(0,0,0,1) 50%, rgba(136,136,136,0.8) 65%, rgba(255,255,255,0) 100%);
 }
 
 .weekview_day {
@@ -95,30 +111,49 @@
 	color:#555;
 }
 
 .weekview_daytext {
 	padding:4px;
 	color:black;
 	font-family:'DejaVu Sans';
-	font-size:9pt;
 	font-weight:normal;
 }
 
+.zoom0 .weekview_daytext {
+	font-size:8pt;
+}
+
+.zoom1 .weekview_daytext {
+	font-size:9pt;
+}
+
+.zoom2 .weekview_daytext {
+	font-size:10pt;
+}
+
+.zoom3 .weekview_daytext {
+	font-size:11pt;
+}
+
+.zoom4 .weekview_daytext {
+	font-size:12pt;
+}
+
 .weekview_marker {
 	color:black;
 	padding-left:1.5px;
 	padding-right:1.5px;
 	margin-right:0.2em;
 	min-width:1ex;
 }
 
 .weekview_cursor {
 	color:white;
 	background-color:black;
-	border-radius:4px;
+	border-radius:0.3em;
 }
 
 
 /* Year View */
 
 #view_year {
 	color:black;
@@ -184,39 +219,57 @@
 
 .yearview_pastday.yearview_day_sat, .yearview_pastday.yearview_day_sun {
 	background-color:rgba(160,160,160,0.5);
 }
 
 #yearview_labeldate {
 	font-family:'DejaVu Sans Condensed';
-	font-size:11pt;
 	font-weight:bold;
 	padding-right:0.8ex;
 }
 
 #yearview_datecontent {
-	font-size:11pt;
 	font-family:'DejaVu Sans';
 }
 
+.zoom0 #yearview_datecontent, .zoom0 #yearview_labeldate {
+	font-size:9pt;
+}
+
+.zoom1 #yearview_datecontent, .zoom1 #yearview_labeldate {
+	font-size:10pt;
+}
+
+.zoom2 #yearview_datecontent, .zoom2 #yearview_labeldate {
+	font-size:11pt;
+}
+
+.zoom3 #yearview_datecontent, .zoom3 #yearview_labeldate {
+	font-size:12pt;
+}
+
+.zoom4 #yearview_datecontent, .zoom4 #yearview_labeldate {
+	font-size:13pt;
+}
+
 #yearview_datecontent_scroller {
 	border:0;
 }
 
 .yearview_marker {
 	padding-left:1.5px;
 	padding-right:1.5px;
 	margin-right:0.2em;
 	min-width:1ex;
 }
 
 .yearview_entry_cursor {
 	color:rgba(255,255,255,0.93);
 	background-color:black;
-	border-radius:4px;
+	border-radius:0.3em;
 }
 
 .yearview_entry_single, .yearview_entry_repeated_day, .yearview_entry_repeated_hour, .yearview_entry_repeated_minute, .yearview_entry_repeated_second {
 	background-image:url("disc.svg");
 	background-size:100% auto;
 	background-position:center;
 	background-repeat:no-repeat;
@@ -293,44 +346,86 @@
 }
 
 
 /* Todo View */
 
 .todoview_title {
 	font-family:'DejaVu Sans';
-	font-size:11pt;
 	font-weight:bold;
 }
 
+.zoom0 .todoview_title {
+	font-size:9pt;
+}
+
+.zoom1 .todoview_title {
+	font-size:10pt;
+}
+
+.zoom2 .todoview_title {
+	font-size:11pt;
+}
+
+.zoom3 .todoview_title {
+	font-size:12pt;
+}
+
+.zoom4 .todoview_title {
+	font-size:13pt;
+}
+
 .todoview_list {
 	/* make lists half width of view-1, so two to-do lists fit nicely */
 	min-width:299px;
 }
 
 .todoview_list:not(:first-child) {
 	border-left:solid #888 1px;
 	}
 
 .todoview_items {
 	padding:4px;
 	font-family:'DejaVu Sans';
+}
+
+.todoview_item {
+	padding-top:0.1em;
+}
+
+.zoom0 .todoview_items {
+	font-size:8pt;
+}
+
+.zoom1 .todoview_items {
+	font-size:9pt;
+}
+
+.zoom2 .todoview_items {
 	font-size:10pt;
 }
 
+.zoom3 .todoview_items {
+	font-size:11pt;
+}
+
+.zoom4 .todoview_items {
+	font-size:12pt;
+}
+
 .todoview_marker {
 	padding-left:1.5px;
 	padding-right:1.5px;
 	margin-right:0.2em;
 	min-width:1ex;
 }
 
 .todoview_cursor {
 	color:white;
 	background-color:black;
-	border-radius:4px;
+	border-radius:0.3em;
 }
 
 .needs-action > .todoview_itemtext {
 	color:red;
 	font-weight:bold;
 }
```

### Comparing `pygenda-0.2.6/pygenda/glade/dialog_event.glade` & `pygenda-0.2.7/pygenda/glade/dialog_event.glade`

 * *Files 1% similar despite different names*

#### Comparing `pygenda-0.2.6/pygenda/glade/dialog_event.glade` & `pygenda-0.2.7/pygenda/glade/dialog_event.glade`

```diff
@@ -192,14 +192,15 @@
                           <object class="GtkRadioButton">
                             <property name="label" translatable="yes">Yes</property>
                             <property name="visible">True</property>
                             <property name="can-focus">True</property>
                             <property name="receives-default">False</property>
                             <property name="draw-indicator">True</property>
                             <property name="group">radiobutton_timed_no</property>
+                            <signal name="toggled" handler="timed_toggled" swapped="no"/>
                           </object>
                           <packing>
                             <property name="expand">False</property>
                             <property name="fill">True</property>
                             <property name="position">1</property>
                           </packing>
                         </child>
@@ -207,14 +208,15 @@
                           <object class="GtkRadioButton">
                             <property name="label" translatable="yes">All day</property>
                             <property name="visible">True</property>
                             <property name="can-focus">True</property>
                             <property name="receives-default">False</property>
                             <property name="draw-indicator">True</property>
                             <property name="group">radiobutton_timed_no</property>
+                            <signal name="toggled" handler="allday_toggled" swapped="no"/>
                           </object>
                           <packing>
                             <property name="expand">False</property>
                             <property name="fill">True</property>
                             <property name="position">2</property>
                           </packing>
                         </child>
@@ -395,14 +397,15 @@
                           <item id="YEARLY" translatable="yes">Yearly</item>
                           <item id="MONTHLY" translatable="yes">Monthly</item>
                           <item id="MONTHLY-MONTHDAY" translatable="yes">Monthly by day</item>
                           <item id="MONTHLY-WEEKDAY" translatable="yes">Monthly by weekday</item>
                           <item id="WEEKLY" translatable="yes">Weekly</item>
                           <item id="DAILY" translatable="yes">Daily</item>
                         </items>
+                        <signal name="changed" handler="reptype_changed" swapped="no"/>
                       </object>
                       <packing>
                         <property name="left-attach">1</property>
                         <property name="top-attach">0</property>
                       </packing>
                     </child>
                     <child>
@@ -667,14 +670,15 @@
                               <object class="GtkCheckButton" id="repeat_forever">
                                 <property name="visible">True</property>
                                 <property name="can-focus">True</property>
                                 <property name="receives-default">False</property>
                                 <property name="halign">start</property>
                                 <property name="active">True</property>
                                 <property name="draw-indicator">True</property>
+                                <signal name="toggled" handler="repforever_toggled" swapped="no"/>
                               </object>
                               <packing>
                                 <property name="expand">False</property>
                                 <property name="fill">True</property>
                                 <property name="position">1</property>
                               </packing>
                             </child>
@@ -813,14 +817,15 @@
                             </child>
                             <child>
                               <object class="GtkSwitch" id="alarm-set">
                                 <property name="visible">True</property>
                                 <property name="can-focus">True</property>
                                 <property name="halign">start</property>
                                 <property name="valign">center</property>
+                                <signal name="state-set" handler="alarmset_changed" swapped="no"/>
                               </object>
                               <packing>
                                 <property name="expand">False</property>
                                 <property name="fill">True</property>
                                 <property name="position">1</property>
                               </packing>
                             </child>
@@ -849,14 +854,16 @@
                                   <object class="GtkTreeView" id="alarm-list">
                                     <property name="visible">True</property>
                                     <property name="can-focus">True</property>
                                     <property name="headers-clickable">False</property>
                                     <property name="enable-search">False</property>
                                     <property name="show-expanders">False</property>
                                     <property name="activate-on-single-click">True</property>
+                                    <signal name="focus-out-event" handler="alarmlist_focusout" swapped="no"/>
+                                    <signal name="key-press-event" handler="alarmlist_keypress" swapped="no"/>
                                     <child internal-child="selection">
                                       <object class="GtkTreeSelection"/>
                                     </child>
                                   </object>
                                 </child>
                               </object>
                             </child>
```

### Comparing `pygenda-0.2.6/pygenda/glade/dialog_find.glade` & `pygenda-0.2.7/pygenda/glade/dialog_find.glade`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/pygenda/glade/dialog_todo.glade` & `pygenda-0.2.7/pygenda/glade/dialog_todo.glade`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/pygenda/glade/main.glade` & `pygenda-0.2.7/pygenda/glade/main.glade`

 * *Files 1% similar despite different names*

#### Comparing `pygenda-0.2.6/pygenda/glade/main.glade` & `pygenda-0.2.7/pygenda/glade/main.glade`

```diff
@@ -53,41 +53,20 @@
                 <property name="label" translatable="yes">_File</property>
                 <property name="use-underline">True</property>
                 <child type="submenu">
                   <object class="GtkMenu">
                     <property name="visible">True</property>
                     <property name="can-focus">False</property>
                     <child>
-                      <object class="GtkImageMenuItem">
-                        <property name="label">gtk-new</property>
-                        <property name="visible">True</property>
-                        <property name="sensitive">False</property>
-                        <property name="can-focus">False</property>
-                        <property name="use-underline">True</property>
-                        <property name="use-stock">True</property>
-                      </object>
-                    </child>
-                    <child>
-                      <object class="GtkImageMenuItem">
-                        <property name="label">gtk-open</property>
-                        <property name="visible">True</property>
-                        <property name="sensitive">False</property>
-                        <property name="can-focus">False</property>
-                        <property name="use-underline">True</property>
-                        <property name="use-stock">True</property>
-                      </object>
-                    </child>
-                    <child>
-                      <object class="GtkImageMenuItem">
-                        <property name="label">gtk-save-as</property>
+                      <object class="GtkMenuItem">
                         <property name="visible">True</property>
                         <property name="sensitive">False</property>
                         <property name="can-focus">False</property>
+                        <property name="label" translatable="yes">_Import File</property>
                         <property name="use-underline">True</property>
-                        <property name="use-stock">True</property>
                       </object>
                     </child>
                     <child>
                       <object class="GtkSeparatorMenuItem">
                         <property name="visible">True</property>
                         <property name="can-focus">False</property>
                       </object>
@@ -392,31 +371,29 @@
                         </child>
                       </object>
                     </child>
                     <child>
                       <object class="GtkImageMenuItem">
                         <property name="label">gtk-zoom-in</property>
                         <property name="visible">True</property>
-                        <property name="sensitive">False</property>
                         <property name="can-focus">False</property>
                         <property name="use-underline">True</property>
                         <property name="use-stock">True</property>
-                        <accelerator key="z" signal="activate" modifiers="GDK_CONTROL_MASK"/>
+                        <signal name="activate" handler="menuitem_zoomin" swapped="no"/>
                         <accelerator key="plus" signal="activate" modifiers="GDK_CONTROL_MASK"/>
                       </object>
                     </child>
                     <child>
                       <object class="GtkImageMenuItem">
                         <property name="label">gtk-zoom-out</property>
                         <property name="visible">True</property>
-                        <property name="sensitive">False</property>
                         <property name="can-focus">False</property>
                         <property name="use-underline">True</property>
                         <property name="use-stock">True</property>
-                        <accelerator key="z" signal="activate" modifiers="GDK_SHIFT_MASK | GDK_CONTROL_MASK"/>
+                        <signal name="activate" handler="menuitem_zoomout" swapped="no"/>
                         <accelerator key="minus" signal="activate" modifiers="GDK_CONTROL_MASK"/>
                       </object>
                     </child>
                     <child>
                       <object class="GtkImageMenuItem" id="menuelt-fullscreen">
                         <property name="label">gtk-fullscreen</property>
                         <property name="visible">True</property>
@@ -583,19 +560,18 @@
                     <property name="fill">True</property>
                     <property name="position">2</property>
                   </packing>
                 </child>
                 <child>
                   <object class="GtkButton" id="button3">
                     <property name="visible">True</property>
-                    <property name="sensitive">False</property>
                     <property name="can-focus">False</property>
                     <property name="focus-on-click">False</property>
                     <property name="receives-default">False</property>
-                    <signal name="clicked" handler="button3_clicked" swapped="no"/>
+                    <signal name="button-release-event" handler="button3_clicked" swapped="no"/>
                     <child>
                       <object class="GtkLabel">
                         <property name="visible">True</property>
                         <property name="can-focus">False</property>
                         <property name="label" translatable="yes">Zoom</property>
                         <property name="justify">center</property>
                       </object>
```

### Comparing `pygenda-0.2.6/pygenda/glade/view_week.glade` & `pygenda-0.2.7/pygenda/glade/view_week.glade`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/pygenda/glade/view_year.glade` & `pygenda-0.2.7/pygenda/glade/view_year.glade`

 * *Files 3% similar despite different names*

#### Comparing `pygenda-0.2.6/pygenda/glade/view_year.glade` & `pygenda-0.2.7/pygenda/glade/view_year.glade`

```diff
@@ -75,14 +75,15 @@
       </packing>
     </child>
     <child>
       <object class="GtkEventBox" id="year_grid_events">
         <property name="visible">True</property>
         <property name="can-focus">False</property>
         <property name="visible-window">False</property>
+        <signal name="button-press-event" handler="year_grid_click" swapped="no"/>
         <child>
           <!-- n-columns=37 n-rows=12 -->
           <object class="GtkGrid" id="year_grid_days">
             <property name="name">yearview_daygrid</property>
             <property name="visible">True</property>
             <property name="can-focus">False</property>
             <property name="hexpand">True</property>
@@ -116,14 +117,16 @@
             <property name="position">0</property>
           </packing>
         </child>
         <child>
           <object class="GtkEventBox" id="year_datecontent_events">
             <property name="visible">True</property>
             <property name="can-focus">False</property>
+            <signal name="button-press-event" handler="year_dtcont_click" swapped="no"/>
+            <signal name="draw" handler="year_dtcont_draw" swapped="no"/>
             <child>
               <object class="GtkScrolledWindow" id="year_datecontent_scroll">
                 <property name="name">yearview_datecontent_scroller</property>
                 <property name="visible">True</property>
                 <property name="can-focus">True</property>
                 <property name="hexpand">True</property>
                 <property name="hscrollbar-policy">never</property>
```

### Comparing `pygenda-0.2.6/pygenda/locale/en_US/LC_MESSAGES/pygenda.po` & `pygenda-0.2.7/pygenda/locale/en_US/LC_MESSAGES/pygenda.po`

 * *Files 18% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 #
 # Matthew Lewis <pygenda@semiprime.com>, 2022,2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Pygenda\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-14 19:04+0100\n"
-"PO-Revision-Date: 2023-03-14 19:04+0100\n"
+"POT-Creation-Date: 2023-04-19 23:07+0200\n"
+"PO-Revision-Date: 2023-04-19 23:07+0200\n"
 "Last-Translator: Matthew Lewis <pygenda@semiprime.com>\n"
 "Language: en_US\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: glade/dialog_event.glade:999 glade/dialog_todo.glade:202
+#: glade/dialog_event.glade:1006 glade/dialog_todo.glade:202
 msgid "Cancelled"
 msgstr "Canceled"
 
-#: glade/main.glade:331
+#: glade/main.glade:310
 msgid "Cance_lled"
 msgstr "Cance_led"
```

### Comparing `pygenda-0.2.6/pygenda/locale/fr/LC_MESSAGES/pygenda.mo` & `pygenda-0.2.7/pygenda/locale/fr/LC_MESSAGES/pygenda.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Pygenda\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2023-03-14 19:04+0100\n"
+"PO-Revision-Date: 2023-04-23 19:39+0200\n"
 "Last-Translator: Matthew Lewis <pygenda@semiprime.com>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
@@ -80,22 +80,22 @@
 "style=\"italic\" weight=\"bold\">pas</span> les alarmes.\n"
 "Pour activer des alarmes, il faut un programme séparé pour s’en charger.\n"
 "(Pour enlever cet avertissement, voir la documentation.)"
 
 msgid ""
 "A calendar/agenda application written in Python/GTK3. The UI is inspired by "
 "the Agenda apps on the Psion Series 3 and Series 5 PDAs.\n"
-"WARNING: This is in-development code, released as a preview for developers. "
+"WARNING: This is in-development code, released for testing and feedback. "
 "There will be bugs; please report them to: pygenda@semiprime.com."
 msgstr ""
 "Une application agenda écrite en Python/GTK3. L’interface utilisateur "
 "s’inspire des applications Agenda des PDAs Series 3 et 5 de Psion.\n"
 "ATTENTION : Cette application est en cours de développement et elle est "
-"publiée en avant-première pour les développeurs/euses. Il y aura des "
-"bogues ; veuillez les rapporter à : pygenda@semiprime.com."
+"publiée à des fins de test et feedback. Il y aura des bogues ; veuillez les "
+"rapporter à : pygenda@semiprime.com."
 
 msgid "Action"
 msgstr "Action"
 
 msgid "Action required"
 msgstr "Action requise"
 
@@ -436,14 +436,17 @@
 
 msgid "_Go To…"
 msgstr "_Aller à…"
 
 msgid "_Help"
 msgstr "Aid_e"
 
+msgid "_Import File"
+msgstr "_Importer fichier"
+
 msgid "_New Event…"
 msgstr "_Nouvel évènement…"
 
 msgid "_None"
 msgstr "_Rien"
 
 msgid "_Tentative"
```

### Comparing `pygenda-0.2.6/pygenda/locale/fr/LC_MESSAGES/pygenda.po` & `pygenda-0.2.7/pygenda/locale/fr/LC_MESSAGES/pygenda.po`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 #
 # Matthew Lewis <pygenda@semiprime.com>, 2022,2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Pygenda\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-14 19:04+0100\n"
-"PO-Revision-Date: 2023-03-14 19:04+0100\n"
+"POT-Creation-Date: 2023-04-19 23:07+0200\n"
+"PO-Revision-Date: 2023-04-23 19:39+0200\n"
 "Last-Translator: Matthew Lewis <pygenda@semiprime.com>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
@@ -70,15 +70,15 @@
 msgid "End date/time:"
 msgstr "Date/heure de fin :"
 
 #: pygenda_dialog_entryprops.py:138
 msgid "End date:"
 msgstr "Date de fin :"
 
-#: pygenda_dialog_entryprops.py:141 glade/dialog_event.glade:258
+#: pygenda_dialog_entryprops.py:141 glade/dialog_event.glade:260
 msgid "Duration:"
 msgstr "Durée :"
 
 #: pygenda_dialog_entryprops.py:149
 msgid " (timezone: {:s})"
 msgstr " (fuseau horaire : {:s})"
 
@@ -140,35 +140,35 @@
 msgid "Exception dates:"
 msgstr "Dates omises :"
 
 #: pygenda_dialog_entryprops.py:178
 msgid ";"
 msgstr " ;"
 
-#: pygenda_dialog_entryprops.py:184 glade/dialog_event.glade:376
+#: pygenda_dialog_entryprops.py:184 glade/dialog_event.glade:378
 msgid "Repeats:"
 msgstr "Répétition :"
 
-#: pygenda_dialog_entryprops.py:195 glade/dialog_event.glade:979
+#: pygenda_dialog_entryprops.py:195 glade/dialog_event.glade:986
 #: glade/dialog_todo.glade:181
 msgid "Status:"
 msgstr "Statut :"
 
-#: pygenda_dialog_entryprops.py:215 pygenda_dialog_event.py:454
+#: pygenda_dialog_entryprops.py:215 pygenda_dialog_event.py:459
 # Added by hand - not detected by gettext
 msgid "Audio"
 msgstr "Audio"
 
 msgid "Display"
 msgstr "Afficher"
 
 msgid "Email"
 msgstr "E-mail"
 
-#: pygenda_dialog_entryprops.py:230 pygenda_dialog_event.py:459
+#: pygenda_dialog_entryprops.py:230 pygenda_dialog_event.py:464
 msgid "“{:s}”"
 msgstr "« {:s} »"
 
 #: pygenda_dialog_entryprops.py:234
 msgid "Alarms:"
 msgstr "Alarmes :"
 
@@ -177,45 +177,45 @@
 msgstr "Description ({}) :"
 
 #: pygenda_dialog_entryprops.py:249 pygenda_dialog_entryprops.py:252
 #: glade/dialog_event.glade:107 glade/dialog_todo.glade:86
 msgid "Description:"
 msgstr "Description :"
 
-#: pygenda_dialog_event.py:263
+#: pygenda_dialog_event.py:264
 msgid "Time before event"
 msgstr "Temps avant l’évènement"
 
-#: pygenda_dialog_event.py:264
+#: pygenda_dialog_event.py:265
 msgid "Action"
 msgstr "Action"
 
-#: pygenda_dialog_event.py:711 glade/main.glade:523
+#: pygenda_dialog_event.py:718 glade/main.glade:500
 msgid "New Event"
 msgstr "Nouvel\névènement"
 
-#: pygenda_dialog_event.py:723
+#: pygenda_dialog_event.py:730
 msgid "Edit Event"
 msgstr "Modifier évènement"
 
-#: pygenda_dialog_event.py:1012 glade/dialog_event.glade:394
-#: glade/dialog_event.glade:726 glade/dialog_event.glade:997
+#: pygenda_dialog_event.py:1019 glade/dialog_event.glade:396
+#: glade/dialog_event.glade:730 glade/dialog_event.glade:1004
 #: glade/dialog_todo.glade:159 glade/dialog_todo.glade:198
 msgid "None"
 msgstr "Rien"
 
-#: pygenda_dialog_event.py:1385
+#: pygenda_dialog_event.py:1394
 msgid "Exception dates"
 msgstr "Dates omises"
 
-#: pygenda_dialog_event.py:1402
+#: pygenda_dialog_event.py:1411
 msgid "Add date"
 msgstr "Ajouter date"
 
-#: pygenda_dialog_event.py:1423
+#: pygenda_dialog_event.py:1432
 msgid "Remove date(s)"
 msgstr "Retirer date(s)"
 
 #: pygenda_dialog_find.py:67
 msgid "Find results"
 msgstr "Resultats de recherche"
 
@@ -227,76 +227,76 @@
 msgid "New To-do"
 msgstr "Nouvelle tâche"
 
 #: pygenda_dialog_todo.py:88
 msgid "Edit To-do"
 msgstr "Modifier tâche"
 
-#: pygenda_gui.py:824
+#: pygenda_gui.py:866
 msgid "Delete Entry"
 msgstr "Supprimer l’entrée"
 
-#: pygenda_gui.py:830
+#: pygenda_gui.py:872
 msgid "Delete all repeats:\n“{:s}”?"
 msgstr "Supprimer toutes les entrées\n« {:s} » ?"
 
-#: pygenda_gui.py:832
+#: pygenda_gui.py:874
 msgid "Delete entry:\n“{:s}”?"
 msgstr "Supprimer l’entrée\n« {:s} » ?"
 
-#: pygenda_gui.py:860 glade/main.glade:573
+#: pygenda_gui.py:902 glade/main.glade:550
 msgid "Go To"
 msgstr "Aller à"
 
-#: pygenda_gui.py:872
+#: pygenda_gui.py:914
 msgid "Go"
 msgstr "Y aller"
 
-#: pygenda_gui.py:909
+#: pygenda_gui.py:953
 msgid ""
 "A calendar/agenda application written in Python/GTK3. The UI is inspired by "
 "the Agenda apps on the Psion Series 3 and Series 5 PDAs.\n"
-"WARNING: This is in-development code, released as a preview for developers. "
+"WARNING: This is in-development code, released for testing and feedback. "
 "There will be bugs; please report them to: pygenda@semiprime.com."
 msgstr ""
 "Une application agenda écrite en Python/GTK3. L’interface utilisateur "
 "s’inspire des applications Agenda des PDAs Series 3 et 5 de Psion.\n"
 "ATTENTION : Cette application est en cours de développement et elle est "
-"publiée en avant-première pour les développeurs/euses. Il y aura des "
-"bogues ; veuillez les rapporter à : pygenda@semiprime.com."
+"publiée à des fins de test et feedback. Il y aura des bogues ; veuillez "
+"les rapporter à : pygenda@semiprime.com."
 
 #: pygenda_view_todo.py:44
 msgid "To-do"
 msgstr "Tâches"
 
-#: pygenda_view_todo.py:60
+#: pygenda_view_todo.py:63
 msgid "_Todo View"
 msgstr "Mode _Tâches"
 
-#: pygenda_view_week.py:63
+#: pygenda_view_week.py:66
 msgid "_Week View"
 msgstr "Mode _Hebdomadaire"
 
-#: pygenda_view_week.py:68
+#: pygenda_view_week.py:71
 msgid "week_view_accel"
 msgstr "h"
 
-#: pygenda_view_week.py:195
+#: pygenda_view_week.py:204
 msgid "Week 53/Week 1"
 msgstr "Semaine 53/Semaine 1"
 
-#: pygenda_view_week.py:197
+#: pygenda_view_week.py:206
 msgid "Week {}"
 msgstr "Semaine {}"
 
-#: pygenda_view_year.py:67
+#: pygenda_view_year.py:69
 msgid "_Year View"
 msgstr "Mode _Annuelle"
 
-#: pygenda_view_year.py:72
+#: pygenda_view_year.py:74
 msgid "year_view_accel"
 msgstr "a"
 
 #: pygenda_widgets.py:64
 msgid "ymdhm"
 msgstr "amjhm"
 
@@ -312,201 +312,201 @@
 msgid "No"
 msgstr "Non"
 
 #: glade/dialog_event.glade:193
 msgid "Yes"
 msgstr "Oui"
 
-#: glade/dialog_event.glade:208
+#: glade/dialog_event.glade:209
 msgid "All day"
 msgstr "Journée"
 
-#: glade/dialog_event.glade:242
+#: glade/dialog_event.glade:244
 msgid "Start time:"
 msgstr "Commencer à :"
 
-#: glade/dialog_event.glade:274
+#: glade/dialog_event.glade:276
 msgid "End time:"
 msgstr "Heure de fin :"
 
-#: glade/dialog_event.glade:320
+#: glade/dialog_event.glade:322
 msgid "Days:"
 msgstr "Jours :"
 
-#: glade/dialog_event.glade:361
+#: glade/dialog_event.glade:363
 msgid "Time"
 msgstr "Heure"
 
-#: glade/dialog_event.glade:395
+#: glade/dialog_event.glade:397
 msgid "Yearly"
 msgstr "Annuelle"
 
-#: glade/dialog_event.glade:396
+#: glade/dialog_event.glade:398
 msgid "Monthly"
 msgstr "Mensuelle"
 
-#: glade/dialog_event.glade:397
+#: glade/dialog_event.glade:399
 msgid "Monthly by day"
 msgstr "Mensuelle par jour"
 
-#: glade/dialog_event.glade:398
+#: glade/dialog_event.glade:400
 msgid "Monthly by weekday"
 msgstr "Mensuelle par jour de la semaine"
 
-#: glade/dialog_event.glade:399
+#: glade/dialog_event.glade:401
 msgid "Weekly"
 msgstr "Hebdomadaire"
 
-#: glade/dialog_event.glade:400
+#: glade/dialog_event.glade:402
 msgid "Daily"
 msgstr "Quotidienne"
 
-#: glade/dialog_event.glade:416
+#: glade/dialog_event.glade:419
 msgid "Repeat on:"
 msgstr "Répéter le :"
 
-#: glade/dialog_event.glade:445
+#: glade/dialog_event.glade:448
 msgid "Last day"
 msgstr "Dernier jour"
 
-#: glade/dialog_event.glade:446
+#: glade/dialog_event.glade:449
 msgid "2nd last day"
 msgstr "2e au dernier jour"
 
-#: glade/dialog_event.glade:447
+#: glade/dialog_event.glade:450
 msgid "3rd last day"
 msgstr "3e au dernier jour"
 
-#: glade/dialog_event.glade:448
+#: glade/dialog_event.glade:451
 msgid "4th last day"
 msgstr "4e au dernier jour"
 
-#: glade/dialog_event.glade:449
+#: glade/dialog_event.glade:452
 msgid "5th last day"
 msgstr "5e au dernier jour"
 
-#: glade/dialog_event.glade:450
+#: glade/dialog_event.glade:453
 msgid "6th last day"
 msgstr "6e au dernier jour"
 
-#: glade/dialog_event.glade:451
+#: glade/dialog_event.glade:454
 msgid "7th last day"
 msgstr "7e au dernier jour"
 
-#: glade/dialog_event.glade:477
+#: glade/dialog_event.glade:480
 msgid "1st"
 msgstr "1er"
 
-#: glade/dialog_event.glade:478
+#: glade/dialog_event.glade:481
 msgid "2nd"
 msgstr "2e"
 
-#: glade/dialog_event.glade:479
+#: glade/dialog_event.glade:482
 msgid "3rd"
 msgstr "3e"
 
-#: glade/dialog_event.glade:480
+#: glade/dialog_event.glade:483
 msgid "4th"
 msgstr "4e"
 
-#: glade/dialog_event.glade:481
+#: glade/dialog_event.glade:484
 msgid "5th"
 msgstr "5e"
 
-#: glade/dialog_event.glade:482
+#: glade/dialog_event.glade:485
 msgid "Last"
 msgstr "Dernier"
 
-#: glade/dialog_event.glade:483
+#: glade/dialog_event.glade:486
 msgid "2nd last"
 msgstr "2e au dernier"
 
-#: glade/dialog_event.glade:484
+#: glade/dialog_event.glade:487
 msgid "3rd last"
 msgstr "3e au dernier"
 
-#: glade/dialog_event.glade:485
+#: glade/dialog_event.glade:488
 msgid "4th last"
 msgstr "4e au dernier"
 
-#: glade/dialog_event.glade:486
+#: glade/dialog_event.glade:489
 msgid "5th last"
 msgstr "5e au dernier"
 
-#: glade/dialog_event.glade:535
+#: glade/dialog_event.glade:538
 msgid "Period:"
 msgstr "Période :"
 
-#: glade/dialog_event.glade:551
+#: glade/dialog_event.glade:554
 msgid "Repeat Forever:"
 msgstr "Répéter à jamais :"
 
-#: glade/dialog_event.glade:577
+#: glade/dialog_event.glade:580
 msgid "Occurrences:"
 msgstr "Occurrences :"
 
-#: glade/dialog_event.glade:593
+#: glade/dialog_event.glade:596
 msgid "Until:"
 msgstr "Jusqu’à :"
 
-#: glade/dialog_event.glade:618
+#: glade/dialog_event.glade:621
 msgid "Exceptions:"
 msgstr "Dates omises :"
 
-#: glade/dialog_event.glade:778
+#: glade/dialog_event.glade:782
 msgid "Repeats"
 msgstr "Répétitions"
 
-#: glade/dialog_event.glade:803
+#: glade/dialog_event.glade:807
 msgid "Alarm(s) set:"
 msgstr "Alarme(s) activée(s) :"
 
-#: glade/dialog_event.glade:887
+#: glade/dialog_event.glade:894
 msgid ""
 "<span weight=\"bold\">Warning:</span> Pygenda will <span style=\"italic\" weight=\"bold\">not</span> sound/display alarms.\n"
 "A separate alarm handler is required for alarms to activate.\n"
 "(To remove this warning, see the documentation.)"
 msgstr ""
 "<span weight=\"bold\">Attention :</span> Pygenda n’active <span style=\"italic\" weight=\"bold\">pas</span> les alarmes.\n"
 "Pour activer des alarmes, il faut un programme séparé pour s’en charger.\n"
 "(Pour enlever cet avertissement, voir la documentation.)"
 
-#: glade/dialog_event.glade:901
+#: glade/dialog_event.glade:908
 msgid "Understood"
 msgstr "Je comprends"
 
-#: glade/dialog_event.glade:932
+#: glade/dialog_event.glade:939
 msgid "Alarms"
 msgstr "Alarmes"
 
-#: glade/dialog_event.glade:949
+#: glade/dialog_event.glade:956
 msgid "Location:"
 msgstr "Lieu :"
 
-#: glade/dialog_event.glade:998
+#: glade/dialog_event.glade:1005
 msgid "Tentative"
 msgstr "Provisoire"
 
-#: glade/dialog_event.glade:999 glade/dialog_todo.glade:202
+#: glade/dialog_event.glade:1006 glade/dialog_todo.glade:202
 msgid "Cancelled"
 msgstr "Annulé"
 
-#: glade/dialog_event.glade:1000
+#: glade/dialog_event.glade:1007
 msgid "Confirmed"
 msgstr "Confirmé"
 
-#: glade/dialog_event.glade:1014
+#: glade/dialog_event.glade:1021
 msgid ""
 "Details will go here:\n"
 "long description, attendees…"
 msgstr ""
 "Les détails seront ici :\n"
 "description détaillée, partipants…"
 
-#: glade/dialog_event.glade:1033
+#: glade/dialog_event.glade:1040
 msgid "Details"
 msgstr "Détails"
 
 #: glade/dialog_find.glade:25
 msgid "Find"
 msgstr "Rechercher"
 
@@ -542,114 +542,118 @@
 msgid "Completed"
 msgstr "Achevé"
 
 #: glade/main.glade:53
 msgid "_File"
 msgstr "_Fichier"
 
-#: glade/main.glade:114
+#: glade/main.glade:64
+msgid "_Import File"
+msgstr "_Importer fichier"
+
+#: glade/main.glade:93
 msgid "_Edit"
 msgstr "É_dition"
 
-#: glade/main.glade:161
+#: glade/main.glade:140
 msgid "_Delete…"
 msgstr "_Supprimer…"
 
-#: glade/main.glade:180
+#: glade/main.glade:159
 msgid "E_ntry"
 msgstr "E_ntrée"
 
-#: glade/main.glade:190
+#: glade/main.glade:169
 msgid "_New Event…"
 msgstr "_Nouvel évènement…"
 
-#: glade/main.glade:200
+#: glade/main.glade:179
 msgid "New _To-do…"
 msgstr "Nouvelle _tâche…"
 
-#: glade/main.glade:210
+#: glade/main.glade:189
 msgid "Show _Properties"
 msgstr "Afficher _propriétés"
 
-#: glade/main.glade:225
+#: glade/main.glade:204
 msgid "Edit _Time…"
 msgstr "Modifier _heure…"
 
-#: glade/main.glade:235
+#: glade/main.glade:214
 msgid "Edit _Repeats…"
 msgstr "Modifier _répétitions…"
 
-#: glade/main.glade:245
+#: glade/main.glade:224
 msgid "Edit _Alarms…"
 msgstr "Modifier _alarmes…"
 
-#: glade/main.glade:255
+#: glade/main.glade:234
 msgid "Edit _Details…"
 msgstr "Modifier _détails…"
 
-#: glade/main.glade:271
+#: glade/main.glade:250
 msgid "Set _Status"
 msgstr "_Statut"
 
-#: glade/main.glade:281
+#: glade/main.glade:260
 msgid "_None"
 msgstr "_Rien"
 
-#: glade/main.glade:291
+#: glade/main.glade:270
 msgid "_Confirmed"
 msgstr "_Confirmé"
 
-#: glade/main.glade:301
+#: glade/main.glade:280
 msgid "_Action required"
 msgstr "_Action requise"
 
-#: glade/main.glade:311
+#: glade/main.glade:290
 msgid "In _progress"
 msgstr "En _cours"
 
-#: glade/main.glade:321
+#: glade/main.glade:300
 msgid "_Completed"
 msgstr "_Achevé"
 
-#: glade/main.glade:331
+#: glade/main.glade:310
 msgid "Cance_lled"
 msgstr "_Annulé"
 
-#: glade/main.glade:341
+#: glade/main.glade:320
 msgid "_Tentative"
 msgstr "_Provisoire"
 
-#: glade/main.glade:359
+#: glade/main.glade:338
 msgid "_View"
 msgstr "_Afficharge"
 
-#: glade/main.glade:369
+#: glade/main.glade:348
 msgid "_View Mode"
 msgstr "_Mode"
 
-#: glade/main.glade:379
+#: glade/main.glade:358
 msgid "Switch _View"
 msgstr "Changer mode"
 
-#: glade/main.glade:438
+#: glade/main.glade:415
 msgid "_Tools"
 msgstr "_Outils"
 
-#: glade/main.glade:448
+#: glade/main.glade:425
 msgid "_Go To…"
 msgstr "_Aller à…"
 
-#: glade/main.glade:456
+#: glade/main.glade:433
 msgid "_Find…"
 msgstr "_Rechercher…"
 
-#: glade/main.glade:474
+#: glade/main.glade:451
 msgid "_Help"
 msgstr "Aid_e"
 
-#: glade/main.glade:548
+#: glade/main.glade:525
 msgid "View"
 msgstr "Mode"
 
-#: glade/main.glade:599
+#: glade/main.glade:575
 msgid "Zoom"
 msgstr "Zoom"
```

### Comparing `pygenda-0.2.6/pygenda/mypy.ini` & `pygenda-0.2.7/pygenda/mypy.ini`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/pygenda/pygenda_calendar.py` & `pygenda-0.2.7/pygenda/pygenda_calendar.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/pygenda/pygenda_config.py` & `pygenda-0.2.7/pygenda/pygenda_config.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/pygenda/pygenda_dialog_entryprops.py` & `pygenda-0.2.7/pygenda/pygenda_dialog_entryprops.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/pygenda/pygenda_dialog_event.py` & `pygenda-0.2.7/pygenda/pygenda_dialog_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,16 +137,23 @@
         # Called from GUI init_stage2().
 
         # Load glade file
         GUI.load_glade_file('dialog_event.glade')
 
         # Connect signal handlers
         HANDLERS = {
+            'timed_toggled': cls._do_timed_toggle,
+            'allday_toggled': cls._do_allday_toggle,
+            'reptype_changed': cls._reptype_changed,
+            'repforever_toggled': cls._do_repeatforever_toggle,
             'exceptions_modify': cls.dialog_repeat_exceptions,
-            'alarms_understood': cls.alarms_understood
+            'alarms_understood': cls.alarms_understood,
+            'alarmset_changed': cls._do_alarmset_toggle,
+            'alarmlist_focusout': cls._alarmlist_focusloss,
+            'alarmlist_keypress': cls._alarmlist_keypress,
             }
         GUI._builder.connect_signals(HANDLERS)
 
         # Get some references to dialog elements in glade
         cls.dialog = GUI._builder.get_object('dialog_event')
         if (not cls.dialog): # Sanity check
             raise NameError('Dialog Event not found')
@@ -184,17 +191,14 @@
         tbox.show_all()
 
         # Make lists of revealers, so they can be hidden/revealed
         cls.revs_timedur = cls._revealers_from_ids('revealer_time_l', 'revealer_time_e')
         cls.revs_allday = cls._revealers_from_ids('revealer_allday_l', 'revealer_allday_e')
         cls.wid_allday_count = GUI._builder.get_object('allday_count')
 
-        cls.wid_timed_buttons[1].connect('toggled', cls._do_timed_toggle)
-        cls.wid_timed_buttons[2].connect('toggled', cls._do_allday_toggle)
-
         # We keep references to these connections, so then can be (un)blocked.
         cls._tmdur_handler_time = cls.wid_time.connect('changed', cls._tmdur_changed, 0)
         cls._tmdur_handler_dur = cls.wid_dur.connect('changed', cls._tmdur_changed, 1)
         cls._tmdur_handler_endtime = cls.wid_endtime.connect('changed', cls._tmdur_changed, 2)
 
         # By default the signal is *blocked* - unblock when dialog active
         cls._block_tmdur_signals()
@@ -205,22 +209,20 @@
         # Initialise widgets etc in the Event dialog under the "Repeats" tab.
         # Called on app startup.
         cls.wid_rep_type = GUI._builder.get_object('combo_repeat_type')
         cls.revs_repeat = cls._revealers_from_ids('revealer_repeat_l','revealer_repeat_e')
         cls.revs_rep_monthdays = cls._revealers_from_ids('revealer_repeat_monthday_e')
         cls.revs_rep_weekdays = cls._revealers_from_ids('revealer_repeat_weekday_e')
         cls.revs_rep_monthweekdays = cls._revealers_from_ids('revealer_repeat_day_l')
-        cls.wid_rep_type.connect('changed', cls._reptype_changed)
 
         cls.wid_rep_interval = GUI._builder.get_object('repeat_interval')
         cls.wid_rep_forever = GUI._builder.get_object('repeat_forever')
         cls.wid_repbymonthday = GUI._builder.get_object('combo_bydaymonth')
         cls.wid_repbyweekday_day = GUI._builder.get_object('combo_byday_day')
         cls.wid_repbyweekday_ord = GUI._builder.get_object('combo_byday_ord')
-        cls.wid_rep_forever.connect('toggled', cls._do_repeatforever_toggle)
 
         cls.wid_rep_occs = GUI._builder.get_object('repeat_occurrences')
         cls.wid_rep_enddt = WidgetDate()
         rbox = GUI._builder.get_object('revealer_repeat_until_e').get_child() # Should be a GtkBox
         rbox.add(cls.wid_rep_enddt)
         rbox.show_all()
         cls.revs_rep_ends = cls._revealers_from_ids('revealer_repeat_until_l', 'revealer_repeat_until_e')
@@ -251,23 +253,20 @@
     @classmethod
     def _init_alarmfields(cls) -> None:
         # Initialise widgets etc in the Event dialog under the "Alarm" tab.
         # Called on app startup.
         cls.wid_alarmstack = GUI._builder.get_object('alarm-stack')
         cls.wid_alarmset = GUI._builder.get_object('alarm-set')
         cls._revealer_alarmlist = GUI._builder.get_object('revealer_alarmlist')
-        cls.wid_alarmset.connect('state-set', cls._do_alarmset_toggle)
 
         cls.wid_alarmlist = GUI._builder.get_object('alarm-list')
         cls.alarmlist_model = Gtk.ListStore(object, str, str) # AlarmInfo + cols
         cls.wid_alarmlist.set_model(cls.alarmlist_model)
         cls.wid_alarmlist.append_column(Gtk.TreeViewColumn(_('Time before event'),Gtk.CellRendererText(), text=1))
         cls.wid_alarmlist.append_column(Gtk.TreeViewColumn(_('Action'), Gtk.CellRendererText(), text=2))
-        cls.wid_alarmlist.connect('key-press-event', cls._alarmlist_keypress)
-        cls.wid_alarmlist.connect('focus-out-event', cls._alarmlist_focusloss)
 
         # Read config settings
         td_str = Config.get('new_event','timed_default_alarm_before')
         cls._default_alarm_before = parse_timedelta(td_str)
 
 
     @classmethod
@@ -329,45 +328,48 @@
         # Change _empty_desc_allowed True->False
         # Leave unchanged if is None
         if cls._empty_desc_allowed:
             cls._empty_desc_allowed = False
 
 
     @classmethod
-    def _do_timed_toggle(cls, wid:Gtk.RadioButton) -> None:
+    def _do_timed_toggle(cls, wid:Gtk.RadioButton) -> bool:
         # Callback. Called when "timed" radio button changes state.
         # Reveals/hides appropriate sub-obtions, and flags that
         # dialog state had been changed.
         ti = cls.wid_timed_buttons[1].get_active()
         cls._do_multireveal(cls.revs_timedur, ti)
         cls._cancel_empty_desc_allowed()
+        return True # don't propagate event
 
 
     @classmethod
-    def _do_allday_toggle(cls, wid:Gtk.RadioButton) -> None:
+    def _do_allday_toggle(cls, wid:Gtk.RadioButton) -> bool:
         # Callback. Called when "all day" radio button changes state.
         # Reveals/hides appropriate sub-obtions, and flags that
         # dialog state had been changed.
         ad = cls.wid_timed_buttons[2].get_active()
         cls._do_multireveal(cls.revs_allday, ad)
         cls._cancel_empty_desc_allowed()
+        return True # don't propagate event
 
 
     @classmethod
-    def _desc_changed(cls, wid:Gtk.Entry) -> None:
+    def _desc_changed(cls, wid:Gtk.Entry) -> bool:
         # Callback. Called when event description is changed by user.
         # Flags that dialog state had been changed.
         # Removes error state styling if it is no longer needed.
         if cls.wid_desc.get_text(): # if desc field is non-empty
             cls._cancel_empty_desc_allowed()
         cls._is_valid_event(set_style=False) # remove error styles if present
+        return True # don't propagate event
 
 
     @classmethod
-    def _reptype_changed(cls, wid:Gtk.ComboBox) -> None:
+    def _reptype_changed(cls, wid:Gtk.ComboBox) -> bool:
         # Callback. Called when event repeat type is changed by user.
         # Reveals/hides relevant sub-options.
         # wid should be the repeat-type combobox
         st = wid.get_active()>0
         cls._do_multireveal(cls.revs_repeat, st)
         monthday = (wid.get_active_id()=='MONTHLY-MONTHDAY')
         weekday = (wid.get_active_id()=='MONTHLY-WEEKDAY') # Booleans
@@ -400,18 +402,19 @@
                     # Value will be, e.g. "1st", "2nd" (Tues of month)
                     cls.wid_repbyweekday_ord.set_active_id(str(1+(sdt.day-1)//7))
                 else:
                     # Want, e.g. "last" (Friday of month)
                     rem = monthrange(sdt.year,sdt.month)[1]-sdt.day
                     cls.wid_repbyweekday_ord.set_active_id(str(-1-(rem//7)))
         cls._cancel_empty_desc_allowed()
+        return True # don't propagate event
 
 
     @classmethod
-    def _do_repeatforever_toggle(cls, wid:Gtk.Button) -> None:
+    def _do_repeatforever_toggle(cls, wid:Gtk.Button) -> bool:
         # Callback. Called when repeat-forever state is changed by user.
         # Reveals/hides relevant sub-options.
         st = not wid.get_active() #If *not* forever, we show repeat-til options
         cls._do_multireveal(cls.revs_rep_ends, st)
         if st:
             # Want to make sure revealed elements are synced
             if cls.rep_occs_determines_end:
@@ -421,27 +424,29 @@
                 sdt = cls.get_date_start()
                 edt = cls.wid_rep_enddt.get_date_or_none()
                 if sdt is not None and (edt is None or edt < sdt):
                     cls.wid_rep_enddt.set_date(sdt)
                     cls.wid_rep_occs.set_value(1)
 
         cls._cancel_empty_desc_allowed()
+        return True # don't propagate event
 
 
     @classmethod
-    def _do_alarmset_toggle(cls, wid:Gtk.Widget, state:bool) -> None:
-        # Callback. Called when alarm set state is changed by user.
+    def _do_alarmset_toggle(cls, wid:Gtk.Widget, state:bool) -> bool:
+        # Callback. Called when alarm set state is changed.
         # Reveals/hides alarm list.
         if state and len(cls.alarmlist_model)==0:
             # User just enabled alarms, so if no alarms, create default ones
             cls._add_alarm(AlarmInfo(-cls._default_alarm_before,action='AUDIO'))
             cls._add_alarm(AlarmInfo(-cls._default_alarm_before,action='DISPLAY',desc=cls.wid_desc.get_text()))
             # Also, user has interacted with settings, so expect a valid entry
             cls._cancel_empty_desc_allowed()
         cls._revealer_alarmlist.set_reveal_child(state)
+        return True # don't propagate event
 
 
     @classmethod
     def _add_alarm(cls, a_info:AlarmInfo) -> None:
         # Adds an alarm to alarm list
         itr = cls.alarmlist_model.append(None)
         cls._set_alarm_row(itr, a_info)
@@ -510,15 +515,15 @@
         cls.wid_repbyweekday_ord.handler_unblock(cls._rep_handler_wdayord)
         cls.wid_rep_interval.handler_unblock(cls._rep_handler_inter)
         cls.wid_rep_occs.handler_unblock(cls._rep_handler_occs)
         cls.wid_rep_enddt.handler_unblock(cls._rep_handler_enddt)
 
 
     @classmethod
-    def _tmdur_changed(cls, wid:Gtk.Widget, el:int) -> None:
+    def _tmdur_changed(cls, wid:Gtk.Widget, el:int) -> bool:
         # Callback. Called when starttime/endtime/duration changed.
         # 'el' paramenter indicates which one changed (but could use wid).
         sdt = cls.get_date_start()
         stm = cls.wid_time.get_time_or_none()
         d = cls.wid_dur.get_duration_or_none()
         etm = cls.wid_endtime.get_time_or_none()
         if sdt is not None and stm is not None and d is not None and etm is not None:
@@ -539,18 +544,19 @@
                     if end_dttm<st_dttm:
                         end_dttm += timedelta(days=1)
                     cls.wid_dur.set_duration(end_dttm - st_dttm)
             finally:
                 cls._unblock_tmdur_signals()
         cls._cancel_empty_desc_allowed()
         cls._is_valid_event(set_style=False) # remove error styles if present
+        return True # don't propagate event
 
 
     @classmethod
-    def _repend_changed(cls, wid:Gtk.Widget, el:int) -> None:
+    def _repend_changed(cls, wid:Gtk.Widget, el:int) -> bool:
         # Handler for signals from any widget that might result in either the
         # repeat end-date or occurence count changing. Prompts recalculation
         # and possibly also updates which of end-date/occurences is the leader.
         # Variable el indicates if either possible leader was updated.
         if el == 1: # Occurrences edited, make it "leader"
             cls.rep_occs_determines_end = True
             cls._set_occs_min(1)
@@ -560,14 +566,15 @@
         cls._block_rep_occend_signals() # prevent accidental recursion
         try:
             cls._sync_rep_occs_end()
         finally:
             cls._unblock_rep_occend_signals()
         cls._cancel_empty_desc_allowed()
         cls._is_valid_event(set_style=False) # remove error styles if present
+        return True # don't propagate event
 
 
     @classmethod
     def _set_occs_min(cls, mn:int) -> None:
         # quick method to set minimum of the occurrences spinbutton
         mx = cls.wid_rep_occs.get_range().max
         cls.wid_rep_occs.set_range(mn,mx)
@@ -1244,29 +1251,31 @@
                 r = 1
         except ValueError:
             r = 1
         return r
 
 
     @classmethod
-    def dialog_repeat_exceptions(cls, *args) -> None:
+    def dialog_repeat_exceptions(cls, *args) -> bool:
         # Callback for +/- button to open sub-dialog for "repeat exceptions"
         edc = ExceptionsDialogController(cls.exception_list, parent=cls.dialog)
         result = edc.run()
         if result==Gtk.ResponseType.OK:
             dates = sorted(edc.get_dates())
             cls.exception_list = dates
             cls._set_label_rep_list()
         edc.destroy()
+        return True # event handled - don't propagate event
 
 
     @classmethod
-    def alarms_understood(cls, *args) -> None:
+    def alarms_understood(cls, *args) -> bool:
         # Handler for Alarms Understood button - show content
         cls.wid_alarmstack.set_visible_child_name('content')
+        return True # event handled - don't propagate event
 
 
     @classmethod
     def _alarmlist_keypress(cls, wid:Gtk.Widget, ev:Gdk.EventKey) -> bool:
         # Handler for key-press/repeat when alarmlist is focused
         if ev.keyval in (Gdk.KEY_BackSpace, Gdk.KEY_Delete):
             store,row = wid.get_selection().get_selected()
```

### Comparing `pygenda-0.2.6/pygenda/pygenda_dialog_find.py` & `pygenda-0.2.7/pygenda/pygenda_dialog_find.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/pygenda/pygenda_dialog_todo.py` & `pygenda-0.2.7/pygenda/pygenda_dialog_todo.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/pygenda/pygenda_entryinfo.py` & `pygenda-0.2.7/pygenda/pygenda_entryinfo.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/pygenda/pygenda_gui.py` & `pygenda-0.2.7/pygenda/pygenda_gui.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,14 +89,16 @@
     date_order = ''
     date_formatting_numeric = ''
     date_formatting_text = ''
     date_formatting_text_noyear = ''
     date_formatting_textabb = ''
     date_formatting_textabb_noyear = ''
 
+    _plus_minus_zoom = False
+
     # For startup
     _starting_cal = True
     _loading_indicator = None
 
     Config.set_defaults('global',{
         'language': '', # use OS language
         'hide_titlebar_when_maximized': False,
@@ -106,14 +108,15 @@
         'date_fmt_text': guess_date_fmt_text_from_locale(),
         'date_fmt_text_noyear': '', # construct from date_fmt_text
         'date_fmt_textabb': '', # construct from date_fmt_text
         'date_fmt_textabb_noyear': '', # construct from date_fmtabb_text
         '24hr': False,
         'start_week_day': 0, # 0 = Monday, 6 = Sunday
         'tab_elts_datetime': False,
+        'plus_minus_zoom': True,
         })
     Config.set_defaults('startup',{
         'maximize': False,
         'fullscreen': False,
         'view': False,
         'softbutton_display': '',
         })
@@ -172,22 +175,24 @@
             'menuitem_stat_confirmed': lambda a: cls.handler_stat_toggle('CONFIRMED'),
             'menuitem_stat_canceled': lambda a: cls.handler_stat_toggle('CANCELLED'),
             'menuitem_stat_tentative': lambda a: cls.handler_stat_toggle('TENTATIVE'),
             'menuitem_stat_needsaction': lambda a: cls.handler_stat_toggle('NEEDS-ACTION'),
             'menuitem_stat_inprocess': lambda a: cls.handler_stat_toggle('IN-PROCESS'),
             'menuitem_stat_completed': lambda a: cls.handler_stat_toggle('COMPLETED'),
             'menuitem_switchview': cls.switch_view,
+            'menuitem_zoomin': lambda a: cls.zoom(+1),
+            'menuitem_zoomout': lambda a: cls.zoom(-1),
             'menuitem_fullscreen': cls.toggle_fullscreen,
             'menuitem_goto': cls.dialog_goto,
             'menuitem_find': cls.handler_find,
             'menuitem_about': cls.dialog_about,
             'button0_clicked': cls.handler_newevent,
             'button1_clicked': cls.switch_view,
             'button2_clicked': cls.dialog_goto,
-            'button3_clicked': cls.debug, # zoom, to be decided/implemented
+            'button3_clicked': cls.zoom_button,
             }
         cls._builder.connect_signals(HANDLERS)
 
         cls._box_view_cont = cls._builder.get_object('box_view_cont')
         if (not cls._box_view_cont): # Sanity check
             raise NameError('View container not found')
 
@@ -324,30 +329,37 @@
         cls._box_view_cont.pack_start(cls._eventbox, True, True, 0)
         cls._box_view_cont.reorder_child(cls._eventbox, view_pos)
         cls._eventbox.add(cls.view_widgets[cls._view_idx])
         cls._eventbox.connect('key-press-event', cls.keypress)
         cls.view_widgets[cls._view_idx].grab_focus() # so it gets keypresses
         del(cls._box_view_cont) # don't need this anymore
 
+        cls._init_config()
         cls._init_dialogs()
 
         # Add functionality to spinbuttons not provided by GTK
         cls._init_spinbuttons()
         cls._init_comboboxes()
         cls._init_entryboxes()
 
         # Menu bar & softbutton bar made insensitive in .glade for startup.
         # We make them sensitive here before activating view.
         cls._builder.get_object('menu_bar').set_sensitive(True)
         cls._builder.get_object('box_buttons').set_sensitive(True)
 
-        cls.view_redraw() # Draw active view
+        cls.view_redraw(True) # Draw active view, including entries
         cls._eventbox.show_all()
 
 
+    @classmethod
+    def _init_config(cls) -> None:
+        # Read config settings at startup
+        cls._plus_minus_zoom = Config.get_bool('global','plus_minus_zoom')
+
+
     @staticmethod
     def _init_dialogs() -> None:
         # Import and initialise dialog classes.
         # Doing imports here avoids circular dependencies.
         global EventDialogController, EventPropertyBeyondEditDialog, TodoDialogController, EntryPropertiesDialog, FindDialogController
 
         from .pygenda_dialog_event import EventDialogController, EventPropertyBeyondEditDialog
@@ -494,38 +506,48 @@
             for id in cls._menu_elts_stat_event:
                 id.hide()
             for id in cls._menu_elts_stat_todo:
                 id.show()
 
 
     @classmethod
-    def keypress(cls, wid:Gtk.Widget, ev:Gdk.EventKey) -> None:
+    def keypress(cls, wid:Gtk.Widget, ev:Gdk.EventKey) -> bool:
         # Called whenever a key is pressed/repeated when View in focus
-        if ev.keyval==Gdk.KEY_Escape and cls._toggle_view_idx >= 0:
-            cls.switch_view(None, cls._toggle_view_idx)
-        cls.views[cls._view_idx].keypress(wid,ev)
+        if cls._plus_minus_zoom:
+            if ev.keyval==Gdk.KEY_plus:
+                cls.zoom(+1)
+                return True # handled
+            elif ev.keyval==Gdk.KEY_minus:
+                cls.zoom(-1)
+                return True # handled
+        if ev.keyval==Gdk.KEY_Escape:
+            if cls._toggle_view_idx >= 0:
+                cls.switch_view(None, cls._toggle_view_idx)
+        else:
+            cls.views[cls._view_idx].keypress(wid,ev)
+        return True # event handled - don't propagate
 
 
     @staticmethod
     def _spinbutton_keypress(wid:Gtk.SpinButton, ev:Gdk.EventKey) -> bool:
         # Called to handle extra spinbutton keyboard controls
         shiftdown = ev.state&Gdk.ModifierType.SHIFT_MASK
         if ev.keyval in GUI.SPINBUTTON_INC_KEY or (shiftdown and ev.keyval==Gdk.KEY_Up):
             wid.update() # So if user types "5" then "+" value changes to "6"
             wid.spin(Gtk.SpinType.STEP_FORWARD, 1)
-            return True # done
+            return True # done, don't propagate
         if ev.keyval in GUI.SPINBUTTON_DEC_KEY or (shiftdown and ev.keyval==Gdk.KEY_Down):
             wid.update()
             wid.spin(Gtk.SpinType.STEP_BACKWARD, 1)
             return True # done
         if ev.keyval==Gdk.KEY_Up:
             return wid.get_toplevel().child_focus(Gtk.DirectionType.UP)
         if ev.keyval==Gdk.KEY_Down:
             return wid.get_toplevel().child_focus(Gtk.DirectionType.DOWN)
-        return False # propagate event
+        return False # unhandled, so propagate event
 
 
     @staticmethod
     def _combobox_keypress(wid:Gtk.ComboBox, ev:Gdk.EventKey) -> bool:
         # Called to handle extra combobox keyboard controls
         # BUG!! This is not called when the combobox is in "popout" state
         if ev.keyval==Gdk.KEY_Return:
@@ -544,15 +566,15 @@
             wid.set_active(a)
             return True # done
         if ev.keyval in GUI.SPINBUTTON_DEC_KEY or (shiftdown and ev.keyval==Gdk.KEY_Up):
             if a<0:
                 a = 0
             a = (a-1)%count
             wid.set_active(a)
-            return True # done
+            return True # done, don't propagate
 
         if ev.keyval==Gdk.KEY_Up:
             return wid.get_toplevel().child_focus(Gtk.DirectionType.UP)
         if ev.keyval==Gdk.KEY_Down:
             return wid.get_toplevel().child_focus(Gtk.DirectionType.DOWN)
         if ev.keyval in (Gdk.KEY_Left,Gdk.KEY_Right):
             # Return - otherwise detected as alphabetic (not sure why!)
@@ -567,15 +589,15 @@
                 it = mdl.iter_next(it)
                 if it is None: # at end of list, loop to top!
                     it = mdl.get_iter_first()
                 ch1 = mdl.get(it,0)[0][0].lower()
                 if ch==ch1:
                     wid.set_active((a+i)%count)
                     break
-            return True # done
+            return True # done, don't propagate
 
         return False # propagate event
 
 
     @staticmethod
     def _focusout_unhighlight(wid:Gtk.Widget, ev:Gdk.EventKey) -> bool:
         # Called to handle remove highlight from entry box/spinbutton
@@ -590,35 +612,36 @@
     def view_redraw(cls, en_changes:bool=False) -> None:
         # Redraw the currently active view.
         # en_changes: bool, True if displayed entries need updating too
         cls.views[cls._view_idx].redraw(en_changes=en_changes)
 
 
     @classmethod
-    def switch_view(cls, wid:Gtk.Widget, idx:int=None, redraw:bool=True) -> None:
+    def switch_view(cls, wid:Gtk.Widget, idx:int=None, redraw:bool=True) -> bool:
         # Callback from UI widget (e.g. menu, softbutton) to change view.
         # idx = index of new view (otherwise goes to next view in list)
         if idx is None:
             # Go to next view in list
             cls._toggle_view_idx = cls._view_idx
             cls._view_idx = (cls._view_idx+1)%len(cls.views)
         elif cls._view_idx == idx:
-            return # No change, so skip redraw
+            return True # No change, so skip redraw & don't propagate event
         else:
             cls._toggle_view_idx = cls._view_idx
             cls._view_idx = idx
         cls._eventbox.remove(cls._eventbox.get_child())
         new_view = cls.views[cls._view_idx]
         new_view.renew_display()
         if redraw:
             new_view.redraw(en_changes=True)
         new_wid = cls.view_widgets[cls._view_idx]
         cls._eventbox.add(new_wid)
         new_wid.grab_focus()
         new_wid.show_all()
+        return True # don't propagate event
 
 
     @classmethod
     def cursor_goto_date(cls, dt:dt_date) -> None:
         # Call view to set current cursor date.
         # If current view does not support setting date (e.g. Todo View)
         # try next view etc., and make successful view active.
@@ -664,101 +687,112 @@
     def main(cls) -> None:
         # Run the man Gtk loop
         Gtk.main()
 
 
     # Signal handling functions
     @classmethod
-    def exit(cls, *args) -> None:
+    def exit(cls, *args) -> bool:
         # Callback for various types of exit signal (command line, menus...)
         Gtk.main_quit()
+        return True # don't propagate event
 
     @classmethod
-    def handler_newevent(cls, *args) -> None:
-        # Callback for new event signal (menu, softbutton)
+    def handler_newevent(cls, *args) -> bool:
+        # Callback for "Create new event" signal (menu, softbutton)
         date = cls.views[cls._view_idx].cursor_date()
         EventDialogController.new_event(date=date)
+        return True # don't propagate event
 
     @classmethod
-    def handler_find(cls, *args) -> None:
-        # Callback for find signal (menu)
-        FindDialogController.find()
-
-    @classmethod
-    def handler_newtodo(cls, *args) -> None:
-        # Callback for new todo signal (menu)
+    def handler_newtodo(cls, *args) -> bool:
+        # Callback for "Create new todo" signal (menu)
         lst = cls.views[cls._view_idx].cursor_todo_list()
         TodoDialogController.new_todo(list_idx=lst)
+        return True # don't propagate event
+
+    @classmethod
+    def handler_find(cls, *args) -> bool:
+        # Callback for find signal (menu)
+        FindDialogController.find()
+        return True # don't propagate event
 
     @classmethod
-    def handler_showentryprops(cls, *args) -> None:
-        # Callback for show-entry-props signal (menu item)
+    def handler_showentryprops(cls, *args) -> bool:
+        # Callback for "show entry properties" signal (menu item)
         en = cls.views[cls._view_idx].get_cursor_entry()
         if en:
             cls.dialog_showentryprops(en)
+        return True # don't propagate event
 
     @classmethod
-    def handler_edittime(cls, *args) -> None:
-        # Callback for change-entry-time signal (menu item)
+    def handler_edittime(cls, *args) -> bool:
+        # Callback for "edit entry time" signal (menu item)
         en = cls.views[cls._view_idx].get_cursor_entry()
         if en:
             cls.edit_or_display_event(en, EventDialogController.TAB_TIME)
+        return True # don't propagate event
 
     @classmethod
-    def handler_editrepeats(cls, *args) -> None:
-        # Callback for change-entry-repeats signal (menu item)
+    def handler_editrepeats(cls, *args) -> bool:
+        # Callback for "edit entry repeats" signal (menu item)
         en = cls.views[cls._view_idx].get_cursor_entry()
         if en:
             cls.edit_or_display_event(en, EventDialogController.TAB_REPEATS)
+        return True # don't propagate event
 
     @classmethod
-    def handler_editalarm(cls, *args) -> None:
-        # Callback for change-entry-alarm signal (menu item)
+    def handler_editalarm(cls, *args) -> bool:
+        # Callback for "edit entry alarms" signal (menu item)
         en = cls.views[cls._view_idx].get_cursor_entry()
         if en:
             cls.edit_or_display_event(en, EventDialogController.TAB_ALARM)
+        return True # don't propagate event
 
     @classmethod
-    def handler_editdetails(cls, *args) -> None:
-        # Callback for change-entry-details signal (menu item)
+    def handler_editdetails(cls, *args) -> bool:
+        # Callback for "edit entry details" signal (menu item)
         en = cls.views[cls._view_idx].get_cursor_entry()
         if en:
             cls.edit_or_display_event(en, EventDialogController.TAB_DETAILS)
+        return True # don't propagate event
 
 
     @classmethod
     def edit_or_display_event(cls, en:iEvent, subtab:int=None) -> None:
         # Bring up dialog to edit event, or show details if not editable
         try:
             EventDialogController.edit_event(en, subtab)
         except EventPropertyBeyondEditDialog as exc:
             print('Warning: {:s} - showing entry properties'.format(str(exc)), file=stderr)
             cls.dialog_showentryprops(en)
 
 
     @classmethod
-    def handler_stat_toggle(cls, stat:Optional[str]) -> None:
+    def handler_stat_toggle(cls, stat:Optional[str]) -> bool:
         # Handle signals from menu to change current entry's status.
         # Paramenter stat is None or text string for status (eg 'CONFIRMED').
         en = cls.views[cls._view_idx].get_cursor_entry()
         if en:
             Calendar.set_toggle_status_entry(en, stat)
             cls.view_redraw(en_changes=True)
+        return True # don't propagate event
 
 
     @classmethod
-    def delete_request(cls, *args) -> None:
+    def delete_request(cls, *args) -> bool:
         # Callback to implement "delete" from GUI, e.g. backspace key pressed
         en = cls.views[cls._view_idx].get_cursor_entry()
         if en is not None:
             cls.dialog_deleteentry(en)
+        return True # don't propagate event
 
 
     @classmethod
-    def cut_request(cls, *args) -> None:
+    def cut_request(cls, *args) -> bool:
         # Handler to implement "cut" from GUI, e.g. cut clicked in menu
         en = cls.views[cls._view_idx].get_cursor_entry()
         if en and 'SUMMARY' in en:
             if cls._lib_clip is None:
                 # Don't do fallback - might lead to unexpected data loss
                 print('Warning: No clipboard library, cut not available', file=stderr)
             elif 'RRULE' in en: # repeating entry
@@ -770,56 +804,64 @@
                 print('Warning: Cutting repeating entries not implemented', file=stderr)
             else:
                 txtbuf = bytes(en['SUMMARY'], 'utf-8')
                 calbuf = en.to_ical()
                 cls._lib_clip.set_cb(ctypes.create_string_buffer(txtbuf),ctypes.create_string_buffer(calbuf))
                 Calendar.delete_entry(en)
                 cls.view_redraw(en_changes=True)
+        return True # don't propagate event
 
 
     @classmethod
-    def copy_request(cls, *args) -> None:
+    def copy_request(cls, *args) -> bool:
         # Handler to implement "copy" from GUI, e.g. copy clicked in menu
         en = cls.views[cls._view_idx].get_cursor_entry()
         if en and 'SUMMARY' in en:
             if cls._lib_clip is None:
                 print('Warning: No clipboard library, fallback to text copy', file=stderr)
                 cb = Gtk.Clipboard.get(Gdk.SELECTION_CLIPBOARD)
                 txt = en['SUMMARY']
                 cb.set_text(txt, -1)
             else:
                 txtbuf = bytes(en['SUMMARY'], 'utf-8')
                 calbuf = en.to_ical()
                 cls._lib_clip.set_cb(ctypes.create_string_buffer(txtbuf),ctypes.create_string_buffer(calbuf))
+        return True # don't propagate event
 
 
     @classmethod
-    def paste_request(cls, *args) -> None:
+    def paste_request(cls, *args) -> bool:
         # Handler to implement "paste" from GUI, e.g. paste clicked in menu
         cb = Gtk.Clipboard.get(Gdk.SELECTION_CLIPBOARD)
 
         # First, we try requesting a 'text/calendar' type from the clipboard
         sdat = cb.wait_for_contents(Gdk.Atom.intern('text/calendar', False))
         try:
             ical = iCalendar.from_ical(sdat.get_data())
             en = ical.walk()[0]
             cls.views[cls._view_idx].new_entry_from_example(en)
             cls.view_redraw(en_changes=True)
-            return
         except:
-            None
+            # Fallback: request plain text from clipboard
+            txt = cb.wait_for_text()
+            if txt: # might be None
+                txt = cls._sanitise_pasted_text(txt)
+                # Type of entry created depends on View, so call View paste fn
+                if txt:
+                    cls.views[cls._view_idx].paste_text(txt)
+        return True # don't propagate event
 
-        # Fallback: request plain text from clipboard
-        txt = cb.wait_for_text()
-        if txt is not None:
-            txt = txt.strip()
-            txt = txt.replace('\n',' ')
-            txt = txt.replace('\t',' ')
-            # What type of entry is created will depend on view, so call current view paste fn
-            cls.views[cls._view_idx].paste_text(txt)
+
+    @staticmethod
+    def _sanitise_pasted_text(txt:str) -> str:
+        # Clean up text from clipboard so it's suitable as an entry summary
+        txt = txt.strip()
+        txt = txt.replace('\n',' ')
+        txt = txt.replace('\t',' ')
+        return txt
 
 
     @classmethod
     def dialog_deleteentry(cls, en:iEvent) -> None:
         # Dialog to implement "delete" from GUI, e.g. backspace key
         dialog = Gtk.Dialog(title=_('Delete Entry'), parent=cls._window,
             flags=Gtk.DialogFlags.MODAL|Gtk.DialogFlags.DESTROY_WITH_PARENT,
@@ -851,15 +893,15 @@
         # Used if requested from menu or, e.g., for read-only entries.
         dialog = EntryPropertiesDialog(entry, parent=cls._window)
         response = dialog.run()
         dialog.destroy()
 
 
     @classmethod
-    def dialog_goto(cls, *args) -> None:
+    def dialog_goto(cls, *args) -> bool:
         # Called to implement "go to" from GUI, e.g. button
         dialog = Gtk.Dialog(title=_('Go To'), parent=cls._window,
             flags=Gtk.DialogFlags.MODAL|Gtk.DialogFlags.DESTROY_WITH_PARENT,
             buttons=(Gtk.STOCK_CANCEL, Gtk.ResponseType.CLOSE))
         wdate = WidgetDate(cls.views[cls._view_idx].cursor_date())
         if (not dialog or not wdate): # Allocation check
             raise NameError('Dialog Goto creation failure')
@@ -881,60 +923,73 @@
                 break
             # Date is invalid, add error styling
             wdate.get_style_context().add_class(GUI.STYLE_ERR)
         if response == Gtk.ResponseType.APPLY:
             cls.cursor_goto_date(dt)
             cls.view_redraw(en_changes=False)
         dialog.destroy()
+        return True # don't propagate event
 
 
     @staticmethod
-    def check_date_fixed(wid:WidgetDate) -> None:
+    def check_date_fixed(wid:WidgetDate) -> bool:
         # Removes error highlight if date is valid (e.g. not 30th Feb)
         # Would be nice to make this a method of WidgetDate class.
         # Can be used as a callback, e.g. attached to 'changed' signal
         if wid.get_date_or_none() is not None:
             wid.get_style_context().remove_class(GUI.STYLE_ERR)
+        return False # propagate event
 
 
     @classmethod
-    def dialog_about(cls, *args) -> None:
-        # Display the "About" dialog
+    def dialog_about(cls, *args) -> bool:
+        # Display the "About Pygenda" dialog
         dialog = Gtk.AboutDialog(parent=cls._window)
         dialog.set_program_name('Pygenda')
         dialog.set_copyright(u'Copyright © 2022,2023 Matthew Lewis')
         dialog.set_license_type(Gtk.License.GPL_3_0_ONLY)
         dialog.set_logo_icon_name('x-office-calendar')
         dialog.set_authors(('Matthew Lewis',))
         dialog.set_version('version {:s}'.format(__version__))
-        dialog.set_comments(_(u'A calendar/agenda application written in Python/GTK3. The UI is inspired by the Agenda apps on the Psion Series 3 and Series 5 PDAs.\nWARNING: This is in-development code, released as a preview for developers. There will be bugs; please report them to: pygenda@semiprime.com.'))
+        dialog.set_comments(_(u'A calendar/agenda application written in Python/GTK3. The UI is inspired by the Agenda apps on the Psion Series 3 and Series 5 PDAs.\nWARNING: This is in-development code, released for testing and feedback. There will be bugs; please report them to: pygenda@semiprime.com.'))
         dialog.show_all()
         dialog.run()
         dialog.destroy()
+        return True # don't propagate event
 
 
     @classmethod
-    def toggle_fullscreen(cls, *args) -> None:
+    def toggle_fullscreen(cls, *args) -> bool:
         # Callback to toggle fullscreen mode on/off (e.g. from menu)
         cls._is_fullscreen = not cls._is_fullscreen
         if cls._is_fullscreen:
             cls._window.fullscreen()
             cls._menu_elt_fullscreen.set_label('gtk-leave-fullscreen')
             cls._menu_elt_fullscreen.set_image(cls._image_leave_fs)
         else:
             cls._window.unfullscreen()
             cls._menu_elt_fullscreen.set_label('gtk-fullscreen')
             cls._menu_elt_fullscreen.set_image(cls._image_enter_fs)
+        return True # don't propagate event
+
+
+    @classmethod
+    def zoom_button(cls, wid:Gtk.Widget, ev:Gdk.EventKey) -> bool:
+        # Zoom handler for Zoom soft-button
+        cls.zoom(-1 if ev.state&(Gdk.ModifierType.SHIFT_MASK|Gdk.ModifierType.CONTROL_MASK) else +1)
+        return True # don't propagate event
 
 
     @classmethod
-    def debug(cls, *args):
-        # Temporary callback - delete me !!!!
-        # Placeholder until we decide what fourth button does
-        print('Button clicked {}'.format(args[0]))
+    def zoom(cls, inc:int) -> bool:
+        # Callback for zoom-in/out menu items
+        # Zoom by inc, so zoom-in if inc==+1; zoom-out if inc==-1
+        # Call current view to do the work
+        cls.views[cls._view_idx].zoom(inc)
+        return True # don't propagate event
 
 
     @classmethod
     def todo_titles_default_cats(cls) -> Tuple[list,list]:
         # Return titles and default categories of todo lists
         try:
             todo_idx = cls._VIEWS.index('Todo')
```

### Comparing `pygenda-0.2.6/pygenda/pygenda_util.py` & `pygenda-0.2.7/pygenda/pygenda_util.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/pygenda/pygenda_view.py` & `pygenda-0.2.7/pygenda/pygenda_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from gi.repository.Pango import WrapMode as PWrapMode
 
 from icalendar import cal as iCal, Event as iEvent, Todo as iTodo
 from datetime import date as dt_date, datetime as dt_datetime, timedelta
 from typing import Optional, Union
 
 from .pygenda_gui import GUI
+from .pygenda_config import Config
 from .pygenda_dialog_event import EventDialogController
 from .pygenda_util import datetime_to_time, datetime_to_date, date_to_datetime, format_time, format_compact_date, format_compact_time, format_compact_datetime, dt_lte
 from .pygenda_calendar import Calendar
 from .pygenda_entryinfo import EntryInfo
 
 
 # Base class for pygenda Views (Week View, Year View, etc.)
@@ -64,14 +65,25 @@
     def init(cls) -> Gtk.Widget:
         # Initialise view and return Gtk widget for that view.
         # Called from GUI._init_views() on startup.
         return None
 
 
     @classmethod
+    def init_zoom(cls, config_gp:str, ctx:Gtk.StyleContext) -> None:
+        # Initialise zoom level
+        # Called during initialisation by child class.
+        cls.zoom_lvls = Config.get_int(config_gp,'zoom_levels') # type:ignore
+        cls.zoom_lvl = Config.get_int(config_gp,'default_zoom') # type:ignore
+        cls.zoom_lvl %= cls.zoom_lvls # type:ignore
+        cls.zoom_ctx = ctx # type:ignore
+        cls.zoom_ctx.add_class('zoom'+str(cls.zoom_lvl)) # type:ignore
+
+
+    @classmethod
     def renew_display(cls) -> None:
         # Called when we switch to this view.
         # Used to reset local state; default null implementation may be enough.
         pass
 
 
     @classmethod
@@ -147,14 +159,25 @@
     def cursor_goto_todo(cls, todo:iTodo, list_idx:int) -> bool:
         # Move cursor to given todo in given list.
         # Return True if can (False if can't) jump to todo in this view.
         # Default implementation does nothing & returns False.
         return False
 
 
+    @classmethod
+    def zoom(cls, inc:int) -> None:
+        # Zoom by inc, so zoom-in if inc==+1; zoom-out if inc==-1
+        # Assumes zoom_init() has been called.
+        # If not using this system, View should supply its own zoom().
+        # !! Note: might be better if it kept the cursor visible
+        cls.zoom_ctx.remove_class('zoom'+str(cls.zoom_lvl)) # type:ignore
+        cls.zoom_lvl = (cls.zoom_lvl+inc)%cls.zoom_lvls # type:ignore
+        cls.zoom_ctx.add_class('zoom'+str(cls.zoom_lvl)) # type:ignore
+
+
     @staticmethod
     def entry_text_label(ev:iCal.Event, dt_st:dt_date, dt_end:dt_date, add_location:bool=False) -> Gtk.Label:
         # Returns a GtkLabel with entry summary + icons as content.
         # Used by Week & Year views to display entries.
         lab = Gtk.Label()
         lab.set_line_wrap(True)
         lab.set_line_wrap_mode(PWrapMode.WORD_CHAR)
@@ -360,21 +383,23 @@
     _BULLET = u'•'
     _BULLET_ALLDAY = u'✦' # alternatives:❖⍟✪⦿❂♦⧫⏣⎔⌾⌘⌑⎊⎈⁕⧓⚫⚭⚙✷✦
     _BULLET_MULTIDAY_START = u'‣'
     _BULLET_ONGOING = u'»'
     _BULLET_TODO = u'🅣' # alternative:Ⓣ
 
     @classmethod
-    def marker_label(cls, ev:iCal.Event, dt_st:dt_date) -> Gtk.Label:
+    def marker_label(cls, ev:iCal.Event, dt_st:dt_date, is_ongoing:bool=False) -> Gtk.Label:
         # Returns bullet or entry time suitable for marking entries.
         # Used to display entries in Week and Year views.
         lab = Gtk.Label()
         lab.set_halign(Gtk.Align.END)
         lab.set_valign(Gtk.Align.START)
-        if datetime_to_time(dt_st)!=False:
+        if is_ongoing:
+            mark = cls._BULLET_ONGOING
+        elif datetime_to_time(dt_st)!=False:
             mark = format_time(dt_st, True)
         elif type(ev) is iCal.Todo:
             mark = cls._BULLET_TODO
         elif 'DTEND' in ev:
             if dt_lte(ev['DTEND'].dt, ev['DTSTART'].dt+timedelta(days=1)):
                 mark = cls._BULLET_ALLDAY
             else:
```

### Comparing `pygenda-0.2.6/pygenda/pygenda_view_todo.py` & `pygenda-0.2.7/pygenda/pygenda_view_week.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
-# pygenda_view_todo.py
-# Provides the "To-Do View" for Pygenda.
+# pygenda_view_week.py
+# Provides the "Week View" for Pygenda.
 #
 # Copyright (C) 2022,2023 Matthew Lewis
 #
 # This file is part of Pygenda.
 #
 # Pygenda is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -19,501 +19,503 @@
 # You should have received a copy of the GNU General Public License
 # along with Pygenda. If not, see <https://www.gnu.org/licenses/>.
 
 
 from gi import require_version as gi_require_version
 gi_require_version('Gtk', '3.0')
 from gi.repository import Gtk, Gdk, GLib
-from gi.repository.Pango import WrapMode as PWrapMode
 
-from icalendar import cal as iCal, Event as iEvent, Todo as iTodo
+from calendar import day_abbr,month_name
+from datetime import time as dt_time, date as dt_date, datetime as dt_datetime, timedelta
+from icalendar import cal as iCal
 from locale import gettext as _
-from typing import Optional, List, Union
+from typing import Optional
 
 # pygenda components
-from .pygenda_view import View
+from .pygenda_view import View, View_DayUnit_Base
 from .pygenda_calendar import Calendar
 from .pygenda_config import Config
+from .pygenda_util import start_of_week, day_in_week, month_abbr, start_end_dts_occ, dt_lt, dt_lte
 from .pygenda_gui import GUI
-from .pygenda_dialog_todo import TodoDialogController
-from .pygenda_entryinfo import EntryInfo
+from .pygenda_dialog_event import EventDialogController
 
 
-# Singleton class for Todo View
-class View_Todo(View):
-    Config.set_defaults('todo_view',{
-        'list0_title': _('To-do'),
+# Singleton class for Week View
+class View_Week(View_DayUnit_Base):
+    Config.set_defaults('week_view',{
+        'pageleft_datepos': 'left',
+        'pageright_datepos': 'right',
+        'show_ongoing_event': 'first_day',
+        'show_event_location': 'always',
+        'zoom_levels': 5,
+        'default_zoom': 1,
     })
 
-    _cursor_list = 0
-    _cursor_idx_in_list = 0
-    _last_cursor_list = None
-    _last_cursor_idx_in_list = None
-    _list_items = None # type: list
-    _target_listidx = None
-    _target_todo = None
-    _scroll_to_cursor_required = False
-    CURSOR_STYLE = 'todoview_cursor'
+    _day_ent_count = [0]*7 # entry count for each day
+    _day_entries = [[], [], [], [], [], [], []]
+    _week_viewed = None # So view will be fully redrawn when needed
+    _last_cursor = None
+    _scroll_to_cursor_in_day = None
+    _target_entry = None
+    CURSOR_STYLE = 'weekview_cursor'
+
+    SHOW_LOC_ALWAYS = 1 # constant 'enum' for _show_location flag
 
     @staticmethod
     def view_name() -> str:
         # Return (localised) string to use in menu
-        return _('_Todo View')
+        return _('_Week View')
 
     @staticmethod
     def accel_key() -> int:
         # Return (localised) keycode for menu shortcut
-        k = _('todo_view_accel')
+        k = _('week_view_accel')
         return ord(k[0]) if len(k)>0 else 0
 
 
     @classmethod
     def init(cls) -> Gtk.Widget:
         # Called on startup.
         # Gets view framework from glade file & tweaks/adds a few elements.
         # Returns widget containing view.
-        cls._init_parse_list_config()
-        cls._init_todo_widgets()
+        GUI.load_glade_file('view_week.glade')
+        cls._topbox = GUI._builder.get_object('view_week')
+        cls._month_label = GUI._builder.get_object('week_label_month')
+        cls._weekno_label = GUI._builder.get_object('week_label_weekno')
+        cls._init_week_widgets()
         cls._init_keymap()
-        return cls._topboxscroll
+        cls._init_config()
+        cls.init_zoom('week_view', cls._topbox.get_style_context())
+        return cls._topbox
 
 
     @classmethod
-    def _init_parse_list_config(cls) -> None:
-        # Read & parse config settings
-        i = 0
-        cls._list_titles = []
-        cls._list_filters = []
-        cls._list_default_cats = []
-        while True:
-            try:
-                title = Config.get('todo_view','list{}_title'.format(i))
-            except:
-                break
-            try:
-                filt = Config.get('todo_view','list{}_filter'.format(i))
-            except:
-                filt = None
-            cls._list_titles.append(title)
-            cls._list_filters.append(filt)
-            cls._list_default_cats.append(cls._default_cats_from_filter(filt))
-            i += 1
-        cls._list_count = i
-        cls._item_counts = [0]*cls._list_count
-
-
-    @staticmethod
-    def _default_cats_from_filter(filt:Optional[str]) -> Optional[list]:
-        # Return list of categories that will match given filter string.
-        # For now this is quite simple, but in the future it may support
-        # more complex filters (e.g. project1 AND this_week).
-        if not filt or filt=='UNCATEGORIZED':
-            return None
-        return [filt]
-
-
-    @classmethod
-    def _init_todo_widgets(cls) -> None:
-        # Initialise widgets - create list labels, entry spaces etc.
-        # First make the top-level container
-        cls._topboxscroll = Gtk.ScrolledWindow()
-        cls._topboxscroll.set_name('view_todo')
-        cls._topboxscroll.set_policy(Gtk.PolicyType.AUTOMATIC,Gtk.PolicyType.NEVER)
-        cls._topboxscroll.set_overlay_scrolling(False)
-        cls._topboxscroll.set_hexpand(True)
-        list_hbox = Gtk.Box(orientation=Gtk.Orientation.HORIZONTAL)
-        list_hbox.set_homogeneous(True)
-        cls._topboxscroll.add(list_hbox)
-        list_hbox.connect('draw', cls._pre_draw)
-
-        # Now add vertical boxes for each list
-        cls._list_container = []
-        for i in range(cls._list_count):
-            new_list = Gtk.Box(orientation=Gtk.Orientation.VERTICAL)
-            new_list.get_style_context().add_class('todoview_list')
-            new_title = Gtk.Label(cls._list_titles[i])
-            new_title.get_style_context().add_class('todoview_title')
-            new_eventbox_title = Gtk.EventBox()
-            new_eventbox_title.connect('button_press_event', cls.click_title, i)
-            new_eventbox_title.add(new_title)
-            new_list.add(new_eventbox_title)
-            new_list_scroller = Gtk.ScrolledWindow()
-            new_list_scroller.set_policy(Gtk.PolicyType.NEVER, Gtk.PolicyType.AUTOMATIC)
-            new_list_scroller.set_overlay_scrolling(False)
-            new_list_scroller.set_vexpand(True)
-            new_list_scroller.get_style_context().add_class('todoview_listcontent')
-            new_eventbox_list = Gtk.EventBox()
-            new_eventbox_list.connect('button_press_event', cls.click_list, i)
-            new_eventbox_list.add(new_list_scroller)
-            new_list.add(new_eventbox_list)
-            new_list_content = Gtk.Box(orientation=Gtk.Orientation.VERTICAL)
-            new_list_scroller.add(new_list_content)
-            cls._list_container.append(new_list_scroller)
-            list_hbox.add(new_list)
+    def _init_week_widgets(cls) -> None:
+        # Initialise widgets - create day labels, entry spaces etc.
+        # Do this here so it take account of start_week_day setting,
+        # page*_datepos settings, and set CSS styles for each day.
+
+        # Create widgets for day labels & text spaces
+        cls._day_eventbox = []
+        cls._day_label = []
+        cls._day_rows = []
+        cls._day_scroll = []
+        st_wk = Config.get_int('global','start_week_day')
+        dpos_r = Config.get('week_view','pageleft_datepos')=='right'
+        day_ab = ('mon','tue','wed','thu','fri','sat','sun')#don't trans
+        for i in range(7):
+            # create event box & contained box
+            cls._day_eventbox.append(Gtk.EventBox())
+            day_box = Gtk.Box()
+            ctx = day_box.get_style_context()
+            # Add classes for css flexibility
+            ctx.add_class('weekview_day')
+            ctx.add_class('weekview_day{:d}'.format(i))
+            ctx.add_class('weekview_{:s}'.format(day_ab[(i+st_wk)%7]))
+            cls._day_eventbox[i].add(day_box)
+            cls._day_eventbox[i].connect('button_press_event', cls.click_date)
+            # labels
+            cls._day_label.append(Gtk.Label())
+            cls._day_label[i].set_justify(Gtk.Justification.CENTER)
+            cls._day_label[i].set_xalign(0.5)
+            cls._day_label[i].set_yalign(0.5)
+            ctx = cls._day_label[i].get_style_context()
+            ctx.add_class('weekview_labelday')
+            if i==3: # starting rightpage
+                dpos_r = Config.get('week_view','pageright_datepos')=='right'
+            if dpos_r:
+                day_box.pack_end(cls._day_label[i], False, False, 0)
+            else:
+                day_box.pack_start(cls._day_label[i], False, False, 0)
+            # scroller & textview
+            day_scroller = Gtk.ScrolledWindow()
+            cls._day_scroll.append(day_scroller)
+            day_scroller.set_policy(Gtk.PolicyType.NEVER, Gtk.PolicyType.AUTOMATIC)
+            day_scroller.set_overlay_scrolling(False)
+            day_scroller.set_hexpand(True)
+            cls._day_rows.append(Gtk.Box(orientation=Gtk.Orientation.VERTICAL))
+            day_scroller.add(cls._day_rows[i])
+            ctx = cls._day_rows[i].get_style_context()
+            ctx.add_class('weekview_daytext')
+            cls._day_rows[i].connect('draw', cls._pre_datecontent_draw, i)
+            day_box.pack_start(day_scroller, True, True, 0)
+
+        # Attach elements to pages
+        page_l = GUI._builder.get_object('week_page_l')
+        page_r = GUI._builder.get_object('week_page_r')
+        for i in range(3): # Left
+            page_l.pack_start(cls._day_eventbox[i], True, True, 0)
+        for i in range(3,7): # ... and right
+            page_r.pack_start(cls._day_eventbox[i], True, True, 0)
 
 
     @classmethod
     def _init_keymap(cls) -> None:
         # Initialises KEYMAP for class. Called from init() since it needs
         # to be called after class construction, so that functions exist.
         cls._KEYMAP = {
             Gdk.KEY_Up: lambda: cls._cursor_move_up(),
             Gdk.KEY_Down: lambda: cls._cursor_move_dn(),
             Gdk.KEY_Right: lambda: cls._cursor_move_rt(),
             Gdk.KEY_Left: lambda: cls._cursor_move_lt(),
-            Gdk.KEY_Home: lambda: cls._cursor_move_list(0),
-            Gdk.KEY_End: lambda: cls._cursor_move_list(-1),
-            Gdk.KEY_Page_Up: lambda: cls._cursor_move_index(0),
-            Gdk.KEY_Page_Down: lambda: cls._cursor_move_index(-1),
+            Gdk.KEY_space: lambda: cls._cursor_move_today(),
             Gdk.KEY_Return: lambda: cls.cursor_edit_entry(),
         }
 
 
     @classmethod
-    def get_cursor_entry(cls) -> Optional[iTodo]:
-        # Returns entry at cursor position, or None if cursor not on entry.
-        # Called from cursor_edit_entry() & delete_request().
-        if len(cls._list_items[cls._cursor_list]) == 0:
-            return None
-        return cls._list_items[cls._cursor_list][cls._cursor_idx_in_list]
+    def _init_config(cls) -> None:
+        # Initialisation from config settings.
+        # Set _show_ongoing flag from config.
+        show_ongoing = Config.get('week_view','show_ongoing_event')
+        map = {'every_day':1, 'first_day':0}
+        cls._show_ongoing = map[show_ongoing] if show_ongoing in map else 0
+
+        # Set _show_location flag from config.
+        show_loc = Config.get('week_view','show_event_location')
+        map = {'always':cls.SHOW_LOC_ALWAYS, 'never':0}
+        cls._show_location = map[show_loc] if show_loc in map else 0
 
 
     @classmethod
-    def new_entry_from_example(cls, en:Union[iEvent,iTodo]) -> None:
-        # Creates new entry based on entry en. Used for pasting entries.
-        # Type of entry depends on View (e.g. Todo View -> to-do item).
-        cats = cls._list_default_cats[cls._cursor_list]
-        new_en = Calendar.new_entry_from_example(en, e_type=EntryInfo.TYPE_TODO, e_cats=cats)
-        cls.cursor_goto_todo(new_en, cls._cursor_list)
-
+    def _set_label_text(cls) -> None:
+        # Sets date and month label text and style classes.
+        # Called on view redraw.
+        cls._last_cursor = None
+        dt = start_of_week(View._cursor_date)
+        cls._week_viewed = dt
+        dt_end = dt + timedelta(days=6)
+        # Month label
+        if dt.month == dt_end.month:
+            mn = month_name[dt.month].capitalize()
+            ml = u'{mon:s} {yr:d}'.format(mon=mn, yr=dt.year)
+        elif dt.year == dt_end.year:
+            msn = month_abbr[dt.month].capitalize()
+            ml = u'{mon_st:s} – {mon_end:s} {yr:d}'.format(mon_st=msn, mon_end=month_abbr[dt_end.month], yr=dt.year)
+        else: # month & year different
+            msn = month_abbr[dt.month].capitalize()
+            ml = u'{mon_st:s} {yr_st:d} – {mon_end:s} {yr_end:d}'.format(mon_st=msn, mon_end=month_abbr[dt_end.month], yr_st=dt.year, yr_end=dt_end.year)
+        cls._month_label.set_text(ml)
+
+        # Week number label
+        # Week 1 is the first to include 4+ days of year.
+        # E.g. if week starts Monday then Wk1 is first to include a Thursday.
+        wkno = (dt.timetuple().tm_yday+9)//7
+        if wkno==53 and dt.day>=29:
+            wkno_txt = _('Week 53/Week 1')
+        else:
+            wkno_txt = _('Week {}').format(wkno)
+        cls._weekno_label.set_text(wkno_txt)
 
-    @classmethod
-    def paste_text(cls, txt:str) -> None:
-        # Handle pasting of text in Todo view.
-        # Open a New Todo dialog with description initialised as txt,
-        # and to-do list set from current cursor position.
-        GLib.idle_add(lambda x: TodoDialogController.new_todo(txt=x, list_idx=cls.cursor_todo_list()), txt)
+        # Day labels
+        today = dt_date.today()
+        for i in range(7):
+            ctx = cls._day_eventbox[i].get_style_context()
+            if dt<today:
+                ctx.add_class('weekview_pastday')
+            else:
+                ctx.remove_class('weekview_pastday')
+            if dt==today:
+                ctx.add_class('weekview_today')
+            else:
+                ctx.remove_class('weekview_today')
+
+            dn = day_abbr[dt.weekday()]
+            if dn[-1]=='.':
+                dn = dn[:-1] # remove dot
+            cls._day_label[i].set_text(u'{day:s}\n{date:d}'.format(day=dn,date=dt.day))
+            dt += timedelta(days=1)
 
 
     @classmethod
-    def cursor_todo_list(cls) -> int:
-        # Returns index of todo list with cursor.
-        # Used by "new todo" etc to initialise dialog with focused todo list.
-        return cls._cursor_list
+    def _set_entry_text(cls) -> None:
+        # Sets label text and style classes for event-displaying labels.
+        # Called on view redraw.
+        cls._last_cursor = None
+        dt = start_of_week(View._cursor_date)
+        cls._day_entries = [[], [], [], [], [], [], []] # reset stored events
+        cls._day_ent_count = [0]*7
+        sorted_occurrences = Calendar.occurrence_list(dt, dt+timedelta(days=7))
+        itr = iter(sorted_occurrences)
+        try:
+            occ = next(itr)
+        except StopIteration:
+            occ = None
+        if cls._show_ongoing:
+            ongoing = [] # !! Replace with call to calendar
+            rollover_dt = dt # Might want this to be 2am or something
+        oneday = timedelta(days=1)
+        for i in range(7):
+            dt_nxt = dt + oneday
+            # Delete anything previously written to day v-box
+            cls._day_rows[i].foreach(Gtk.Widget.destroy)
+            if cls._show_ongoing:
+                # Add rows for the ongoing events
+                rollover_dt += oneday
+                j = 0
+                while j < len(ongoing):
+                    occo = ongoing[j]
+                    occ_dt_sta,occ_dt_end = start_end_dts_occ(occo)
+                    cls._add_day_entry_row(occo[0], occ_dt_sta, occ_dt_end, i, show_loc=False, is_ongoing=True)
+                    # If this occurrence ends here, remove it from 'ongoing'
+                    if dt_lte(occ_dt_end, rollover_dt):
+                        ongoing.pop(j)
+                    else:
+                        j += 1
+            # Now we add events that start on this day
+            while True:
+                if occ is None:
+                    break
+                occ_dt_sta,occ_dt_end = start_end_dts_occ(occ)
+                if dt_lte(dt_nxt, occ_dt_sta):
+                    # into next day so break this loop
+                    break
+                # First, see if we've hit the cursor target entry
+                if cls._target_entry is not None and cls._target_entry is occ[0] and dt==View._cursor_date:
+                    View._cursor_idx_in_date = cls._day_ent_count[i]
+                    cls._target_entry = None
+                cls._add_day_entry_row(occ[0], occ_dt_sta, occ_dt_end, i, cls._show_location)
+                if cls._show_ongoing:
+                    # Add to 'ongoing' list if occurrence goes into next day
+                    if occ_dt_end and dt_lt(rollover_dt, occ_dt_end):
+                        ongoing.append(occ)
+                try:
+                    occ = next(itr)
+                except StopIteration:
+                    occ = None
+            if cls._day_ent_count[i]==0:
+                # an empty day, need something for cursor
+                mark_label = Gtk.Label()
+                ctx = mark_label.get_style_context()
+                ctx.add_class('weekview_marker')
+                mark_label.set_halign(Gtk.Align.START) # else cursor fills line
+                cls._day_rows[i].add(mark_label)
+            dt = dt_nxt
+            cls._day_rows[i].show_all()
+        cls._target_entry = None # just in case - should be done already
 
 
     @classmethod
-    def cursor_goto_todo(cls, todo:iTodo, list_idx:int) -> bool:
-        # Move cursor to given todo in given list.
-        # Return True to indicate this is possible in this view.
-        # Set targets, but don't move yet, since we want to redraw view
-        # & to use recalculated todo order to determine cursor position.
-        cls._target_listidx = list_idx
-        cls._target_todo = todo
-        return True
+    def _add_day_entry_row(cls, ev:iCal.Event, dt_st:dt_date, dt_end:dt_date, dayidx:int, show_loc:bool, is_ongoing:bool=False) -> None:
+        # Add Gtk labels for event 'ev', occurrence at time/date from 'dt_st'
+        # to 'dt_end', in day 'dayidx' (e.g. 0=Monday if week starts Monday).
+        # Used when displaying week contents.
+        row = Gtk.Box()
+        # Create entry mark (bullet or time) & add to row
+        mark_label = cls.marker_label(ev, dt_st, is_ongoing)
+        ctx = mark_label.get_style_context()
+        ctx.add_class('weekview_marker') # add style for CSS
+        row.add(mark_label)
+        # Create entry content label & add to row
+        cont_label = cls.entry_text_label(ev, dt_st, dt_end, add_location=show_loc)
+        cont_label.set_hexpand(True) # Also sets hexpand_set to True
+        row.add(cont_label)
+        cls._day_rows[dayidx].add(row)
+        cls._day_entries[dayidx].append(ev)
+        cls._day_ent_count[dayidx] += 1
 
 
     @classmethod
-    def redraw(cls, en_changes:bool) -> None:
-        # Called when redraw required
-        # en_changes: bool indicating if displayed entries need updating too
-        if not en_changes:
-            return
-        cls._last_cursor_list = None
-        cls._last_cursor_idx_in_list = None
-        for cont in cls._list_container:
-            cont.get_child().destroy()
-        todos = Calendar.todo_list()
-        cls._list_items = []
-        for i in range(len(cls._list_container)):
-            new_list_content = Gtk.Box(orientation=Gtk.Orientation.VERTICAL)
-            count = 0
-            cls._list_items.append([])
-            for td in todos:
-                if cls._todo_matches_filter(td, cls._list_filters[i]):
-                    if cls._target_todo is not None and cls._target_todo is td:
-                        cls._cursor_list = i
-                        cls._cursor_idx_in_list = count
-                        if i>=cls._target_listidx:
-                            # We've reached the target list, so go no further
-                            cls._target_listidx = None
-                            cls._target_todo = None
-                    row = Gtk.Box()
-                    ctx = row.get_style_context()
-                    ctx.add_class('todoview_item')
-                    # Potential markers: ①-0x245f ➀-0x277f ❶-0x2775 ➊-0x2789
-                    mark_label = Gtk.Label(chr(0x2789+td['PRIORITY']) if 'PRIORITY' in td else u'•')
-                    mark_label.set_halign(Gtk.Align.END)
-                    mark_label.set_valign(Gtk.Align.START)
-                    mark_label.get_style_context().add_class('todoview_marker')
-                    row.add(mark_label)
-                    item_text = Gtk.Label(td['SUMMARY'] if 'SUMMARY' in td else '')
-                    item_text.get_style_context().add_class('todoview_itemtext')
-                    item_text.set_xalign(0)
-                    item_text.set_yalign(0)
-                    item_text.set_line_wrap(True)
-                    item_text.set_line_wrap_mode(PWrapMode.WORD_CHAR)
-                    if 'STATUS' in td and td['STATUS'] in Calendar.STATUS_LIST_TODO:
-                        ctx.add_class(td['STATUS'].lower())
-                    row.add(item_text)
-                    new_list_content.add(row)
-                    cls._list_items[-1].append(td)
-                    count += 1
-            cls._item_counts[i] = count
-            if count==0:
-                # an empty list, need something for cursor
-                mark_label = Gtk.Label()
-                mark_label.set_halign(Gtk.Align.START) # else cursor fills line
-                ctx = mark_label.get_style_context()
-                ctx.add_class('todoview_marker')
-                new_list_content.add(mark_label)
-            new_list_content.get_style_context().add_class('todoview_items')
-            cls._list_container[i].add(new_list_content)
-            cls._list_container[i].show_all()
-        # Reset target (though in theory this should already be done)
-        cls._target_listidx = None
-        cls._target_todo = None
-        cls._show_cursor()
+    def _show_cursor(cls) -> None:
+        # Locates bullet/date corresponding to the current cursor and adds
+        # 'weekview_cursor' class to it so cursor is visible via CSS styling.
+        dy = day_in_week(View._cursor_date)
+        ecount = cls._day_ent_count[dy]
+        i = View._cursor_idx_in_date
+        if i < 0 or i >= ecount:
+            i = max(0,ecount-1)
+            View._cursor_idx_in_date = i
+        cls._hide_cursor()
+        row = cls._day_rows[dy].get_children()[i]
+        if ecount==0:
+            mk = row
+        else:
+            mk = row.get_children()[0]
+        ctx = mk.get_style_context()
+        ctx.add_class(cls.CURSOR_STYLE)
+        cls._last_cursor = int(dy+8*i)
+        if cls._day_ent_count[dy] > 0:
+            # We may need to scroll content to show entry at cursor.
+            cls._day_rows[dy].queue_draw()
+            cls._scroll_to_cursor_in_day = dy # to be read in draw handler
+        else:
+            cls._scroll_to_cursor_in_day = None
+        GUI.set_menu_elts(on_event=(ecount!=0)) # Enable/disable hide menu items
 
 
-    @staticmethod
-    def _todo_matches_filter(td:iTodo, filt:Optional[str]) -> bool:
-        # Return True if categories of to-do item match filter
-        if filt is None:
-            return True
-        cats = View_Todo._get_categories(td)
-        if not cats:
-            return filt=='UNCATEGORIZED'
-        return filt in cats
+    @classmethod
+    def _pre_datecontent_draw(cls, wid:Gtk.Widget, _, day:int) -> bool:
+        # Callback called on 'draw' event on date_content.
+        # Called before drawing date content.
+        # Used to scroll window when cursor has been moved (since we
+        # need to have calculated the layout to know where to scoll to).
+        if cls._scroll_to_cursor_in_day == day:
+            cls.scroll_to_row(cls._day_rows[day], View._cursor_idx_in_date, cls._day_scroll[day])
+            cls._scroll_to_cursor_in_day = None
+        return False # propagate event
 
 
-    @staticmethod
-    def _get_categories(td:iTodo) -> list:
-        # Return list of categories of the given to-do item
-        if 'CATEGORIES' not in td:
-            cats = [] # type: List[str]
-        elif isinstance(td['CATEGORIES'],list):
-            cats = []
-            for clist in td['CATEGORIES']:
-                if isinstance(clist,str):
-                    cats.extend([c for c in clist.split(',') if c])
-                else:
-                    cats.extend([c for c in clist.cats if c])
-        elif isinstance(td['CATEGORIES'],str):
-            cats = [c for c in td['CATEGORIES'].split(',') if c]
-        else:
-            cats = [c for c in td['CATEGORIES'].cats if c]
-        return cats
+    @classmethod
+    def _hide_cursor(cls) -> None:
+        # Clears 'weekview_cursor' style class from cursor position,
+        # so cursor is no longer visible.
+        if cls._last_cursor is not None:
+            # _last_cursor is an int split into two parts:
+            # Lower 3 bits give day, other higher bits give entry within day
+            dy = cls._last_cursor%8
+            row = cls._day_rows[dy].get_children()[cls._last_cursor//8]
+            if cls._day_ent_count[dy]==0:
+                mk = row
+            else:
+                mk = row.get_children()[0]
+            ctx = mk.get_style_context()
+            ctx.remove_class(cls.CURSOR_STYLE)
+            cls._last_cursor = None
 
 
     @classmethod
-    def click_title(cls, wid:Gtk.Widget, ev:Gdk.EventButton, list_idx:int) -> None:
-        # Callback. Called whenever a list title is clicked/tapped.
-        # Moves cursor to top of list/item clicked
-        cls._cursor_move_list(list_idx)
-        cls._cursor_move_index(0)
-        cls._scroll_to_cursor_required = True
+    def cursor_set_date(cls, dt:dt_date, idx:int=0) -> bool:
+        # Set current cursor date & index in date.
+        # Override default method & return True to indicate success.
+        View._cursor_date = dt
+        View._cursor_idx_in_date = idx
+        return True
 
 
     @classmethod
-    def click_list(cls, wid:Gtk.Widget, ev:Gdk.EventButton, list_idx:int) -> None:
-        # Callback. Called whenever list content is clicked/tapped.
-        # Moves cursor to list/item clicked
-        cls._cursor_move_list(list_idx)
-        scroller = cls._list_container[list_idx]
-        vwport = scroller.get_children()[0]
-        row_vbox = vwport.get_children()[0]
-        # Pixels above the first row:
-        ycount = cls._top_spacing(scroller)
-        ycount += cls._top_spacing(vwport)
-        ycount += cls._top_spacing(row_vbox)
-        # Take account of list's vertical scrollbar:
-        ycount -= cls._list_container[list_idx].get_vadjustment().get_value()
-        # Look through rows until cumulative height exceeds click ycoord
-        row_spacing = row_vbox.get_spacing()
-        rows = row_vbox.get_children()
-        ycount -= row_spacing//2 # adjust for no spacing above first row
-        i = 0
-        for r in rows:
-            ycount += r.get_allocated_height()
-            ycount += row_spacing
-            if ycount > ev.y:
-                break
-            i += 1
-        cls._cursor_move_index(i)
-        cls._scroll_to_cursor_required = True
+    def get_cursor_entry(cls) -> iCal.Event:
+        # Returns entry at cursor position, or None if cursor not on entry.
+        # Called from cursor_edit_entry() & delete_request().
+        dy = day_in_week(View._cursor_date)
+        if cls._day_ent_count[dy]==0:
+            return None
+        return cls._day_entries[dy][View._cursor_idx_in_date]
 
 
-    @staticmethod
-    def _top_spacing(wid:Gtk.Widget) -> float:
-        # Return total size of top padding+border+margin of widget
-        ctx = wid.get_style_context()
-        pad = ctx.get_padding(Gtk.StateFlags.NORMAL)
-        bord = ctx.get_border(Gtk.StateFlags.NORMAL)
-        marg = ctx.get_margin(Gtk.StateFlags.NORMAL)
-        return pad.top + bord.top + marg.top
+    @classmethod
+    def renew_display(cls) -> None:
+        # Called when we switch to this view to reset state.
+        cls._week_viewed = None
 
 
     @classmethod
-    def _show_cursor(cls) -> None:
-        # Locates bullet corresponding to the current cursor and adds
-        # 'todoview_cursor' class to it, so cursor is visible via CSS styling.
-
-        # First correct cursor if required (e.g. item was deleted)
-        if not (0 <= cls._cursor_list < cls._list_count):
-            cls._cursor_list = max(0, cls._list_count-1)
-        icount = cls._item_counts[cls._cursor_list]
-        if not (0 <= cls._cursor_idx_in_list < icount):
-            cls._cursor_idx_in_list = max(0, icount-1)
+    def redraw(cls, en_changes:bool) -> None:
+        # Called when redraw required.
+        # en_changes: bool indicating if displayed entries need updating too
+        if cls._week_viewed != start_of_week(View._cursor_date):
+            cls._set_label_text()
+            en_changes = True
+        if en_changes:
+            cls._set_entry_text()
+        cls._show_cursor()
 
-        cls._hide_cursor()
 
-        ctx = cls._get_cursor_ctx(cls._cursor_list, cls._cursor_idx_in_list)
-        if ctx is not None:
-            ctx.add_class(cls.CURSOR_STYLE)
-        cls._last_cursor_list = cls._cursor_list
-        cls._last_cursor_idx_in_list = cls._cursor_idx_in_list
-        # Add scroll call to idle, in case column widths not yet determined
-        cls._scroll_to_cursor_required = True
-        GUI.set_menu_elts(on_todo=(icount!=0)) # Enable/disable hide menu items
+    @classmethod
+    def _cursor_move_up(cls) -> None:
+        # Callback for user moving cursor up.
+        View._cursor_idx_in_date -= 1
+        if View._cursor_idx_in_date < 0:
+            cls.cursor_inc(timedelta(days=-1))
+            # Leave idx_in_date as -1 since that signals last entry
+            View._today_toggle_date = None
+        else:
+            cls._show_cursor()
 
 
     @classmethod
-    def _pre_draw(cls, wid:Gtk.Widget, _) -> None:
-        # Callback called on 'draw' event on date_content.
-        # Called before drawing date content.
-        # Used to scroll window when cursor has been moved (since we
-        # need to have calculated the layout to know where to scoll to).
-        if cls._scroll_to_cursor_required:
-            cls._scroll_to_cursor()
-            cls._scroll_to_cursor_required = False
+    def _cursor_move_dn(cls) -> None:
+        # Callback for user moving cursor down.
+        View._cursor_idx_in_date += 1
+        dy = day_in_week(View._cursor_date)
+        if View._cursor_idx_in_date >= cls._day_ent_count[dy]:
+            cls.cursor_inc(timedelta(days=1), 0)
+            View._today_toggle_date = None
+        else:
+            cls._show_cursor()
 
 
     @classmethod
-    def _hide_cursor(cls) -> None:
-        # Clears 'todoview_cursor' style class from cursor position,
-        # so cursor is no longer visible.
-        if cls._last_cursor_list is not None:
-            ctx = cls._get_cursor_ctx(cls._last_cursor_list, cls._last_cursor_idx_in_list)
-            if ctx is not None:
-                ctx.remove_class(cls.CURSOR_STYLE)
-            cls._last_cursor_list = None
-            cls._last_cursor_idx_in_list = None
+    def _cursor_move_lt(cls) -> None:
+        # Callback for user moving cursor left.
+        i = day_in_week(View._cursor_date)
+        d = -7 if i<3 else (-3 if i==3 else -4)
+        cls.cursor_inc(timedelta(days=d), 0)
+        View._today_toggle_date = None
 
 
     @classmethod
-    def _get_cursor_ctx(cls, c_list:int, c_i_in_list:int) -> Gtk.StyleContext:
-        # Returns a StyleContext object for to-do cursor coordinates
-        # c_list & c_i_in_list
-        lst = cls._list_container[c_list].get_child().get_child()
-        item = lst.get_children()[c_i_in_list]
-        if cls._item_counts[c_list]==0:
-            ci = item
-        else:
-            ci = item.get_children()[0]
-        return ci.get_style_context()
+    def _cursor_move_rt(cls) -> None:
+        # Callback for user moving cursor right.
+        i = day_in_week(View._cursor_date)
+        d = 4 if i<3 else 7
+        cls.cursor_inc(timedelta(days=d), 0)
+        View._today_toggle_date = None
 
 
     @classmethod
-    def _scroll_to_cursor(cls) -> None:
-        # If required, scroll view elements so that cursor is visible.
-        # Note: If view is not yet laid-out, calculation not correct.
-        # Hence this will be called in 'draw' event handler, so layout is done.
-        list_width = cls._list_container[0].get_allocated_width() # homogeneous
-        view_width = cls._topboxscroll.get_allocated_width()
-        maxv = cls._cursor_list*list_width # left edge of list at left of view
-        minv = (cls._cursor_list+1)*list_width-view_width # rt edge @ rt of view
-        adj = cls._topboxscroll.get_hadjustment()
-        cur = adj.get_value()
-        if minv > maxv:
-            minv = maxv # If list is wider than view, then show left edge
-        if cur > maxv:
-            adj.set_value(maxv)
-        elif cur < minv:
-            adj.set_value(minv)
-
-        # Now the vertical scrolling...
-        list_scroller = cls._list_container[cls._cursor_list]
-        list_box = list_scroller.get_child().get_child()
-        list_item_wids = list_box.get_children()
-        maxv = list_box.get_spacing()*cls._cursor_idx_in_list
-        for i in range(cls._cursor_idx_in_list):
-            maxv += list_item_wids[i].get_allocated_height()
-        minv = maxv + list_item_wids[cls._cursor_idx_in_list].get_allocated_height()
-        minv -= list_scroller.get_allocated_height()
-        # Take into account padding/margin etc.
-        ctx = list_box.get_style_context()
-        pad = ctx.get_padding(Gtk.StateFlags.NORMAL)
-        bord = ctx.get_border(Gtk.StateFlags.NORMAL)
-        marg = ctx.get_margin(Gtk.StateFlags.NORMAL)
-        minv += pad.top + bord.top + marg.top + pad.bottom
-        if minv > maxv:
-            minv = maxv # If item is taller than view, then show top
-        adj = list_scroller.get_vadjustment()
-        cur = adj.get_value()
-        if cur > maxv:
-            adj.set_value(maxv)
-        elif cur < minv:
-            adj.set_value(minv)
+    def _cursor_move_today(cls) -> None:
+        # Callback for user toggling cursor between today & another date
+        today = dt_date.today()
+        if View._cursor_date != today:
+            View._today_toggle_date = View._cursor_date
+            View._today_toggle_idx = View._cursor_idx_in_date
+            cls.cursor_set_date(today)
+            cls.redraw(en_changes=False)
+        elif View._today_toggle_date is not None:
+            cls.cursor_set_date(View._today_toggle_date, idx=View._today_toggle_idx)
+            cls.redraw(en_changes=False)
 
 
     @classmethod
     def keypress(cls, wid:Gtk.Widget, ev:Gdk.EventKey) -> None:
-        # Handle key press event in Todo view.
+        # Handle key press event in Week view.
         # Called (from GUI.keypress()) on keypress (or repeat) event
         try:
             f = cls._KEYMAP[ev.keyval]
             GLib.idle_add(f)
         except KeyError:
-            # If it's a character key, take as first of new todo
+            # If it's a character key, take as first of new entry
             # !! Bug: only works for ASCII characters
             if ev.state & (Gdk.ModifierType.CONTROL_MASK|Gdk.ModifierType.MOD1_MASK)==0 and Gdk.KEY_exclam <= ev.keyval <= Gdk.KEY_asciitilde:
-                GLib.idle_add(lambda x: TodoDialogController.new_todo(txt=x, list_idx=cls.cursor_todo_list()), chr(ev.keyval))
+                date = cls.cursor_date()
+                GLib.idle_add(EventDialogController.new_event, chr(ev.keyval), date)
 
 
     @classmethod
-    def _cursor_move_up(cls) -> None:
-        # Callback for user moving cursor up
-        cls._cursor_idx_in_list -= 1 # Cursor correction will fix if <0
-        cls._show_cursor()
+    def click_date(cls, wid:Gtk.Widget, ev:Gdk.EventButton) -> bool:
+        # Callback. Called whenever a date is clicked/tapped.
+        # Moves cursor to date/item clicked
+        try:
+            new_day = cls._day_eventbox.index(wid)
+        except ValueError:
+            return False # propagate event
 
-    @classmethod
-    def _cursor_move_dn(cls) -> None:
-        # Callback for user moving cursor down
-        if cls._item_counts[cls._cursor_list] > 0:
-            cls._cursor_idx_in_list = (cls._cursor_idx_in_list+1)%cls._item_counts[cls._cursor_list]
-            cls._show_cursor()
+        new_idx = 0 # default index if not going to specific entry
 
-    @classmethod
-    def _cursor_move_rt(cls) -> None:
-        # Callback for user moving cursor right
-        cls._cursor_list = (cls._cursor_list+1)%cls._list_count
-        cls._show_cursor()
+        # Has user clicked on a specific entry within day?
+        # If so, move the cursor to that entry.
+        if cls._day_ent_count[new_day] > 1: # Only check if >1 entry in the day
+            # Check if clicked in day's label area
+            d_wids = wid.get_child().get_children()
+            ll = isinstance(d_wids[0],Gtk.Label) # True if left label
+            if ll != (ev.x < d_wids[0].get_allocated_width()): # Clicked entries
+                # We're not clicking in date label area, use y to calc entry
+                new_idx = cls.y_to_day_row(cls._day_rows[new_day], ev.y, cls._day_ent_count[new_day], cls._day_scroll[new_day])
 
-    @classmethod
-    def _cursor_move_lt(cls) -> None:
-        # Callback for user moving cursor left
-        cls._cursor_list -= 1 # Cursor correction will fix if <0
-        cls._show_cursor()
+        GLib.idle_add(cls._jump_to_date, cls._day_index_to_date(new_day), new_idx)
+        return True # event handled - don't propagate
 
-    @classmethod
-    def _cursor_move_list(cls, lst:int) -> None:
-        # Callback for user moving cursor to list
-        cls._cursor_list = lst
-        cls._show_cursor()
 
     @classmethod
-    def _cursor_move_index(cls, idx:int) -> None:
-        # Callback for user moving cursor to idx in current list
-        cls._cursor_idx_in_list = idx
-        cls._show_cursor()
+    def _jump_to_date(cls, dt:dt_date, idx:int) -> None:
+        # Idle callback to move cursor to given date, e.g. on click
+        cls.cursor_set_date(dt, idx=idx)
+        cls.redraw(en_changes=False)
+
 
     @classmethod
-    def cursor_edit_entry(cls) -> None:
-        # Opens a todo edit dialog for the entry at the cursor,
-        # or to create a new todo if the cursor is not on entry.
-        # Assigned to the 'Enter' key.
-        en = cls.get_cursor_entry()
-        if en is None:
-            TodoDialogController.new_todo(list_idx=cls.cursor_todo_list())
-        else:
-            TodoDialogController.edit_todo(en, list_idx=cls.cursor_todo_list())
+    def _day_index_to_date(cls, idx:int) -> Optional[dt_date]:
+        # Given an day index idx=0...6 of day cell in the visible Week View,
+        # return the corresponding date
+        if cls._week_viewed is None:
+            return None
+        return cls._week_viewed+timedelta(days=idx)
```

### Comparing `pygenda-0.2.6/pygenda/pygenda_view_year.py` & `pygenda-0.2.7/pygenda/pygenda_view_year.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 from .pygenda_util import start_end_dts_occ
 
 
 # Singleton class for Year View
 class View_Year(View_DayUnit_Base):
     Config.set_defaults('year_view',{
         'show_event_location': 'always',
+        'zoom_levels': 5,
+        'default_zoom': 2,
     })
 
     DAY_CLASS = [ 'yearview_day_{}'.format(s) for s in ['mon','tue','wed','thu','fri','sat','sun'] ]
     GRID_COLUMNS = 37
     GRID_ROWS = 12 # One per month
     GRID_CURSOR_STYLE = 'yearview_cursor'
     ENTRY_CURSOR_STYLE = 'yearview_entry_cursor'
@@ -80,22 +82,28 @@
         # Returns widget containing view.
         GUI.load_glade_file('view_year.glade')
         cls._topbox = GUI._builder.get_object('view_year')
         cls._grid_cells = GUI._builder.get_object('year_grid_days')
         cls._date_label = GUI._builder.get_object('year_datelabel')
         cls._date_content_scroll = GUI._builder.get_object('year_datecontent_scroll')
         cls._date_content = GUI._builder.get_object('year_datecontent')
-        cls._date_content.connect('draw', cls._pre_datecontent_draw)
         cls._draw_day_month_labels()
         cls._init_keymap()
         cls._init_grid()
         cls._init_config()
+        cls.init_zoom('year_view', cls._topbox.get_style_context())
+
+        # Connect signal handlers
+        HANDLERS = {
+            'year_grid_click': cls.click_grid,
+            'year_dtcont_click': cls.click_events,
+            'year_dtcont_draw': cls._pre_datecontent_draw,
+            }
+        GUI._builder.connect_signals(HANDLERS)
 
-        GUI._builder.get_object('year_grid_events').connect('button_press_event', cls.click_grid)
-        GUI._builder.get_object('year_datecontent_events').connect('button_press_event', cls.click_events)
         return cls._topbox
 
 
     @classmethod
     def _draw_day_month_labels(cls) -> None:
         # Adds text to grid day and month labels.
         # Called only at initialisation.
@@ -166,15 +174,15 @@
         # Draws year - adds formatting classes to cells, labels to some dates.
         # Called on redraw if year has changed.
         # Function a bit disorganised, tidying might be beneficial...
         c_date = View._cursor_date
         yr = c_date.year
         cls._year_viewed = yr
         l = GUI._builder.get_object('year_yearlabel')
-        l.set_text('{:d}'.format(yr))
+        l.set_text(str(yr))
 
         st_wk = Config.get_int('global','start_week_day')
         mon_labs = GUI._builder.get_object('month_names').get_children()
         day_labs = GUI._builder.get_object('day_names').get_children()
         date = dt_date(year=yr,month=1,day=1)
         oneday = timedelta(days=1)
         today = dt_date.today()
@@ -212,15 +220,15 @@
             for d in range(daycount):
                 # Potential optimisations here? Central columns are always in
                 # year, so no need to remove&re-add class yearview_daycell etc.
                 # Also if not start of week, will never be start of week,
                 # so we know label text is already ''.
                 t = ''
                 if day==st_wk or d==0 or d==daycount-1:
-                    t = '{:d}'.format(d+1)
+                    t = str(d+1)
                 l = cls._grid_cells.get_child_at(col,m-1)
                 l.set_text(t)
                 ctx = l.get_style_context()
                 cls.remove_all_classes(ctx)
                 ctx.add_class('yearview_daycell')
                 ctx.add_class(cls.DAY_CLASS[day])
                 if date<today:
@@ -333,22 +341,23 @@
         ctx.add_class(cls.ENTRY_CURSOR_STYLE)
         cls._last_entry_cursor = i
         cls._scroll_to_cursor_required = True # to be read in draw handler
         GUI.set_menu_elts(on_event=True) # Enable menu items
 
 
     @classmethod
-    def _pre_datecontent_draw(cls, wid:Gtk.Widget, _) -> None:
+    def _pre_datecontent_draw(cls, wid:Gtk.Widget, _) -> bool:
         # Callback called on 'draw' event on date_content.
         # Called before drawing date content.
         # Used to scroll window when cursor has been moved (since we
         # need to have calculated the layout to know where to scoll to).
         if cls._scroll_to_cursor_required:
             cls.scroll_to_row(cls._date_content, View._cursor_idx_in_date, cls._date_content_scroll)
             cls._scroll_to_cursor_required = False
+        return False # propagate event
 
 
     @classmethod
     def _hide_entry_cursor(cls) -> None:
         # Remove style from entry cursor (= cursor in lower section of view)
         if cls._last_entry_cursor is not None:
             mk = cls._date_content.get_children()[cls._last_entry_cursor].get_children()[0]
@@ -586,32 +595,34 @@
             pass
         if ev.state & (Gdk.ModifierType.CONTROL_MASK|Gdk.ModifierType.MOD1_MASK)==0 and Gdk.KEY_exclam <= ev.keyval <= Gdk.KEY_asciitilde:
             date = cls.cursor_date()
             GLib.idle_add(EventDialogController.new_event, chr(ev.keyval), date, priority=GLib.PRIORITY_HIGH_IDLE+30)
 
 
     @classmethod
-    def click_grid(cls, wid:Gtk.Widget, ev:Gdk.EventButton) -> None:
+    def click_grid(cls, wid:Gtk.Widget, ev:Gdk.EventButton) -> bool:
         # Callback. Called whenever day grid is clicked/tapped.
         # Move grid (main) cursor to cell that was clicked.
         x = int(cls.GRID_COLUMNS*ev.x/wid.get_allocated_width())
         y = int(cls.GRID_ROWS*ev.y/wid.get_allocated_height())
         dt = cls._cell_to_date_clamped(x, y, cls._year_viewed)
         GLib.idle_add(cls._jump_to_date, dt, priority=GLib.PRIORITY_HIGH_IDLE+30)
+        return True # event handled - don't propagate
 
 
     @classmethod
-    def click_events(cls, wid:Gtk.Widget, ev:Gdk.EventButton) -> None:
+    def click_events(cls, wid:Gtk.Widget, ev:Gdk.EventButton) -> bool:
         # Callback. Called whenever events area at bottom is clicked/tapped.
         # Move entry cursor to entry that was clicked
         new_idx = cls.y_to_day_row(cls._date_content, ev.y, cls._date_content_count, cls._date_content_scroll)
         if View._cursor_idx_in_date != new_idx:
             View._cursor_idx_in_date = new_idx
             cls._hide_entry_cursor()
             cls._show_entry_cursor()
+        return True # event handled - don't propagate
 
 
     @classmethod
     def _jump_to_date(cls, dt:dt_date) -> None:
         # Idle callback to move grid cursor to given date, e.g. on click
         cls.cursor_set_date(dt, reset_target_col=True)
         cls.redraw(en_changes=False)
```

### Comparing `pygenda-0.2.6/pygenda/pygenda_widgets.py` & `pygenda-0.2.7/pygenda/pygenda_widgets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 #
 # pygenda_widgets.py
 # Date, Time and Duration entry widgets for Pygenda.
 #
-# Copyright (C) 2022 Matthew Lewis
+# Copyright (C) 2022,2023 Matthew Lewis
 #
 # This file is part of Pygenda.
 #
 # Pygenda is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, version 3.
 #
@@ -92,26 +92,28 @@
         for i in range(len(self._elts)):
             self._elts[i].connect('key-press-event', self._key_event, i)
             self._elts[i].connect('changed', self._changed)
             self._elts[i].connect('focus-out-event', self._focus_out)
             self._elts[i].connect('focus-in-event', self._focus_in)
 
 
-    def _focus_in(self, entry:Gtk.Widget, ev:Gdk.EventFocus) -> None:
+    def _focus_in(self, entry:Gtk.Widget, ev:Gdk.EventFocus) -> bool:
         # Event callback for when any sub-field gets the focus
         # This and the next function allow us to style whole widget with .focus
         # We update counter to avoid unnecessary remove/add styles
         if self._focus_count==0:
             self.get_style_context().add_class(self.FOCUS_STYLE)
         self._focus_count += 1
+        return False # propagate event
 
-    def _focus_out(self, entry:Gtk.Widget, ev:Gdk.EventFocus) -> None:
+    def _focus_out(self, entry:Gtk.Widget, ev:Gdk.EventFocus) -> bool:
         # Event callback for when any sub-field looses the focus
         # Do the work in idle so in leave/enter pairs, leave happens last
         GLib.idle_add(_WidgetDateTimeBase._do_focus_out, self)
+        return False # propagate event
 
     def _do_focus_out(self) -> None:
         # Idle event callback for when any sub-field loses focus
         self._focus_count -= 1
         if self._focus_count==0:
             self.get_style_context().remove_class(self.FOCUS_STYLE)
 
@@ -186,40 +188,42 @@
         except ValueError:
             pass
 
         # Type a digit
         if ev.keyval>=Gdk.KEY_0 and ev.keyval<=Gdk.KEY_9:
             if at_end and one_from_max and idx+1<len(self._elts):
                 # In this case, handle insert and move to next field here
-                entry.insert_text('{:d}'.format(ev.keyval-Gdk.KEY_0),-1)
+                entry.insert_text(str(ev.keyval-Gdk.KEY_0),-1)
                 self._elts[idx+1].grab_focus()
                 return True
             # Otherwise number keys can safely be handled by standard code
             return False
         # Return False to allow key to be handled if it's in "safe" list
         return ev.keyval not in (self.ALLOWED_KEYS_WITH_CTRL if ev.state==Gdk.ModifierType.CONTROL_MASK else self.ALLOWED_KEYS)
 
 
-    def _changed(self, entry:Gtk.Widget) -> None:
+    def _changed(self, entry:Gtk.Widget) -> bool:
         # If one subcomponent changes, cascade 'changed' signal down
         self.emit('changed')
+        return False # propagate event
 
 
     @staticmethod
-    def validate_entry(entry:Gtk.Entry, ev:Gdk.EventFocus, mn:int, mx:int, pad:int) -> None:
+    def validate_entry(entry:Gtk.Entry, ev:Gdk.EventFocus, mn:int, mx:int, pad:int) -> bool:
         # Helper function to validate (and correct) date/time fields.
         # Used as callback function when focus leaves the field.
         entry.select_region(0,0) # remove highlight
         try:
             v = int(entry.get_text())
             v = max(mn,v)
             v = min(mx,v)
         except ValueError:
             v = mn
         entry.set_text('{{:0{:d}d}}'.format(pad).format(v))
+        return False # propagate event - in case it's used elsewhere
 
 
     def grab_focus(self) -> None:
         # Provide implementation of widget class's grab_focus()
         self._elts[0].grab_focus()
 
 
@@ -483,15 +487,15 @@
         else: # 12hr
             h = tm.hour
             self.field_ampm.set_active_id('a' if h<12 else 'p')
             if h==0:
                 h = 12
             elif h>12:
                 h -= 12
-            self.field_hour.set_text('{:d}'.format(h))
+            self.field_hour.set_text(str(h))
         self.field_min.set_text('{:02d}'.format(tm.minute))
 
 
     def get_time(self) -> dt_time:
         # Get widget contents. Raises ValueError if time invalid.
         h = int(self.field_hour.get_text())
         if not self.is24:
@@ -548,25 +552,25 @@
         self._init_navigation() # So we can navigate among elements
 
 
     def set_duration(self, timed:timedelta) -> None:
         # Set widget contents.
         tot_min = int(timed.total_seconds()//60)
         hr,mn = divmod(tot_min,60)
-        self.field_hour.set_text('{:d}'.format(hr))
+        self.field_hour.set_text(str(hr))
         self.field_min.set_text('{:02d}'.format(mn))
 
 
     def get_duration(self) -> timedelta:
         # Get widget contents. Raises ValueError if duration invalid.
-        h = int(self.field_hour.get_text())
-        m = int(self.field_min.get_text())
-        if not (0<=m<60) or h<0:
+        hr = int(self.field_hour.get_text())
+        mn = int(self.field_min.get_text())
+        if not (0<=mn<60) or hr<0:
             raise(ValueError)
-        td = timedelta(hours=h, minutes=m)
+        td = timedelta(hours=hr, minutes=mn)
         return td
 
 
     def get_duration_or_none(self) -> Optional[timedelta]:
         # Get widget contents. Returns None if duration invalid.
         try:
             return self.get_duration()
```

### Comparing `pygenda-0.2.6/pygenda.egg-info/PKG-INFO` & `pygenda-0.2.7/pygenda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pygenda
-Version: 0.2.6
+Version: 0.2.7
 Summary: An agenda application inspired by Agenda programs on Psion PDAs.
 Home-page: https://github.com/semiprime/pygenda
 Author: Matthew Lewis
 Author-email: pygenda@semiprime.com
 License: GPLv3 only
 Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Handhelds/PDA's
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Office/Business :: Scheduling
 Requires-Python: >=3.5
```

### Comparing `pygenda-0.2.6/pygenda.egg-info/SOURCES.txt` & `pygenda-0.2.7/pygenda.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 docs/config-examples/README.md
 docs/config-examples/backgrounds.css
 docs/config-examples/darkmode.css
 docs/config-examples/defaults.ini
 docs/config-examples/gemini.css
 docs/config-examples/gemini.ini
 docs/config-examples/pygenda.desktop
+docs/screenshots/todo_view.png
+docs/screenshots/week_view.png
+docs/screenshots/year_view.png
 pygenda/__main__.py
 pygenda/mypy.ini
 pygenda/pygenda_calendar.py
 pygenda/pygenda_config.py
 pygenda/pygenda_dialog_entryprops.py
 pygenda/pygenda_dialog_event.py
 pygenda/pygenda_dialog_find.py
```

### Comparing `pygenda-0.2.6/setup.py` & `pygenda-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     install_requires = [
         "PyGObject",
         "python-dateutil",
         "icalendar",
         "tzlocal",
     ],
     classifiers = [
-        "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 3 - Alpha",
         "Environment :: Handhelds/PDA's",
         "Environment :: X11 Applications :: GTK",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Topic :: Office/Business :: Scheduling",
     ],
```

### Comparing `pygenda-0.2.6/test/maketest_example.py` & `pygenda-0.2.7/test/maketest_example.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/test/maketest_large.py` & `pygenda-0.2.7/test/maketest_large.py`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/test/test01_small.ics` & `pygenda-0.2.7/test/test01_small.ics`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/test/test02_repeats.ics` & `pygenda-0.2.7/test/test02_repeats.ics`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/test/test03_errors.ics` & `pygenda-0.2.7/test/test03_errors.ics`

 * *Files identical despite different names*

### Comparing `pygenda-0.2.6/test/test_repeats.py` & `pygenda-0.2.7/test/test_repeats.py`

 * *Files identical despite different names*

