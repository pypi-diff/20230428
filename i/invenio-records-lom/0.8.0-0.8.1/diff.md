# Comparing `tmp/invenio-records-lom-0.8.0.tar.gz` & `tmp/invenio-records-lom-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-records-lom-0.8.0.tar", last modified: Thu Apr 20 11:41:19 2023, max compression
+gzip compressed data, was "invenio-records-lom-0.8.1.tar", last modified: Fri Apr 28 11:55:34 2023, max compression
```

## Comparing `invenio-records-lom-0.8.0.tar` & `invenio-records-lom-0.8.1.tar`

### file list

```diff
@@ -1,161 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.133244 invenio-records-lom-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-20 11:41:19.133244 invenio-records-lom-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.117244 invenio-records-lom-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19741 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/fixtures/demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/jsonschemas/lomrecords/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/jsonschemas/lomrecords/lom-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/oai.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/records/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.113244 invenio-records-lom-0.8.0/invenio_records_lom/records/mappings/os-v2/lomrecords/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/records/mappings/os-v2/lomrecords/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/mappings/os-v2/lomrecords/drafts/draft-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/records/mappings/os-v2/lomrecords/records/
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/mappings/os-v2/lomrecords/records/record-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/relations.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom/resources/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/resources/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15953 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/resources/serializers/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.125244 invenio-records-lom-0.8.0/invenio_records_lom/services/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/services/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/services/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/services/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/services/pids.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.125244 invenio-records-lom-0.8.0/invenio_records_lom/services/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/services/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/services/schemas/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/services/schemas/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/services/schemas/records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/services/services.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/services/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.113244 invenio-records-lom-0.8.0/invenio_records_lom/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.113244 invenio-records-lom-0.8.0/invenio_records_lom/static/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.125244 invenio-records-lom-0.8.0/invenio_records_lom/static/templates/invenio_records_lom/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/static/templates/invenio_records_lom/results.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.113244 invenio-records-lom-0.8.0/invenio_records_lom/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.125244 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/record.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.125244 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/deposit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/export.html
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/files.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.125244 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/macros/files.html
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/macros/tree.html
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/uploads.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.125244 invenio-records-lom-0.8.0/invenio_records_lom/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.113244 invenio-records-lom-0.8.0/invenio_records_lom/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.129244 invenio-records-lom-0.8.0/invenio_records_lom/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.113244 invenio-records-lom-0.8.0/invenio_records_lom/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.129244 invenio-records-lom-0.8.0/invenio_records_lom/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/translations/en/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.129244 invenio-records-lom-0.8.0/invenio_records_lom/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.129244 invenio-records-lom-0.8.0/invenio_records_lom/ui/records/
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/records/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/records/deposits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/records/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/records/records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.129244 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.113244 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.113244 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.113244 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.113244 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.129244 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/
--rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/LOMDepositForm.js
--rw-r--r--   0 runner    (1001) docker     (123)    10784 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/components.js
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/debug.js
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/fields.js
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/serializers.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.129244 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/components.js
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.113244 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/less/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.129244 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/less/invenio_records_lom/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/less/invenio_records_lom/theme.less
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.133244 invenio-records-lom-0.8.0/invenio_records_lom/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    64221 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/utils/OEFOS2012_DE_CTI_20211111_154218_utf8.csv
--rw-r--r--   0 runner    (1001) docker     (123)    64211 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/utils/OEFOS2012_EN_CTI_20211111_154228_utf8.csv
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/utils/learning_resource_types.json
--rw-r--r--   0 runner    (1001) docker     (123)    19681 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/utils/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/invenio_records_lom/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.121244 invenio-records-lom-0.8.0/invenio_records_lom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-20 11:41:19.000000 invenio-records-lom-0.8.0/invenio_records_lom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-04-20 11:41:19.000000 invenio-records-lom-0.8.0/invenio_records_lom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 11:41:19.000000 invenio-records-lom-0.8.0/invenio_records_lom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-20 11:41:19.000000 invenio-records-lom-0.8.0/invenio_records_lom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 11:41:19.000000 invenio-records-lom-0.8.0/invenio_records_lom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-20 11:41:19.000000 invenio-records-lom-0.8.0/invenio_records_lom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 11:41:19.000000 invenio-records-lom-0.8.0/invenio_records_lom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      737 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-04-20 11:41:19.133244 invenio-records-lom-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:41:19.133244 invenio-records-lom-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/tests/test_invenio_records_lom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/tests/test_pids_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/tests/test_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-20 11:41:12.000000 invenio-records-lom-0.8.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.442551 invenio-records-lom-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-28 11:55:34.442551 invenio-records-lom-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.430551 invenio-records-lom-0.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.430551 invenio-records-lom-0.8.1/invenio_records_lom/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19741 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/fixtures/demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom/jsonschemas/lomrecords/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/jsonschemas/lomrecords/lom-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/oai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.426551 invenio-records-lom-0.8.1/invenio_records_lom/records/mappings/os-v2/lomrecords/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom/records/mappings/os-v2/lomrecords/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/mappings/os-v2/lomrecords/drafts/draft-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom/records/mappings/os-v2/lomrecords/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/mappings/os-v2/lomrecords/records/record-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom/resources/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/resources/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15953 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/resources/serializers/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.438551 invenio-records-lom-0.8.1/invenio_records_lom/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/services/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/services/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/services/pids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.438551 invenio-records-lom-0.8.1/invenio_records_lom/services/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/services/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/services/schemas/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/services/schemas/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/services/schemas/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/services/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/services/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.426551 invenio-records-lom-0.8.1/invenio_records_lom/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.426551 invenio-records-lom-0.8.1/invenio_records_lom/static/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.438551 invenio-records-lom-0.8.1/invenio_records_lom/static/templates/invenio_records_lom/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/static/templates/invenio_records_lom/results.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.426551 invenio-records-lom-0.8.1/invenio_records_lom/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.438551 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/not_licensed_text.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/record.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.438551 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/deposit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/export.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/files.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.438551 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/macros/files.html
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/macros/tree.html
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/uploads.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.438551 invenio-records-lom-0.8.1/invenio_records_lom/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.426551 invenio-records-lom-0.8.1/invenio_records_lom/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.438551 invenio-records-lom-0.8.1/invenio_records_lom/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.426551 invenio-records-lom-0.8.1/invenio_records_lom/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.438551 invenio-records-lom-0.8.1/invenio_records_lom/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.438551 invenio-records-lom-0.8.1/invenio_records_lom/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.438551 invenio-records-lom-0.8.1/invenio_records_lom/ui/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/records/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/records/deposits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/records/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/records/records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.442551 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.426551 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.426551 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.426551 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.426551 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.442551 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/LOMDepositForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10784 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/components.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/debug.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/fields.js
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/serializers.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.442551 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/components.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.426551 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.442551 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/less/invenio_records_lom/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/less/invenio_records_lom/theme.less
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.442551 invenio-records-lom-0.8.1/invenio_records_lom/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    64221 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/utils/OEFOS2012_DE_CTI_20211111_154218_utf8.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    64211 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/utils/OEFOS2012_EN_CTI_20211111_154228_utf8.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/utils/learning_resource_types.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19681 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/utils/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-28 11:55:34.000000 invenio-records-lom-0.8.1/invenio_records_lom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-04-28 11:55:34.000000 invenio-records-lom-0.8.1/invenio_records_lom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:55:34.000000 invenio-records-lom-0.8.1/invenio_records_lom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-28 11:55:34.000000 invenio-records-lom-0.8.1/invenio_records_lom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:55:34.000000 invenio-records-lom-0.8.1/invenio_records_lom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-28 11:55:34.000000 invenio-records-lom-0.8.1/invenio_records_lom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-28 11:55:34.000000 invenio-records-lom-0.8.1/invenio_records_lom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      737 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-04-28 11:55:34.446551 invenio-records-lom-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.442551 invenio-records-lom-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/tests/test_invenio_records_lom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/tests/test_pids_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/tests/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/tests/test_utils.py
```

### Comparing `invenio-records-lom-0.8.0/.editorconfig` & `invenio-records-lom-0.8.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/CHANGES.rst` & `invenio-records-lom-0.8.1/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 
     invenio-records-lom is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.8.1 (release 2023-04-28)
