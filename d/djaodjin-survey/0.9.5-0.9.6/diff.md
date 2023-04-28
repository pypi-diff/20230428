# Comparing `tmp/djaodjin-survey-0.9.5.tar.gz` & `tmp/djaodjin-survey-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djaodjin-survey-0.9.5.tar", last modified: Tue Apr 18 19:58:10 2023, max compression
+gzip compressed data, was "djaodjin-survey-0.9.6.tar", last modified: Fri Apr 28 01:52:28 2023, max compression
```

## Comparing `djaodjin-survey-0.9.5.tar` & `djaodjin-survey-0.9.6.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.470100 djaodjin-survey-0.9.5/
--rw-r--r--   0 smirolo    (501) staff       (20)     1318 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/LICENSE.txt
--rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/MANIFEST.in
--rw-r--r--   0 smirolo    (501) staff       (20)     1888 2023-04-18 19:58:10.470164 djaodjin-survey-0.9.5/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     1129 2023-04-18 19:35:08.000000 djaodjin-survey-0.9.5/README.md
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.461467 djaodjin-survey-0.9.5/djaodjin_survey.egg-info/
--rw-r--r--   0 smirolo    (501) staff       (20)     1888 2023-04-18 19:58:10.000000 djaodjin-survey-0.9.5/djaodjin_survey.egg-info/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     2399 2023-04-18 19:58:10.000000 djaodjin-survey-0.9.5/djaodjin_survey.egg-info/SOURCES.txt
--rw-r--r--   0 smirolo    (501) staff       (20)        1 2023-04-18 19:58:10.000000 djaodjin-survey-0.9.5/djaodjin_survey.egg-info/dependency_links.txt
--rw-r--r--   0 smirolo    (501) staff       (20)       73 2023-04-18 19:58:10.000000 djaodjin-survey-0.9.5/djaodjin_survey.egg-info/requires.txt
--rw-r--r--   0 smirolo    (501) staff       (20)        7 2023-04-18 19:58:10.000000 djaodjin-survey-0.9.5/djaodjin_survey.egg-info/top_level.txt
--rw-r--r--   0 smirolo    (501) staff       (20)     1358 2023-04-18 19:54:04.000000 djaodjin-survey-0.9.5/pyproject.toml
--rw-r--r--   0 smirolo    (501) staff       (20)       79 2023-04-18 19:58:10.470345 djaodjin-survey-0.9.5/setup.cfg
--rw-r--r--   0 smirolo    (501) staff       (20)     1381 2023-04-18 16:17:24.000000 djaodjin-survey-0.9.5/setup.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.463222 djaodjin-survey-0.9.5/survey/
--rw-r--r--   0 smirolo    (501) staff       (20)     1435 2023-04-18 19:57:54.000000 djaodjin-survey-0.9.5/survey/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1842 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/admin.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.464384 djaodjin-survey-0.9.5/survey/api/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     7333 2022-09-14 00:28:06.000000 djaodjin-survey-0.9.5/survey/api/campaigns.py
--rw-r--r--   0 smirolo    (501) staff       (20)    44811 2023-04-18 18:56:03.000000 djaodjin-survey-0.9.5/survey/api/matrix.py
--rw-r--r--   0 smirolo    (501) staff       (20)    12575 2023-01-27 18:26:55.000000 djaodjin-survey-0.9.5/survey/api/metrics.py
--rw-r--r--   0 smirolo    (501) staff       (20)    23591 2023-03-23 22:52:31.000000 djaodjin-survey-0.9.5/survey/api/portfolios.py
--rw-r--r--   0 smirolo    (501) staff       (20)    56385 2023-04-07 16:36:46.000000 djaodjin-survey-0.9.5/survey/api/sample.py
--rw-r--r--   0 smirolo    (501) staff       (20)    23830 2023-04-14 17:05:47.000000 djaodjin-survey-0.9.5/survey/api/serializers.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2929 2023-03-10 17:42:57.000000 djaodjin-survey-0.9.5/survey/api/serializers_overrides.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5569 2023-04-13 17:06:50.000000 djaodjin-survey-0.9.5/survey/api/units.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4094 2022-09-26 17:15:24.000000 djaodjin-survey-0.9.5/survey/compat.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2316 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/docs.py
--rw-r--r--   0 smirolo    (501) staff       (20)    17450 2023-04-07 16:40:09.000000 djaodjin-survey-0.9.5/survey/filters.py
--rw-r--r--   0 smirolo    (501) staff       (20)     8639 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/forms.py
--rw-r--r--   0 smirolo    (501) staff       (20)     6173 2023-04-05 16:25:51.000000 djaodjin-survey-0.9.5/survey/helpers.py
--rw-r--r--   0 smirolo    (501) staff       (20)    14690 2023-04-18 18:56:44.000000 djaodjin-survey-0.9.5/survey/mixins.py
--rw-r--r--   0 smirolo    (501) staff       (20)    39683 2023-04-05 17:20:30.000000 djaodjin-survey-0.9.5/survey/models.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4007 2023-04-05 18:59:23.000000 djaodjin-survey-0.9.5/survey/pagination.py
--rw-r--r--   0 smirolo    (501) staff       (20)    13064 2023-04-05 17:26:46.000000 djaodjin-survey-0.9.5/survey/queries.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4395 2023-03-21 20:59:50.000000 djaodjin-survey-0.9.5/survey/settings.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1955 2022-10-04 20:48:04.000000 djaodjin-survey-0.9.5/survey/signals.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.459556 djaodjin-survey-0.9.5/survey/static/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.464512 djaodjin-survey-0.9.5/survey/static/css/
--rw-r--r--   0 smirolo    (501) staff       (20)      296 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/static/css/matrix-chart.css
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.465399 djaodjin-survey-0.9.5/survey/static/js/
--rw-r--r--   0 smirolo    (501) staff       (20)    12547 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/static/js/djaodjin-categorize.js
--rw-r--r--   0 smirolo    (501) staff       (20)    15443 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/static/js/djaodjin-matrix.js
--rw-r--r--   0 smirolo    (501) staff       (20)    51604 2023-04-14 15:55:35.000000 djaodjin-survey-0.9.5/survey/static/js/djaodjin-resources-vue.js
--rw-r--r--   0 smirolo    (501) staff       (20)     5462 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/static/js/djaodjin-set.js
--rw-r--r--   0 smirolo    (501) staff       (20)    17193 2023-04-14 16:37:55.000000 djaodjin-survey-0.9.5/survey/static/js/djaodjin-survey-vue.js
--rw-r--r--   0 smirolo    (501) staff       (20)      544 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/static/js/djaodjin-survey.js
--rw-r--r--   0 smirolo    (501) staff       (20)    12995 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/static/js/matrix-chart.js
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.459669 djaodjin-survey-0.9.5/survey/templates/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.466755 djaodjin-survey-0.9.5/survey/templates/survey/
--rw-r--r--   0 smirolo    (501) staff       (20)      667 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/answer_form.html
--rw-r--r--   0 smirolo    (501) staff       (20)      249 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/campaign_form.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.466869 djaodjin-survey-0.9.5/survey/templates/survey/campaigns/
--rw-r--r--   0 smirolo    (501) staff       (20)     1184 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/campaigns/index.html
--rw-r--r--   0 smirolo    (501) staff       (20)     2529 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/categorize.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.467192 djaodjin-survey-0.9.5/survey/templates/survey/matrix/
--rw-r--r--   0 smirolo    (501) staff       (20)       62 2023-01-19 22:34:30.000000 djaodjin-survey-0.9.5/survey/templates/survey/matrix/compare.html
--rw-r--r--   0 smirolo    (501) staff       (20)     2087 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/matrix/index.html
--rw-r--r--   0 smirolo    (501) staff       (20)     4088 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/matrix/matrix.html
--rw-r--r--   0 smirolo    (501) staff       (20)     9287 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/portfolios.html
--rw-r--r--   0 smirolo    (501) staff       (20)      249 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/question_form.html
--rw-r--r--   0 smirolo    (501) staff       (20)     1572 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/question_list.html
--rw-r--r--   0 smirolo    (501) staff       (20)      471 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/respondent_list.html
--rw-r--r--   0 smirolo    (501) staff       (20)     2077 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/result.html
--rw-r--r--   0 smirolo    (501) staff       (20)      983 2023-03-10 17:29:52.000000 djaodjin-survey-0.9.5/survey/templates/survey/result_quizz.html
--rw-r--r--   0 smirolo    (501) staff       (20)      562 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/sample_create.html
--rw-r--r--   0 smirolo    (501) staff       (20)      356 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/sample_update.html
--rw-r--r--   0 smirolo    (501) staff       (20)      245 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/send.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.467409 djaodjin-survey-0.9.5/survey/templatetags/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templatetags/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1769 2023-02-10 21:30:25.000000 djaodjin-survey-0.9.5/survey/templatetags/survey_tags.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.467519 djaodjin-survey-0.9.5/survey/urls/
--rw-r--r--   0 smirolo    (501) staff       (20)     1533 2022-09-25 23:08:10.000000 djaodjin-survey-0.9.5/survey/urls/__init__.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.468301 djaodjin-survey-0.9.5/survey/urls/api/
--rw-r--r--   0 smirolo    (501) staff       (20)     1718 2023-03-22 18:00:00.000000 djaodjin-survey-0.9.5/survey/urls/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1653 2022-09-26 00:12:56.000000 djaodjin-survey-0.9.5/survey/urls/api/campaigns.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2772 2022-09-26 02:10:24.000000 djaodjin-survey-0.9.5/survey/urls/api/filters.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2125 2023-04-07 17:48:09.000000 djaodjin-survey-0.9.5/survey/urls/api/matrix.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1717 2022-09-26 00:13:35.000000 djaodjin-survey-0.9.5/survey/urls/api/metrics.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1622 2022-09-26 00:12:26.000000 djaodjin-survey-0.9.5/survey/urls/api/noauth.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2390 2023-03-07 21:45:05.000000 djaodjin-survey-0.9.5/survey/urls/api/portfolios.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.468638 djaodjin-survey-0.9.5/survey/urls/api/sample/
--rw-r--r--   0 smirolo    (501) staff       (20)     1512 2022-09-26 00:09:27.000000 djaodjin-survey-0.9.5/survey/urls/api/sample/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1722 2023-02-21 21:54:31.000000 djaodjin-survey-0.9.5/survey/urls/api/sample/reset.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2830 2023-04-07 17:59:33.000000 djaodjin-survey-0.9.5/survey/urls/api/sample/update.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.469227 djaodjin-survey-0.9.5/survey/urls/views/
--rw-r--r--   0 smirolo    (501) staff       (20)     1714 2023-03-22 18:07:23.000000 djaodjin-survey-0.9.5/survey/urls/views/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2942 2022-09-26 00:06:32.000000 djaodjin-survey-0.9.5/survey/urls/views/campaigns.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2105 2023-01-19 22:50:22.000000 djaodjin-survey-0.9.5/survey/urls/views/matrices.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1894 2023-01-25 23:37:48.000000 djaodjin-survey-0.9.5/survey/urls/views/portfolios.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2180 2022-09-26 00:14:39.000000 djaodjin-survey-0.9.5/survey/urls/views/samples.py
--rw-r--r--   0 smirolo    (501) staff       (20)     9367 2023-04-17 20:51:27.000000 djaodjin-survey-0.9.5/survey/utils.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.469985 djaodjin-survey-0.9.5/survey/views/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/views/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     8457 2023-03-21 21:02:40.000000 djaodjin-survey-0.9.5/survey/views/campaigns.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5626 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/views/createquestion.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1898 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/views/edit.py
--rw-r--r--   0 smirolo    (501) staff       (20)     6155 2023-04-07 17:48:37.000000 djaodjin-survey-0.9.5/survey/views/matrix.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4391 2023-03-21 21:10:13.000000 djaodjin-survey-0.9.5/survey/views/portfolios.py
--rw-r--r--   0 smirolo    (501) staff       (20)    11685 2023-03-21 20:44:41.000000 djaodjin-survey-0.9.5/survey/views/sample.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.934970 djaodjin-survey-0.9.6/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1318 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/LICENSE.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/MANIFEST.in
+-rw-r--r--   0 smirolo    (501) staff       (20)     1981 2023-04-28 01:52:28.935036 djaodjin-survey-0.9.6/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     1222 2023-04-28 01:50:26.000000 djaodjin-survey-0.9.6/README.md
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.917536 djaodjin-survey-0.9.6/djaodjin_survey.egg-info/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1981 2023-04-28 01:52:28.000000 djaodjin-survey-0.9.6/djaodjin_survey.egg-info/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     2399 2023-04-28 01:52:28.000000 djaodjin-survey-0.9.6/djaodjin_survey.egg-info/SOURCES.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        1 2023-04-28 01:52:28.000000 djaodjin-survey-0.9.6/djaodjin_survey.egg-info/dependency_links.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)       73 2023-04-28 01:52:28.000000 djaodjin-survey-0.9.6/djaodjin_survey.egg-info/requires.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        7 2023-04-28 01:52:28.000000 djaodjin-survey-0.9.6/djaodjin_survey.egg-info/top_level.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)     1358 2023-04-18 19:54:04.000000 djaodjin-survey-0.9.6/pyproject.toml
+-rw-r--r--   0 smirolo    (501) staff       (20)       79 2023-04-28 01:52:28.935243 djaodjin-survey-0.9.6/setup.cfg
+-rw-r--r--   0 smirolo    (501) staff       (20)     1381 2023-04-18 16:17:24.000000 djaodjin-survey-0.9.6/setup.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.921543 djaodjin-survey-0.9.6/survey/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1435 2023-04-28 01:50:37.000000 djaodjin-survey-0.9.6/survey/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1842 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/admin.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.924667 djaodjin-survey-0.9.6/survey/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     7333 2022-09-14 00:28:06.000000 djaodjin-survey-0.9.6/survey/api/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    45132 2023-04-20 22:58:59.000000 djaodjin-survey-0.9.6/survey/api/matrix.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    12575 2023-01-27 18:26:55.000000 djaodjin-survey-0.9.6/survey/api/metrics.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    23591 2023-03-23 22:52:31.000000 djaodjin-survey-0.9.6/survey/api/portfolios.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    56385 2023-04-07 16:36:46.000000 djaodjin-survey-0.9.6/survey/api/sample.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    23875 2023-04-20 22:58:12.000000 djaodjin-survey-0.9.6/survey/api/serializers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2929 2023-03-10 17:42:57.000000 djaodjin-survey-0.9.6/survey/api/serializers_overrides.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     5569 2023-04-13 17:06:50.000000 djaodjin-survey-0.9.6/survey/api/units.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4094 2022-09-26 17:15:24.000000 djaodjin-survey-0.9.6/survey/compat.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2316 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/docs.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    17450 2023-04-07 16:40:09.000000 djaodjin-survey-0.9.6/survey/filters.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     8639 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/forms.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6173 2023-04-05 16:25:51.000000 djaodjin-survey-0.9.6/survey/helpers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    14690 2023-04-18 18:56:44.000000 djaodjin-survey-0.9.6/survey/mixins.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    39683 2023-04-05 17:20:30.000000 djaodjin-survey-0.9.6/survey/models.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4007 2023-04-05 18:59:23.000000 djaodjin-survey-0.9.6/survey/pagination.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    13064 2023-04-05 17:26:46.000000 djaodjin-survey-0.9.6/survey/queries.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4395 2023-03-21 20:59:50.000000 djaodjin-survey-0.9.6/survey/settings.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1955 2022-10-04 20:48:04.000000 djaodjin-survey-0.9.6/survey/signals.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.915319 djaodjin-survey-0.9.6/survey/static/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.924927 djaodjin-survey-0.9.6/survey/static/css/
+-rw-r--r--   0 smirolo    (501) staff       (20)      296 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/static/css/matrix-chart.css
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.926879 djaodjin-survey-0.9.6/survey/static/js/
+-rw-r--r--   0 smirolo    (501) staff       (20)    12547 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/static/js/djaodjin-categorize.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    15443 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/static/js/djaodjin-matrix.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    51604 2023-04-14 15:55:35.000000 djaodjin-survey-0.9.6/survey/static/js/djaodjin-resources-vue.js
+-rw-r--r--   0 smirolo    (501) staff       (20)     5462 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/static/js/djaodjin-set.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    17193 2023-04-14 16:37:55.000000 djaodjin-survey-0.9.6/survey/static/js/djaodjin-survey-vue.js
+-rw-r--r--   0 smirolo    (501) staff       (20)      544 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/static/js/djaodjin-survey.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    12995 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/static/js/matrix-chart.js
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.915434 djaodjin-survey-0.9.6/survey/templates/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.928635 djaodjin-survey-0.9.6/survey/templates/survey/
+-rw-r--r--   0 smirolo    (501) staff       (20)      667 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/answer_form.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      249 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/campaign_form.html
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.928770 djaodjin-survey-0.9.6/survey/templates/survey/campaigns/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1184 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/campaigns/index.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     2529 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/categorize.html
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.929430 djaodjin-survey-0.9.6/survey/templates/survey/matrix/
+-rw-r--r--   0 smirolo    (501) staff       (20)       62 2023-01-19 22:34:30.000000 djaodjin-survey-0.9.6/survey/templates/survey/matrix/compare.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     2087 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/matrix/index.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     4088 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/matrix/matrix.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     9287 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/portfolios.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      249 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/question_form.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     1572 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/question_list.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      471 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/respondent_list.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     2077 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/result.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      983 2023-03-10 17:29:52.000000 djaodjin-survey-0.9.6/survey/templates/survey/result_quizz.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      562 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/sample_create.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      356 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/sample_update.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      245 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/send.html
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.929655 djaodjin-survey-0.9.6/survey/templatetags/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templatetags/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1769 2023-02-10 21:30:25.000000 djaodjin-survey-0.9.6/survey/templatetags/survey_tags.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.929873 djaodjin-survey-0.9.6/survey/urls/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1533 2022-09-25 23:08:10.000000 djaodjin-survey-0.9.6/survey/urls/__init__.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.931523 djaodjin-survey-0.9.6/survey/urls/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1718 2023-03-22 18:00:00.000000 djaodjin-survey-0.9.6/survey/urls/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1653 2022-09-26 00:12:56.000000 djaodjin-survey-0.9.6/survey/urls/api/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2772 2022-09-26 02:10:24.000000 djaodjin-survey-0.9.6/survey/urls/api/filters.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2125 2023-04-07 17:48:09.000000 djaodjin-survey-0.9.6/survey/urls/api/matrix.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1717 2022-09-26 00:13:35.000000 djaodjin-survey-0.9.6/survey/urls/api/metrics.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1622 2022-09-26 00:12:26.000000 djaodjin-survey-0.9.6/survey/urls/api/noauth.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2390 2023-03-07 21:45:05.000000 djaodjin-survey-0.9.6/survey/urls/api/portfolios.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.932192 djaodjin-survey-0.9.6/survey/urls/api/sample/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1512 2022-09-26 00:09:27.000000 djaodjin-survey-0.9.6/survey/urls/api/sample/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1722 2023-02-21 21:54:31.000000 djaodjin-survey-0.9.6/survey/urls/api/sample/reset.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2830 2023-04-07 17:59:33.000000 djaodjin-survey-0.9.6/survey/urls/api/sample/update.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.933471 djaodjin-survey-0.9.6/survey/urls/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1714 2023-03-22 18:07:23.000000 djaodjin-survey-0.9.6/survey/urls/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2942 2022-09-26 00:06:32.000000 djaodjin-survey-0.9.6/survey/urls/views/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2105 2023-01-19 22:50:22.000000 djaodjin-survey-0.9.6/survey/urls/views/matrices.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1894 2023-01-25 23:37:48.000000 djaodjin-survey-0.9.6/survey/urls/views/portfolios.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2180 2022-09-26 00:14:39.000000 djaodjin-survey-0.9.6/survey/urls/views/samples.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     9471 2023-04-20 22:32:58.000000 djaodjin-survey-0.9.6/survey/utils.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.934726 djaodjin-survey-0.9.6/survey/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     8457 2023-03-21 21:02:40.000000 djaodjin-survey-0.9.6/survey/views/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     5626 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/views/createquestion.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1898 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/views/edit.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6155 2023-04-07 17:48:37.000000 djaodjin-survey-0.9.6/survey/views/matrix.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4391 2023-03-21 21:10:13.000000 djaodjin-survey-0.9.6/survey/views/portfolios.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    11685 2023-03-21 20:44:41.000000 djaodjin-survey-0.9.6/survey/views/sample.py
```

### Comparing `djaodjin-survey-0.9.5/LICENSE.txt` & `djaodjin-survey-0.9.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/PKG-INFO` & `djaodjin-survey-0.9.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djaodjin-survey
-Version: 0.9.5
+Version: 0.9.6
 Summary: Django app for qualitative and quantitative surveys
 Author-email: The DjaoDjin Team <help@djaodjin.com>
 Maintainer-email: The DjaoDjin Team <help@djaodjin.com>
 License: BSD-2-Clause
 Project-URL: repository, https://github.com/djaodjin/djaodjin-survey
 Project-URL: documentation, https://djaodjin-survey.readthedocs.io/
 Project-URL: changelog, https://github.com/djaodjin/djaodjin-survey/changelog
