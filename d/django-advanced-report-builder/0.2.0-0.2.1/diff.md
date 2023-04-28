# Comparing `tmp/django-advanced-report-builder-0.2.0.tar.gz` & `tmp/django-advanced-report-builder-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-advanced-report-builder-0.2.0.tar", last modified: Wed Apr 26 11:22:43 2023, max compression
+gzip compressed data, was "django-advanced-report-builder-0.2.1.tar", last modified: Fri Apr 28 16:06:48 2023, max compression
```

## Comparing `django-advanced-report-builder-0.2.0.tar` & `django-advanced-report-builder-0.2.1.tar`

### file list

```diff
@@ -1,199 +1,200 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.782446 django-advanced-report-builder-0.2.0/
--rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)       91 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/MANIFEST.in
--rw-r--r--   0 tom        (501) staff       (20)      683 2023-04-26 11:22:43.782196 django-advanced-report-builder-0.2.0/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      171 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.706790 django-advanced-report-builder-0.2.0/advanced_report_builder/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     4012 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/admin.py
--rw-r--r--   0 tom        (501) staff       (20)      218 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/apps.py
--rw-r--r--   0 tom        (501) staff       (20)     3394 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/columns.py
--rw-r--r--   0 tom        (501) staff       (20)       40 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/customise.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.709371 django-advanced-report-builder-0.2.0/advanced_report_builder/data_merge/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/data_merge/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3830 2023-03-06 12:34:46.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/data_merge/utils.py
--rw-r--r--   0 tom        (501) staff       (20)      951 2023-03-29 16:03:43.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/data_merge/widget.py
--rw-r--r--   0 tom        (501) staff       (20)     5477 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/duplicate.py
--rw-r--r--   0 tom        (501) staff       (20)      192 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/exceptions.py
--rw-r--r--   0 tom        (501) staff       (20)    10853 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/field_types.py
--rw-r--r--   0 tom        (501) staff       (20)    13799 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/filter_query.py
--rw-r--r--   0 tom        (501) staff       (20)     7914 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/globals.py
--rw-r--r--   0 tom        (501) staff       (20)     1308 2023-04-17 09:39:11.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/includes.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.713752 django-advanced-report-builder-0.2.0/advanced_report_builder/migrations/
--rw-r--r--   0 tom        (501) staff       (20)    14109 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/migrations/0001_initial.py
--rw-r--r--   0 tom        (501) staff       (20)      591 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/migrations/0002_auto_20220209_1657.py
--rw-r--r--   0 tom        (501) staff       (20)     1734 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/migrations/0003_auto_20220215_1219.py
--rw-r--r--   0 tom        (501) staff       (20)      955 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/migrations/0004_customreport.py
--rw-r--r--   0 tom        (501) staff       (20)     3623 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/migrations/0005_auto_20220303_0958.py
--rw-r--r--   0 tom        (501) staff       (20)      914 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/migrations/0006_auto_20220310_1147.py
--rw-r--r--   0 tom        (501) staff       (20)      607 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/migrations/0007_auto_20220322_1939.py
--rw-r--r--   0 tom        (501) staff       (20)      827 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/migrations/0008_auto_20220404_1144.py
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/migrations/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    18911 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/models.py
--rw-r--r--   0 tom        (501) staff       (20)      532 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/report_builder.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.681946 django-advanced-report-builder-0.2.0/advanced_report_builder/static/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.684007 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.682137 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/chart-js/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.719641 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/
--rw-r--r--   0 tom        (501) staff       (20)   334540 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.esm.js
--rw-r--r--   0 tom        (501) staff       (20)   405847 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.js
--rw-r--r--   0 tom        (501) staff       (20)   193925 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.min.js
--rw-r--r--   0 tom        (501) staff       (20)     1430 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-adapter-moment.min.js
--rw-r--r--   0 tom        (501) staff       (20)    12893 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-plugin-datalabels.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.720137 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/
--rw-r--r--   0 tom        (501) staff       (20)    72125 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/helpers.segment.js
--rw-r--r--   0 tom        (501) staff       (20)     2352 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/helpers.esm.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.682691 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/d3/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.729384 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/d3/js/
--rw-r--r--   0 tom        (501) staff       (20)   575002 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/d3/js/d3.js
--rw-r--r--   0 tom        (501) staff       (20)   275533 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/d3/js/d3.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.682479 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.721505 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/
--rw-r--r--   0 tom        (501) staff       (20)   205600 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.js
--rw-r--r--   0 tom        (501) staff       (20)    58945 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.682906 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dashboard/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.730776 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dashboard/js/
--rw-r--r--   0 tom        (501) staff       (20)      563 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dashboard/js/dashboard.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.683132 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dot/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.736366 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dot/js/
--rwxr-xr-x   0 tom        (501) staff       (20)      578 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dot/js/.gitignore
--rwxr-xr-x   0 tom        (501) staff       (20)      122 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dot/js/.travis.yml
--rwxr-xr-x   0 tom        (501) staff       (20)     1176 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dot/js/LICENSE-DOT.txt
--rwxr-xr-x   0 tom        (501) staff       (20)     3291 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dot/js/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.737092 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dot/js/bin/
--rwxr-xr-x   0 tom        (501) staff       (20)     1442 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dot/js/bin/dot-packer
--rwxr-xr-x   0 tom        (501) staff       (20)      443 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dot/js/bower.json
--rwxr-xr-x   0 tom        (501) staff       (20)     5175 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dot/js/doT.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3374 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dot/js/doT.min.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1758 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dot/js/doU.js
--rwxr-xr-x   0 tom        (501) staff       (20)     5190 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dot/js/index.js
--rwxr-xr-x   0 tom        (501) staff       (20)      920 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dot/js/package.json
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.683822 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.737876 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/
--rwxr-xr-x   0 tom        (501) staff       (20)     4390 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1324 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.685141 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.739634 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/
--rwxr-xr-x   0 tom        (501) staff       (20)     3765 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.css
--rwxr-xr-x   0 tom        (501) staff       (20)     3253 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.min.css
--rwxr-xr-x   0 tom        (501) staff       (20)     3756 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.css
--rwxr-xr-x   0 tom        (501) staff       (20)     3248 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.min.css
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.748418 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/
--rwxr-xr-x   0 tom        (501) staff       (20)     2962 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ar.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2540 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.az.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3082 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.bg.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2494 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.cs.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1431 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.da.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2309 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.de.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3273 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.el.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2672 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.en.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2662 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.es.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3216 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fa-IR.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2917 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fr.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2952 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.he.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2522 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.it.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2299 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.nl.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1412 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.no.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2645 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pl.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2787 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-BR.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2451 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-PT.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1310 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ro.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2955 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ru.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2627 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.sq.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2782 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.tr.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3062 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ua.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2503 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.zh-CN.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.751058 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.684958 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.751573 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/
--rwxr-xr-x   0 tom        (501) staff       (20)     1212 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/plugin.js
--rwxr-xr-x   0 tom        (501) staff       (20)   191499 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.js
--rwxr-xr-x   0 tom        (501) staff       (20)    72607 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.min.js
--rwxr-xr-x   0 tom        (501) staff       (20)   201158 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.js
--rwxr-xr-x   0 tom        (501) staff       (20)    77072 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.752264 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/
--rwxr-xr-x   0 tom        (501) staff       (20)      442 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/dark.scss
--rwxr-xr-x   0 tom        (501) staff       (20)     3887 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/default.scss
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.756299 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/
--rwxr-xr-x   0 tom        (501) staff       (20)      266 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_bt-checkbox.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      194 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_bt-tooltip-errors.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      616 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_filter-description.scss
--rwxr-xr-x   0 tom        (501) staff       (20)       83 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_invert.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      469 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_sortable.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      194 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/bt-tooltip-errors.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      616 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/filter-description.scss
--rwxr-xr-x   0 tom        (501) staff       (20)       83 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/invert.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      465 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/sortable.scss
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.685698 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.757694 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.759345 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/charts/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.759760 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/charts/bar/
--rw-r--r--   0 tom        (501) staff       (20)     4581 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/charts/bar/middle.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.761076 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/charts/funnel/
--rw-r--r--   0 tom        (501) staff       (20)     1362 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/charts/funnel/middle.html
--rw-r--r--   0 tom        (501) staff       (20)     1007 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/charts/funnel/report.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.761593 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/charts/line/
--rw-r--r--   0 tom        (501) staff       (20)     4020 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/charts/line/middle.html
--rw-r--r--   0 tom        (501) staff       (20)      486 2023-04-26 11:14:19.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/charts/modal.html
--rw-r--r--   0 tom        (501) staff       (20)      273 2023-04-26 11:15:43.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/charts/modal_field.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.762083 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/charts/pie/
--rw-r--r--   0 tom        (501) staff       (20)     2084 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/charts/pie/middle.html
--rw-r--r--   0 tom        (501) staff       (20)      858 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/charts/report.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.762349 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/data_merge/
--rw-r--r--   0 tom        (501) staff       (20)     2975 2023-03-29 15:59:37.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/data_merge/data_merge.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.763777 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/datatables/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.764255 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/datatables/fields/
--rw-r--r--   0 tom        (501) staff       (20)      254 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/datatables/fields/modal.html
--rw-r--r--   0 tom        (501) staff       (20)     3320 2023-04-26 11:10:44.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/datatables/fields/single_query_builder.html
--rw-r--r--   0 tom        (501) staff       (20)      377 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/datatables/modal.html
--rw-r--r--   0 tom        (501) staff       (20)      593 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/datatables/onclick_menu.html
--rw-r--r--   0 tom        (501) staff       (20)      256 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/datatables/query_modal.html
--rw-r--r--   0 tom        (501) staff       (20)     1127 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/datatables/report.html
--rw-r--r--   0 tom        (501) staff       (20)     8185 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/datatables/select_pivot.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.765629 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/kanban/
--rw-r--r--   0 tom        (501) staff       (20)      499 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/kanban/description_modal.html
--rw-r--r--   0 tom        (501) staff       (20)     2038 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/kanban/middle.html
--rw-r--r--   0 tom        (501) staff       (20)      308 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/kanban/modal.html
--rw-r--r--   0 tom        (501) staff       (20)     1961 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/kanban/report.html
--rw-r--r--   0 tom        (501) staff       (20)     3468 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/query_builder.html
--rw-r--r--   0 tom        (501) staff       (20)     9491 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/select_column.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.766546 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/single_values/
--rw-r--r--   0 tom        (501) staff       (20)     1896 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/single_values/middle.html
--rw-r--r--   0 tom        (501) staff       (20)      623 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/single_values/modal.html
--rw-r--r--   0 tom        (501) staff       (20)     1643 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/single_values/report.html
--rw-r--r--   0 tom        (501) staff       (20)      327 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/toggle.py
--rw-r--r--   0 tom        (501) staff       (20)     3830 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/urls.py
--rw-r--r--   0 tom        (501) staff       (20)     4447 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/utils.py
--rw-r--r--   0 tom        (501) staff       (20)    12521 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/variable_date.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.777693 django-advanced-report-builder-0.2.0/advanced_report_builder/views/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/views/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    11547 2023-04-26 11:15:43.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/views/bar_charts.py
--rw-r--r--   0 tom        (501) staff       (20)    16346 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/views/charts_base.py
--rw-r--r--   0 tom        (501) staff       (20)     3020 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/views/custom.py
--rw-r--r--   0 tom        (501) staff       (20)     8659 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/views/dashboard.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.779398 django-advanced-report-builder-0.2.0/advanced_report_builder/views/datatables/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/views/datatables/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     6801 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/views/datatables/datatables.py
--rw-r--r--   0 tom        (501) staff       (20)    25412 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/views/datatables/modal.py
--rw-r--r--   0 tom        (501) staff       (20)    11394 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/views/datatables/utils.py
--rw-r--r--   0 tom        (501) staff       (20)     8731 2023-04-26 11:15:43.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/views/funnel_charts.py
--rw-r--r--   0 tom        (501) staff       (20)    32161 2023-03-29 16:04:49.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/views/kanban.py
--rw-r--r--   0 tom        (501) staff       (20)    12985 2023-04-26 11:15:43.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/views/line_charts.py
--rw-r--r--   0 tom        (501) staff       (20)    21031 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/views/modals_base.py
--rw-r--r--   0 tom        (501) staff       (20)     8692 2023-04-26 11:15:43.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/views/pie_charts.py
--rw-r--r--   0 tom        (501) staff       (20)      443 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/views/report.py
--rw-r--r--   0 tom        (501) staff       (20)     7812 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/views/report_utils_mixin.py
--rw-r--r--   0 tom        (501) staff       (20)     4750 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/views/reports.py
--rw-r--r--   0 tom        (501) staff       (20)    20469 2023-04-26 10:44:11.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/views/single_values.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.780337 django-advanced-report-builder-0.2.0/advanced_report_builder/views/targets/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/views/targets/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3021 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/views/targets/utils.py
--rw-r--r--   0 tom        (501) staff       (20)      898 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.0/advanced_report_builder/views/targets/views.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-26 11:22:43.781860 django-advanced-report-builder-0.2.0/django_advanced_report_builder.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)      683 2023-04-26 11:22:43.000000 django-advanced-report-builder-0.2.0/django_advanced_report_builder.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)    10834 2023-04-26 11:22:43.000000 django-advanced-report-builder-0.2.0/django_advanced_report_builder.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-04-26 11:22:43.000000 django-advanced-report-builder-0.2.0/django_advanced_report_builder.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)      149 2023-04-26 11:22:43.000000 django-advanced-report-builder-0.2.0/django_advanced_report_builder.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)       24 2023-04-26 11:22:43.000000 django-advanced-report-builder-0.2.0/django_advanced_report_builder.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-04-26 11:22:43.782529 django-advanced-report-builder-0.2.0/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)      974 2023-04-26 11:17:19.000000 django-advanced-report-builder-0.2.0/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.275588 django-advanced-report-builder-0.2.1/
+-rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)       91 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)      683 2023-04-28 16:06:48.275385 django-advanced-report-builder-0.2.1/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      171 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.167868 django-advanced-report-builder-0.2.1/advanced_report_builder/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     4012 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/admin.py
+-rw-r--r--   0 tom        (501) staff       (20)      218 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/apps.py
+-rw-r--r--   0 tom        (501) staff       (20)     3394 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/columns.py
+-rw-r--r--   0 tom        (501) staff       (20)       40 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/customise.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.169879 django-advanced-report-builder-0.2.1/advanced_report_builder/data_merge/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/data_merge/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3830 2023-03-06 12:34:46.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/data_merge/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)      951 2023-03-29 16:03:43.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/data_merge/widget.py
+-rw-r--r--   0 tom        (501) staff       (20)     5477 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/duplicate.py
+-rw-r--r--   0 tom        (501) staff       (20)      192 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/exceptions.py
+-rw-r--r--   0 tom        (501) staff       (20)    10853 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/field_types.py
+-rw-r--r--   0 tom        (501) staff       (20)    13799 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/filter_query.py
+-rw-r--r--   0 tom        (501) staff       (20)     8022 2023-04-28 15:54:22.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/globals.py
+-rw-r--r--   0 tom        (501) staff       (20)     1308 2023-04-17 09:39:11.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/includes.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.186137 django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/
+-rw-r--r--   0 tom        (501) staff       (20)    14109 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0001_initial.py
+-rw-r--r--   0 tom        (501) staff       (20)      591 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0002_auto_20220209_1657.py
+-rw-r--r--   0 tom        (501) staff       (20)     1734 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0003_auto_20220215_1219.py
+-rw-r--r--   0 tom        (501) staff       (20)      955 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0004_customreport.py
+-rw-r--r--   0 tom        (501) staff       (20)     3623 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0005_auto_20220303_0958.py
+-rw-r--r--   0 tom        (501) staff       (20)      914 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0006_auto_20220310_1147.py
+-rw-r--r--   0 tom        (501) staff       (20)      607 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0007_auto_20220322_1939.py
+-rw-r--r--   0 tom        (501) staff       (20)      827 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0008_auto_20220404_1144.py
+-rw-r--r--   0 tom        (501) staff       (20)     2485 2023-04-28 15:54:41.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0009_auto_20230428_1554.py
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    19474 2023-04-28 15:43:12.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/models.py
+-rw-r--r--   0 tom        (501) staff       (20)      532 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/report_builder.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.134033 django-advanced-report-builder-0.2.1/advanced_report_builder/static/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.136030 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.134234 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.195069 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/
+-rw-r--r--   0 tom        (501) staff       (20)   334540 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.esm.js
+-rw-r--r--   0 tom        (501) staff       (20)   405847 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.js
+-rw-r--r--   0 tom        (501) staff       (20)   193925 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.min.js
+-rw-r--r--   0 tom        (501) staff       (20)     1430 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-adapter-moment.min.js
+-rw-r--r--   0 tom        (501) staff       (20)    12893 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-plugin-datalabels.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.195790 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/
+-rw-r--r--   0 tom        (501) staff       (20)    72125 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/helpers.segment.js
+-rw-r--r--   0 tom        (501) staff       (20)     2352 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/helpers.esm.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.134771 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.201811 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3/js/
+-rw-r--r--   0 tom        (501) staff       (20)   575002 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3/js/d3.js
+-rw-r--r--   0 tom        (501) staff       (20)   275533 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3/js/d3.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.134564 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3-funnel/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.199284 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/
+-rw-r--r--   0 tom        (501) staff       (20)   205600 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.js
+-rw-r--r--   0 tom        (501) staff       (20)    58945 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.134977 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dashboard/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.203090 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dashboard/js/
+-rw-r--r--   0 tom        (501) staff       (20)      563 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dashboard/js/dashboard.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.135176 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.210951 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/
+-rwxr-xr-x   0 tom        (501) staff       (20)      578 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/.gitignore
+-rwxr-xr-x   0 tom        (501) staff       (20)      122 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/.travis.yml
+-rwxr-xr-x   0 tom        (501) staff       (20)     1176 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/LICENSE-DOT.txt
+-rwxr-xr-x   0 tom        (501) staff       (20)     3291 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.211565 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/bin/
+-rwxr-xr-x   0 tom        (501) staff       (20)     1442 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/bin/dot-packer
+-rwxr-xr-x   0 tom        (501) staff       (20)      443 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/bower.json
+-rwxr-xr-x   0 tom        (501) staff       (20)     5175 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/doT.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3374 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/doT.min.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1758 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/doU.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     5190 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/index.js
+-rwxr-xr-x   0 tom        (501) staff       (20)      920 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/package.json
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.135838 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/jquery_extendext/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.212613 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/
+-rwxr-xr-x   0 tom        (501) staff       (20)     4390 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1324 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.137145 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.224054 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/
+-rwxr-xr-x   0 tom        (501) staff       (20)     3765 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.css
+-rwxr-xr-x   0 tom        (501) staff       (20)     3253 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.min.css
+-rwxr-xr-x   0 tom        (501) staff       (20)     3756 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.css
+-rwxr-xr-x   0 tom        (501) staff       (20)     3248 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.min.css
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.241217 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/
+-rwxr-xr-x   0 tom        (501) staff       (20)     2962 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ar.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2540 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.az.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3082 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.bg.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2494 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.cs.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1431 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.da.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2309 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.de.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3273 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.el.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2672 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.en.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2662 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.es.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3216 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fa-IR.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2917 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fr.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2952 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.he.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2522 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.it.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2299 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.nl.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1412 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.no.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2645 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pl.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2787 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-BR.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2451 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-PT.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1310 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ro.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2955 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ru.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2627 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.sq.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2782 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.tr.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3062 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ua.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2503 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.zh-CN.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.244223 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.136899 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.244768 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/
+-rwxr-xr-x   0 tom        (501) staff       (20)     1212 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/plugin.js
+-rwxr-xr-x   0 tom        (501) staff       (20)   191499 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.js
+-rwxr-xr-x   0 tom        (501) staff       (20)    72607 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.min.js
+-rwxr-xr-x   0 tom        (501) staff       (20)   201158 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.js
+-rwxr-xr-x   0 tom        (501) staff       (20)    77072 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.245554 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/
+-rwxr-xr-x   0 tom        (501) staff       (20)      442 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/dark.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)     3887 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/default.scss
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.249710 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/
+-rwxr-xr-x   0 tom        (501) staff       (20)      266 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_bt-checkbox.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      194 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_bt-tooltip-errors.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      616 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_filter-description.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)       83 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_invert.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      469 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_sortable.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      194 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/bt-tooltip-errors.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      616 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/filter-description.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)       83 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/invert.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      465 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/sortable.scss
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.138123 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.250526 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.252047 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.252477 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/bar/
+-rw-r--r--   0 tom        (501) staff       (20)     4581 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/bar/middle.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.253279 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/funnel/
+-rw-r--r--   0 tom        (501) staff       (20)     1362 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/funnel/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)     1007 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/funnel/report.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.253687 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/line/
+-rw-r--r--   0 tom        (501) staff       (20)     4020 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/line/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)      486 2023-04-26 11:14:19.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)      273 2023-04-26 11:15:43.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/modal_field.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.254181 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/pie/
+-rw-r--r--   0 tom        (501) staff       (20)     2084 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/pie/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)      858 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/report.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.254544 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/data_merge/
+-rw-r--r--   0 tom        (501) staff       (20)     2975 2023-03-29 15:59:37.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/data_merge/data_merge.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.256645 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.257471 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/fields/
+-rw-r--r--   0 tom        (501) staff       (20)      254 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/fields/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     3320 2023-04-26 11:10:44.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/fields/single_query_builder.html
+-rw-r--r--   0 tom        (501) staff       (20)      377 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)      593 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/onclick_menu.html
+-rw-r--r--   0 tom        (501) staff       (20)      256 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/query_modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     1127 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/report.html
+-rw-r--r--   0 tom        (501) staff       (20)     8185 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/select_pivot.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.259648 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/kanban/
+-rw-r--r--   0 tom        (501) staff       (20)      499 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/kanban/description_modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     2038 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/kanban/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)      308 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/kanban/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     1961 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/kanban/report.html
+-rw-r--r--   0 tom        (501) staff       (20)     3468 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/query_builder.html
+-rw-r--r--   0 tom        (501) staff       (20)     9491 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/select_column.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.260903 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/single_values/
+-rw-r--r--   0 tom        (501) staff       (20)     1896 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/single_values/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)      623 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/single_values/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     1643 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/single_values/report.html
+-rw-r--r--   0 tom        (501) staff       (20)      327 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/toggle.py
+-rw-r--r--   0 tom        (501) staff       (20)     3830 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/urls.py
+-rw-r--r--   0 tom        (501) staff       (20)     4447 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)    12521 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/variable_date.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.266459 django-advanced-report-builder-0.2.1/advanced_report_builder/views/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    11547 2023-04-26 11:15:43.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/bar_charts.py
+-rw-r--r--   0 tom        (501) staff       (20)    18240 2023-04-28 15:13:27.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/charts_base.py
+-rw-r--r--   0 tom        (501) staff       (20)     3020 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/custom.py
+-rw-r--r--   0 tom        (501) staff       (20)     8659 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/dashboard.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.267865 django-advanced-report-builder-0.2.1/advanced_report_builder/views/datatables/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/datatables/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     6801 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/datatables/datatables.py
+-rw-r--r--   0 tom        (501) staff       (20)    25412 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/datatables/modal.py
+-rw-r--r--   0 tom        (501) staff       (20)    11394 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/datatables/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)     8731 2023-04-26 11:15:43.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/funnel_charts.py
+-rw-r--r--   0 tom        (501) staff       (20)    32161 2023-03-29 16:04:49.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/kanban.py
+-rw-r--r--   0 tom        (501) staff       (20)    12985 2023-04-26 11:15:43.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/line_charts.py
+-rw-r--r--   0 tom        (501) staff       (20)    21031 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/modals_base.py
+-rw-r--r--   0 tom        (501) staff       (20)     8692 2023-04-26 11:15:43.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/pie_charts.py
+-rw-r--r--   0 tom        (501) staff       (20)      443 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/report.py
+-rw-r--r--   0 tom        (501) staff       (20)     8210 2023-04-28 13:58:37.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/report_utils_mixin.py
+-rw-r--r--   0 tom        (501) staff       (20)     4750 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/reports.py
+-rw-r--r--   0 tom        (501) staff       (20)    22838 2023-04-28 15:43:12.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/single_values.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.270701 django-advanced-report-builder-0.2.1/advanced_report_builder/views/targets/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/targets/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3021 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/targets/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)      898 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.2.1/advanced_report_builder/views/targets/views.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-04-28 16:06:48.274844 django-advanced-report-builder-0.2.1/django_advanced_report_builder.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)      683 2023-04-28 16:06:48.000000 django-advanced-report-builder-0.2.1/django_advanced_report_builder.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)    10896 2023-04-28 16:06:48.000000 django-advanced-report-builder-0.2.1/django_advanced_report_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-04-28 16:06:48.000000 django-advanced-report-builder-0.2.1/django_advanced_report_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)      149 2023-04-28 16:06:48.000000 django-advanced-report-builder-0.2.1/django_advanced_report_builder.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)       24 2023-04-28 16:06:48.000000 django-advanced-report-builder-0.2.1/django_advanced_report_builder.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-04-28 16:06:48.275641 django-advanced-report-builder-0.2.1/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)      974 2023-04-28 16:04:12.000000 django-advanced-report-builder-0.2.1/setup.py
```

### Comparing `django-advanced-report-builder-0.2.0/LICENSE` & `django-advanced-report-builder-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/PKG-INFO` & `django-advanced-report-builder-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-advanced-report-builder
-Version: 0.2.0
+Version: 0.2.1
 Summary: Django app that allows you to build reports from modals
 Home-page: https://github.com/django-advance-utils/django-advanced-report-builder
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/admin.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/admin.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/columns.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/columns.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/data_merge/utils.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/data_merge/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/data_merge/widget.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/data_merge/widget.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/duplicate.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/duplicate.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/field_types.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/field_types.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/filter_query.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/filter_query.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/globals.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/globals.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,31 +36,31 @@
                           ANNOTATION_VALUE_QUARTER: 'quarter',
                           ANNOTATION_VALUE_MONTH: 'month',
                           ANNOTATION_VALUE_WEEK: 'week',
                           ANNOTATION_VALUE_DAY: 'day'}
 
 
 ANNOTATION_CHOICE_SUM = 1
