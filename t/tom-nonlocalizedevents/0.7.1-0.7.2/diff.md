# Comparing `tmp/tom_nonlocalizedevents-0.7.1.tar.gz` & `tmp/tom_nonlocalizedevents-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tom_nonlocalizedevents-0.7.1.tar", max compression
+gzip compressed data, was "tom_nonlocalizedevents-0.7.2.tar", max compression
```

## Comparing `tom_nonlocalizedevents-0.7.1.tar` & `tom_nonlocalizedevents-0.7.2.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0    35149 2023-04-27 23:47:39.937205 tom_nonlocalizedevents-0.7.1/LICENSE
--rw-r--r--   0        0        0     5324 2023-04-27 23:47:39.937205 tom_nonlocalizedevents-0.7.1/README.md
--rw-r--r--   0        0        0     2632 2023-04-27 23:48:03.054996 tom_nonlocalizedevents-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      144 2023-04-27 23:48:03.054996 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/__init__.py
--rw-r--r--   0        0        0      459 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/admin.py
--rw-r--r--   0        0        0        0 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/alertstream_handlers/__init__.py
--rw-r--r--   0        0        0     5307 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/alertstream_handlers/gcn_event_handler.py
--rw-r--r--   0        0        0     4359 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/alertstream_handlers/igwn_event_handler.py
--rw-r--r--   0        0        0      228 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/apps.py
--rw-r--r--   0        0        0    12419 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/healpix_utils.py
--rw-r--r--   0        0        0     3766 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/ingestion.py
--rw-r--r--   0        0        0      437 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0001_initial.py
--rw-r--r--   0        0        0      585 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0002_superevent.py
--rw-r--r--   0        0        0     1075 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0003_auto_20210225_0034.py
--rw-r--r--   0        0        0      460 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0004_superevent_superevent_type.py
--rw-r--r--   0        0        0      543 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0005_auto_20210319_2241.py
--rw-r--r--   0        0        0     1015 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0006_auto_20210827_2346.py
--rw-r--r--   0        0        0      409 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0007_eventcandidate_viable.py
--rw-r--r--   0        0        0      411 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0008_eventcandidate_priority.py
--rw-r--r--   0        0        0      365 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0009_rename_superevent_nonlocalizedevent.py
--rw-r--r--   0        0        0     1434 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0010_rename_more_superevent_fields.py
--rw-r--r--   0        0        0     2028 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0011_eventcandidate_viability_reason_and_more.py
--rw-r--r--   0        0        0      574 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0012_nonlocalizedevent_event_subtype.py
--rw-r--r--   0        0        0     2510 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0013_eventcandidate_healpix_and_more.py
--rw-r--r--   0        0        0     2082 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0014_credibleregion_and_more.py
--rw-r--r--   0        0        0     4567 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0015_eventsequence_and_more.py
--rw-r--r--   0        0        0     3814 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0016_externalcoincidence_alter_eventsequence_options_and_more.py
--rw-r--r--   0        0        0        0 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/__init__.py
--rw-r--r--   0        0        0     9742 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/models.py
--rw-r--r--   0        0        0     6850 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/serializers.py
--rw-r--r--   0        0        0        0 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/signals/__init__.py
--rw-r--r--   0        0        0     1459 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/signals/handlers.py
--rw-r--r--   0        0        0       99 2023-04-27 23:47:39.945206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/static/tom_nonlocalizedevents/css/main.css
--rw-r--r--   0        0        0   218067 2023-04-27 23:47:39.945206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/css/superevent_vue_app.css
--rw-r--r--   0        0        0  1780610 2023-04-27 23:47:39.957207 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/js/superevent_vue_app.js
--rw-r--r--   0        0        0      416 2023-04-27 23:47:39.957207 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/webpack-stats.json
--rw-r--r--   0        0        0      168 2023-04-27 23:47:39.957207 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/detail.html
--rw-r--r--   0        0        0     1606 2023-04-27 23:47:39.957207 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/index.html
--rw-r--r--   0        0        0      490 2023-04-27 23:47:39.957207 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/superevent_vue_app.html
--rw-r--r--   0        0        0        0 2023-04-27 23:47:39.957207 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/tests/__init__.py
--rw-r--r--   0        0        0      693 2023-04-27 23:47:39.957207 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/tests/factories.py
--rw-r--r--   0        0        0     2879 2023-04-27 23:47:39.957207 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/tests/tests.py
--rw-r--r--   0        0        0     1120 2023-04-27 23:47:39.957207 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/urls.py
--rw-r--r--   0        0        0     6577 2023-04-27 23:47:39.957207 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/views.py
--rw-r--r--   0        0        0     7523 1970-01-01 00:00:00.000000 tom_nonlocalizedevents-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-28 21:04:24.549482 tom_nonlocalizedevents-0.7.2/LICENSE
+-rw-r--r--   0        0        0     5324 2023-04-28 21:04:24.549482 tom_nonlocalizedevents-0.7.2/README.md
+-rw-r--r--   0        0        0     2632 2023-04-28 21:04:49.621361 tom_nonlocalizedevents-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      144 2023-04-28 21:04:49.621361 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/__init__.py
+-rw-r--r--   0        0        0      459 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/admin.py
+-rw-r--r--   0        0        0        0 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/alertstream_handlers/__init__.py
+-rw-r--r--   0        0        0     5307 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/alertstream_handlers/gcn_event_handler.py
+-rw-r--r--   0        0        0     4359 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/alertstream_handlers/igwn_event_handler.py
+-rw-r--r--   0        0        0      228 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/apps.py
+-rw-r--r--   0        0        0    12419 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/healpix_utils.py
+-rw-r--r--   0        0        0     3766 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/ingestion.py
+-rw-r--r--   0        0        0      437 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0001_initial.py
+-rw-r--r--   0        0        0      585 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0002_superevent.py
+-rw-r--r--   0        0        0     1075 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0003_auto_20210225_0034.py
+-rw-r--r--   0        0        0      460 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0004_superevent_superevent_type.py
+-rw-r--r--   0        0        0      543 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0005_auto_20210319_2241.py
+-rw-r--r--   0        0        0     1015 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0006_auto_20210827_2346.py
+-rw-r--r--   0        0        0      409 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0007_eventcandidate_viable.py
+-rw-r--r--   0        0        0      411 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0008_eventcandidate_priority.py
+-rw-r--r--   0        0        0      365 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0009_rename_superevent_nonlocalizedevent.py
+-rw-r--r--   0        0        0     1434 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0010_rename_more_superevent_fields.py
+-rw-r--r--   0        0        0     2028 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0011_eventcandidate_viability_reason_and_more.py
+-rw-r--r--   0        0        0      574 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0012_nonlocalizedevent_event_subtype.py
+-rw-r--r--   0        0        0     2510 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0013_eventcandidate_healpix_and_more.py
+-rw-r--r--   0        0        0     2082 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0014_credibleregion_and_more.py
+-rw-r--r--   0        0        0     4567 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0015_eventsequence_and_more.py
+-rw-r--r--   0        0        0     3814 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0016_externalcoincidence_alter_eventsequence_options_and_more.py
+-rw-r--r--   0        0        0      872 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0017_alter_eventsequence_external_coincidence_and_more.py
+-rw-r--r--   0        0        0        0 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/__init__.py
+-rw-r--r--   0        0        0     9757 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/models.py
+-rw-r--r--   0        0        0     6850 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/serializers.py
+-rw-r--r--   0        0        0        0 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/signals/__init__.py
+-rw-r--r--   0        0        0     1459 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/signals/handlers.py
+-rw-r--r--   0        0        0       99 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/static/tom_nonlocalizedevents/css/main.css
+-rw-r--r--   0        0        0   218067 2023-04-28 21:04:24.553482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/css/superevent_vue_app.css
+-rw-r--r--   0        0        0  1780610 2023-04-28 21:04:24.565482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/js/superevent_vue_app.js
+-rw-r--r--   0        0        0      416 2023-04-28 21:04:24.565482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/webpack-stats.json
+-rw-r--r--   0        0        0      168 2023-04-28 21:04:24.565482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/detail.html
+-rw-r--r--   0        0        0     1606 2023-04-28 21:04:24.565482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/index.html
+-rw-r--r--   0        0        0      490 2023-04-28 21:04:24.565482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/superevent_vue_app.html
+-rw-r--r--   0        0        0        0 2023-04-28 21:04:24.565482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/tests/__init__.py
+-rw-r--r--   0        0        0      693 2023-04-28 21:04:24.565482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/tests/factories.py
+-rw-r--r--   0        0        0     2879 2023-04-28 21:04:24.565482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/tests/tests.py
+-rw-r--r--   0        0        0     1120 2023-04-28 21:04:24.565482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/urls.py
+-rw-r--r--   0        0        0     6577 2023-04-28 21:04:24.565482 tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/views.py
+-rw-r--r--   0        0        0     7523 1970-01-01 00:00:00.000000 tom_nonlocalizedevents-0.7.2/PKG-INFO
```

### Comparing `tom_nonlocalizedevents-0.7.1/LICENSE` & `tom_nonlocalizedevents-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/README.md` & `tom_nonlocalizedevents-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/pyproject.toml` & `tom_nonlocalizedevents-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "tom-nonlocalizedevents"
 # this version is a placeholder: version supplied by poetry-dynamic-versioning