+
+- upload: require license permission
+
+
 Version v0.8.0 (release 2023-04-20)
 
 - make compatible with invenio v11
 - support DOI, publishing, deleting
 
 
 Version v0.7.2 (release 2023-03-15)
```

### Comparing `invenio-records-lom-0.8.0/CONTRIBUTING.rst` & `invenio-records-lom-0.8.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/INSTALL.rst` & `invenio-records-lom-0.8.1/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/LICENSE` & `invenio-records-lom-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/MANIFEST.in` & `invenio-records-lom-0.8.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/PKG-INFO` & `invenio-records-lom-0.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-records-lom
-Version: 0.8.0
+Version: 0.8.1
 Summary: "Invenio data model for Learning Object Metadata."
 Home-page: https://github.com/tu-graz-library/invenio-records-lom
 Author: "Graz University of Technology"
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio record LOM learning object metadata
 Platform: any
@@ -59,14 +59,19 @@
 
     invenio-records-lom is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.8.1 (release 2023-04-28)
+
+- upload: require license permission
+
+
 Version v0.8.0 (release 2023-04-20)
 
 - make compatible with invenio v11
 - support DOI, publishing, deleting
 
 
 Version v0.7.2 (release 2023-03-15)
```

### Comparing `invenio-records-lom-0.8.0/README.rst` & `invenio-records-lom-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/babel.ini` & `invenio-records-lom-0.8.1/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/docs/Makefile` & `invenio-records-lom-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/docs/conf.py` & `invenio-records-lom-0.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/docs/index.rst` & `invenio-records-lom-0.8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/docs/make.bat` & `invenio-records-lom-0.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/cli.py` & `invenio-records-lom-0.8.1/invenio_records_lom/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/config.py` & `invenio-records-lom-0.8.1/invenio_records_lom/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/ext.py` & `invenio-records-lom-0.8.1/invenio_records_lom/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/fixtures/demo.py` & `invenio-records-lom-0.8.1/invenio_records_lom/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/jsonschemas/lomrecords/lom-v1.0.0.json` & `invenio-records-lom-0.8.1/invenio_records_lom/jsonschemas/lomrecords/lom-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/oai.py` & `invenio-records-lom-0.8.1/invenio_records_lom/oai.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/records/__init__.py` & `invenio-records-lom-0.8.1/invenio_records_lom/records/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/records/api.py` & `invenio-records-lom-0.8.1/invenio_records_lom/records/api.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/records/mappings/os-v2/lomrecords/drafts/draft-v1.0.0.json` & `invenio-records-lom-0.8.1/invenio_records_lom/records/mappings/os-v2/lomrecords/drafts/draft-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/records/mappings/os-v2/lomrecords/records/record-v1.0.0.json` & `invenio-records-lom-0.8.1/invenio_records_lom/records/mappings/os-v2/lomrecords/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/records/models.py` & `invenio-records-lom-0.8.1/invenio_records_lom/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/__init__.py` & `invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/context.py` & `invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/context.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/providers.py` & `invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/providers.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/relations.py` & `invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/relations.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/resolver.py` & `invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/resolver.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/records/systemfields/results.py` & `invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/results.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/resources/__init__.py` & `invenio-records-lom-0.8.1/invenio_records_lom/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/resources/config.py` & `invenio-records-lom-0.8.1/invenio_records_lom/resources/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/resources/resources.py` & `invenio-records-lom-0.8.1/invenio_records_lom/resources/resources.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/resources/serializers/__init__.py` & `invenio-records-lom-0.8.1/invenio_records_lom/resources/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/resources/serializers/schemas.py` & `invenio-records-lom-0.8.1/invenio_records_lom/resources/serializers/schemas.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/services/__init__.py` & `invenio-records-lom-0.8.1/invenio_records_lom/services/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/services/components.py` & `invenio-records-lom-0.8.1/invenio_records_lom/services/components.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/services/config.py` & `invenio-records-lom-0.8.1/invenio_records_lom/services/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/services/permissions.py` & `invenio-records-lom-0.8.1/invenio_records_lom/services/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/services/pids.py` & `invenio-records-lom-0.8.1/invenio_records_lom/services/pids.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/services/schemas/fields.py` & `invenio-records-lom-0.8.1/invenio_records_lom/services/schemas/fields.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/services/schemas/metadata.py` & `invenio-records-lom-0.8.1/invenio_records_lom/services/schemas/metadata.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/services/schemas/records.py` & `invenio-records-lom-0.8.1/invenio_records_lom/services/schemas/records.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/services/services.py` & `invenio-records-lom-0.8.1/invenio_records_lom/services/services.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/services/tasks.py` & `invenio-records-lom-0.8.1/invenio_records_lom/services/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/static/templates/invenio_records_lom/results.html` & `invenio-records-lom-0.8.1/invenio_records_lom/static/templates/invenio_records_lom/results.html`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/record.html` & `invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/record.html`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/deposit.html` & `invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/deposit.html`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/export.html` & `invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/export.html`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/files.html` & `invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/files.html`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/macros/files.html` & `invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/macros/files.html`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/records/macros/tree.html` & `invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/macros/tree.html`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/search.html` & `invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/search.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,7 +15,8 @@
 {%- endblock %}
 
 {%- block page_body %}
 
 <div id="invenio-search-lom-config" data-invenio-search-config='{{ search_app_lom_config() | tojson }}'></div>
 
 {%- endblock page_body %}
+
```

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/templates/invenio_records_lom/uploads.html` & `invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/uploads.html`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/translations/de/LC_MESSAGES/messages.po` & `invenio-records-lom-0.8.1/invenio_records_lom/translations/en/LC_MESSAGES/messages.po`

 * *Files 16% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio_records_lom 0.1.0\n"
 "Report-Msgid-Bugs-To: info@tugraz.at\n"
 "POT-Creation-Date: 2022-03-25 13:22+0100\n"
 "PO-Revision-Date: 2022-03-25 13:31+0100\n"
 "Last-Translator:  <christoph.ladurner@tugraz.at>\n"