@@ -45,18 +45,19 @@
 Releases
 ========
 
 Tested with
 
 - **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/))
 - **Python:** 3.10, **Django:** 4.2 (latest)
-- **Python:** 2.7, **Django:** 1.11 (legacy) (see testsite/requirements-legacy.txt)
+- **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
 
-0.9.4
+0.9.6
 
-  * publishes distribution using pyproject.toml
-  * edits a question default unit
+  * serializes default_unit.system correctly in benchmarks API
+  * renames data series name from 'printable_name' to 'title' for consistency
+  * computes rate on target dates
 
 [previous release notes](changelog)
 
 
 Models have been completely re-designed between version 0.1.7 and 0.2.0
```

### Comparing `djaodjin-survey-0.9.5/README.md` & `djaodjin-survey-0.9.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -26,18 +26,19 @@
 Releases
 ========
 
 Tested with
 
 - **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/))
 - **Python:** 3.10, **Django:** 4.2 (latest)
-- **Python:** 2.7, **Django:** 1.11 (legacy) (see testsite/requirements-legacy.txt)
+- **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
 
-0.9.4
+0.9.6
 
-  * publishes distribution using pyproject.toml
-  * edits a question default unit
+  * serializes default_unit.system correctly in benchmarks API
+  * renames data series name from 'printable_name' to 'title' for consistency
+  * computes rate on target dates
 
 [previous release notes](changelog)
 
 
 Models have been completely re-designed between version 0.1.7 and 0.2.0