-ANNOTATION_CHOICE_MAX = 2
-ANNOTATION_CHOICE_MIN = 3
+ANNOTATION_CHOICE_MAXIMUM = 2
+ANNOTATION_CHOICE_MINIMUM = 3
 ANNOTATION_CHOICE_COUNT = 4
-ANNOTATION_CHOICE_AVG = 5
+ANNOTATION_CHOICE_AVERAGE_SUM_FROM_COUNT = 5
 
 
 ANNOTATIONS_CHOICES = [(ANNOTATION_CHOICE_SUM, 'Sum'),
-                       (ANNOTATION_CHOICE_MAX, 'Max'),
-                       (ANNOTATION_CHOICE_MIN, 'Min'),
+                       (ANNOTATION_CHOICE_MAXIMUM, 'Maximum'),
+                       (ANNOTATION_CHOICE_MINIMUM, 'Minimum'),
                        (ANNOTATION_CHOICE_COUNT, 'Count'),
-                       (ANNOTATION_CHOICE_AVG, 'Avg')]
+                       (ANNOTATION_CHOICE_AVERAGE_SUM_FROM_COUNT, 'Average Sum from Count')]
 
 ANNOTATION_FUNCTIONS = {ANNOTATION_CHOICE_SUM: Sum,
-                        ANNOTATION_CHOICE_MAX: Max,
-                        ANNOTATION_CHOICE_MIN: Min,
+                        ANNOTATION_CHOICE_MAXIMUM: Max,
+                        ANNOTATION_CHOICE_MINIMUM: Min,
                         ANNOTATION_CHOICE_COUNT: Count,
-                        ANNOTATION_CHOICE_AVG: Avg}
+                        ANNOTATION_CHOICE_AVERAGE_SUM_FROM_COUNT: Avg}
 
 DATE_FORMAT_TYPE_DD_MM_YY_SLASH = 1
 DATE_FORMAT_TYPE_DD_MM_YYYY_SLASH = 2
 DATE_FORMAT_TYPE_MM_DD_YY_SLASH = 3
 DATE_FORMAT_TYPE_MM_DD_YYYY_SLASH = 4
 DATE_FORMAT_TYPE_DD_MM_YY_DASH = 5
 DATE_FORMAT_TYPE_DD_MM_YYYY_DASH = 6
