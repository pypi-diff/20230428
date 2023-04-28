# Comparing `tmp/lndb-0.44.6.tar.gz` & `tmp/lndb-0.44.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lndb-0.44.6.tar", last modified: Thu Apr 27 17:05:47 2023, max compression
+gzip compressed data, was "lndb-0.44.7.tar", last modified: Fri Apr 28 05:57:26 2023, max compression
```

## Comparing `lndb-0.44.6.tar` & `lndb-0.44.7.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0     3832 2023-04-10 14:26:28.783318 lndb-0.44.6/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-03-15 08:56:55.830020 lndb-0.44.6/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-03-15 08:56:55.830119 lndb-0.44.6/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-03-15 08:56:55.830224 lndb-0.44.6/.gitignore
--rw-r--r--   0        0        0     1777 2023-04-24 09:27:00.933000 lndb-0.44.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-03-15 08:56:55.830520 lndb-0.44.6/LICENSE
--rw-r--r--   0        0        0      173 2023-03-27 05:09:16.038571 lndb-0.44.6/README.md
--rw-r--r--   0        0        0       52 2023-03-15 08:56:55.830736 lndb-0.44.6/docs/api.md
--rw-r--r--   0        0        0    48038 2023-04-27 17:04:52.978133 lndb-0.44.6/docs/changelog.md
--rw-r--r--   0        0        0     4832 2023-03-15 08:56:55.831086 lndb-0.44.6/docs/faq/check-synchronization.ipynb
--rw-r--r--   0        0        0     3334 2023-03-15 08:56:55.831186 lndb-0.44.6/docs/faq/clone.ipynb
--rw-r--r--   0        0        0     8397 2023-03-27 05:09:16.039131 lndb-0.44.6/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      166 2023-03-27 05:09:16.039234 lndb-0.44.6/docs/faq/index.md
--rw-r--r--   0        0        0     1182 2023-04-22 15:24:35.393597 lndb-0.44.6/docs/faq/manage-migrations.ipynb
--rw-r--r--   0        0        0     3248 2023-03-15 08:56:55.831660 lndb-0.44.6/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     2798 2023-04-10 14:26:28.783932 lndb-0.44.6/docs/faq/test-migrations-e2e.ipynb
--rw-r--r--   0        0        0     2073 2023-04-10 14:26:28.784059 lndb-0.44.6/docs/faq/test-migrations-unit.ipynb
--rw-r--r--   0        0        0     5163 2023-03-27 05:09:16.039598 lndb-0.44.6/docs/guide/01-setup-user.ipynb
--rw-r--r--   0        0        0    10238 2023-04-27 10:15:48.138286 lndb-0.44.6/docs/guide/02-init-instance.ipynb
--rw-r--r--   0        0        0     6419 2023-04-27 10:15:48.138461 lndb-0.44.6/docs/guide/03-load-instance.ipynb
--rw-r--r--   0        0        0     6390 2023-04-24 09:27:00.941223 lndb-0.44.6/docs/guide/04-set-storage.ipynb
--rw-r--r--   0        0        0     3746 2023-04-26 05:23:05.373464 lndb-0.44.6/docs/guide/05-schema-modules.ipynb
--rw-r--r--   0        0        0     1496 2023-03-27 05:09:16.039994 lndb-0.44.6/docs/guide/06-info.ipynb
--rw-r--r--   0        0        0     2689 2023-04-21 03:09:31.419101 lndb-0.44.6/docs/guide/07-delete.ipynb
--rw-r--r--   0        0        0      129 2023-03-15 08:56:55.832700 lndb-0.44.6/docs/guide/index.md
--rw-r--r--   0        0        0     3158 2023-04-22 15:24:35.394504 lndb-0.44.6/docs/guide/migrate.md
--rw-r--r--   0        0        0      126 2023-03-15 08:56:55.832922 lndb-0.44.6/docs/index.md
--rw-r--r--   0        0        0      118 2023-03-15 08:56:55.833018 lndb-0.44.6/lamin-project.yaml
--rw-r--r--   0        0        0     1993 2023-04-27 17:04:10.694916 lndb-0.44.6/lndb/__init__.py
--rw-r--r--   0        0        0     4697 2023-04-27 17:03:55.795190 lndb-0.44.6/lndb/__main__.py
--rw-r--r--   0        0        0      100 2023-03-15 08:56:55.833550 lndb-0.44.6/lndb/_assets/__init__.py
--rw-r--r--   0        0        0     1414 2023-04-10 14:26:28.784379 lndb-0.44.6/lndb/_check_instance_setup.py
--rw-r--r--   0        0        0      221 2023-04-27 10:15:48.138789 lndb-0.44.6/lndb/_check_versions.py
--rw-r--r--   0        0        0      567 2023-04-10 14:26:28.784709 lndb-0.44.6/lndb/_close.py
--rw-r--r--   0        0        0     2146 2023-04-10 14:26:28.784835 lndb-0.44.6/lndb/_delete.py
--rw-r--r--   0        0        0      329 2023-04-26 05:23:05.375280 lndb-0.44.6/lndb/_info.py
--rw-r--r--   0        0        0     6035 2023-04-27 10:15:48.139549 lndb-0.44.6/lndb/_init_instance.py
--rw-r--r--   0        0        0     6729 2023-04-27 10:15:48.140360 lndb-0.44.6/lndb/_load_instance.py
--rw-r--r--   0        0        0      135 2023-04-10 14:26:28.785194 lndb-0.44.6/lndb/_migrate/__init__.py
--rw-r--r--   0        0        0      723 2023-04-10 14:26:28.785299 lndb-0.44.6/lndb/_migrate/alembic.ini
--rw-r--r--   0        0        0     3704 2023-04-26 05:23:05.375597 lndb-0.44.6/lndb/_migrate/core.py
--rw-r--r--   0        0        0     7644 2023-04-22 15:24:35.395863 lndb-0.44.6/lndb/_migrate/deploy.py
--rw-r--r--   0        0        0     3179 2023-03-15 08:56:55.834680 lndb-0.44.6/lndb/_migrate/env.py
--rw-r--r--   0        0        0      334 2023-04-26 05:23:05.375756 lndb-0.44.6/lndb/_migrate/script.py.mako
--rw-r--r--   0        0        0     4840 2023-04-10 14:26:28.785570 lndb-0.44.6/lndb/_migrate/utils.py
--rw-r--r--   0        0        0      803 2023-04-27 10:15:48.140662 lndb-0.44.6/lndb/_register_instance.py
--rw-r--r--   0        0        0     1020 2023-03-15 08:56:55.834857 lndb-0.44.6/lndb/_schema.py
--rw-r--r--   0        0        0     1830 2023-04-24 09:27:00.946199 lndb-0.44.6/lndb/_set.py
--rw-r--r--   0        0        0     2189 2023-04-19 06:33:40.117765 lndb-0.44.6/lndb/_settings.py
--rw-r--r--   0        0        0       87 2023-03-15 08:56:55.835145 lndb-0.44.6/lndb/_settings_load.py
--rw-r--r--   0        0        0       72 2023-03-15 08:56:55.835215 lndb-0.44.6/lndb/_settings_store.py
--rw-r--r--   0        0        0     3902 2023-04-21 03:09:31.420591 lndb-0.44.6/lndb/_setup_user.py
--rw-r--r--   0        0        0      533 2023-04-10 14:26:28.785901 lndb-0.44.6/lndb/dev/__init__.py
--rw-r--r--   0        0        0     4030 2023-03-28 04:03:47.769616 lndb-0.44.6/lndb/dev/_clone.py
--rw-r--r--   0        0        0     6226 2023-04-10 14:26:28.786021 lndb-0.44.6/lndb/dev/_db.py
--rw-r--r--   0        0        0     2491 2023-03-15 08:56:55.835748 lndb-0.44.6/lndb/dev/_deprecated.py
--rw-r--r--   0        0        0      240 2023-03-15 08:56:55.835829 lndb-0.44.6/lndb/dev/_docs.py
--rw-r--r--   0        0        0     5317 2023-04-10 14:26:28.786141 lndb-0.44.6/lndb/dev/_exclusion.py
--rw-r--r--   0        0        0     8946 2023-04-27 10:15:48.140982 lndb-0.44.6/lndb/dev/_settings_instance.py
--rw-r--r--   0        0        0     2629 2023-03-27 05:09:16.041820 lndb-0.44.6/lndb/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-03-15 08:56:55.836258 lndb-0.44.6/lndb/dev/_settings_save.py
--rw-r--r--   0        0        0     2314 2023-04-10 14:26:28.786361 lndb-0.44.6/lndb/dev/_settings_store.py
--rw-r--r--   0        0        0      976 2023-03-15 08:56:55.836438 lndb-0.44.6/lndb/dev/_settings_user.py
--rw-r--r--   0        0        0     2446 2023-03-20 10:25:09.955595 lndb-0.44.6/lndb/dev/_setup_knowledge.py
--rw-r--r--   0        0        0     7204 2023-04-23 05:23:25.735656 lndb-0.44.6/lndb/dev/_setup_schema.py
--rw-r--r--   0        0        0     5288 2023-04-24 09:27:00.951105 lndb-0.44.6/lndb/dev/_storage.py
--rw-r--r--   0        0        0      140 2023-03-15 08:56:55.836803 lndb-0.44.6/lndb/dev/_testdb.py
--rw-r--r--   0        0        0     2536 2023-04-10 14:26:28.786692 lndb-0.44.6/lndb/dev/upath.py
--rw-r--r--   0        0        0      356 2023-04-10 14:26:28.786816 lndb-0.44.6/lndb/test/__init__.py
--rw-r--r--   0        0        0       50 2023-03-15 08:56:55.837137 lndb-0.44.6/lndb/test/_env.py
--rw-r--r--   0        0        0     3911 2023-04-27 10:15:48.141161 lndb-0.44.6/lndb/test/_migrations_e2e.py
--rw-r--r--   0        0        0     6646 2023-04-10 14:26:28.787063 lndb-0.44.6/lndb/test/_migrations_unit.py
--rw-r--r--   0        0        0      310 2023-03-15 08:56:55.837581 lndb-0.44.6/lndb/test/_nox.py
--rw-r--r--   0        0        0      188 2023-03-15 08:56:55.837695 lndb-0.44.6/lndb/test/nox.py
--rw-r--r--   0        0        0     1003 2023-04-10 14:26:28.787186 lndb-0.44.6/noxfile.py
--rw-r--r--   0        0        0     1396 2023-04-27 10:15:48.141448 lndb-0.44.6/pyproject.toml
--rw-r--r--   0        0        0      513 2023-04-10 14:26:28.787386 lndb-0.44.6/tests/test_bionty.py
--rw-r--r--   0        0        0      680 2023-03-15 08:56:55.838152 lndb-0.44.6/tests/test_init_instance.py
--rw-r--r--   0        0        0      384 2023-04-18 16:24:58.325988 lndb-0.44.6/tests/test_notebooks.py
--rw-r--r--   0        0        0     1198 1970-01-01 00:00:00.000000 lndb-0.44.6/PKG-INFO
+-rw-r--r--   0        0        0     3832 2023-04-10 14:26:28.783318 lndb-0.44.7/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-03-15 08:56:55.830020 lndb-0.44.7/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-03-15 08:56:55.830119 lndb-0.44.7/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-03-15 08:56:55.830224 lndb-0.44.7/.gitignore
+-rw-r--r--   0        0        0     1777 2023-04-24 09:27:00.933000 lndb-0.44.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-03-15 08:56:55.830520 lndb-0.44.7/LICENSE
+-rw-r--r--   0        0        0      173 2023-03-27 05:09:16.038571 lndb-0.44.7/README.md
+-rw-r--r--   0        0        0       52 2023-03-15 08:56:55.830736 lndb-0.44.7/docs/api.md
+-rw-r--r--   0        0        0    48191 2023-04-28 05:56:59.401992 lndb-0.44.7/docs/changelog.md
+-rw-r--r--   0        0        0     4832 2023-03-15 08:56:55.831086 lndb-0.44.7/docs/faq/check-synchronization.ipynb
+-rw-r--r--   0        0        0     3334 2023-03-15 08:56:55.831186 lndb-0.44.7/docs/faq/clone.ipynb
+-rw-r--r--   0        0        0     8397 2023-03-27 05:09:16.039131 lndb-0.44.7/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      166 2023-03-27 05:09:16.039234 lndb-0.44.7/docs/faq/index.md
+-rw-r--r--   0        0        0     1182 2023-04-22 15:24:35.393597 lndb-0.44.7/docs/faq/manage-migrations.ipynb
+-rw-r--r--   0        0        0     3248 2023-03-15 08:56:55.831660 lndb-0.44.7/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     2798 2023-04-10 14:26:28.783932 lndb-0.44.7/docs/faq/test-migrations-e2e.ipynb
+-rw-r--r--   0        0        0     2073 2023-04-10 14:26:28.784059 lndb-0.44.7/docs/faq/test-migrations-unit.ipynb
+-rw-r--r--   0        0        0     5163 2023-03-27 05:09:16.039598 lndb-0.44.7/docs/guide/01-setup-user.ipynb
+-rw-r--r--   0        0        0    10238 2023-04-27 10:15:48.138286 lndb-0.44.7/docs/guide/02-init-instance.ipynb
+-rw-r--r--   0        0        0     6419 2023-04-27 10:15:48.138461 lndb-0.44.7/docs/guide/03-load-instance.ipynb
+-rw-r--r--   0        0        0     6390 2023-04-24 09:27:00.941223 lndb-0.44.7/docs/guide/04-set-storage.ipynb
+-rw-r--r--   0        0        0     3746 2023-04-26 05:23:05.373464 lndb-0.44.7/docs/guide/05-schema-modules.ipynb
+-rw-r--r--   0        0        0     1496 2023-03-27 05:09:16.039994 lndb-0.44.7/docs/guide/06-info.ipynb
+-rw-r--r--   0        0        0     2689 2023-04-21 03:09:31.419101 lndb-0.44.7/docs/guide/07-delete.ipynb
+-rw-r--r--   0        0        0      129 2023-03-15 08:56:55.832700 lndb-0.44.7/docs/guide/index.md
+-rw-r--r--   0        0        0     3158 2023-04-22 15:24:35.394504 lndb-0.44.7/docs/guide/migrate.md
+-rw-r--r--   0        0        0      126 2023-03-15 08:56:55.832922 lndb-0.44.7/docs/index.md
+-rw-r--r--   0        0        0      118 2023-03-15 08:56:55.833018 lndb-0.44.7/lamin-project.yaml
+-rw-r--r--   0        0        0     1993 2023-04-28 05:56:52.880114 lndb-0.44.7/lndb/__init__.py
+-rw-r--r--   0        0        0     4697 2023-04-27 17:03:55.795190 lndb-0.44.7/lndb/__main__.py
+-rw-r--r--   0        0        0      100 2023-03-15 08:56:55.833550 lndb-0.44.7/lndb/_assets/__init__.py
+-rw-r--r--   0        0        0     1414 2023-04-10 14:26:28.784379 lndb-0.44.7/lndb/_check_instance_setup.py
+-rw-r--r--   0        0        0      221 2023-04-28 05:45:57.926671 lndb-0.44.7/lndb/_check_versions.py
+-rw-r--r--   0        0        0      567 2023-04-10 14:26:28.784709 lndb-0.44.7/lndb/_close.py
+-rw-r--r--   0        0        0     2146 2023-04-10 14:26:28.784835 lndb-0.44.7/lndb/_delete.py
+-rw-r--r--   0        0        0      329 2023-04-26 05:23:05.375280 lndb-0.44.7/lndb/_info.py
+-rw-r--r--   0        0        0     6035 2023-04-27 10:15:48.139549 lndb-0.44.7/lndb/_init_instance.py
+-rw-r--r--   0        0        0     6729 2023-04-27 10:15:48.140360 lndb-0.44.7/lndb/_load_instance.py
+-rw-r--r--   0        0        0      135 2023-04-10 14:26:28.785194 lndb-0.44.7/lndb/_migrate/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-10 14:26:28.785299 lndb-0.44.7/lndb/_migrate/alembic.ini
+-rw-r--r--   0        0        0     3704 2023-04-26 05:23:05.375597 lndb-0.44.7/lndb/_migrate/core.py
+-rw-r--r--   0        0        0     7644 2023-04-22 15:24:35.395863 lndb-0.44.7/lndb/_migrate/deploy.py
+-rw-r--r--   0        0        0     3179 2023-03-15 08:56:55.834680 lndb-0.44.7/lndb/_migrate/env.py
+-rw-r--r--   0        0        0      334 2023-04-26 05:23:05.375756 lndb-0.44.7/lndb/_migrate/script.py.mako
+-rw-r--r--   0        0        0     4840 2023-04-10 14:26:28.785570 lndb-0.44.7/lndb/_migrate/utils.py
+-rw-r--r--   0        0        0      803 2023-04-27 10:15:48.140662 lndb-0.44.7/lndb/_register_instance.py
+-rw-r--r--   0        0        0     1020 2023-03-15 08:56:55.834857 lndb-0.44.7/lndb/_schema.py
+-rw-r--r--   0        0        0     1830 2023-04-24 09:27:00.946199 lndb-0.44.7/lndb/_set.py
+-rw-r--r--   0        0        0     2189 2023-04-19 06:33:40.117765 lndb-0.44.7/lndb/_settings.py
+-rw-r--r--   0        0        0       87 2023-03-15 08:56:55.835145 lndb-0.44.7/lndb/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-03-15 08:56:55.835215 lndb-0.44.7/lndb/_settings_store.py
+-rw-r--r--   0        0        0     3902 2023-04-21 03:09:31.420591 lndb-0.44.7/lndb/_setup_user.py
+-rw-r--r--   0        0        0      533 2023-04-10 14:26:28.785901 lndb-0.44.7/lndb/dev/__init__.py
+-rw-r--r--   0        0        0     4030 2023-03-28 04:03:47.769616 lndb-0.44.7/lndb/dev/_clone.py
+-rw-r--r--   0        0        0     6226 2023-04-10 14:26:28.786021 lndb-0.44.7/lndb/dev/_db.py
+-rw-r--r--   0        0        0     2491 2023-03-15 08:56:55.835748 lndb-0.44.7/lndb/dev/_deprecated.py
+-rw-r--r--   0        0        0      240 2023-03-15 08:56:55.835829 lndb-0.44.7/lndb/dev/_docs.py
+-rw-r--r--   0        0        0     5317 2023-04-10 14:26:28.786141 lndb-0.44.7/lndb/dev/_exclusion.py
+-rw-r--r--   0        0        0     8946 2023-04-27 10:15:48.140982 lndb-0.44.7/lndb/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2629 2023-03-27 05:09:16.041820 lndb-0.44.7/lndb/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-03-15 08:56:55.836258 lndb-0.44.7/lndb/dev/_settings_save.py
+-rw-r--r--   0        0        0     2314 2023-04-10 14:26:28.786361 lndb-0.44.7/lndb/dev/_settings_store.py
+-rw-r--r--   0        0        0      976 2023-03-15 08:56:55.836438 lndb-0.44.7/lndb/dev/_settings_user.py
+-rw-r--r--   0        0        0     2446 2023-03-20 10:25:09.955595 lndb-0.44.7/lndb/dev/_setup_knowledge.py
+-rw-r--r--   0        0        0     7204 2023-04-23 05:23:25.735656 lndb-0.44.7/lndb/dev/_setup_schema.py
+-rw-r--r--   0        0        0     5288 2023-04-24 09:27:00.951105 lndb-0.44.7/lndb/dev/_storage.py
+-rw-r--r--   0        0        0      140 2023-03-15 08:56:55.836803 lndb-0.44.7/lndb/dev/_testdb.py
+-rw-r--r--   0        0        0     2536 2023-04-10 14:26:28.786692 lndb-0.44.7/lndb/dev/upath.py
+-rw-r--r--   0        0        0      356 2023-04-10 14:26:28.786816 lndb-0.44.7/lndb/test/__init__.py
+-rw-r--r--   0        0        0       50 2023-03-15 08:56:55.837137 lndb-0.44.7/lndb/test/_env.py
+-rw-r--r--   0        0        0     3911 2023-04-27 10:15:48.141161 lndb-0.44.7/lndb/test/_migrations_e2e.py
+-rw-r--r--   0        0        0     6646 2023-04-10 14:26:28.787063 lndb-0.44.7/lndb/test/_migrations_unit.py
+-rw-r--r--   0        0        0      310 2023-03-15 08:56:55.837581 lndb-0.44.7/lndb/test/_nox.py
+-rw-r--r--   0        0        0      188 2023-03-15 08:56:55.837695 lndb-0.44.7/lndb/test/nox.py
+-rw-r--r--   0        0        0     1003 2023-04-10 14:26:28.787186 lndb-0.44.7/noxfile.py
+-rw-r--r--   0        0        0     1396 2023-04-28 05:45:57.926943 lndb-0.44.7/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-04-10 14:26:28.787386 lndb-0.44.7/tests/test_bionty.py
+-rw-r--r--   0        0        0      680 2023-03-15 08:56:55.838152 lndb-0.44.7/tests/test_init_instance.py
+-rw-r--r--   0        0        0      384 2023-04-18 16:24:58.325988 lndb-0.44.7/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1198 1970-01-01 00:00:00.000000 lndb-0.44.7/PKG-INFO
```

### Comparing `lndb-0.44.6/.github/workflows/build.yml` & `lndb-0.44.7/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/.github/workflows/latest-changes.yml` & `lndb-0.44.7/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/.gitignore` & `lndb-0.44.7/.gitignore`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/.pre-commit-config.yaml` & `lndb-0.44.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/LICENSE` & `lndb-0.44.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/docs/changelog.md` & `lndb-0.44.7/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+⬆️ Upgrade lnhub-rest to 0.9.4 | [373](https://github.com/laminlabs/lndb/pull/373) | [sunnyosun](https://github.com/sunnyosun) | 2023-04-28 | 0.44.7
 🚑 Fix load | [372](https://github.com/laminlabs/lndb/pull/372) | [sunnyosun](https://github.com/sunnyosun) | 2023-04-27 | 0.44.6
 ✨ Add `--storage` arg to `lamin load` | [370](https://github.com/laminlabs/lndb/pull/370) | [falexwolf](https://github.com/falexwolf) | 2023-04-27 |
 ⬆️ Upgrade lnhub-rest | [369](https://github.com/laminlabs/lndb/pull/369) | [fredericenard](https://github.com/fredericenard) | 2023-04-25 | 0.44.5
 ✨ Allow to set additional fsspec kwargs for cloud instances | [366](https://github.com/laminlabs/lndb/pull/366) | [Koncopd](https://github.com/Koncopd) | 2023-04-23 | 0.44.4
 ⬆️ Upgrade lnhub-rest to 0.8.2 | [365](https://github.com/laminlabs/lndb/pull/365) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 | 0.44.2
 🚸 New migration deployment logic that also factors in migration ids | [364](https://github.com/laminlabs/lndb/pull/364) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 |
 🚸 Mute warning about DB not reachable in init | [363](https://github.com/laminlabs/lndb/pull/363) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 |
```