```

### Comparing `djaodjin-survey-0.9.5/djaodjin_survey.egg-info/PKG-INFO` & `djaodjin-survey-0.9.6/djaodjin_survey.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djaodjin-survey
-Version: 0.9.5
+Version: 0.9.6
 Summary: Django app for qualitative and quantitative surveys
 Author-email: The DjaoDjin Team <help@djaodjin.com>
 Maintainer-email: The DjaoDjin Team <help@djaodjin.com>
 License: BSD-2-Clause
 Project-URL: repository, https://github.com/djaodjin/djaodjin-survey
 Project-URL: documentation, https://djaodjin-survey.readthedocs.io/
 Project-URL: changelog, https://github.com/djaodjin/djaodjin-survey/changelog
@@ -45,18 +45,19 @@
 Releases
 ========
 
 Tested with
 
 - **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/))
 - **Python:** 3.10, **Django:** 4.2 (latest)
-- **Python:** 2.7, **Django:** 1.11 (legacy) (see testsite/requirements-legacy.txt)
+- **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
 
-0.9.4
+0.9.6
 
-  * publishes distribution using pyproject.toml
-  * edits a question default unit
+  * serializes default_unit.system correctly in benchmarks API
+  * renames data series name from 'printable_name' to 'title' for consistency
+  * computes rate on target dates
 
 [previous release notes](changelog)
 
 
 Models have been completely re-designed between version 0.1.7 and 0.2.0