```

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/includes.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/includes.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/migrations/0001_initial.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/migrations/0002_auto_20220209_1657.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0002_auto_20220209_1657.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/migrations/0003_auto_20220215_1219.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0003_auto_20220215_1219.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/migrations/0004_customreport.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0004_customreport.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/migrations/0005_auto_20220303_0958.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0005_auto_20220303_0958.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/migrations/0006_auto_20220310_1147.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0006_auto_20220310_1147.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/migrations/0007_auto_20220322_1939.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0007_auto_20220322_1939.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/migrations/0008_auto_20220404_1144.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/migrations/0008_auto_20220404_1144.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/models.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from django.utils.dates import MONTHS
 from django_datatables.columns import DatatableColumn, NoHeadingColumn, ManyToManyColumn
 from django_datatables.model_def import DatatableModel
 from time_stamped_model.models import TimeStampedModel
 
 from advanced_report_builder.globals import DISPLAY_OPTION_CHOICES, DISPLAY_OPTION_2_PER_ROW, DISPLAY_OPTION_NONE, \
     DISPLAY_OPTION_CLASSES, ANNOTATION_VALUE_CHOICES, ANNOTATIONS_CHOICES, ANNOTATION_CHOICE_COUNT, \
-    ANNOTATION_CHART_SCALE
+    ANNOTATION_CHART_SCALE, ANNOTATION_CHOICE_SUM, ANNOTATION_CHOICE_MAXIMUM, ANNOTATION_CHOICE_MINIMUM, ANNOTATION_CHOICE_AVERAGE_SUM_FROM_COUNT
 
 
 class Target(TimeStampedModel):
     TARGET_TYPE_COUNT = 1
     TARGET_TYPE_MONEY = 2
     TARGET_TYPE_PERCENTAGE = 3
 
@@ -231,35 +231,41 @@
 
 class SingleValueReport(Report):
     SINGLE_VALUE_TYPE_COUNT = 1
     SINGLE_VALUE_TYPE_SUM = 2
     SINGLE_VALUE_TYPE_COUNT_AND_SUM = 3
     SINGLE_VALUE_TYPE_PERCENT = 4
     SINGLE_VALUE_TYPE_PERCENT_FROM_COUNT = 5
-    SINGLE_VALUE_TYPE_AVERAGE = 6
+    SINGLE_VALUE_TYPE_AVERAGE_SUM_FROM_COUNT = 6
+    SINGLE_VALUE_TYPE_AVERAGE_SUM_OVER_TIME = 7
 
     SINGLE_VALUE_TYPE_CHOICES = (
         (SINGLE_VALUE_TYPE_COUNT, 'Count'),
         (SINGLE_VALUE_TYPE_SUM, 'Sum'),
         (SINGLE_VALUE_TYPE_COUNT_AND_SUM, 'Count & Sum'),
         (SINGLE_VALUE_TYPE_PERCENT, 'Percent'),
         (SINGLE_VALUE_TYPE_PERCENT_FROM_COUNT, 'Percent from Count'),
-        (SINGLE_VALUE_TYPE_AVERAGE, 'Average')
+        (SINGLE_VALUE_TYPE_AVERAGE_SUM_FROM_COUNT, 'Average Sum from Count'),
+        (SINGLE_VALUE_TYPE_AVERAGE_SUM_OVER_TIME, 'Average Sum over Time')
     )
 
     tile_colour = models.CharField(max_length=10, blank=True, null=True)
     field = models.CharField(max_length=200, blank=True, null=True)  # denominator
     numerator = models.CharField(max_length=200, blank=True, null=True)
     single_value_type = models.PositiveSmallIntegerField(choices=SINGLE_VALUE_TYPE_CHOICES,
                                                          default=SINGLE_VALUE_TYPE_COUNT)
     prefix = models.CharField(max_length=64, blank=True, null=True)
     decimal_places = models.IntegerField(default=0)
     show_breakdown = models.BooleanField(default=False)
     breakdown_fields = models.JSONField(null=True, blank=True)
 
+    average_scale = models.PositiveSmallIntegerField(choices=ANNOTATION_VALUE_CHOICES, blank=True, null=True)
+    average_start_period = models.PositiveSmallIntegerField(blank=True, null=True)
+    average_end_period = models.PositiveSmallIntegerField(blank=True, null=True)
+
     def is_percentage(self):
         return self.single_value_type in [self.SINGLE_VALUE_TYPE_PERCENT,
                                           self.SINGLE_VALUE_TYPE_PERCENT_FROM_COUNT]
 
 
 class BarChartReport(Report):
```

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/report_builder.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/report_builder.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.esm.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.esm.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.min.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-adapter-moment.min.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-adapter-moment.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-plugin-datalabels.min.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-plugin-datalabels.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/helpers.segment.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/helpers.segment.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/helpers.esm.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/helpers.esm.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/d3/js/d3.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3/js/d3.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/d3/js/d3.min.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3/js/d3.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.min.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dashboard/js/dashboard.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dashboard/js/dashboard.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dot/js/.gitignore` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/.gitignore`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dot/js/LICENSE-DOT.txt` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/LICENSE-DOT.txt`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dot/js/README.md` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/README.md`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dot/js/bin/dot-packer` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/bin/dot-packer`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dot/js/doT.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/doT.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dot/js/doT.min.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/doT.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dot/js/doU.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/doU.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dot/js/index.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/index.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/dot/js/package.json` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/dot/js/package.json`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.min.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.css` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.css`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.min.css` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.min.css`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.css` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.css`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.min.css` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.min.css`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ar.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ar.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.az.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.az.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.bg.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.bg.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.cs.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.cs.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.da.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.da.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.de.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.de.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.el.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.el.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.en.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.en.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.es.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.es.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fa-IR.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fa-IR.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fr.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fr.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.he.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.he.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.it.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.it.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.nl.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.nl.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.no.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.no.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pl.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pl.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-BR.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-BR.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-PT.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-PT.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ro.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ro.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ru.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ru.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.sq.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.sq.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.tr.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.tr.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ua.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ua.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.zh-CN.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.zh-CN.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/plugin.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/plugin.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.min.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.min.js` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/default.scss` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/default.scss`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_filter-description.scss` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_filter-description.scss`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/filter-description.scss` & `django-advanced-report-builder-0.2.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/filter-description.scss`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/charts/bar/middle.html` & `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/bar/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/charts/funnel/middle.html` & `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/funnel/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/charts/funnel/report.html` & `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/funnel/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/charts/line/middle.html` & `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/line/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/charts/pie/middle.html` & `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/pie/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/charts/report.html` & `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/charts/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/data_merge/data_merge.html` & `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/data_merge/data_merge.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/datatables/fields/single_query_builder.html` & `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/fields/single_query_builder.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/datatables/onclick_menu.html` & `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/onclick_menu.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/datatables/report.html` & `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/datatables/select_pivot.html` & `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/datatables/select_pivot.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/kanban/middle.html` & `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/kanban/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/kanban/report.html` & `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/kanban/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/query_builder.html` & `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/query_builder.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/select_column.html` & `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/select_column.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/single_values/middle.html` & `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/single_values/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/single_values/modal.html` & `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/single_values/modal.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/templates/advanced_report_builder/single_values/report.html` & `django-advanced-report-builder-0.2.1/advanced_report_builder/templates/advanced_report_builder/single_values/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/urls.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/urls.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/utils.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/variable_date.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/variable_date.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/views/bar_charts.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/views/bar_charts.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/views/charts_base.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/views/charts_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import base64
 import json
 from datetime import timedelta, datetime
 
 from crispy_forms.bootstrap import StrictButton
 from date_offset.date_offset import DateOffset
