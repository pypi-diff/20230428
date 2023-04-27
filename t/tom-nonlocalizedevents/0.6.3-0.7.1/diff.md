# Comparing `tmp/tom_nonlocalizedevents-0.6.3.tar.gz` & `tmp/tom_nonlocalizedevents-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tom_nonlocalizedevents-0.6.3.tar", max compression
+gzip compressed data, was "tom_nonlocalizedevents-0.7.1.tar", max compression
```

## Comparing `tom_nonlocalizedevents-0.6.3.tar` & `tom_nonlocalizedevents-0.7.1.tar`

### file list

```diff
@@ -1,42 +1,45 @@
--rw-r--r--   0        0        0    35149 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/LICENSE
--rw-r--r--   0        0        0     4715 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/README.md
--rw-r--r--   0        0        0     2643 2023-04-05 00:45:35.957812 tom_nonlocalizedevents-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      144 2023-04-05 00:45:35.961812 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/__init__.py
--rw-r--r--   0        0        0      301 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/admin.py
--rw-r--r--   0        0        0        0 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/alertstream_handlers/__init__.py
--rw-r--r--   0        0        0     4355 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/alertstream_handlers/gw_event_handler.py
--rw-r--r--   0        0        0      228 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/apps.py
--rw-r--r--   0        0        0     8600 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/healpix_utils.py
--rw-r--r--   0        0        0      437 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0001_initial.py
--rw-r--r--   0        0        0      585 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0002_superevent.py
--rw-r--r--   0        0        0     1075 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0003_auto_20210225_0034.py
--rw-r--r--   0        0        0      460 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0004_superevent_superevent_type.py
--rw-r--r--   0        0        0      543 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0005_auto_20210319_2241.py
--rw-r--r--   0        0        0     1015 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0006_auto_20210827_2346.py
--rw-r--r--   0        0        0      409 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0007_eventcandidate_viable.py
--rw-r--r--   0        0        0      411 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0008_eventcandidate_priority.py
--rw-r--r--   0        0        0      365 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0009_rename_superevent_nonlocalizedevent.py
--rw-r--r--   0        0        0     1434 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0010_rename_more_superevent_fields.py
--rw-r--r--   0        0        0     2028 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0011_eventcandidate_viability_reason_and_more.py
--rw-r--r--   0        0        0      574 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0012_nonlocalizedevent_event_subtype.py
--rw-r--r--   0        0        0     2510 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0013_eventcandidate_healpix_and_more.py
--rw-r--r--   0        0        0     2082 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0014_credibleregion_and_more.py
--rw-r--r--   0        0        0     4567 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0015_eventsequence_and_more.py
--rw-r--r--   0        0        0        0 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/__init__.py
--rw-r--r--   0        0        0     8780 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/models.py
--rw-r--r--   0        0        0     6666 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/serializers.py
--rw-r--r--   0        0        0        0 2023-04-05 00:45:16.169905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/signals/__init__.py
--rw-r--r--   0        0        0     1459 2023-04-05 00:45:16.173905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/signals/handlers.py
--rw-r--r--   0        0        0       99 2023-04-05 00:45:16.173905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/static/tom_nonlocalizedevents/css/main.css
--rw-r--r--   0        0        0   218067 2023-04-05 00:45:16.173905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/css/superevent_vue_app.css
--rw-r--r--   0        0        0  1778632 2023-04-05 00:45:16.181905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/js/superevent_vue_app.js
--rw-r--r--   0        0        0      416 2023-04-05 00:45:16.181905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/webpack-stats.json
--rw-r--r--   0        0        0      168 2023-04-05 00:45:16.181905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/detail.html
--rw-r--r--   0        0        0     1606 2023-04-05 00:45:16.185905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/index.html
--rw-r--r--   0        0        0      539 2023-04-05 00:45:16.185905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/superevent_vue_app.html
--rw-r--r--   0        0        0        0 2023-04-05 00:45:16.185905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/tests/__init__.py
--rw-r--r--   0        0        0      702 2023-04-05 00:45:16.185905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/tests/factories.py
--rw-r--r--   0        0        0     2907 2023-04-05 00:45:16.185905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/tests/tests.py
--rw-r--r--   0        0        0     1120 2023-04-05 00:45:16.185905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/urls.py
--rw-r--r--   0        0        0     8500 2023-04-05 00:45:16.185905 tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/views.py
--rw-r--r--   0        0        0     6856 1970-01-01 00:00:00.000000 tom_nonlocalizedevents-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-27 23:47:39.937205 tom_nonlocalizedevents-0.7.1/LICENSE
+-rw-r--r--   0        0        0     5324 2023-04-27 23:47:39.937205 tom_nonlocalizedevents-0.7.1/README.md
+-rw-r--r--   0        0        0     2632 2023-04-27 23:48:03.054996 tom_nonlocalizedevents-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      144 2023-04-27 23:48:03.054996 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/__init__.py
+-rw-r--r--   0        0        0      459 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/admin.py
+-rw-r--r--   0        0        0        0 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/alertstream_handlers/__init__.py
+-rw-r--r--   0        0        0     5307 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/alertstream_handlers/gcn_event_handler.py
+-rw-r--r--   0        0        0     4359 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/alertstream_handlers/igwn_event_handler.py
+-rw-r--r--   0        0        0      228 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/apps.py
+-rw-r--r--   0        0        0    12419 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/healpix_utils.py
+-rw-r--r--   0        0        0     3766 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/ingestion.py
+-rw-r--r--   0        0        0      437 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0001_initial.py
+-rw-r--r--   0        0        0      585 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0002_superevent.py
+-rw-r--r--   0        0        0     1075 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0003_auto_20210225_0034.py
+-rw-r--r--   0        0        0      460 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0004_superevent_superevent_type.py
+-rw-r--r--   0        0        0      543 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0005_auto_20210319_2241.py
+-rw-r--r--   0        0        0     1015 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0006_auto_20210827_2346.py
+-rw-r--r--   0        0        0      409 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0007_eventcandidate_viable.py
+-rw-r--r--   0        0        0      411 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0008_eventcandidate_priority.py
+-rw-r--r--   0        0        0      365 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0009_rename_superevent_nonlocalizedevent.py
+-rw-r--r--   0        0        0     1434 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0010_rename_more_superevent_fields.py
+-rw-r--r--   0        0        0     2028 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0011_eventcandidate_viability_reason_and_more.py
+-rw-r--r--   0        0        0      574 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0012_nonlocalizedevent_event_subtype.py
+-rw-r--r--   0        0        0     2510 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0013_eventcandidate_healpix_and_more.py
+-rw-r--r--   0        0        0     2082 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0014_credibleregion_and_more.py
+-rw-r--r--   0        0        0     4567 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0015_eventsequence_and_more.py
+-rw-r--r--   0        0        0     3814 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0016_externalcoincidence_alter_eventsequence_options_and_more.py
+-rw-r--r--   0        0        0        0 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/__init__.py
+-rw-r--r--   0        0        0     9742 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/models.py
+-rw-r--r--   0        0        0     6850 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/serializers.py
+-rw-r--r--   0        0        0        0 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/signals/__init__.py
+-rw-r--r--   0        0        0     1459 2023-04-27 23:47:39.941206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/signals/handlers.py
+-rw-r--r--   0        0        0       99 2023-04-27 23:47:39.945206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/static/tom_nonlocalizedevents/css/main.css
+-rw-r--r--   0        0        0   218067 2023-04-27 23:47:39.945206 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/css/superevent_vue_app.css
+-rw-r--r--   0        0        0  1780610 2023-04-27 23:47:39.957207 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/js/superevent_vue_app.js
+-rw-r--r--   0        0        0      416 2023-04-27 23:47:39.957207 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/webpack-stats.json
+-rw-r--r--   0        0        0      168 2023-04-27 23:47:39.957207 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/detail.html
+-rw-r--r--   0        0        0     1606 2023-04-27 23:47:39.957207 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/index.html
+-rw-r--r--   0        0        0      490 2023-04-27 23:47:39.957207 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/superevent_vue_app.html
+-rw-r--r--   0        0        0        0 2023-04-27 23:47:39.957207 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/tests/__init__.py
+-rw-r--r--   0        0        0      693 2023-04-27 23:47:39.957207 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/tests/factories.py
+-rw-r--r--   0        0        0     2879 2023-04-27 23:47:39.957207 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/tests/tests.py
+-rw-r--r--   0        0        0     1120 2023-04-27 23:47:39.957207 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/urls.py
+-rw-r--r--   0        0        0     6577 2023-04-27 23:47:39.957207 tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/views.py
+-rw-r--r--   0        0        0     7523 1970-01-01 00:00:00.000000 tom_nonlocalizedevents-0.7.1/PKG-INFO
```

### Comparing `tom_nonlocalizedevents-0.6.3/LICENSE` & `tom_nonlocalizedevents-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.6.3/README.md` & `tom_nonlocalizedevents-0.7.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![pypi](https://img.shields.io/pypi/v/tom-superevents.svg)](https://pypi.python.org/pypi/tom-superevents)
+[![pypi](https://img.shields.io/pypi/v/tom-nonlocalizedevents.svg)](https://pypi.python.org/pypi/tom-nonlocalizedevents)
 [![run-tests](https://github.com/TOMToolkit/tom_nonlocalizedevents/actions/workflows/run-tests.yml/badge.svg)](https://github.com/TOMToolkit/tom_nonlocalizedevents/actions/workflows/run-tests.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/cbcf7ce565d8450f86fff863ef061ff9)](https://www.codacy.com/gh/TOMToolkit/tom_nonlocalizedevents/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=TOMToolkit/tom_nonlocalizedevents&amp;utm_campaign=Badge_Grade)
 [![Coverage Status](https://coveralls.io/repos/github/TOMToolkit/tom_nonlocalizedevents/badge.svg?branch=main)](https://coveralls.io/github/TOMToolkit/tom_nonlocalizedevents?branch=main)
 
 # GW Superevent (or GRB, Neutrino) EM follow-up
 
 This reusable TOM Toolkit app provides support for gravitational wave (GW) superevent
@@ -66,18 +66,19 @@
 
 5. Set environment variables below to configure different connections:
 
 | Env variable | Description | Default |
 | ------------ | ----------- | ------- |
 | `SA_DB_CONNECTION_URL` | Location of your django postgres database used for sqlalchemy | by default, this uses Django `default` DB for the project |
 | `CREDIBLE_REGION_PROBABILITIES` | JSON List of Credible Region probabilities to automatically check each candidate target for | `'[0.25, 0.5, 0.75, 0.9, 0.95]'` |
+| `SAVE_TEST_ALERTS` | Boolean on if you want to save test nonlocalizedevents into your database (those with event_id beginning with 'M') | `true` |
 
 6. In your TOM project, make sure to run `python manage.py collectstatic` after installing this app, to collect its Vue pages into your `staticfiles` directory.
 
-7. If you want to automatically ingest GW events into your TOM, you should also install the `tom_alertstreams` app into your TOM and configure it to use the tom_nonlocalizedevents handler to ingest GW events: `tom_nonlocalizedevents.alertstream_handlers.gw_event_handler.handle_message`. There is also a handler to handle retractions via the `handle_retraction` method in that package. These are currently written to work with LVC GW messages.
+7. If you want to automatically ingest GW events into your TOM, you should also install the `tom_alertstreams` app into your TOM and configure it to use the tom_nonlocalizedevents handler to ingest GW events. The preferred way is to use the hop `igwn.gwalerts` topic and set it to the handler `tom_nonlocalizedevents.alertstream_handlers.igwn_event_handler.handle_igwn_message`. This format has the newest Ligo O4 fields. There is legacy support for the gcn classic over kafka plaintext formatted LVC alerts using the handler `tom_nonlocalizedevents.alertstream_handlers.gcn_event_handler.handle_message`. There is also a handler to handle retractions via the `handle_retraction` method in that package. For an example of what needs to be in your settings to configure `tom_alertstreams` for these streams, look [here](https://github.com/LCOGT/hermes/blob/dev/hermes_base/settings.py#L232)
 
 ## Development
 
 When any changes are made to this library, the vue files will need to be build and bundled and committed into the repo so that they can be bundled and deployed with the django package. This means that after making any vue changes, you must run `npm run build` within the `tom_nonlocalizedevents_vue` directory once, which will install the built files into `tom_nonlocalizedevents/static/`, and then those built files will need to be committed into the repo. This allows django projects using this library to get those files when running `python manage.py collectstatic`.
 
 ## Running the tests
```

### Comparing `tom_nonlocalizedevents-0.6.3/pyproject.toml` & `tom_nonlocalizedevents-0.7.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "tom-nonlocalizedevents"
 # this version is a placeholder: version supplied by poetry-dynamic-versioning
-version = "0.6.3"
+version = "0.7.1"
 description = "Reusable TOMToolkit app to support gravitational wave superevent and other nonlocalized event EM follow-up observations."
 authors = ["TOM Toolkit Project <tomtoolkit@lco.global>", "David Collom <dcollom@lco.global>", "Lindy Lindstrom <llindstrom@lco.global>", "Jonathan Nation <jnation@lco.global>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/TOMToolkit/tom_nonlocalizedevents"
 keywords = ["tomtoolkit", "astronomy", "astrophysics", "cosmology", "science"]
 classifiers = [
@@ -30,25 +30,26 @@
     { include = "tom_nonlocalizedevents" }
 ]
 
 [tool.setuptools_scm]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
+astropy = ">=5.2"
 gracedb-sdk = "^0.1"
+hop-client = ">=0.8"
 python-dateutil = "^2.8"
 django-webpack-loader = "1.6.0"
 tomtoolkit = "^2.10"
 voevent-parse = "^1.0"
 django-filter = ">=21.0 <22.0"
-healpix-alchemy = ">=1.0.0"
+healpix-alchemy = ">=1.0.2"
 astropy-healpix = ">=0.7"
-# pinning to 0.11.0 b/c 0.12.0 removes IntervalSet
-MOCPy = "==0.11.0"
-SQLAlchemy = "^1.4.42"
+MOCPy = ">=0.12.2"
+SQLAlchemy = ">=1.4.42"
 psycopg2-binary = "^2.9.4"
 "ligo.skymap" = "^1.0.3"
 
 [tool.poetry.dev-dependencies]
 coverage = "^6.3.2"
 factory_boy = "^3.1.0"
 pytest = "^3.0.3"
```

### Comparing `tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/alertstream_handlers/gw_event_handler.py` & `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/alertstream_handlers/gcn_event_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 ''' This class defines a message handler for a tom_alertstreams connection to GW events
 
 '''
 import logging
 import os
 import traceback
+import requests
+from django.conf import settings
 
 from tom_nonlocalizedevents.models import NonLocalizedEvent, EventSequence
-from tom_nonlocalizedevents.healpix_utils import create_localization_for_multiorder_fits
+from tom_nonlocalizedevents.healpix_utils import create_localization_for_skymap
 
 logger = logging.getLogger(__name__)
 
 
 EXPECTED_FIELDS = [
-    'TRIGGER_NUM',
-    'SEQUENCE_NUM',
-    'NOTICE_TYPE',
-    'SKYMAP_FITS_URL'
+    'trigger_num',
+    'sequence_num',
+    'notice_type',
+    'skymap_fits_url'
 ]
 
 
-def extract_fields(message, expected_fields):
-    fields = {}
-    keys = message.split('\n')
-    for key in keys:
-        if key:
-            field_name = key.split(':')[0]
-            if field_name in expected_fields:
-                fields[field_name] = key.split(':', maxsplit=1)[1].strip()
-    if set(expected_fields) != set(fields.keys()):
-        logger.warning(f"Incoming GW message did not have the expected fields, ignoring it: {keys}")
-        return {}
-
-    return fields
+def extract_all_fields(message):
+    parsed_fields = {}
+    for line in message.splitlines():
+        entry = line.split(':', maxsplit=1)
+        if len(entry) > 1:
+            if entry[0].strip() == 'COMMENTS' and 'comments' in parsed_fields:
+                parsed_fields['comments'] += entry[1].lstrip()
+            else:
+                parsed_fields[entry[0].strip().lower()] = entry[1].strip()
+    return parsed_fields
 
 
 def get_moc_url_from_skymap_fits_url(skymap_fits_url):
     base, filename = os.path.split(skymap_fits_url)
     # Repair broken skymap filenames given in gcn mock alerts right now
     if filename.endswith('.fit'):
         filename = filename + 's'
@@ -44,62 +43,87 @@
     filename = filename.replace('bayestar.fits.gz', 'bayestar.multiorder.fits')
     return os.path.join(base, filename)
 
 
 def handle_message(message):
     # It receives a bytestring message or a Kafka message in the LIGO GW format
     # fields must be extracted from the message text and stored into in the model
+    # It returns the nonlocalizedevent and event sequence ingested or None, None.
     if not isinstance(message, bytes):
         bytes_message = message.value()
     else:
         bytes_message = message
-    fields = extract_fields(bytes_message.decode('utf-8'), EXPECTED_FIELDS)
+    logger.warning(f"Processing message: {bytes_message.decode('utf-8')}")
+    fields = extract_all_fields(bytes_message.decode('utf-8'))
+    if not all(field in fields.keys() for field in EXPECTED_FIELDS):
+        logger.warning(f"Incoming GW message did not have the expected fields, ignoring it: {fields.keys()}")
+        return
+
+    if fields and fields['trigger_num'].startswith('M') and not settings.SAVE_TEST_ALERTS:
+        return
+
     if fields:
         nonlocalizedevent, nle_created = NonLocalizedEvent.objects.get_or_create(
-            event_id=fields['TRIGGER_NUM'],
+            event_id=fields['trigger_num'],
             event_type=NonLocalizedEvent.NonLocalizedEventType.GRAVITATIONAL_WAVE,
         )
         if nle_created:
-            logger.info(f"Ingested a new GW event with id {fields['TRIGGER_NUM']} from alertstream")
+            logger.info(f"Ingested a new GW event with id {fields['trigger_num']} from alertstream")
         # Next attempt to ingest and build the localization of the event
+        skymap_url = get_moc_url_from_skymap_fits_url(fields['skymap_fits_url'])
         try:
-            localization = create_localization_for_multiorder_fits(
+            skymap_resp = requests.get(skymap_url)
+            skymap_resp.raise_for_status()
+            localization = create_localization_for_skymap(
                 nonlocalizedevent=nonlocalizedevent,
-                multiorder_fits_url=get_moc_url_from_skymap_fits_url(fields['SKYMAP_FITS_URL'])
+                skymap_bytes=skymap_resp.content,
+                skymap_url=skymap_url
             )
         except Exception as e:
             localization = None
-            logger.error(f'Could not create EventLocalization for messsage: {fields}. Exception: {e}')
+            logger.error(
+                f"Failed to retrieve and process localization from skymap file at {skymap_url}. Exception: {e}"
+            )
             logger.error(traceback.format_exc())
 
         # Now ingest the sequence for that event
         event_sequence, es_created = EventSequence.objects.update_or_create(
             nonlocalizedevent=nonlocalizedevent,
             localization=localization,
-            sequence_id=fields['SEQUENCE_NUM'],
+            sequence_id=fields['sequence_num'],
             defaults={
-                'event_subtype': fields['NOTICE_TYPE']
+                'event_subtype': fields['notice_type'],
+                'details': fields,
+                'ingestor_source': 'gcn'
             }
         )
         if es_created and localization is None:
             warning_msg = (f'{"Creating" if es_created else "Updating"} EventSequence without EventLocalization:'
                            f'{event_sequence} for NonLocalizedEvent: {nonlocalizedevent}')
             logger.warning(warning_msg)
 
+        return nonlocalizedevent, event_sequence
+    return None, None
+
 
 def handle_retraction(message):
     # It receives a bytestring message or a Kafka message in the LIGO GW format
     # For a retraction message, we just set the events status to retracted if it exists.
     if not isinstance(message, bytes):
         bytes_message = message.value()
     else:
         bytes_message = message
     # Just need the event_id from the retraction messages
-    fields = extract_fields(bytes_message.decode('utf-8'), ['TRIGGER_NUM'])
+    fields = extract_all_fields(bytes_message.decode('utf-8'))
+    if 'trigger_num' not in fields:
+        logger.warning("Retraction notice missing 'trigger_num' field, ignoring.")
+        return
     # Then set the state to 'RETRACTED' for the event matching that id
     try:
-        retracted_event = NonLocalizedEvent.objects.get(event_id=fields['TRIGGER_NUM'])
+        retracted_event = NonLocalizedEvent.objects.get(event_id=fields['trigger_num'])
         retracted_event.state = NonLocalizedEvent.NonLocalizedEventState.RETRACTED
         retracted_event.save()
+        return retracted_event
     except NonLocalizedEvent.DoesNotExist:
-        logger.warning((f"Got a Retraction notice for event id {fields['TRIGGER_NUM']}"
+        logger.warning((f"Got a Retraction notice for event id {fields['trigger_num']}"
                         f"which does not exist in the database"))
+    return None
```

### Comparing `tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/healpix_utils.py` & `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,210 +1,270 @@
-''' This set of methods supports generating and querying healpix MOC maps for GW events,
-    using healpix_alchemy and model mappings with sql_alchemy queries.
-'''
-from astropy.table import Table
-from astropy.io import fits
-from tom_nonlocalizedevents.models import EventCandidate, SkymapTile, EventLocalization, CredibleRegion
-from django.db import transaction
+from django.db import models
+from django.contrib.postgres.fields import BigIntegerRangeField
+from django.contrib.postgres.indexes import SpGistIndex
 from django.conf import settings
-from healpix_alchemy.constants import HPX, LEVEL
-from healpix_alchemy.types import Tile, Point
-import sqlalchemy as sa
-from sqlalchemy.orm import relationship, declarative_base, Session
-from astropy_healpix import uniq_to_level_ipix
-from mocpy import MOC
-from ligo.skymap import distance
-from dateutil.parser import parse
-import os
-import sys
-import json
+
+from tom_targets.models import Target
+
+import numpy as np
+from psycopg2.extensions import register_adapter, AsIs
+from healpix_alchemy.constants import HPX
+from astropy.coordinates import SkyCoord
+from urllib.parse import urljoin
 import logging
 
-# from django.db.models import Sum, Subquery, F, Min
-# from tom_nonlocalizedevents_base.settings import DATABASES
+
+def adapt_numpy_float64(np_float64):
+    return AsIs(np_float64)
+
+
+def adapt_numpy_int64(np_int64):
+    return AsIs(np_int64)
+
+
+register_adapter(np.float64, adapt_numpy_float64)
+register_adapter(np.int64, adapt_numpy_int64)
 
 
 logger = logging.getLogger(__name__)
 
-POOL_RECYCLE = 4 * 60 * 60
-SA_DB_CONNECTION_URL = os.getenv(
-    'SA_DB_CONNECTION_URL',
-    (f"postgresql://{settings.DATABASES['default']['USER']}:{settings.DATABASES['default']['PASSWORD']}"
-     f"@{settings.DATABASES['default']['HOST']}:{settings.DATABASES['default']['PORT']}"
-     f"/{settings.DATABASES['default']['NAME']}"))
-CREDIBLE_REGION_PROBABILITIES = sorted(json.loads(os.getenv(
-    'CREDIBLE_REGION_PROBABILITIES', '[0.25, 0.5, 0.75, 0.9, 0.95]')), reverse=True)
-
-Base = declarative_base()
-sa_engine = sa.create_engine(SA_DB_CONNECTION_URL, pool_recycle=POOL_RECYCLE)
-
-
-def uniq_to_bigintrange(value):
-    level, ipix = uniq_to_level_ipix(value)
-    shift = 2 * (LEVEL - level)
-    return (ipix << shift, (ipix + 1) << shift)
-
-
-def sequence_to_bigintrange(sequence):
-    return f'[{sequence[0]},{sequence[1]})'
-
-
-def tiles_from_moc(moc):
-    return (f'[{lo},{hi})' for lo, hi in moc._interval_set.nested)
-
-
-def tiles_from_polygon_skycoord(polygon):
-    return tiles_from_moc(MOC.from_polygon_skycoord(polygon.transform_to(HPX.frame)))
-
-
-def create_localization_for_multiorder_fits(nonlocalizedevent, multiorder_fits_url):
-    ''' Takes in a GraceDB url to multiorder fits file and creates the skymap tiles in db
-    '''
-    logger.info(f"Creating localization for {nonlocalizedevent.event_id} with MOC skymap {multiorder_fits_url}")
-    header = fits.getheader(multiorder_fits_url, 1)
-    creation_date = parse(header.get('DATE'))
-    try:
-        localization = EventLocalization.objects.get(nonlocalizedevent=nonlocalizedevent, date=creation_date)
-    except EventLocalization.DoesNotExist:
-        distance_mean = header.get('DISTMEAN')
-        distance_std = header.get('DISTSTD')
-        data = Table.read(multiorder_fits_url)
-        row_dist_mean, row_dist_std, _ = distance.parameters_to_moments(data['DISTMU'], data['DISTSIGMA'])
-        with transaction.atomic():
-            localization = EventLocalization.objects.create(
-                nonlocalizedevent=nonlocalizedevent,
-                distance_mean=distance_mean,
-                distance_std=distance_std,
-                skymap_moc_file_url=multiorder_fits_url,
-                date=creation_date
+
+class NonLocalizedEvent(models.Model):
+    """Represents a NonLocalizedEvent being followed-up upon by this TOM.
+
+    A NonLocalizedEvent is distinguished from a Target in that it is localized to a region of the sky
+    (vs. a specific RA,DEC). The potential Targets in the localization region must be identified,
+    prioritized, and categorized (retired, of-interest, etc) for follow-up EM observations
+
+    For the moment, this is rather GraceDB (GW) specific, but sh/could be generalized to work
+    with gamma-ray burst and neutrino events.
+    """
+
+    class NonLocalizedEventType(models.TextChoices):
+        GRAVITATIONAL_WAVE = 'GW', 'Gravitational Wave'
+        GAMMA_RAY_BURST = 'GRB', 'Gamma-ray Burst'
+        NEUTRINO = 'NU', 'Neutrino'
+        UNKNOWN = 'UNK', 'Unknown'
+
+    class NonLocalizedEventState(models.TextChoices):
+        ACTIVE = 'ACTIVE'
+        INACTIVE = 'INACTIVE'
+        RETRACTED = 'RETRACTED'
+
+    state = models.CharField(
+        max_length=16,
+        choices=NonLocalizedEventState.choices,
+        default=NonLocalizedEventState.ACTIVE,
+        help_text='The current state of this NonLocalizedEvent'
+    )
+
+    event_type = models.CharField(
+        max_length=3,
+        choices=NonLocalizedEventType.choices,
+        default=NonLocalizedEventType.GRAVITATIONAL_WAVE,
+        help_text='The type of NonLocalizedEvent, used for determining how to ingest and display it'
+    )
+    # TODO: ask Curtis/Rachel/Andy about generalized use cases.
+    event_id = models.CharField(
+        max_length=64,
+        help_text='Unique identifer for the event. I.E. the TRIGGER_NUM for a GW event.'
+    )
+
+    created = models.DateTimeField(auto_now_add=True)
+    modified = models.DateTimeField(auto_now=True)
+
+    class Meta:
+        constraints = [
+            models.UniqueConstraint(fields=['event_id'], name='unique_event_id')
+        ]
+
+    @property
+    def gracedb_url(self):
+        """Construct and return the GraceDB URL for this nonlocalizedevent from the event_id Field.
+
+        for example, https://gracedb.ligo.org/superevents/S200316bj/
+        """
+        # TODO: add check that superevent_type is GRAVITATIONAL_WAVE
+        return f"https://gracedb.ligo.org/superevents/{self.event_id}/"
+
+    @property
+    def treasuremap_url(self):
+        """Construct and return the Treasure Map (treasuremap.space) URL for this nonlocalizedevent
+        from the event_id Field.
+
+        for example: http://treasuremap.space/alerts?graceids=S200219ac
+        """
+        # TODO: add check that superevent_type is GRAVITATIONAL_WAVE
+        return f"http://treasuremap.space/alerts?graceids={self.event_id}"
+
+    @property
+    def hermes_url(self):
+        """Construct and return the hermes details page URL for this nonlocalizedevent
+
+        for example: http://hermes.lco.global/nonlocalizedevent/S200316bj/
+        """
+        return urljoin(settings.HERMES_API_URL, f'/nonlocalizedevent/{self.event_id}/')
+
+    def __str__(self):
+        return f"{self.event_id}"
+
+
+class EventLocalization(models.Model):
+    """Represents a region of the sky in which a nonlocalizedevent may have taken place.
+    """
+    nonlocalizedevent = models.ForeignKey(NonLocalizedEvent, related_name='localizations', on_delete=models.CASCADE)
+    created = models.DateTimeField(auto_now_add=True)
+    modified = models.DateTimeField(auto_now=True)
+    date = models.DateTimeField(
+        help_text='The datestamp of this localizations creation.'
+    )
+    skymap_url = models.URLField(
+        default='',
+        help_text='The URL to a file containing skymap file for used to generate this localization.'
+    )
+    skymap_version = models.PositiveSmallIntegerField(
+        null=True, blank=True,
+        help_text='The version of the skymap for this localization'
+    )
+    skymap_hash = models.UUIDField(
+        null=True, blank=True,
+        help_text='A UUID from an md5 hash of the raw skymap file contents, used to detect when it has changed'
+    )
+    distance_mean = models.FloatField(
+        default=0,
+        help_text='The posterior mean distance in Mpc.'
+    )
+    distance_std = models.FloatField(
+        default=0,
+        help_text='The posterior standard deviation of the distance in Mpc.'
+    )
+    area_50 = models.FloatField(
+        null=True, blank=True,
+        help_text='The 50 percent confidence region area'
+    )
+    area_90 = models.FloatField(
+        null=True, blank=True,
+        help_text='The 90 percent confidence region area'
+    )
+
+    class Meta:
+        constraints = [
+            models.UniqueConstraint(
+                fields=['nonlocalizedevent', 'skymap_hash'],
+                name='unique_skymap_per_nonlocalizedevent'
+            )
+        ]
+
+
+class ExternalCoincidence(models.Model):
+    details = models.JSONField(
+        null=True, blank=True,
+        help_text='Contains the payload of the external coincidence section of the alert'
+    )
+    localization = models.ForeignKey(
+        EventLocalization, related_name='external_coincidences',
+        null=True, on_delete=models.SET_NULL
+    )
+
+
+class EventSequence(models.Model):
+    nonlocalizedevent = models.ForeignKey(NonLocalizedEvent, related_name='sequences', on_delete=models.CASCADE)
+    localization = models.ForeignKey(EventLocalization, related_name='sequences', null=True, on_delete=models.SET_NULL)
+    external_coincidence = models.ForeignKey(
+        ExternalCoincidence, related_name='sequences',
+        null=True, blank=True, on_delete=models.SET_NULL
+    )
+    details = models.JSONField(
+        null=True, blank=True,
+        help_text='Contains the payload of the event section of the alert'
+    )
+    sequence_id = models.PositiveIntegerField(
+        default=1,
+        help_text='The version / update number of this event. I.E. the SEQUENCE_NUM for a GW event.'
+    )
+    event_subtype = models.CharField(
+        max_length=256,
+        default='',
+        help_text='The subtype of the event. Options are type specific, i.e. GW events have initial, '
+                  'preliminary, update types.'
+    )
+    ingestor_source = models.CharField(default='', help_text='The source of this alert - i.e. which stream is it from?')
+    created = models.DateTimeField(auto_now_add=True)
+    modified = models.DateTimeField(auto_now=True)
+
+    class Meta:
+        ordering = ["sequence_id"]
+        constraints = [
+            models.UniqueConstraint(
+                fields=['nonlocalizedevent', 'sequence_id'],
+                name='unique_sequence_per_nonlocalizedevent'
             )
-            for i, row in enumerate(data):
-                # This is necessary to make sure we don't get an underflow error in postgres
-                # when operating with the probdensity float field
-                probdensity = row['PROBDENSITY'] if row['PROBDENSITY'] > sys.float_info.min else 0
-                SkymapTile.objects.create(
-                    localization=localization,
-                    tile=uniq_to_bigintrange(row['UNIQ']),
-                    probdensity=probdensity,
-                    distance_mean=row_dist_mean[i],
-                    distance_std=row_dist_std[i]
-                )
-    return localization
-
-
-# healpix_alchemy models pointing to django ORM models, for building a sql alchemy query
-class SaSkymap(Base):
-    __tablename__ = 'tom_nonlocalizedevents_eventlocalization'
-    id = sa.Column(sa.Integer, primary_key=True)
-    tiles = relationship(lambda: SaSkymapTile)
-
-
-class SaSkymapTile(Base):
-    __tablename__ = 'tom_nonlocalizedevents_skymaptile'
-    id = sa.Column(sa.Integer, primary_key=True)
-    localization_id = sa.Column(sa.ForeignKey(SaSkymap.id), primary_key=True)
-    tile = sa.Column(Tile, primary_key=True, index=True)
-    probdensity = sa.Column(sa.Float, nullable=False)
-    distance_mean = sa.Column(sa.Float, nullable=False)
-    distance_std = sa.Column(sa.Float, nullable=False)
-
-
-class SaTarget(Base):
-    __tablename__ = 'tom_targets_target'
-    id = sa.Column(sa.Integer, primary_key=True)
-    distance = sa.Column(sa.Float, nullable=True)
-    distance_err = sa.Column(sa.Float, nullable=True)
-
-
-class SaEventCandidate(Base):
-    __tablename__ = 'tom_nonlocalizedevents_eventcandidate'
-    id = sa.Column(sa.Integer, primary_key=True)
-    target_id = sa.Column(sa.ForeignKey(SaTarget.id), primary_key=True)
-    healpix = sa.Column(Point, index=True, nullable=False)
-
-
-def update_all_credible_region_percents_for_candidates(eventlocalization, event_candidate_ids=None):
-    ''' This helper function runs through the defined set of discrete credible region probabilities
-        and creates or updates the probability of a credible region for each of the event candidates
-        that fall within the event localization's credible region of that priority
-    '''
-    if not event_candidate_ids:
-        event_candidate_ids = list(eventlocalization.nonlocalizedevent.candidates.values_list('pk', flat=True))
-    for probability in CREDIBLE_REGION_PROBABILITIES:
-        update_credible_region_percent_for_candidates(eventlocalization, probability, event_candidate_ids)
-
-
-def update_credible_region_percent_for_candidates(eventlocalization, prob, event_candidate_ids=None):
-    ''' This function creates a credible region linkage with probability prob for each of the event candidate
-        ids supplied if they fall within that prob for the event location specified.
-    '''
-    if not event_candidate_ids:
-        event_candidate_ids = list(eventlocalization.nonlocalizedevent.candidates.values_list('pk', flat=True))
-
-    session = Session(sa_engine)
-
-    cum_prob = sa.func.sum(
-        SaSkymapTile.probdensity * SaSkymapTile.tile.area
-    ).over(
-        order_by=SaSkymapTile.probdensity.desc()
-    ).label(
-        'cum_prob'
-    )
-
-    subquery = sa.select(
-        SaSkymapTile.probdensity,
-        cum_prob
-    ).filter(
-        SaSkymapTile.localization_id == eventlocalization.id
-    ).subquery()
-
-    min_probdensity = sa.select(
-        sa.func.min(subquery.columns.probdensity)
-    ).filter(
-        subquery.columns.cum_prob <= prob
-    ).scalar_subquery()
-
-    query = sa.select(
-        SaEventCandidate.id
-    ).filter(
-        SaEventCandidate.id.in_(event_candidate_ids),
-        SaSkymapTile.localization_id == eventlocalization.id,
-        SaSkymapTile.tile.contains(SaEventCandidate.healpix),
-        SaSkymapTile.probdensity >= min_probdensity
-    )
-
-    results = session.execute(query)
-
-    for sa_event_candidate_id in results:
-        CredibleRegion.objects.update_or_create(
-            candidate=EventCandidate.objects.get(id=sa_event_candidate_id[0]),
-            localization=eventlocalization,
-            defaults={
-                'smallest_percent': int(prob * 100.0)
-            }
-        )
-
-
-# def point_in_range_django(eventlocalization, prob):
-# This code is a beginning attempt to translate the healpix_alchemy query from sql_alchemy to django ORM
-# It is non-functional and needs more work to get right.
-#     event_candidate_ids = list(eventlocalization.nonlocalizedevent.candidates.values_list('pk', flat=True))
-
-#     SkymapTile.objects.order_by('-probdensity').aggregate(cum_prob=Sum(F('probdensity') * F('tile__area')))
-
-#     cum_prob = SkymapTile.objects.order_by('-probdensity').alias(cum_prob=Sum(F('probdensity') *
-#                F('tile__area'))).annotate(cum_prob=F('cum_prob'),
-#     )
-#     min_probdensity = SkymapTile.objects.order_by('-probdensity').alias(
-#         cum_prob=Sum(F('probdensity') * F('tile__area')), min_probdensity=Min(F('probdensity'))).annotate(
-#         cum_prob=F('cum_prob'), min_probdensity=F('min_probdensity')
-#     ).filter(
-#         localization__id=eventlocalization.id,
-#         cum_prob__lte=prob,
-#         probdensity__gte=min_probdensity,
-#         tile__contains=
-#         localization__nonlocalizedevent__candidates
-#     )
-#     candidates = EventCandidate.objects.filter(
-#         nonlocalizedevent=eventlocalization.nonlocalizedevent,
-#         eventlocalization__tiles__contains(healpix)
-#     ).values('id')
+        ]
+
+
+class EventCandidate(models.Model):
+    target = models.ForeignKey(Target, on_delete=models.CASCADE)
+    nonlocalizedevent = models.ForeignKey(NonLocalizedEvent, related_name='candidates', on_delete=models.CASCADE)
+
+    viable = models.BooleanField(
+        default=True,
+        help_text='Whether this event candidate is actively being considered or not'
+    )
+    viability_reason = models.TextField(
+        default='',
+        help_text='Reason why this candidates viability is set the way it is.'
+    )
+    priority = models.IntegerField(
+        default=1,
+        help_text='Internal priority of this Event Candidate'
+    )
+    healpix = models.BigIntegerField(
+        default=-1,
+        help_text='Stores the healpix index for this candidates target, used for MOC lookups'
+    )
+    created = models.DateTimeField(auto_now_add=True)
+    modified = models.DateTimeField(auto_now=True)
+
+    def save(self, *args, **kwargs):
+        if self.target:
+            self.healpix = HPX.skycoord_to_healpix(SkyCoord(self.target.ra, self.target.dec, unit='deg'))
+        super().save(*args, **kwargs)
+
+    class Meta:
+        constraints = [
+            models.UniqueConstraint(fields=['target', 'nonlocalizedevent'], name='unique_target_nonlocalizedevent')
+        ]
+
+    def __str__(self):
+        return f'EventCandidate({self.id}) NonLocalizedEvent: {self.nonlocalizedevent} Target: {self.target}'
+
+
+class CredibleRegion(models.Model):
+    localization = models.ForeignKey(EventLocalization, related_name='credibleregions', on_delete=models.CASCADE)
+    candidate = models.ForeignKey(EventCandidate, related_name='credibleregions', on_delete=models.CASCADE)
+
+    smallest_percent = models.IntegerField(
+        default=100,
+        help_text='Smallest percent credible region this candidate falls into for this localization.'
+    )
+
+    class Meta:
+        constraints = [
+            models.UniqueConstraint(fields=['localization', 'candidate'], name='unique_localization_candidate')
+        ]
+
+
+class SkymapTile(models.Model):
+    """ A healpix_alchemy style tile linked to an event localization
+    """
+    localization = models.ForeignKey(EventLocalization, related_name='tiles', on_delete=models.CASCADE)
+    tile = BigIntegerRangeField(db_index=True)
+    probdensity = models.FloatField(null=False)
+    distance_mean = models.FloatField(
+        default=0
+    )
+    distance_std = models.FloatField(
+        default=0
+    )
+
+    class Meta:
+        indexes = [SpGistIndex(fields=('tile',))]
```

### Comparing `tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0002_superevent.py` & `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0002_superevent.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0003_auto_20210225_0034.py` & `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0003_auto_20210225_0034.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0005_auto_20210319_2241.py` & `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0005_auto_20210319_2241.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0006_auto_20210827_2346.py` & `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0006_auto_20210827_2346.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0010_rename_more_superevent_fields.py` & `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0010_rename_more_superevent_fields.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0011_eventcandidate_viability_reason_and_more.py` & `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0011_eventcandidate_viability_reason_and_more.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0012_nonlocalizedevent_event_subtype.py` & `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0012_nonlocalizedevent_event_subtype.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0013_eventcandidate_healpix_and_more.py` & `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0013_eventcandidate_healpix_and_more.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0014_credibleregion_and_more.py` & `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0014_credibleregion_and_more.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/migrations/0015_eventsequence_and_more.py` & `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/migrations/0015_eventsequence_and_more.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/serializers.py` & `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/serializers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from rest_framework import serializers
 from tom_targets.models import Target
 from tom_targets.serializers import TargetSerializer
 
 from tom_nonlocalizedevents.models import (CredibleRegion, EventCandidate, EventLocalization,
-                                           EventSequence, NonLocalizedEvent)
+                                           EventSequence, NonLocalizedEvent, ExternalCoincidence)
 
 # from healpix_alchemy.constants import PIXEL_AREA, HPX
 # from astropy.coordinates import SkyCoord
 import logging
 
 logger = logging.getLogger(__name__)
 
@@ -82,20 +82,19 @@
                     target = target_serializer.save()
                     logger.info(f"Created target {target.id} with name {target.name}")
             validated_data['target'] = target
             del validated_data['target_fields']
         return super().create(validated_data)
 
     def get_credible_regions(self, instance):
-        sequence_id_to_credible_region_percent = {}
+        localization_id_to_credible_region_percent = {}
         credibleregions = instance.credibleregions.all()
         for cr in credibleregions:
-            for sequence in cr.localization.sequences.all():
-                sequence_id_to_credible_region_percent[sequence.sequence_id] = cr.smallest_percent
-        return sequence_id_to_credible_region_percent
+            localization_id_to_credible_region_percent[cr.localization.id] = cr.smallest_percent
+        return localization_id_to_credible_region_percent
 
     def to_representation(self, instance):
         representation = super().to_representation(instance)
         # TODO: this is a little unorthodox. it's convenient for now to handle the data from
         # the ForiengKey objects, but that should be handled separately by their own serializers.
         # (and to_representation could be left undisturbed).
         representation['target'] = TargetSerializer(Target.objects.get(pk=representation['target'])).data
@@ -103,27 +102,33 @@
             pk=representation['nonlocalizedevent']).event_id
         return representation
 
 
 class EventLocalizationSerializer(serializers.HyperlinkedModelSerializer):
     class Meta:
         model = EventLocalization
-        fields = ['id', 'date', 'skymap_moc_file_url', 'distance_mean', 'distance_std']
+        fields = ['id', 'date', 'skymap_url', 'skymap_version', 'area_50', 'area_90', 'distance_mean', 'distance_std']
+
+
+class ExternalCoincidence(serializers.HyperlinkedModelSerializer):
+    localization = EventLocalizationSerializer(read_only=True)
+
+    class Meta:
+        model = ExternalCoincidence
+        fields = ['details', 'localization']
 
 
 class EventSequenceSerializer(serializers.HyperlinkedModelSerializer):
-    localization = serializers.PrimaryKeyRelatedField(read_only=True)
-    skymap_fits_url = serializers.SerializerMethodField(read_only=True)
+    localization = EventLocalizationSerializer(read_only=True)
+    external_coincidence = ExternalCoincidence(read_only=True)
 
     class Meta:
         model = EventSequence
-        fields = ['id', 'sequence_id', 'event_subtype', 'localization', 'skymap_fits_url']
-
-    def get_skymap_fits_url(self, instance):
-        return instance.localization.skymap_moc_file_url
+        fields = ['id', 'created', 'modified', 'sequence_id', 'event_subtype',
+                  'details', 'ingestor_source', 'localization', 'external_coincidence']
 
 
 class NonLocalizedEventSerializer(serializers.HyperlinkedModelSerializer):
     candidates = serializers.SerializerMethodField()
     sequences = EventSequenceSerializer(many=True)
 
     class Meta:
```

### Comparing `tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/signals/handlers.py` & `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/css/superevent_vue_app.css` & `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/css/superevent_vue_app.css`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/js/superevent_vue_app.js` & `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/js/superevent_vue_app.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -8533,15 +8533,15 @@
         let b = [];
         b.push(g({
             paths: ["counter.count"]
         }));
         let M = new o["a"].Store({
             state: {
                 tomApiBaseUrl: "http://localhost:8000",
-                hermesApiBaseUrl: "http://hermes-dev.lco.gtn",
+                hermesApiBaseUrl: "https://hermes.lco.global",
                 tomAxiosConfig: {},
                 hermesAxiosConfig: {}
             },
             plugins: b,
             modules: {
                 counter: y
             },
@@ -8581,48 +8581,51 @@
                         "no-body": ""
                     }
                 }, [a("b-card-title", {
                     staticClass: "text-center font-weight-bold superevent-banner",
                     staticStyle: {
                         "font-size": "xxx-large"
                     }
-                }, [e._v(e._s(e.event_id))]), a("b-tabs", {
+                }, [e._v(e._s(e.superevent_data.event_id))]), a("b-tabs", {
                     attrs: {
                         card: "",
                         pills: "",
                         "active-nav-item-class": "font-weight-bold"
                     }
-                }, e._l(e.unpacked_sequences, (function(t, n) {
+                }, e._l(e.expandedSequences, (function(t, n) {
                     return a("b-tab", {
                         key: t.sequence_id,
                         attrs: {
                             "no-body": "",
-                            title: e.getTabTitle(t.sequence_id, t.created),
-                            active: n + 1 == e.unpacked_sequences.length,
+                            title: e.getTabTitle(t),
+                            active: n + 1 == e.expandedSequences.length,
                             lazy: ""
                         },
                         on: {
                             click: function(a) {
                                 e.tab = t.sequence_id
                             }
                         }
                     }, [a("superevent-detail", {
                         ref: "sequence_" + t.sequence_id.toString(),
                         refInFor: !0,
                         attrs: {
-                            supereventPk: e.superevent_pk,
-                            supereventId: e.event_id,
-                            supereventHermesData: e.superevent_data,
-                            sequenceId: t.sequence_id
+                            supereventPk: e.superevent_data.id,
+                            supereventId: e.superevent_data.event_id,
+                            sequence: t,
+                            candidates: e.superevent_data.candidates,
+                            alerts: e.references
                         }
                     })], 1)
                 })), 1)], 1)], 1)])
             },
             w = [],
-            H = function() {
+            H = a("2ef0"),
+            k = a.n(H),
+            A = function() {
                 var e = this,
                     t = e.$createElement,
                     a = e._self._c || t;
                 return a("div", [a("div", e._l(e.messages, (function(t) {
                     return a("b-alert", {
                         key: t,
                         attrs: {
@@ -8630,20 +8633,20 @@
                             dismissable: ""
                         }
                     }, [e._v(" " + e._s(t) + " ")])
                 })), 1), a("div", {
                     directives: [{
                         name: "show",
                         rawName: "v-show",
-                        value: void 0 !== e.supereventHermesData.sequences,
-                        expression: "supereventHermesData.sequences !== undefined"
+                        value: void 0 !== e.sequence,
+                        expression: "sequence !== undefined"
                     }]
                 }, [a("gravitational-wave-banner", {
                     attrs: {
-                        eventAttributes: e.superevent_attributes,
+                        sequence: e.sequence,
                         supereventId: e.supereventId
                     }
                 })], 1), a("b-row", {
                     staticStyle: {
                         "margin-top": "6px"
                     }
                 }, [a("b-col", {
@@ -8696,38 +8699,36 @@
                 })], 1)], 1), a("hr"), a("b-row", [a("b-col", {
                     attrs: {
                         cols: "12"
                     }
                 }, [a("h3", [e._v("Active Candidates")]), a("candidate-target-table", {
                     attrs: {
                         candidates: this.viableCandidates,
-                        sequenceId: this.sequenceId
+                        sequenceId: this.sequence.sequence_id
                     },
                     on: {
                         "toggle-viability": e.onToggleViability,
                         "change-priority": e.onChangePriority
                     }
                 })], 1)], 1), a("b-row", [a("b-col", {
                     attrs: {
                         cols: "12"
                     }
                 }, [a("h3", [e._v("Retired Candidates")]), a("candidate-target-table", {
                     attrs: {
                         candidates: this.nonViableCandidates,
-                        sequenceId: this.sequenceId
+                        sequenceId: this.sequence.sequence_id
                     },
                     on: {
                         "toggle-viability": e.onToggleViability,
                         "change-priority": e.onChangePriority
                     }
                 })], 1)], 1), a("hr")], 1)
             },
-            k = [],
-            A = a("2ef0"),
-            S = a.n(A),
+            S = [],
             V = (a("bf37"), function() {
                 var e = this,
                     t = e.$createElement,
                     a = e._self._c || t;
                 return a("div", [a("b-button", {
                     directives: [{
                         name: "b-modal",
@@ -8995,15 +8996,15 @@
                                 console.log("Unable to create target: " + e)
                             })
                         }).catch(e => {
                             console.log("Unable to retrieve groups: " + e)
                         })
                     },
                     onSelectTarget(e, t) {
-                        !0 === t ? S.a.includes(this.selectedTargets, e.item.id) || this.selectedTargets.push(e.item.id) : this.selectedTargets = this.selectedTargets.filter((function(t) {
+                        !0 === t ? k.a.includes(this.selectedTargets, e.item.id) || this.selectedTargets.push(e.item.id) : this.selectedTargets = this.selectedTargets.filter((function(t) {
                             return t !== e.item.id
                         }))
                     }
                 }
             },
             D = T;
 
@@ -9447,15 +9448,15 @@
                                 this.$bvModal.hide("candidate-from-target-modal"), this.$emit("created-target-candidates", e.data.length)
                             }).catch(e => {
                                 console.log("Unable to create eventcandidates for new targets: " + e), this.submissionError = e.response.data
                             })
                         })
                     },
                     onSelectGroup(e, t) {
-                        !0 === t ? S.a.includes(this.selectedGroups, e.item) || this.selectedGroups.push(e.item) : this.selectedGroups = this.selectedGroups.filter((function(t) {
+                        !0 === t ? k.a.includes(this.selectedGroups, e.item) || this.selectedGroups.push(e.item) : this.selectedGroups = this.selectedGroups.filter((function(t) {
                             return t !== e.item
                         }))
                     }
                 }
             },
             Q = Z,
             ee = C(Q, K, X, !1, null, null, null),
@@ -9465,122 +9466,152 @@
                     t = e.$createElement,
                     a = e._self._c || t;
                 return a("div", [a("b-jumbotron", {
                     staticClass: "py-4 pl-3 text-white superevent-banner",
                     attrs: {
                         id: "superevent-banner"
                     }
-                }, [a("b-row", [a("b-col", [a("h3", [a("span", [e._v("MassGap: " + e._s(e.safeGetEventAttributes("prob_massgap", -1, !0)))])])]), a("b-col", [a("h3", [a("span", [e._v("NSBH: " + e._s(e.safeGetEventAttributes("prob_nsbh", -1, !0)))])])]), a("b-col", [a("h3", [a("span", [e._v("Remnant: " + e._s(e.safeGetEventAttributes("prob_remnant", -1, !0)))])])]), a("b-col", [a("h3", [a("span", [e._v("90%: " + e._s(parseFloat(e.safeGetEventAttributes("area_90")).toFixed(2)))])])]), a("b-col", [a("h3", [a("span", [e._v("FAR: " + e._s(e.safeGetEventAttributes("far", -1, !0)))])])])], 1), a("b-row", [a("b-col", [a("h3", [a("span", [e._v("BNS: " + e._s(e.safeGetEventAttributes("prob_bns", -1, !0)))])])]), a("b-col", [a("h3", [a("span", [e._v("Terrestrial: " + e._s(e.safeGetEventAttributes("prob_terres", -1, !0)))])])]), a("b-col", [a("h3", [a("span", [e._v("BBH: " + e._s(e.safeGetEventAttributes("prob_bbh", -1, !0)))])])]), a("b-col", [a("h3", [a("span", [e._v("50%: " + e._s(parseFloat(e.safeGetEventAttributes("area_50")).toFixed(2)))])])]), a("b-col", [a("h3", [a("span", [e._v("NS/Rem: " + e._s(e.safeGetEventAttributes("prob_ns", -1, !0)))])])])], 1)], 1)], 1)
+                }, [a("b-row", [a("b-col", ["gcn" === e.sequence.ingestor_source.toLowerCase() ? a("h3", [a("span", [e._v("NS: " + e._s(e.safeGetEventAttributes("details.prob_ns", -1, !0).toPrecision(3)))])]) : a("h3", [a("span", [e._v("Instruments: " + e._s(e.safeGetEventAttributes("details.instruments", []).join(",")))])])]), a("b-col", [a("h3", [a("span", [e._v("NSBH: " + e._s(e.safeGetEventAttributes(this.nsbhPath, -1, !0).toPrecision(3)))])])]), a("b-col", [a("h3", [a("span", [e._v("FAR: " + e._s(e.safeGetEventAttributes("details.far", -1, !0).toPrecision(3)))])])]), a("b-col", [a("h3", [a("span", [e._v("90%: " + e._s(parseFloat(e.safeGetEventAttributes(this.area90Path)).toPrecision(4)))])])]), e.hasExternalCoincidence ? a("b-col", [a("h3", [a("span", [e._v("GCN #: " + e._s(e.safeGetEventAttributes("external_coincidence.details.gcn_notice_id", -1)))])])]) : e._e()], 1), a("b-row", [a("b-col", [a("h3", [a("span", [e._v("BNS: " + e._s(e.safeGetEventAttributes(this.bnsPath, -1, !0).toPrecision(3)))])])]), a("b-col", [a("h3", [a("span", [e._v("Terrestrial: " + e._s(e.safeGetEventAttributes(this.terrestrialPath, -1, !0).toPrecision(3)))])])]), a("b-col", [a("h3", [a("span", [e._v("BBH: " + e._s(e.safeGetEventAttributes(this.bbhPath, -1, !0).toPrecision(3)))])])]), a("b-col", [a("h3", [a("span", [e._v("50%: " + e._s(parseFloat(e.safeGetEventAttributes(this.area50Path)).toPrecision(4)))])])]), e.hasExternalCoincidence ? a("b-col", [a("h3", [a("span", [e._v("Observatory: " + e._s(e.safeGetEventAttributes("external_coincidence.details.observatory", "")))])])]) : e._e()], 1)], 1)], 1)
             },
             ne = [],
             re = {
                 name: "GravitationalWaveBanner",
                 props: {
-                    eventAttributes: {
+                    sequence: {
                         type: Object,
                         required: !0
                     },
                     supereventId: String
                 },
+                computed: {
+                    hasExternalCoincidence() {
+                        return !k.a.isNil(this.sequence.external_coincidence) && !k.a.isEmpty(this.sequence.external_coincidence)
+                    },
+                    nsbhPath() {
+                        return "gcn" === this.sequence.ingestor_source.toLowerCase() ? "details.prob_nsbh" : "details.classification.NSBH"
+                    },
+                    bbhPath() {
+                        return "gcn" === this.sequence.ingestor_source.toLowerCase() ? "details.prob_bbh" : "details.classification.BBH"
+                    },
+                    bnsPath() {
+                        return "gcn" === this.sequence.ingestor_source.toLowerCase() ? "details.prob_bns" : "details.classification.BNS"
+                    },
+                    terrestrialPath() {
+                        return "gcn" === this.sequence.ingestor_source.toLowerCase() ? "details.prob_terres" : "details.classification.Terrestrial"
+                    },
+                    area50Path() {
+                        return this.hasExternalCoincidence ? "external_coincidence.localization.area_50" : "localization.area_50"
+                    },
+                    area90Path() {
+                        return this.hasExternalCoincidence ? "external_coincidence.localization.area_90" : "localization.area_90"
+                    }
+                },
                 methods: {
                     safeGetEventAttributes(e, t = 0, a = !1) {
-                        return void 0 !== this.eventAttributes && void 0 !== this.eventAttributes[e] ? a && "string" === typeof this.eventAttributes[e] ? this.eventAttributes[e].split(" ")[0] : this.eventAttributes[e] : t
+                        if (k.a.isObjectLike(this.sequence)) {
+                            var n = k.a.get(this.sequence, e, t);
+                            return a && "string" === typeof n && (n = n.split(" ")[0]), isNaN(parseFloat(n)) ? n : parseFloat(n)
+                        }
+                        return t
                     }
                 }
             },
             ie = re,
             oe = C(ie, ae, ne, !1, null, null, null),
             se = oe.exports,
             le = {
                 name: "SupereventDetail",
                 props: {
                     supereventPk: Number,
                     supereventId: String,
-                    sequenceId: Number,
-                    supereventHermesData: {
+                    sequence: {
                         type: Object,
                         required: !0
+                    },
+                    alerts: {
+                        type: Array,
+                        required: !0
+                    },
+                    candidates: {
+                        type: Array,
+                        required: !0
                     }
                 },
                 components: {
                     AddCandidateModal: x,
                     AlertsTable: R,
                     CreateTargetModal: te,
                     CandidateTargetTable: J,
                     GravitationalWaveBanner: se
                 },
                 data: function() {
                     return {
-                        alerts: [],
                         alert_fields: [{
                             key: "identifier"
                         }, {
                             key: "timestamp",
                             sortable: !0
                         }, {
                             key: "from"
                         }, {
                             key: "subject"
                         }],
                         messages: [],
                         eventCandidates: [],
                         selectedAlerts: [],
-                        superevent_data: {},
-                        superevent_attributes: {},
-                        sequence_skymap_fits_url: ""
+                        superevent_data: {}
                     }
                 },
                 computed: {
+                    hasExternalCoincidence() {
+                        return !k.a.isNil(this.sequence.external_coincidence) && !k.a.isEmpty(this.sequence.external_coincidence)
+                    },
+                    skymapVersion() {
+                        return this.hasExternalCoincidence ? k.a.get(this.sequence, "external_coincidence.localization.skymap_version", void 0) : k.a.get(this.sequence, "localization.skymap_version", void 0)
+                    },
+                    skymapUrl() {
+                        return this.hasExternalCoincidence ? k.a.get(this.sequence, "external_coincidence.localization.skymap_url", void 0) : k.a.get(this.sequence, "localization.skymap_url", void 0)
+                    },
                     viableCandidates() {
                         return this.eventCandidates.filter(e => e.viable)
                     },
                     nonViableCandidates() {
                         return this.eventCandidates.filter(e => !e.viable)
                     }
                 },
                 created() {
-                    this.getSupereventData(), this.setupSupereventHermesData()
-                },
-                watch: {
-                    supereventHermesData: function() {
-                        this.setupSupereventHermesData()
-                    }
+                    this.processEventCandidates()
                 },
                 methods: {
+                    processEventCandidates() {
+                        this.eventCandidates = [], this.candidates.forEach(e => {
+                            this.hasExternalCoincidence ? this.sequence.external_coincidence.localization.id.toString() in e["credible_regions"] ? e["credible_region"] = e["credible_regions"][this.sequence.external_coincidence.localization.id.toString()] : e["credible_region"] = 100 : this.sequence.localization.id.toString() in e["credible_regions"] ? e["credible_region"] = e["credible_regions"][this.sequence.localization.id.toString()] : e["credible_region"] = 100, this.eventCandidates.push(e)
+                        })
+                    },
                     getSupereventData() {
                         let e = this.eventCandidates.slice();
-                        this.eventCandidates = [], r.a.get(`${this.$store.state.tomApiBaseUrl}/api/nonlocalizedevents/${this.supereventPk}`).then(e => {
+                        this.eventCandidates = [], r.a.get(`${this.$store.state.tomApiBaseUrl}/api/nonlocalizedevents/${this.supereventPk}/`).then(e => {
                             e["data"]["candidates"].forEach(e => {
-                                this.sequenceId.toString() in e["credible_regions"] ? e["credible_region"] = e["credible_regions"][this.sequenceId.toString()] : e["credible_region"] = 100, this.eventCandidates.push(e)
-                            });
-                            for (let t in e["data"]["sequences"]) e["data"]["sequences"][t]["sequence_id"] == this.sequenceId && (this.sequence_skymap_fits_url = e["data"]["sequences"][t]["skymap_fits_url"])
+                                this.sequence.sequence_id.toString() in e["credible_regions"] ? e["credible_region"] = e["credible_regions"][this.sequence.sequence_id.toString()] : e["credible_region"] = 100, this.eventCandidates.push(e)
+                            })
                         }).catch(t => {
                             console.log(`getSupereventData: Error getting database data for pk ${this.supereventPk}: ${t}`), this.eventCandidates = e
                         })
                     },
-                    setupSupereventHermesData() {
-                        if (void 0 !== this.supereventHermesData.sequences && this.supereventHermesData.sequences.length > 0) {
-                            for (const e in this.supereventHermesData.sequences)
-                                if (this.supereventHermesData.sequences[e]["sequence_number"] == this.sequenceId) {
-                                    this.superevent_attributes = this.supereventHermesData.sequences[e].message.data;
-                                    break
-                                } this.alerts = this.supereventHermesData.references
-                        }
-                    },
                     getVolumeImageUrl(e = !0) {
-                        let t = ".png";
-                        e && (t = ".volume.png");
-                        let a = this.sequence_skymap_fits_url.replace("LALInference.multiorder.fits", "LALInference" + t);
-                        return a = a.replace("bayestar.multiorder.fits", "bayestar" + t), a
+                        let t = "";
+                        t = e ? "bayestar.volume.png" : this.hasExternalCoincidence ? "combined-ext.png" : "bayestar.png";
+                        let a = "https://gracedb.ligo.org/api/superevents/" + this.supereventId + "/files/" + t;
+                        return void 0 !== this.skymapVersion && (a = a + "," + this.skymapVersion), a
                     },
                     onCreatedCandidates(e) {
                         this.messages.push(`Successfully added ${e} candidates.`), this.getSupereventData()
                     },
                     onSelectAlert(e, t) {
-                        !0 === t ? S.a.includes(this.selectedAlerts, e.item) || this.selectedAlerts.push(e.item) : this.selectedAlerts = this.selectedAlerts.filter((function(t) {
+                        !0 === t ? k.a.includes(this.selectedAlerts, e.item) || this.selectedAlerts.push(e.item) : this.selectedAlerts = this.selectedAlerts.filter((function(t) {
                             return t !== e.item
                         }))
                     },
                     onToggleViability(e, t) {
                         const a = e.item,
                             n = `${this.$store.state.tomApiBaseUrl}/api/eventcandidates/${a.id}/`,
                             i = !a.viable,
@@ -9604,48 +9635,54 @@
                         console.log("onChangePriority -        row.item.id: " + e.item.id), console.log("onChangePriority -  row.item.priority: " + e.item.priority), console.log("onChangePriority - candidate.priority: " + a.priority), console.log("onChangePriority -              event: " + t), r.a.patch(n, o).then(e => {}).catch(e => {
                             console.error("onChangePriority - url: " + n), console.error("onChangePriority - patch: " + JSON.stringify(o)), console.error(`onChangePriority: Error getting database data for ${JSON.stringify(a)}: ${e}`)
                         }), console.log("after PATCH..."), console.log("onChangePriority - candidate.priority: " + a.priority), console.log("onChangePriority -              event: " + t), console.log()
                     }
                 }
             },
             ce = le,
-            ue = C(ce, H, k, !1, null, "353d0214", null),
+            ue = C(ce, A, S, !1, null, "32b2a06c", null),
             de = ue.exports,
             he = {
                 name: "SupereventSequences",
                 props: {
-                    pk: String,
-                    event_id: String,
-                    sequences: String,
+                    superevent: String,
                     hermes_api_url: String,
                     tom_api_url: String
                 },
                 data: function() {
                     return {
-                        unpacked_sequences: JSON.parse(this.sequences),
-                        superevent_pk: parseInt(this.pk),
-                        superevent_data: {}
+                        superevent_data: JSON.parse(this.superevent),
+                        references: []
                     }
                 },
                 components: {
                     SupereventDetail: de
                 },
                 created() {
                     this.$store.commit("setTomApiBaseUrl", this.tom_api_url), this.$store.commit("setHermesApiBaseUrl", this.hermes_api_url), this.getHermesDBData()
                 },
+                computed: {
+                    expandedSequences() {
+                        let e = [];
+                        return this.superevent_data.sequences.forEach(t => {
+                            let a = k.a.cloneDeep(t);
+                            a.external_coincidence = null, e.push(a), k.a.isNil(t.external_coincidence) || k.a.isEmpty(t.external_coincidence) || e.push(t)
+                        }), e
+                    }
+                },
                 methods: {
-                    getTabTitle(e, t) {
-                        let a = new Date(t);
-                        return "Update " + e.toString() + ": " + a.toLocaleString()
+                    getTabTitle(e) {
+                        let t = "";
+                        return t += e.sequence_id.toString() + ": " + k.a.capitalize(e.event_subtype), k.a.isNil(e.external_coincidence) || k.a.isEmpty(e.external_coincidence) || (t += " Combined"), t
                     },
                     getHermesDBData() {
-                        r.a.get(`${this.$store.state.hermesApiBaseUrl}/api/v0/nonlocalizedevents/${this.event_id}/`, this.$store.state.hermesAxiosConfig).then(e => {
-                            this.superevent_data = e["data"]
+                        r.a.get(`${this.$store.state.hermesApiBaseUrl}/api/v0/nonlocalizedevents/${this.superevent_data.event_id}/`, this.$store.state.hermesAxiosConfig).then(e => {
+                            this.references = k.a.get(e["data"], "references", [])
                         }).catch(e => {
-                            console.log(`Error getting details for superevent ${this.event_id}: ${e}`)
+                            console.log(`Error getting references for superevent ${this.superevent_data.event_id}: ${e}`)
                         })
                     }
                 }
             },
             fe = he,
             pe = C(fe, L, w, !1, null, null, null),
             me = pe.exports,
```

### Comparing `tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/index.html` & `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/index.html`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/tests/factories.py` & `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/tests/factories.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,9 +17,9 @@
 
 
 @factory.django.mute_signals(signals.post_save)
 class EventLocalizationFactory(factory.django.DjangoModelFactory):
     class Meta:
         model = EventLocalization
 
-    skymap_moc_file_url = factory.Faker('pystr')
+    skymap_url = factory.Faker('pystr')
     date = factory.Faker('date_time')
```

### Comparing `tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/tests/tests.py` & `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/tests/tests.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 
     def test_nonlocalizedevent_list_api(self):
         """Test NonLocalizedEvent API list endpoint."""
         response = self.client.get(reverse('api:nonlocalizedevent-list'))
 
         self.assertEqual(response.json()['count'], 2)
         self.assertContains(response, f'"event_id":"{self.superevent1.event_id}"')
-        self.assertContains(response, f'"skymap_fits_url":"{self.eventlocalization1.skymap_moc_file_url}"')
+        self.assertContains(response, f'"skymap_url":"{self.eventlocalization1.skymap_url}"')
         self.assertContains(response, f'"event_id":"{self.superevent2.event_id}"')
-        self.assertContains(response, f'"skymap_fits_url":"{self.eventlocalization2.skymap_moc_file_url}"')
+        self.assertContains(response, f'"skymap_url":"{self.eventlocalization2.skymap_url}"')
 
     def test_nonlocalizedevent_index_view(self):
         response = self.client.get(reverse('nonlocalizedevents:index'))
 
         self.assertContains(response, self.superevent1.event_id)
         self.assertContains(response, self.superevent2.event_id)
         self.assertContains(response, reverse('nonlocalizedevents:detail', args=(self.superevent1.pk,)))
```

### Comparing `tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/urls.py` & `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/urls.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,9 +17,9 @@
 # (i.e. {% url 'nonlocalizedevents:detail' <pk> %}
 app_name = 'nonlocalizedevents'
 
 urlpatterns = [
     path('', views.NonLocalizedEventListView.as_view(), name='index'),
     path('<int:pk>/', SupereventPkView.as_view(), name='detail'),
     path('<str:event_id>/', SupereventIdView.as_view(), name='event-detail'),
-    path('alert/createfrom', views.CreateEventFromSCiMMAAlertView.as_view(), name='create-from-alert')
+    path('alert/createfrom', views.CreateEventFromHermesAlertView.as_view(), name='create-from-alert')
 ]
```

### Comparing `tom_nonlocalizedevents-0.6.3/tom_nonlocalizedevents/views.py` & `tom_nonlocalizedevents-0.7.1/tom_nonlocalizedevents/views.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,107 +1,91 @@
 import json
+import logging
 
 from django.contrib import messages
 from django.core.cache import cache
 from django.http import Http404
 from django.shortcuts import redirect
 from django.contrib.auth.mixins import LoginRequiredMixin
 from django.views.generic import ListView, TemplateView
 from django.views.generic.base import View
 from django.urls import reverse
 from django.conf import settings
 
 from rest_framework import permissions, viewsets
 from django_filters.rest_framework import DjangoFilterBackend
 
+from tom_nonlocalizedevents.ingestion import ingest_sequence_from_hermes_message
 from tom_nonlocalizedevents.models import EventCandidate, EventLocalization, NonLocalizedEvent
 from tom_nonlocalizedevents.serializers import (EventCandidateSerializer, EventLocalizationSerializer,
                                                 NonLocalizedEventSerializer)
 
 
+logger = logging.getLogger(__name__)
+
+
 class NonLocalizedEventListView(LoginRequiredMixin, ListView):
     """
     Unadorned Django ListView subclass for NonLocalizedEvent model.
     """
     model = NonLocalizedEvent
     template_name = 'tom_nonlocalizedevents/index.html'
 
     def get_queryset(self):
         # '-created' is most recent first
         qs = NonLocalizedEvent.objects.order_by('-created')
         return qs
 
 
 # from the tom_alerts query_result.html
-
-class CreateEventFromSCiMMAAlertView(View):
+class CreateEventFromHermesAlertView(View):
     """
     Creates the models.NonLocalizedEvent instance and redirect to NonLocalizedEventDetailView
     """
-    pass
 
     def post(self, request, *args, **kwargs):
         """
         """
         # the request.POST is a QueryDict object;
-        # for SCiMMA, alerts: list items are PKs to skip.dev.hop.scimma.org/api/alerts/PK/
         query_id = self.request.POST['query_id']
-        # broker_name = self.request.POST['broker']  # should be "SCIMMA"
-        # broker_class = get_service_class(broker_name)  # should be <class 'tom_scimma.scimma.SCIMMABroker'>
-        alerts = [int(id) for id in request.POST.getlist('alerts', [])]
 
-        errors = []
+        # events is a list[str] of NonLocalizedEvent event_id's: (e.g. 'MS230417a')
+        # (i.e the selected events from the query result form)
+        events = request.POST.getlist('events', [])
+
         # if the user didn't select an alert; warn and re-direct back
-        if not alerts:
-            messages.warning(request, 'Please select at least one alert from which to create an event.')
+        if not events:
+            messages.warning(request, 'Please select at least one Event to create.')
             reverse_url: str = reverse('tom_alerts:run', kwargs={'pk': query_id})
             return redirect(reverse_url)
 
-        # try to extract EventID from Alert and use it to create a NoneLocalizedEvent
-        for alert_id in alerts:
-            cached_alert = json.loads(cache.get(f'alert_{alert_id}'))  # cached by tom_alerts.views.py::RunQueryView
+        # Create NonLocalizedEvents for each of the selected events.
+        for event_id in events:
+            logger.debug(f'Creating event {event_id}...')
+            # extract the Hermes event from the cache
+            # (it was cached by tom_alerts.views.py::RunQueryView)
+            cached_event = json.loads(cache.get(f'alert_{event_id}'))
+
             # early return: alert not in cache
-            if not cached_alert:
-                messages.error(request, 'Could not create event(s). Try re-running the query to refresh the cache.')
+            if not cached_event:
+                messages.error(request, 'Could not createn event(s). Try re-running the query to refresh the cache.')
                 return redirect(reverse('tom_alerts:run', kwargs={'pk': query_id}))
 
-            # early return: alert not LVC/LVC COUNTERPART NOTICE
-            if cached_alert.get('topic', '') != 'lvc.lvc-counterpart':
-                messages.error(request,
-                               ('Only Alerts from the lvc.lvc-counterpart topic have '
-                                'parsed event_trig_num required for Event origination. '
-                                'Please select an appropriate alert.'))
-                return redirect(reverse('tom_alerts:run', kwargs={'pk': query_id}))
+            # the NonLocalizedEvent is created by handling all the messages from
+            # the event sequence as if they were ingested
+            for sequenced_message in cached_event['sequences']:
+                logger.debug(f"Creating sequence from HermesBroker: {sequenced_message}")
+                ingest_sequence_from_hermes_message(sequenced_message)
 
-            # early return: event_trig_num not found in parsed alert message
-            event_trig_num = cached_alert['message'].get('event_trig_num', None)
-            if event_trig_num is None:
-                messages.error(request,
-                               (f'Could not create event for alert: {alert_id}. '
-                                'event_trig_num not found in alert message.'))
-                return redirect(reverse('tom_alerts:run', kwargs={'pk': query_id}))
+        return redirect(reverse('nonlocalizedevents:index'))
 
-            nonlocalizedevent, created = NonLocalizedEvent.objects.get_or_create(event_id=event_trig_num)
-            if not created:
-                # the nonlocalizedevent already existed
-                messages.warning(request, f'Event {event_trig_num} already exists.')
-                errors.append(nonlocalizedevent.event_id)
-
-        if len(alerts) == len(errors):
-            # zero nonlocalizedevents created
-            return redirect(reverse('tom_alerts:run', kwargs={'pk': query_id}))
-        elif len(alerts) == 1:
-            # one nonlocalizedevent created
-            return redirect(reverse('nonlocalizedevents:detail', kwargs={'pk': nonlocalizedevent.pk}))
-        else:
-            # multipe nonlocalizedevent created
-            return redirect(reverse('nonlocalizedevents:index'))
 
+#
 # Django Rest Framework Views
-
+#
 
 class NonLocalizedEventViewSet(viewsets.ModelViewSet):
     """
     DRF API endpoint that allows NonLocalizedEvents to be viewed or edited.
     """
     queryset = NonLocalizedEvent.objects.all()
     serializer_class = NonLocalizedEventSerializer
@@ -158,41 +142,32 @@
 
 
 class SupereventPkView(LoginRequiredMixin, TemplateView):
     template_name = 'tom_nonlocalizedevents/superevent_vue_app.html'
 
     def get_context_data(self, **kwargs: dict) -> dict:
         context = super().get_context_data(**kwargs)
-        superevent = NonLocalizedEvent.objects.get(pk=kwargs['pk'])
-        sequences = list(superevent.sequences.order_by('sequence_id').values(
-            'sequence_id', 'event_subtype', 'created', 'pk'))
-        for sequence in sequences:
-            # Set the created date as a string so it can be in json format
-            sequence['created'] = sequence['created'].isoformat()
-        context['superevent_pk'] = kwargs['pk']
-        context['superevent_id'] = superevent.event_id
-        context['sequences'] = json.dumps(sequences)
-        context['tom_api_url'] = settings.TOM_API_URL
-        context['hermes_api_url'] = settings.HERMES_API_URL
-        return context
+        try:
+            superevent = NonLocalizedEvent.objects.get(pk=kwargs['pk'])
+            data = NonLocalizedEventSerializer(instance=superevent).data
+            context['superevent_data'] = json.dumps(data)
+            context['tom_api_url'] = settings.TOM_API_URL
+            context['hermes_api_url'] = settings.HERMES_API_URL
+            return context
+        except NonLocalizedEvent.DoesNotExist:
+            raise Http404
 
 
 class SupereventIdView(LoginRequiredMixin, TemplateView):
     template_name = 'tom_nonlocalizedevents/superevent_vue_app.html'
 
     def get_context_data(self, **kwargs: dict) -> dict:
         context = super().get_context_data(**kwargs)
         try:
             superevent = NonLocalizedEvent.objects.get(event_id=kwargs['event_id'])
-            sequences = list(superevent.sequences.order_by('sequence_id').values(
-                'sequence_id', 'event_subtype', 'created', 'pk'))
-            for sequence in sequences:
-                # Set the created date as a string so it can be in json format
-                sequence['created'] = sequence['created'].isoformat()
-            context['superevent_id'] = kwargs['event_id']
-            context['superevent_pk'] = superevent.pk
-            context['sequences'] = json.dumps(sequences)
+            data = NonLocalizedEventSerializer(instance=superevent).data
+            context['superevent_data'] = json.dumps(data)
             context['tom_api_url'] = settings.TOM_API_URL
             context['hermes_api_url'] = settings.HERMES_API_URL
             return context
         except NonLocalizedEvent.DoesNotExist:
             raise Http404
```

### Comparing `tom_nonlocalizedevents-0.6.3/PKG-INFO` & `tom_nonlocalizedevents-0.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tom-nonlocalizedevents
-Version: 0.6.3
+Version: 0.7.1
 Summary: Reusable TOMToolkit app to support gravitational wave superevent and other nonlocalized event EM follow-up observations.
 Home-page: https://github.com/TOMToolkit/tom_nonlocalizedevents
 License: GPL-3.0-only
 Keywords: tomtoolkit,astronomy,astrophysics,cosmology,science
 Author: TOM Toolkit Project
 Author-email: tomtoolkit@lco.global
 Requires-Python: >=3.8,<3.12
@@ -25,30 +25,32 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Dist: MOCPy (==0.11.0)
-Requires-Dist: SQLAlchemy (>=1.4.42,<2.0.0)
+Requires-Dist: MOCPy (>=0.12.2)
+Requires-Dist: SQLAlchemy (>=1.4.42)
+Requires-Dist: astropy (>=5.2)
 Requires-Dist: astropy-healpix (>=0.7)
 Requires-Dist: django-filter (>=21.0,<22.0)
 Requires-Dist: django-webpack-loader (==1.6.0)
 Requires-Dist: gracedb-sdk (>=0.1,<0.2)
-Requires-Dist: healpix-alchemy (>=1.0.0)
+Requires-Dist: healpix-alchemy (>=1.0.2)
+Requires-Dist: hop-client (>=0.8)
 Requires-Dist: ligo.skymap (>=1.0.3,<2.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.4,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8,<3.0)
 Requires-Dist: tomtoolkit (>=2.10,<3.0)
 Requires-Dist: voevent-parse (>=1.0,<2.0)
 Project-URL: Repository, https://github.com/TOMToolkit/tom_nonlocalizedevents
 Description-Content-Type: text/markdown
 
-[![pypi](https://img.shields.io/pypi/v/tom-superevents.svg)](https://pypi.python.org/pypi/tom-superevents)
+[![pypi](https://img.shields.io/pypi/v/tom-nonlocalizedevents.svg)](https://pypi.python.org/pypi/tom-nonlocalizedevents)
 [![run-tests](https://github.com/TOMToolkit/tom_nonlocalizedevents/actions/workflows/run-tests.yml/badge.svg)](https://github.com/TOMToolkit/tom_nonlocalizedevents/actions/workflows/run-tests.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/cbcf7ce565d8450f86fff863ef061ff9)](https://www.codacy.com/gh/TOMToolkit/tom_nonlocalizedevents/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=TOMToolkit/tom_nonlocalizedevents&amp;utm_campaign=Badge_Grade)
 [![Coverage Status](https://coveralls.io/repos/github/TOMToolkit/tom_nonlocalizedevents/badge.svg?branch=main)](https://coveralls.io/github/TOMToolkit/tom_nonlocalizedevents?branch=main)
 
 # GW Superevent (or GRB, Neutrino) EM follow-up
 
 This reusable TOM Toolkit app provides support for gravitational wave (GW) superevent
@@ -112,18 +114,19 @@
 
 5. Set environment variables below to configure different connections:
 
 | Env variable | Description | Default |
 | ------------ | ----------- | ------- |
 | `SA_DB_CONNECTION_URL` | Location of your django postgres database used for sqlalchemy | by default, this uses Django `default` DB for the project |
 | `CREDIBLE_REGION_PROBABILITIES` | JSON List of Credible Region probabilities to automatically check each candidate target for | `'[0.25, 0.5, 0.75, 0.9, 0.95]'` |
+| `SAVE_TEST_ALERTS` | Boolean on if you want to save test nonlocalizedevents into your database (those with event_id beginning with 'M') | `true` |
 
 6. In your TOM project, make sure to run `python manage.py collectstatic` after installing this app, to collect its Vue pages into your `staticfiles` directory.
 
-7. If you want to automatically ingest GW events into your TOM, you should also install the `tom_alertstreams` app into your TOM and configure it to use the tom_nonlocalizedevents handler to ingest GW events: `tom_nonlocalizedevents.alertstream_handlers.gw_event_handler.handle_message`. There is also a handler to handle retractions via the `handle_retraction` method in that package. These are currently written to work with LVC GW messages.
+7. If you want to automatically ingest GW events into your TOM, you should also install the `tom_alertstreams` app into your TOM and configure it to use the tom_nonlocalizedevents handler to ingest GW events. The preferred way is to use the hop `igwn.gwalerts` topic and set it to the handler `tom_nonlocalizedevents.alertstream_handlers.igwn_event_handler.handle_igwn_message`. This format has the newest Ligo O4 fields. There is legacy support for the gcn classic over kafka plaintext formatted LVC alerts using the handler `tom_nonlocalizedevents.alertstream_handlers.gcn_event_handler.handle_message`. There is also a handler to handle retractions via the `handle_retraction` method in that package. For an example of what needs to be in your settings to configure `tom_alertstreams` for these streams, look [here](https://github.com/LCOGT/hermes/blob/dev/hermes_base/settings.py#L232)
 
 ## Development
 
 When any changes are made to this library, the vue files will need to be build and bundled and committed into the repo so that they can be bundled and deployed with the django package. This means that after making any vue changes, you must run `npm run build` within the `tom_nonlocalizedevents_vue` directory once, which will install the built files into `tom_nonlocalizedevents/static/`, and then those built files will need to be committed into the repo. This allows django projects using this library to get those files when running `python manage.py collectstatic`.
 
 ## Running the tests
```