-"Language-Team: Deutsch\n"
+"Language-Team: English\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.9.1\n"
-"Language: de_AT\n"
+"Language: en_US\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_records_lom/config.py:27
 msgid "JSON"
 msgstr "JSON"
 
 #: invenio_records_lom/config.py:53 invenio_records_lom/config.py:60
@@ -38,58 +38,58 @@
 
 #: invenio_records_lom/services/schemas/records.py:23
 msgid "Persistent identifier scheme unknown to LOM."
 msgstr "Persistent identifier scheme unknown to LOM."
 
 #: invenio_records_lom/templates/invenio_records_lom/record.html:56
 msgid "General Informations"
-msgstr "Allgemeine Informationen"
+msgstr "General Informations"
 
 #: invenio_records_lom/templates/invenio_records_lom/record.html:65
 msgid "Educational Informations"
-msgstr "Lernziele"
+msgstr "Educational Informations"
 
 #: invenio_records_lom/templates/invenio_records_lom/record.html:96
 msgid "Original Content"
-msgstr "Quelle"
+msgstr "Original Content"
 
 #: invenio_records_lom/templates/invenio_records_lom/record.html:106
 msgid "Export"
 msgstr "Export"
 
 #: invenio_records_lom/templates/invenio_records_lom/records/export.html:26
 msgid "Back to details"