+from dateutil.relativedelta import relativedelta
 from django.apps import apps
 from django.db import ProgrammingError, DataError
 from django.db.models import Q
 from django.shortcuts import get_object_or_404
 from django.utils.safestring import mark_safe
 from django.views.generic import TemplateView
 from django_datatables.datatables import DatatableTable
 from django_menus.menu import MenuItem
 from django_modals.forms import CrispyForm
 
 from advanced_report_builder.columns import ReportBuilderDateColumn
 from advanced_report_builder.exceptions import ReportError
-from advanced_report_builder.globals import NUMBER_FIELDS, ANNOTATION_VALUE_FUNCTIONS
+from advanced_report_builder.globals import NUMBER_FIELDS, ANNOTATION_VALUE_FUNCTIONS, ANNOTATION_VALUE_YEAR, \
+    ANNOTATION_VALUE_QUARTER, ANNOTATION_VALUE_WEEK, ANNOTATION_VALUE_DAY, ANNOTATION_VALUE_MONTH
 from advanced_report_builder.models import ReportType
 from advanced_report_builder.utils import split_slug, get_field_details, split_attr
+from advanced_report_builder.variable_date import VariableDate
 from advanced_report_builder.views.report import ReportBase
 from advanced_report_builder.views.report_utils_mixin import ReportUtilsMixin
 from advanced_report_builder.views.targets.utils import get_target_value
 
 
 class ChartJSTable(DatatableTable):
 