```

### Comparing `djaodjin-survey-0.9.5/djaodjin_survey.egg-info/SOURCES.txt` & `djaodjin-survey-0.9.6/djaodjin_survey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/pyproject.toml` & `djaodjin-survey-0.9.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/setup.py` & `djaodjin-survey-0.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/__init__.py` & `djaodjin-survey-0.9.6/survey/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """
 PEP 386-compliant version number for the survey django app.
 """
 
-__version__ = '0.9.5'
+__version__ = '0.9.6'
```

### Comparing `djaodjin-survey-0.9.5/survey/admin.py` & `djaodjin-survey-0.9.6/survey/admin.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/api/campaigns.py` & `djaodjin-survey-0.9.6/survey/api/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/api/matrix.py` & `djaodjin-survey-0.9.6/survey/api/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,43 +46,20 @@
     get_account_serializer, get_question_serializer)
 from .serializers import (AccountsFilterAddSerializer,
     CompareQuestionSerializer, EditableFilterSerializer, MatrixSerializer,
     SampleBenchmarksSerializer)
 
 LOGGER = logging.getLogger(__name__)
 
-
-class BenchmarkAPIView(QuestionMixin, DateRangeContextMixin, CampaignMixin,
-                       AccountMixin, generics.ListAPIView):
-    """
-    Aggregated benchmark for requested accounts
-
-    **Examples**:
-
-    .. code-block:: http
-
-        GET /api/energy-utility/reporting/sustainability/benchmarks\
-/sustainability HTTP/1.1
-
-    responds
-
-    .. code-block:: json
-
-
-        {
-          "count": 4,
-          "results": []
-        }
-    """
+class BenchmarkMixin(QuestionMixin, DateRangeContextMixin, CampaignMixin,
+                     AccountMixin):
     scale = 1
     default_unit = 'profiles'
     valid_units = ('percentage',)
     title = "Benchmarks"