### Comparing `lndb-0.44.6/docs/faq/check-synchronization.ipynb` & `lndb-0.44.7/docs/faq/check-synchronization.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/docs/faq/clone.ipynb` & `lndb-0.44.7/docs/faq/clone.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/docs/faq/edge-cases-login-init.ipynb` & `lndb-0.44.7/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/docs/faq/manage-migrations.ipynb` & `lndb-0.44.7/docs/faq/manage-migrations.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/docs/faq/switch-environment.ipynb` & `lndb-0.44.7/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/docs/faq/test-migrations-e2e.ipynb` & `lndb-0.44.7/docs/faq/test-migrations-e2e.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/docs/faq/test-migrations-unit.ipynb` & `lndb-0.44.7/docs/faq/test-migrations-unit.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/docs/guide/01-setup-user.ipynb` & `lndb-0.44.7/docs/guide/01-setup-user.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/docs/guide/02-init-instance.ipynb` & `lndb-0.44.7/docs/guide/02-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/docs/guide/03-load-instance.ipynb` & `lndb-0.44.7/docs/guide/03-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/docs/guide/04-set-storage.ipynb` & `lndb-0.44.7/docs/guide/04-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/docs/guide/05-schema-modules.ipynb` & `lndb-0.44.7/docs/guide/05-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/docs/guide/06-info.ipynb` & `lndb-0.44.7/docs/guide/06-info.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/docs/guide/07-delete.ipynb` & `lndb-0.44.7/docs/guide/07-delete.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/docs/guide/migrate.md` & `lndb-0.44.7/docs/guide/migrate.md`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/__init__.py` & `lndb-0.44.7/lndb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 .. autosummary::
    :toctree:
 
    dev
 """
 
-__version__ = "0.44.6"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.44.7"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import _check_versions  # noqa
 from . import dev, test
 from ._close import close  # noqa
```

### Comparing `lndb-0.44.6/lndb/__main__.py` & `lndb-0.44.7/lndb/__main__.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/_check_instance_setup.py` & `lndb-0.44.7/lndb/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/_close.py` & `lndb-0.44.7/lndb/_close.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/_delete.py` & `lndb-0.44.7/lndb/_delete.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/_init_instance.py` & `lndb-0.44.7/lndb/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/_load_instance.py` & `lndb-0.44.7/lndb/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/_migrate/alembic.ini` & `lndb-0.44.7/lndb/_migrate/alembic.ini`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/_migrate/core.py` & `lndb-0.44.7/lndb/_migrate/core.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/_migrate/deploy.py` & `lndb-0.44.7/lndb/_migrate/deploy.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/_migrate/env.py` & `lndb-0.44.7/lndb/_migrate/env.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/_migrate/utils.py` & `lndb-0.44.7/lndb/_migrate/utils.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/_register_instance.py` & `lndb-0.44.7/lndb/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/_schema.py` & `lndb-0.44.7/lndb/_schema.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/_set.py` & `lndb-0.44.7/lndb/_set.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/_settings.py` & `lndb-0.44.7/lndb/_settings.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/_setup_user.py` & `lndb-0.44.7/lndb/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/dev/__init__.py` & `lndb-0.44.7/lndb/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/dev/_clone.py` & `lndb-0.44.7/lndb/dev/_clone.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/dev/_db.py` & `lndb-0.44.7/lndb/dev/_db.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/dev/_deprecated.py` & `lndb-0.44.7/lndb/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/dev/_exclusion.py` & `lndb-0.44.7/lndb/dev/_exclusion.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/dev/_settings_instance.py` & `lndb-0.44.7/lndb/dev/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/dev/_settings_load.py` & `lndb-0.44.7/lndb/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/dev/_settings_save.py` & `lndb-0.44.7/lndb/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/dev/_settings_store.py` & `lndb-0.44.7/lndb/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/dev/_settings_user.py` & `lndb-0.44.7/lndb/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/dev/_setup_knowledge.py` & `lndb-0.44.7/lndb/dev/_setup_knowledge.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/dev/_setup_schema.py` & `lndb-0.44.7/lndb/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/dev/_storage.py` & `lndb-0.44.7/lndb/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/dev/upath.py` & `lndb-0.44.7/lndb/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/test/_migrations_e2e.py` & `lndb-0.44.7/lndb/test/_migrations_e2e.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/lndb/test/_migrations_unit.py` & `lndb-0.44.7/lndb/test/_migrations_unit.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/noxfile.py` & `lndb-0.44.7/noxfile.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/pyproject.toml` & `lndb-0.44.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = [{name = "Lamin Labs", email = "laminlabs@gmail.com"}]
 readme = "README.md"
 dynamic = ["version", "description"]
 dependencies = [
     # PINNED internal LAMIN dependency
     # !!! lnhub_rest cannot be pinned in LaminDB !!!
     # !!! LaminDB should not directly depend on lnhub_rest !!!
-    "lnhub_rest==0.9.3",
+    "lnhub_rest==0.9.4",
     # NO other Lamin packages should be pinned or even be a dependency
     "laminci>=0.3.0",  # disentangle over time
     "lnschema_core>=0.28.0",
     "lamin_logger>=0.2.3",
     # External dependencies
     "pytest_alembic==0.9.1",  # let's pin this as we use internals
     "cloudpathlib",  # we can remove this once lnschema-core is released (2023-04-07)
```

### Comparing `lndb-0.44.6/tests/test_bionty.py` & `lndb-0.44.7/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/tests/test_init_instance.py` & `lndb-0.44.7/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.6/PKG-INFO` & `lndb-0.44.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: lndb
-Version: 0.44.6
+Version: 0.44.7
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
-Requires-Dist: lnhub_rest==0.9.3
+Requires-Dist: lnhub_rest==0.9.4
 Requires-Dist: laminci>=0.3.0
 Requires-Dist: lnschema_core>=0.28.0
 Requires-Dist: lamin_logger>=0.2.3
 Requires-Dist: pytest_alembic==0.9.1
 Requires-Dist: cloudpathlib
 Requires-Dist: sqlmodel>=0.0.8
 Requires-Dist: psycopg2-binary
```