@@ -298,14 +301,43 @@
     def edit_report_menu(request, chart_report_id, slug_str):
         return []
 
     # noinspection PyMethodMayBeStatic
     def queries_menu(self):
         return []
 
+    @staticmethod
+    def get_period_divider(annotation_value_choice, start_date_type, end_date_type):
+        variable_date = VariableDate()
+        start_date_and_time, _, _ = variable_date.get_variable_dates(start_date_type)
+        _, end_date_and_time, _ = variable_date.get_variable_dates(end_date_type)
+        if annotation_value_choice == ANNOTATION_VALUE_YEAR:
+            divider = abs(end_date_and_time.year - start_date_and_time.year) + 1
+        elif annotation_value_choice == ANNOTATION_VALUE_QUARTER:
+            delta = relativedelta(end_date_and_time, start_date_and_time)
+            divider = delta.years * 4 + delta.months // 3
+        elif annotation_value_choice == ANNOTATION_VALUE_MONTH:
+            rdate = relativedelta(end_date_and_time, start_date_and_time)
+            divider = 0
+            if rdate.years is not None and abs(rdate.years) > 0:
+                divider += abs(rdate.years) * 12
+            if rdate.months is not None and abs(rdate.months) > 0:
+                divider += rdate.months
+            if rdate.days is not None and abs(rdate.days) > 0:
+                divider += 1
+        elif annotation_value_choice == ANNOTATION_VALUE_WEEK:
+            monday1 = (start_date_and_time - timedelta(days=start_date_and_time.weekday()))
+            monday2 = (end_date_and_time - timedelta(days=end_date_and_time.weekday()))
+            divider = int((monday2 - monday1).days / 7)
+        elif annotation_value_choice == ANNOTATION_VALUE_DAY:
+            divider = (end_date_and_time - start_date_and_time).days
+        else:
+            raise ReportError('unknown annotation_value_choice')
+        return divider
+
 
 class ChartBaseFieldForm(CrispyForm):
     cancel_class = 'btn-secondary modal-cancel'
 
     def __init__(self, *args, **kwargs):
         self.django_field = None
         self.col_type_override = None