-msgstr "Zurück zu den Details"
+msgstr "Back to details"
 
 #: invenio_records_lom/templates/invenio_records_lom/records/files.html:35
 #: invenio_records_lom/templates/invenio_records_lom/records/macros/files.html:108
 msgid "Files"
-msgstr "Dateien"
+msgstr "Files"
 
 #: invenio_records_lom/templates/invenio_records_lom/records/files.html:43
 #: invenio_records_lom/templates/invenio_records_lom/records/macros/files.html:118
 msgid "Reason"
 msgstr "Reason"
 
 #: invenio_records_lom/templates/invenio_records_lom/records/macros/files.html:57
 msgid "Name"
 msgstr "Name"
 
 #: invenio_records_lom/templates/invenio_records_lom/records/macros/files.html:58
 msgid "Size"
-msgstr "Größe"
+msgstr "Size"
 
 #: invenio_records_lom/templates/invenio_records_lom/records/macros/files.html:78
 msgid ""
 "This is the file fingerprint (checksum), which can be used to verify the "
 "file integrity."
 msgstr ""
-"Das ist die Prüfsumme der Datei, die dafür verwendet werden kann "
-"die Dateiintegrität zu prüfen."
+"This is the file fingerprint (checksum), which can be used to verify the "
+"file integrity."
 
 #: invenio_records_lom/templates/invenio_records_lom/records/macros/files.html:88
 msgid "Preview"