-    serializer_class = SampleBenchmarksSerializer
-    pagination_class = MetricsPagination
 
     @property
     def unit(self):
         #pylint:disable=attribute-defined-outside-init
         if not hasattr(self, '_unit'):
             self._unit = self.default_unit
             param_unit = self.get_query_param('unit')
@@ -100,60 +77,91 @@
         """
         if not prefix.endswith(settings.DB_PATH_SEP):
             prefix = prefix + settings.DB_PATH_SEP
 
         questions_queryset = get_question_model().objects.filter(
             path__startswith=self.db_path).values(
             'pk', 'path', 'ui_hint', 'content__title',
-            'default_unit__slug', 'default_unit__title')
+            'default_unit__slug', 'default_unit__title',
+            'default_unit__system')
         questions_by_key = {question['pk']: {
             'path': question['path'],
             'title': question['content__title'],
             'ui_hint': question['ui_hint'],
             'default_unit': Unit(
                 slug=question['default_unit__slug'],
-                title=question['default_unit__title']),
+                title=question['default_unit__title'],
+                system=question['default_unit__system']),
         } for question in questions_queryset}
 
         self.attach_results(questions_by_key)
 
         return list(six.itervalues(questions_by_key))
 
-
-    def attach_results(self, questions_by_key, account=None):
-        if not account:
-            account = self.account
-
-        # samples that will be counted in the benchmark
+    def _attach_results(self, questions_by_key, accessible_accounts,
+                        title, slug):
         samples = []
-        accessible_accounts = self.get_accessible_accounts([account])
         if accessible_accounts:
             # Calling `get_completed_assessments_at_by` with an `accounts`
             # arguments evaluating to `False` will return all the latest
             # frozen samples.
             samples = Sample.objects.get_completed_assessments_at_by(
                 self.campaign,
                 start_at=self.start_at, ends_at=self.ends_at,
                 accounts=accessible_accounts)
 
+        # samples that will be counted in the benchmark
         if samples:
             questions_by_key = get_benchmarks_enumerated(
                 samples, questions_by_key.keys(), questions_by_key)
             for question in six.itervalues(questions_by_key):
                 if not 'benchmarks' in question:
                     question['benchmarks'] = []
                 account_benchmark = {
-                    'slug': account.slug,
-                    'printable_name': account.printable_name,
+                    'slug': slug,
+                    'title': title,
                     'values': []
                 }
                 for key, val in six.iteritems(question.get('rate', {})):
                     account_benchmark['values'] += [(key, int(val))]
                 question['benchmarks'] += [account_benchmark]
 
+
+    def attach_results(self, questions_by_key, account=None):
+        if not account:
+            account = self.account
+        accessible_accounts = self.get_accessible_accounts([account])
+        self._attach_results(questions_by_key, accessible_accounts,
+            account.printable_name, account.slug)
+
+
+class BenchmarkAPIView(BenchmarkMixin, generics.ListAPIView):
+    """
+    Aggregated benchmark for requested accounts
+
+    **Examples**:
+
+    .. code-block:: http
+
+        GET /api/energy-utility/reporting/sustainability/benchmarks\
+/sustainability HTTP/1.1
+
+    responds
+
+    .. code-block:: json
+
+
+        {
+          "count": 4,
+          "results": []
+        }
+    """
+    serializer_class = SampleBenchmarksSerializer
+    pagination_class = MetricsPagination
+
     def get_serializer_context(self):
         context = super(BenchmarkAPIView, self).get_serializer_context()
         context.update({
             'prefix': self.db_path if self.db_path else settings.DB_PATH_SEP,
         })
         return context
```

### Comparing `djaodjin-survey-0.9.5/survey/api/metrics.py` & `djaodjin-survey-0.9.6/survey/api/metrics.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/api/portfolios.py` & `djaodjin-survey-0.9.6/survey/api/portfolios.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/api/sample.py` & `djaodjin-survey-0.9.6/survey/api/sample.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/api/serializers.py` & `djaodjin-survey-0.9.6/survey/api/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -479,17 +479,17 @@
     max_length = 3
 
 
 class TableSerializer(NoModelSerializer):
 
     slug = serializers.SlugField(
         help_text=_("Unique key in the table for the data series"))
-    printable_name = serializers.CharField(
-        required=False, read_only=True,
-        help_text=_("Name that can be safely used for display in HTML pages"))
+    title = serializers.CharField(required=False, read_only=True,
+        help_text=_("Title of data serie that can be safely used for display"\
+        " in HTML pages"))
     extra = ExtraField(required=False,
         help_text=_("Extra meta data (can be stringify JSON)"))
     values = serializers.ListField(
         child=KeyValueTuple(),
         help_text="Datapoints in the serie")
 
 
@@ -509,15 +509,16 @@
         help_text=_("The scale of the number reported in the tables (ex: 1000"\
         " when numbers are reported in thousands)"))
     unit = serializers.SlugRelatedField(required=False, allow_null=True,
         queryset=Unit.objects.all(), slug_field='slug',
         help_text=_("Unit the measured field is in"))
     title = serializers.CharField(
         help_text=_("Title for the table"))
-    results = TableSerializer(many=True)
+    results = TableSerializer(many=True,
+        help_text=_("Data series"))
 
 
 class CompareQuestionSerializer(QuestionSerializer):
     """
     Serializer for a question in the `results` field of a Compare API call.
     """
     values = serializers.ListField(
```

### Comparing `djaodjin-survey-0.9.5/survey/api/serializers_overrides.py` & `djaodjin-survey-0.9.6/survey/api/serializers_overrides.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/api/units.py` & `djaodjin-survey-0.9.6/survey/api/units.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/compat.py` & `djaodjin-survey-0.9.6/survey/compat.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/docs.py` & `djaodjin-survey-0.9.6/survey/docs.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/filters.py` & `djaodjin-survey-0.9.6/survey/filters.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/forms.py` & `djaodjin-survey-0.9.6/survey/forms.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/helpers.py` & `djaodjin-survey-0.9.6/survey/helpers.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/mixins.py` & `djaodjin-survey-0.9.6/survey/mixins.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/models.py` & `djaodjin-survey-0.9.6/survey/models.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/pagination.py` & `djaodjin-survey-0.9.6/survey/pagination.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/queries.py` & `djaodjin-survey-0.9.6/survey/queries.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/settings.py` & `djaodjin-survey-0.9.6/survey/settings.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/signals.py` & `djaodjin-survey-0.9.6/survey/signals.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/static/js/djaodjin-categorize.js` & `djaodjin-survey-0.9.6/survey/static/js/djaodjin-categorize.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/static/js/djaodjin-matrix.js` & `djaodjin-survey-0.9.6/survey/static/js/djaodjin-matrix.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/static/js/djaodjin-resources-vue.js` & `djaodjin-survey-0.9.6/survey/static/js/djaodjin-resources-vue.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/static/js/djaodjin-set.js` & `djaodjin-survey-0.9.6/survey/static/js/djaodjin-set.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/static/js/djaodjin-survey-vue.js` & `djaodjin-survey-0.9.6/survey/static/js/djaodjin-survey-vue.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/static/js/djaodjin-survey.js` & `djaodjin-survey-0.9.6/survey/static/js/djaodjin-survey.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/static/js/matrix-chart.js` & `djaodjin-survey-0.9.6/survey/static/js/matrix-chart.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/templates/survey/answer_form.html` & `djaodjin-survey-0.9.6/survey/templates/survey/answer_form.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/templates/survey/campaigns/index.html` & `djaodjin-survey-0.9.6/survey/templates/survey/campaigns/index.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/templates/survey/categorize.html` & `djaodjin-survey-0.9.6/survey/templates/survey/categorize.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/templates/survey/matrix/index.html` & `djaodjin-survey-0.9.6/survey/templates/survey/matrix/index.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/templates/survey/matrix/matrix.html` & `djaodjin-survey-0.9.6/survey/templates/survey/matrix/matrix.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/templates/survey/portfolios.html` & `djaodjin-survey-0.9.6/survey/templates/survey/portfolios.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/templates/survey/question_list.html` & `djaodjin-survey-0.9.6/survey/templates/survey/question_list.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/templates/survey/result.html` & `djaodjin-survey-0.9.6/survey/templates/survey/result.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/templates/survey/result_quizz.html` & `djaodjin-survey-0.9.6/survey/templates/survey/result_quizz.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/templates/survey/sample_create.html` & `djaodjin-survey-0.9.6/survey/templates/survey/sample_create.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/templatetags/survey_tags.py` & `djaodjin-survey-0.9.6/survey/templatetags/survey_tags.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/urls/__init__.py` & `djaodjin-survey-0.9.6/survey/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/urls/api/__init__.py` & `djaodjin-survey-0.9.6/survey/urls/api/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/urls/api/campaigns.py` & `djaodjin-survey-0.9.6/survey/urls/api/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/urls/api/filters.py` & `djaodjin-survey-0.9.6/survey/urls/api/filters.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/urls/api/matrix.py` & `djaodjin-survey-0.9.6/survey/urls/api/matrix.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/urls/api/metrics.py` & `djaodjin-survey-0.9.6/survey/urls/api/metrics.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/urls/api/noauth.py` & `djaodjin-survey-0.9.6/survey/urls/api/noauth.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/urls/api/portfolios.py` & `djaodjin-survey-0.9.6/survey/urls/api/portfolios.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/urls/api/sample/__init__.py` & `djaodjin-survey-0.9.6/survey/urls/api/sample/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/urls/api/sample/reset.py` & `djaodjin-survey-0.9.6/survey/urls/api/sample/reset.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/urls/api/sample/update.py` & `djaodjin-survey-0.9.6/survey/urls/api/sample/update.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/urls/views/__init__.py` & `djaodjin-survey-0.9.6/survey/urls/views/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/urls/views/campaigns.py` & `djaodjin-survey-0.9.6/survey/urls/views/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/urls/views/matrices.py` & `djaodjin-survey-0.9.6/survey/urls/views/matrices.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/urls/views/portfolios.py` & `djaodjin-survey-0.9.6/survey/urls/views/portfolios.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/urls/views/samples.py` & `djaodjin-survey-0.9.6/survey/urls/views/samples.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/utils.py` & `djaodjin-survey-0.9.6/survey/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,21 +123,23 @@
         path = row['question__path']
         value = questions_by_key.get(question_pk, {'path': path})
         value.update({'nb_respondents': count})
         if question_pk not in questions_by_key:
             questions_by_key.update({question_pk: value})
 
     # per-choice number of answers
-    for row in Answer.objects.filter(
+    enum_answers = Answer.objects.filter(
             question__in=questions,
             unit_id=F('question__default_unit_id'),
             sample_id__in=samples,
-            question__default_unit__system=Unit.SYSTEM_ENUMERATED,
+            question__default_unit__system__in=[Unit.SYSTEM_ENUMERATED,
+                Unit.SYSTEM_DATETIME], # XXX target year are stored as choices
             unit__enums__id=F('measured')).values('question__id',
-                'measured', 'unit__enums__text').annotate(Count('sample_id')):
+                'unit__enums__text').annotate(Count('sample_id'))
+    for row in enum_answers:
         question_pk = row['question__id']
         count = row['sample_id__count']
         measured = row['unit__enums__text']
         value = questions_by_key.get(question_pk)
         total = value.get('nb_respondents', None)
         rate = value.get('rate', {})
         rate.update({
```

### Comparing `djaodjin-survey-0.9.5/survey/views/campaigns.py` & `djaodjin-survey-0.9.6/survey/views/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/views/createquestion.py` & `djaodjin-survey-0.9.6/survey/views/createquestion.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/views/edit.py` & `djaodjin-survey-0.9.6/survey/views/edit.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/views/matrix.py` & `djaodjin-survey-0.9.6/survey/views/matrix.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/views/portfolios.py` & `djaodjin-survey-0.9.6/survey/views/portfolios.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.5/survey/views/sample.py` & `djaodjin-survey-0.9.6/survey/views/sample.py`

 * *Files identical despite different names*