```

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/views/custom.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/views/custom.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/views/dashboard.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/views/dashboard.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/views/datatables/datatables.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/views/datatables/datatables.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/views/datatables/modal.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/views/datatables/modal.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/views/datatables/utils.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/views/datatables/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/views/funnel_charts.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/views/funnel_charts.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/views/kanban.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/views/kanban.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/views/line_charts.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/views/line_charts.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/views/modals_base.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/views/modals_base.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/views/pie_charts.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/views/pie_charts.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/views/report_utils_mixin.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/views/report_utils_mixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import copy
 import json
 import operator
 from functools import reduce
 
+from django.db.models import FloatField, ExpressionWrapper
+from django.db.models.functions import NullIf
 from django_datatables.columns import CurrencyPenceColumn, CurrencyColumn
 
 from advanced_report_builder.columns import ReportBuilderCurrencyPenceColumn, ReportBuilderCurrencyColumn, \
     ReportBuilderNumberColumn
 from advanced_report_builder.filter_query import FilterQueryMixin
 from advanced_report_builder.globals import ANNOTATION_FUNCTIONS, ANNOTATION_CHOICE_COUNT
 from advanced_report_builder.utils import decode_attribute
@@ -14,15 +16,15 @@
 
 class ReportUtilsMixin(FilterQueryMixin):
     use_annotations = True
     number_field = ReportBuilderNumberColumn
 
     def get_number_field(self, annotations_type, index, table_field, data_attr, fields, col_type_override,
                          extra_filter=None, title_suffix='', multiple_index=0, decimal_places=None,
-                         convert_currency_fields=False, totals=None):
+                         convert_currency_fields=False, totals=None, divider=None):
         field_name = table_field['field']
         css_class = None
         annotation_filter = None
         if annotations_type != 0:
             b64_filter = data_attr.get('filter')
             if b64_filter:
                 _filter = decode_attribute(b64_filter)
@@ -67,14 +69,16 @@
                 self.set_extra_number_field_kwargs(data_attr=data_attr,
                                                    options=number_function_kwargs['options'],
                                                    multiple_index=multiple_index)
                 if annotation_filter:
                     function = function_type(raw_field_name, filter=annotation_filter)
                 else:
                     function = function_type(raw_field_name)
+                if divider:
+                    function = ExpressionWrapper(function / NullIf(divider, 0), output_field=FloatField())
                 if self.use_annotations:
                     number_function_kwargs['annotations'] = {new_field_name: function}
                 else:
                     number_function_kwargs['options']['calculated'] = True
                     number_function_kwargs['aggregations'] = {new_field_name: function}
                     number_function_kwargs['annotations'] = []
 
@@ -88,14 +92,16 @@
                 if annotations_type != 0:
                     new_field_name = f'{annotations_type}_{field_name}_{index}'
                     function_type = ANNOTATION_FUNCTIONS[annotations_type]
                     if annotation_filter:
                         function = function_type(raw_field_name, filter=annotation_filter)
                     else:
                         function = function_type(raw_field_name)
+                    if divider:
+                        function = ExpressionWrapper(function / NullIf(divider, 0), output_field=FloatField())
                     if self.use_annotations:
                         field.annotations = {new_field_name: function}
                     else:
                         field.options['calculated'] = True
                         field.aggregations = {new_field_name: function}
                         field.annotations = []
 
@@ -116,14 +122,15 @@
                                                    multiple_index=multiple_index)
                 new_field_name = f'{annotations_type}_{field_name}_{index}'
                 function_type = ANNOTATION_FUNCTIONS[annotations_type]
                 if annotation_filter:
                     function = function_type(field_name, filter=annotation_filter)
                 else:
                     function = function_type(field_name)
+
                 if self.use_annotations:
                     number_function_kwargs['annotations'] = {new_field_name: function}
                 else:
                     number_function_kwargs['options']['calculated'] = True
                     number_function_kwargs['aggregations'] = {new_field_name: function}
                     number_function_kwargs['annotations'] = []
                 field_name = new_field_name
```

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/views/reports.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/views/reports.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/views/single_values.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/views/single_values.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 
 from django.core.exceptions import ValidationError
 from django.db.models import Count, Sum, ExpressionWrapper, FloatField
 from django.db.models.functions import Coalesce, NullIf