-msgstr "Vorschau"
+msgstr "Preview"
 
 #: invenio_records_lom/templates/invenio_records_lom/records/macros/files.html:93
 msgid "Download"
 msgstr "Download"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/ui/__init__.py` & `invenio-records-lom-0.8.1/invenio_records_lom/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/ui/records/__init__.py` & `invenio-records-lom-0.8.1/invenio_records_lom/ui/records/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/ui/records/decorators.py` & `invenio-records-lom-0.8.1/invenio_records_lom/ui/records/decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,28 @@
 from flask import g, request
 from invenio_records_resources.services.errors import PermissionDeniedError
 from sqlalchemy.orm.exc import NoResultFound
 
 from ...proxies import current_records_lom
 
 
+# TODO: this implementation is a quick hack. it is a workflow of the tu graz and
+# should be implemented within the invenio-workflows-tugraz package
+def license_required(func: callable):
+    """Check if the logged in user has the permission to create oer's."""
+
+    @wraps(func)
+    def decoed(**kwargs):
+        # TODO: for now default false. implement proper check
+        kwargs["is_licensed"] = False
+        return func(**kwargs)
+
+    return decoed
+
+
 def pass_record_latest(func: callable):
     """Retrieve latest version of `record` from db and pass that into decorated function."""
 
     @wraps(func)
     def decoed(**kwargs):
         service = current_records_lom.records_service
         record_latest = service.read_latest(
```

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/ui/records/deposits.py` & `invenio-records-lom-0.8.1/invenio_records_lom/ui/records/deposits.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from invenio_i18n.ext import current_i18n
 from invenio_records_resources.services.files.results import FileList
 from invenio_records_resources.services.records.results import RecordItem
 from invenio_users_resources.proxies import current_user_resources
 
 from ...proxies import current_records_lom
 from ...utils import LOMMetadata, get_oefosdict
-from .decorators import pass_draft, pass_draft_files
+from .decorators import license_required, pass_draft, pass_draft_files
 
 
 def get_deposit_template_context(**extra_form_config_kwargs) -> dict:
     """Get context for deposit-template from db, current_app.config."""
     app_config = current_app.config
     locale = str(current_i18n.locale)
     locale = locale if locale in ["de", "en"] else "en"
@@ -132,20 +132,27 @@
         permissions=draft.has_permissions_to(["new_version", "delete_draft"]),
         record=record,
         searchbar_config=template_context["searchbar_config"],
     )
 
 
 @login_required
-def uploads():
+@license_required
+def uploads(is_licensed: bool = False):
     """Show overview of lom-records uploaded by user, upload further records."""
     avatar_url = current_user_resources.users_service.links_item_tpl.expand(
         g.identity, current_user
     )["avatar"]
+
+    if is_licensed:
+        template = "invenio_records_lom/uploads.html"
+    else:
+        template = "invenio_records_lom/not_licensed_text.html"
+
     return render_template(
-        "invenio_records_lom/uploads.html",
+        template,
         # TODO: newer versions of the original template now also take `searchbar_config` here
         # see `invenio_app_rdm/users_ui/views/dashboard.py:uploads`
         # also see `invenio_app_rdm/users_ui/templates/uploads.html`
         # searchbar_config={"searchUrl": ...},
         user_avatar=avatar_url,
     )
```

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/ui/records/errors.py` & `invenio-records-lom-0.8.1/invenio_records_lom/ui/records/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/ui/records/records.py` & `invenio-records-lom-0.8.1/invenio_records_lom/ui/records/records.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/LOMDepositForm.js` & `invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/LOMDepositForm.js`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/components.js` & `invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/components.js`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/debug.js` & `invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/debug.js`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/fields.js` & `invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/fields.js`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/index.js` & `invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/index.js`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/serializers.js` & `invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/serializers.js`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/components.js` & `invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/components.js`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/index.js` & `invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/index.js`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/config.py` & `invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/views.py` & `invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/views.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/ui/theme/webpack.py` & `invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/utils/OEFOS2012_DE_CTI_20211111_154218_utf8.csv` & `invenio-records-lom-0.8.1/invenio_records_lom/utils/OEFOS2012_DE_CTI_20211111_154218_utf8.csv`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/utils/OEFOS2012_EN_CTI_20211111_154228_utf8.csv` & `invenio-records-lom-0.8.1/invenio_records_lom/utils/OEFOS2012_EN_CTI_20211111_154228_utf8.csv`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/utils/__init__.py` & `invenio-records-lom-0.8.1/invenio_records_lom/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/utils/learning_resource_types.json` & `invenio-records-lom-0.8.1/invenio_records_lom/utils/learning_resource_types.json`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/utils/util.py` & `invenio-records-lom-0.8.1/invenio_records_lom/utils/util.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom/views.py` & `invenio-records-lom-0.8.1/invenio_records_lom/views.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom.egg-info/PKG-INFO` & `invenio-records-lom-0.8.1/invenio_records_lom.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-records-lom
-Version: 0.8.0
+Version: 0.8.1
 Summary: "Invenio data model for Learning Object Metadata."
 Home-page: https://github.com/tu-graz-library/invenio-records-lom
 Author: "Graz University of Technology"
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio record LOM learning object metadata
 Platform: any
@@ -59,14 +59,19 @@
 
     invenio-records-lom is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.8.1 (release 2023-04-28)
+
+- upload: require license permission
+
+
 Version v0.8.0 (release 2023-04-20)
 
 - make compatible with invenio v11
 - support DOI, publishing, deleting
 
 
 Version v0.7.2 (release 2023-03-15)
```

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom.egg-info/SOURCES.txt` & `invenio-records-lom-0.8.1/invenio_records_lom.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 invenio_records_lom/services/tasks.py
 invenio_records_lom/services/schemas/__init__.py
 invenio_records_lom/services/schemas/fields.py
 invenio_records_lom/services/schemas/metadata.py
 invenio_records_lom/services/schemas/records.py
 invenio_records_lom/static/templates/invenio_records_lom/results.html
 invenio_records_lom/templates/invenio_records_lom/base.html
+invenio_records_lom/templates/invenio_records_lom/not_licensed_text.html
 invenio_records_lom/templates/invenio_records_lom/record.html
 invenio_records_lom/templates/invenio_records_lom/search.html
 invenio_records_lom/templates/invenio_records_lom/uploads.html
 invenio_records_lom/templates/invenio_records_lom/records/deposit.html
 invenio_records_lom/templates/invenio_records_lom/records/export.html
 invenio_records_lom/templates/invenio_records_lom/records/files.html
 invenio_records_lom/templates/invenio_records_lom/records/macros/files.html
```

### Comparing `invenio-records-lom-0.8.0/invenio_records_lom.egg-info/entry_points.txt` & `invenio-records-lom-0.8.1/invenio_records_lom.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/run-tests.sh` & `invenio-records-lom-0.8.1/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/setup.cfg` & `invenio-records-lom-0.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/tests/conftest.py` & `invenio-records-lom-0.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/tests/test_cli.py` & `invenio-records-lom-0.8.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/tests/test_invenio_records_lom.py` & `invenio-records-lom-0.8.1/tests/test_invenio_records_lom.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/tests/test_pids_service.py` & `invenio-records-lom-0.8.1/tests/test_pids_service.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/tests/test_service.py` & `invenio-records-lom-0.8.1/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.0/tests/test_utils.py` & `invenio-records-lom-0.8.1/tests/test_utils.py`

 * *Files identical despite different names*