-version = "0.7.1"
+version = "0.7.2"
 description = "Reusable TOMToolkit app to support gravitational wave superevent and other nonlocalized event EM follow-up observations."
 authors = ["TOM Toolkit Project <tomtoolkit@lco.global>", "David Collom <dcollom@lco.global>", "Lindy Lindstrom <llindstrom@lco.global>", "Jonathan Nation <jnation@lco.global>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/TOMToolkit/tom_nonlocalizedevents"
 keywords = ["tomtoolkit", "astronomy", "astrophysics", "cosmology", "science"]
 classifiers = [
```

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/alertstream_handlers/gcn_event_handler.py` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/alertstream_handlers/gcn_event_handler.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/alertstream_handlers/igwn_event_handler.py` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/alertstream_handlers/igwn_event_handler.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/healpix_utils.py` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/healpix_utils.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/ingestion.py` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/ingestion.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0002_superevent.py` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0002_superevent.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0003_auto_20210225_0034.py` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0003_auto_20210225_0034.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0005_auto_20210319_2241.py` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0005_auto_20210319_2241.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0006_auto_20210827_2346.py` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0006_auto_20210827_2346.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0010_rename_more_superevent_fields.py` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0010_rename_more_superevent_fields.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0011_eventcandidate_viability_reason_and_more.py` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0011_eventcandidate_viability_reason_and_more.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0012_nonlocalizedevent_event_subtype.py` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0012_nonlocalizedevent_event_subtype.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0013_eventcandidate_healpix_and_more.py` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0013_eventcandidate_healpix_and_more.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0014_credibleregion_and_more.py` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0014_credibleregion_and_more.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0015_eventsequence_and_more.py` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0015_eventsequence_and_more.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0016_externalcoincidence_alter_eventsequence_options_and_more.py` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/migrations/0016_externalcoincidence_alter_eventsequence_options_and_more.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/models.py` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
     )
     event_subtype = models.CharField(
         max_length=256,
         default='',
         help_text='The subtype of the event. Options are type specific, i.e. GW events have initial, '
                   'preliminary, update types.'
     )
-    ingestor_source = models.CharField(default='', help_text='The source of this alert - i.e. which stream is it from?')
+    ingestor_source = models.CharField(default='', max_length=64, help_text='The source of this alert - i.e. which stream is it from?')
     created = models.DateTimeField(auto_now_add=True)
     modified = models.DateTimeField(auto_now=True)
 
     class Meta:
         ordering = ["sequence_id"]
         constraints = [
             models.UniqueConstraint(
```

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/serializers.py` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/serializers.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/signals/handlers.py` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/css/superevent_vue_app.css` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/css/superevent_vue_app.css`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/js/superevent_vue_app.js` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/js/superevent_vue_app.js`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/index.html` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/index.html`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/tests/factories.py` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/tests/factories.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/tests/tests.py` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/tests/tests.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/urls.py` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/urls.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/views.py` & `tom_nonlocalizedevents-0.7.2/tom_nonlocalizedevents/views.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.1/PKG-INFO` & `tom_nonlocalizedevents-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tom-nonlocalizedevents
-Version: 0.7.1
+Version: 0.7.2
 Summary: Reusable TOMToolkit app to support gravitational wave superevent and other nonlocalized event EM follow-up observations.
 Home-page: https://github.com/TOMToolkit/tom_nonlocalizedevents
 License: GPL-3.0-only
 Keywords: tomtoolkit,astronomy,astrophysics,cosmology,science
 Author: TOM Toolkit Project
 Author-email: tomtoolkit@lco.global
 Requires-Python: >=3.8,<3.12
```