+from django.forms import ChoiceField
 from django.shortcuts import get_object_or_404
 from django.urls import reverse
 from django_datatables.datatables import DatatableTable
 from django_menus.menu import MenuItem
 from django_modals.fields import FieldEx
 from django_modals.helper import show_modal
 from django_modals.modals import Modal
@@ -14,17 +15,18 @@
 from django_modals.widgets.colour_picker import ColourPickerWidget
 from django_modals.widgets.select2 import Select2Multiple
 from django_modals.widgets.widgets import Toggle
 
 from advanced_report_builder.columns import ReportBuilderNumberColumn
 from advanced_report_builder.exceptions import ReportError
 from advanced_report_builder.globals import NUMBER_FIELDS, ANNOTATION_CHOICE_SUM, \
-    ANNOTATION_CHOICE_AVG
+    ANNOTATION_CHOICE_AVERAGE_SUM_FROM_COUNT
 from advanced_report_builder.models import SingleValueReport, ReportType
 from advanced_report_builder.utils import get_field_details
+from advanced_report_builder.variable_date import VariableDate
 from advanced_report_builder.views.charts_base import ChartBaseView
 from advanced_report_builder.views.datatables.modal import TableFieldModal, TableFieldForm
 from advanced_report_builder.views.datatables.utils import TableUtilsMixin
 from advanced_report_builder.views.modals_base import QueryBuilderModalBase
 
 
 class SingleValueView(ChartBaseView):
@@ -33,15 +35,15 @@
     use_annotations = False
 
     def dispatch(self, request, *args, **kwargs):
         self.report = kwargs.get('report')
         self.chart_report = self.report.singlevaluereport
         return super().dispatch(request, *args, **kwargs)
 
-    def _process_aggregations(self, fields, aggregations_type=ANNOTATION_CHOICE_SUM):
+    def _process_aggregations(self, fields, aggregations_type=ANNOTATION_CHOICE_SUM, divider=None):
         field = self.chart_report.field
         base_model = self.chart_report.get_base_modal()
         report_builder_class = getattr(base_model, self.chart_report.report_type.report_builder_class_name, None)
 
         django_field, col_type_override, _, _ = get_field_details(base_model=base_model,
                                                                   field=field,
                                                                   report_builder_class=report_builder_class)
@@ -52,15 +54,16 @@
             self.get_number_field(annotations_type=aggregations_type,
                                   index=0,
                                   data_attr={},
                                   table_field={'field': field, 'title': field},
                                   fields=fields,
                                   col_type_override=col_type_override,
                                   decimal_places=self.chart_report.decimal_places,
-                                  convert_currency_fields=True)
+                                  convert_currency_fields=True,
+                                  divider=divider)
         else:
             raise ReportError('not a number field')
 
     def _get_count(self, fields):
 
         number_function_kwargs = {'aggregations': {'count': Count(1)},
                                   'field': 'count',
@@ -201,24 +204,31 @@
         if single_value_type == SingleValueReport.SINGLE_VALUE_TYPE_COUNT:
             self._get_count(fields=fields)
         elif single_value_type == SingleValueReport.SINGLE_VALUE_TYPE_SUM:
             self._process_aggregations(fields=fields, aggregations_type=ANNOTATION_CHOICE_SUM)
         elif single_value_type == SingleValueReport.SINGLE_VALUE_TYPE_COUNT_AND_SUM:
             self._get_count(fields=fields)
             self._process_aggregations(fields=fields, aggregations_type=ANNOTATION_CHOICE_SUM)
-        elif single_value_type == SingleValueReport.SINGLE_VALUE_TYPE_AVERAGE:
-            self._process_aggregations(fields=fields, aggregations_type=ANNOTATION_CHOICE_AVG)
+        elif single_value_type == SingleValueReport.SINGLE_VALUE_TYPE_AVERAGE_SUM_FROM_COUNT:
+            self._process_aggregations(fields=fields, aggregations_type=ANNOTATION_CHOICE_AVERAGE_SUM_FROM_COUNT)
+        elif single_value_type == SingleValueReport.SINGLE_VALUE_TYPE_AVERAGE_SUM_OVER_TIME:
+            divider = self.get_period_divider(annotation_value_choice=self.chart_report.average_scale,
+                                              start_date_type=self.chart_report.average_start_period,
+                                              end_date_type=self.chart_report.average_end_period)
+            self._process_aggregations(fields=fields, aggregations_type=ANNOTATION_CHOICE_SUM, divider=divider)
         elif single_value_type == SingleValueReport.SINGLE_VALUE_TYPE_PERCENT:
             self._process_percentage(fields=fields)
         elif single_value_type == SingleValueReport.SINGLE_VALUE_TYPE_PERCENT_FROM_COUNT:
             self._process_percentage_from_count(fields=fields)
         return fields
 
     def set_prefix(self):
         self.table.prefix = self.chart_report.prefix
+        if self.table.prefix:
+            self.table.prefix += ' '
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         self.set_prefix()
         self.table.single_value = self.chart_report
         self.table.enable_links = self.kwargs.get('enable_links')
         self.table.datatable_template = 'advanced_report_builder/single_values/middle.html'
@@ -259,14 +269,17 @@
 
     form_fields = ['name',
                    'notes',
                    'report_type',
                    'report_tags',
                    ('single_value_type', {'label': 'Value type'}),
                    ('numerator', {'label': 'Numerator field'}),
+                   'average_scale',
+                   'average_start_period',
+                   'average_end_period',
                    'field',
                    'prefix',
                    'tile_colour',
                    ('decimal_places', {'field_class': 'col-md-5 col-lg-3 input-group-sm'}),
                    'show_breakdown',
                    'breakdown_fields'
                    ]
@@ -288,14 +301,23 @@
              'values': {SingleValueReport.SINGLE_VALUE_TYPE_PERCENT: 'show',
                         SingleValueReport.SINGLE_VALUE_TYPE_PERCENT_FROM_COUNT: 'show'},
              'default': 'hide'},
             {'selector': 'label[for=id_field]',
              'values': {SingleValueReport.SINGLE_VALUE_TYPE_PERCENT: ('html', 'Denominator field')},
              'default': ('html', 'Field')},
 
+            {'selector': '#div_id_average_scale',
+             'values': {SingleValueReport.SINGLE_VALUE_TYPE_AVERAGE_SUM_OVER_TIME: 'show'},
+             'default': 'hide'},
+            {'selector': '#div_id_average_start_period',
+             'values': {SingleValueReport.SINGLE_VALUE_TYPE_AVERAGE_SUM_OVER_TIME: 'show'},
+             'default': 'hide'},
+            {'selector': '#div_id_average_end_period',
+             'values': {SingleValueReport.SINGLE_VALUE_TYPE_AVERAGE_SUM_OVER_TIME: 'show'},
+             'default': 'hide'},
         ])
 
         form.add_trigger('show_breakdown', 'onchange', [
             {'selector': '#div_id_breakdown_fields', 'values': {'checked': 'show'}, 'default': 'hide'},
         ])
 
         if 'data' in _kwargs:
@@ -320,21 +342,28 @@
                          selected_field_id=numerator,
                          report_type=report_type)
 
         self.add_query_data(form, include_extra_query=True)
         form.fields['notes'].widget.attrs['rows'] = 3
         url = reverse('advanced_report_builder:single_value_field_modal',
                       kwargs={'slug': 'selector-99999-data-FIELD_INFO-report_type_id-REPORT_TYPE_ID'})
+
+        range_type_choices = VariableDate.RANGE_TYPE_CHOICES
+        form.fields['average_start_period'] = ChoiceField(required=False, choices=range_type_choices)
+        form.fields['average_end_period'] = ChoiceField(required=False, choices=range_type_choices)
         return ('name',
                 'notes',
                 'report_type',
                 'report_tags',
                 'single_value_type',
                 'numerator',
                 'field',
+                'average_scale',
+                'average_start_period',
+                'average_end_period',
                 'prefix',
                 FieldEx('extra_query_data',
                         template='advanced_report_builder/query_builder.html',
                         ),
                 'tile_colour',
                 'decimal_places',
                 'show_breakdown',
@@ -353,19 +382,28 @@
     def select2_numerator(self, **kwargs):
         return self.get_fields_for_select2(field_type='number',
                                            report_type=kwargs['report_type'],
                                            search_string=kwargs.get('search'))
 
     # noinspection PyUnusedLocal
     def clean(self, form, cleaned_data):
-        if (cleaned_data['single_value_type'] not in [SingleValueReport.SINGLE_VALUE_TYPE_COUNT,
-                                                      SingleValueReport.SINGLE_VALUE_TYPE_PERCENT_FROM_COUNT] and
+        single_value_type = cleaned_data['single_value_type']
+        if (single_value_type not in [SingleValueReport.SINGLE_VALUE_TYPE_COUNT,
+                                      SingleValueReport.SINGLE_VALUE_TYPE_PERCENT_FROM_COUNT] and
                 not cleaned_data['field']):
             raise ValidationError("Please select a field")
 
+        if single_value_type == SingleValueReport.SINGLE_VALUE_TYPE_AVERAGE_SUM_OVER_TIME:
+            if cleaned_data['average_scale'] is None:
+                form.add_error('average_scale', "Please select a time scale")
+            if cleaned_data['average_start_period'] is None:
+                form.add_error('average_start_period', "Please select a start period")
+            if cleaned_data['average_end_period'] is None:
+                form.add_error('average_end_period', "Please select a end period")
+
     def ajax_get_fields(self, **kwargs):
         report_type_id = kwargs['report_type']
         report_builder_fields, base_model = self.get_report_builder_class(report_type_id=report_type_id)
         fields = []
         tables = []
         self._get_fields(base_model=base_model,
                          fields=fields,
```

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/views/targets/utils.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/views/targets/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/advanced_report_builder/views/targets/views.py` & `django-advanced-report-builder-0.2.1/advanced_report_builder/views/targets/views.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.2.0/django_advanced_report_builder.egg-info/PKG-INFO` & `django-advanced-report-builder-0.2.1/django_advanced_report_builder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-advanced-report-builder
-Version: 0.2.0
+Version: 0.2.1
 Summary: Django app that allows you to build reports from modals
 Home-page: https://github.com/django-advance-utils/django-advanced-report-builder
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-advanced-report-builder-0.2.0/django_advanced_report_builder.egg-info/SOURCES.txt` & `django-advanced-report-builder-0.2.1/django_advanced_report_builder.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 advanced_report_builder/migrations/0002_auto_20220209_1657.py
 advanced_report_builder/migrations/0003_auto_20220215_1219.py
 advanced_report_builder/migrations/0004_customreport.py
 advanced_report_builder/migrations/0005_auto_20220303_0958.py
 advanced_report_builder/migrations/0006_auto_20220310_1147.py
 advanced_report_builder/migrations/0007_auto_20220322_1939.py
 advanced_report_builder/migrations/0008_auto_20220404_1144.py
+advanced_report_builder/migrations/0009_auto_20230428_1554.py
 advanced_report_builder/migrations/__init__.py
 advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.esm.js
 advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.js
 advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.min.js
 advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-adapter-moment.min.js
 advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-plugin-datalabels.min.js
 advanced_report_builder/static/advanced_report_builder/chart-js/js/helpers.esm.js
```

### Comparing `django-advanced-report-builder-0.2.0/setup.py` & `django-advanced-report-builder-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-advanced-report-builder",
-    version="0.2.0",
+    version="0.2.1",
     author="Thomas Turner",
     description="Django app that allows you to build reports from modals",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/django-advance-utils/django-advanced-report-builder",
     include_package_data=True,
     packages=['advanced_report_builder'],
```

