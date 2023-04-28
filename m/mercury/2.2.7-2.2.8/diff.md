# Comparing `tmp/mercury-2.2.7.tar.gz` & `tmp/mercury-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-2.2.7.tar", last modified: Tue Apr 25 12:23:23 2023, max compression
+gzip compressed data, was "mercury-2.2.8.tar", last modified: Thu Apr 27 15:44:08 2023, max compression
```

## Comparing `mercury-2.2.7.tar` & `mercury-2.2.8.tar`

### file list

```diff
@@ -1,211 +1,211 @@
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.301584 mercury-2.2.7/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      149 2022-04-19 12:37:24.000000 mercury-2.2.7/MANIFEST.in
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5674 2023-04-25 12:23:23.301584 mercury-2.2.7/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4214 2023-02-15 10:26:45.000000 mercury-2.2.7/README.md
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.269583 mercury-2.2.7/mercury/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       54 2023-04-25 12:22:00.000000 mercury-2.2.7/mercury/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.269583 mercury-2.2.7/mercury/apps/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.7/mercury/apps/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.273583 mercury-2.2.7/mercury/apps/accounts/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.2.7/mercury/apps/accounts/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      459 2023-03-17 11:37:23.000000 mercury-2.2.7/mercury/apps/accounts/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2023-03-01 11:11:00.000000 mercury-2.2.7/mercury/apps/accounts/apps.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      801 2023-03-01 11:11:00.000000 mercury-2.2.7/mercury/apps/accounts/fields.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.273583 mercury-2.2.7/mercury/apps/accounts/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9132 2023-03-29 09:06:05.000000 mercury-2.2.7/mercury/apps/accounts/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.2.7/mercury/apps/accounts/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4715 2023-03-28 08:49:03.000000 mercury-2.2.7/mercury/apps/accounts/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2086 2023-04-06 13:33:42.000000 mercury-2.2.7/mercury/apps/accounts/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2937 2023-03-27 12:26:01.000000 mercury-2.2.7/mercury/apps/accounts/tasks.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.273583 mercury-2.2.7/mercury/apps/accounts/tests/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-16 13:27:44.000000 mercury-2.2.7/mercury/apps/accounts/tests/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7289 2023-03-29 09:06:05.000000 mercury-2.2.7/mercury/apps/accounts/tests/test_accounts.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5543 2023-03-31 10:36:11.000000 mercury-2.2.7/mercury/apps/accounts/tests/test_invitations.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6078 2023-04-06 13:49:54.000000 mercury-2.2.7/mercury/apps/accounts/tests/test_secrets.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11402 2023-03-31 10:52:58.000000 mercury-2.2.7/mercury/apps/accounts/tests/test_sites.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3426 2023-03-29 09:06:05.000000 mercury-2.2.7/mercury/apps/accounts/tests/test_subscription.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2650 2023-03-24 11:47:32.000000 mercury-2.2.7/mercury/apps/accounts/urls.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.273583 mercury-2.2.7/mercury/apps/accounts/views/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-17 08:20:29.000000 mercury-2.2.7/mercury/apps/accounts/views/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2006 2023-03-27 08:34:35.000000 mercury-2.2.7/mercury/apps/accounts/views/accounts.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4308 2023-03-31 10:36:11.000000 mercury-2.2.7/mercury/apps/accounts/views/invitations.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      789 2023-03-24 08:45:58.000000 mercury-2.2.7/mercury/apps/accounts/views/permissions.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2922 2023-04-06 14:49:43.000000 mercury-2.2.7/mercury/apps/accounts/views/secrets.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6372 2023-03-31 10:52:58.000000 mercury-2.2.7/mercury/apps/accounts/views/sites.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4152 2023-03-29 09:06:05.000000 mercury-2.2.7/mercury/apps/accounts/views/subscription.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      436 2023-03-24 08:45:58.000000 mercury-2.2.7/mercury/apps/accounts/views/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.273583 mercury-2.2.7/mercury/apps/nb/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.7/mercury/apps/nb/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5845 2023-04-06 13:49:54.000000 mercury-2.2.7/mercury/apps/nb/exporter.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4086 2023-04-06 13:49:54.000000 mercury-2.2.7/mercury/apps/nb/nbrun.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.273583 mercury-2.2.7/mercury/apps/nb/tests/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-04-05 08:19:32.000000 mercury-2.2.7/mercury/apps/nb/tests/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      854 2023-04-06 13:49:54.000000 mercury-2.2.7/mercury/apps/nb/tests/test_nbrun.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1265 2023-03-17 12:41:34.000000 mercury-2.2.7/mercury/apps/nb/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      403 2023-02-13 14:05:12.000000 mercury-2.2.7/mercury/apps/nb/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.277583 mercury-2.2.7/mercury/apps/nbworker/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.7/mercury/apps/nbworker/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1881 2023-04-21 07:50:26.000000 mercury-2.2.7/mercury/apps/nbworker/__main__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    17411 2023-04-12 08:48:16.000000 mercury-2.2.7/mercury/apps/nbworker/nb.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7485 2023-04-06 14:49:56.000000 mercury-2.2.7/mercury/apps/nbworker/rest.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4864 2023-03-17 08:55:41.000000 mercury-2.2.7/mercury/apps/nbworker/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      701 2023-03-14 07:49:44.000000 mercury-2.2.7/mercury/apps/nbworker/utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2927 2023-04-20 13:08:01.000000 mercury-2.2.7/mercury/apps/nbworker/ws.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.277583 mercury-2.2.7/mercury/apps/notebooks/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.7/mercury/apps/notebooks/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      277 2022-03-09 11:04:20.000000 mercury-2.2.7/mercury/apps/notebooks/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      155 2022-03-09 11:04:20.000000 mercury-2.2.7/mercury/apps/notebooks/apps.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.281583 mercury-2.2.7/mercury/apps/notebooks/management/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.7/mercury/apps/notebooks/management/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.281583 mercury-2.2.7/mercury/apps/notebooks/management/commands/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.7/mercury/apps/notebooks/management/commands/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1279 2022-03-09 11:06:47.000000 mercury-2.2.7/mercury/apps/notebooks/management/commands/add.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      864 2022-03-09 11:06:47.000000 mercury-2.2.7/mercury/apps/notebooks/management/commands/delete.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      545 2022-03-09 11:06:47.000000 mercury-2.2.7/mercury/apps/notebooks/management/commands/list.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3702 2023-02-13 14:05:12.000000 mercury-2.2.7/mercury/apps/notebooks/management/commands/watch.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.281583 mercury-2.2.7/mercury/apps/notebooks/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2300 2023-03-29 09:06:05.000000 mercury-2.2.7/mercury/apps/notebooks/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.7/mercury/apps/notebooks/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1067 2023-03-27 08:29:11.000000 mercury-2.2.7/mercury/apps/notebooks/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      617 2023-03-17 11:38:01.000000 mercury-2.2.7/mercury/apps/notebooks/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4093 2022-05-18 10:19:32.000000 mercury-2.2.7/mercury/apps/notebooks/slides_themes.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11689 2023-04-03 14:44:43.000000 mercury-2.2.7/mercury/apps/notebooks/tasks.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-03-01 11:11:00.000000 mercury-2.2.7/mercury/apps/notebooks/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      567 2023-03-17 12:41:34.000000 mercury-2.2.7/mercury/apps/notebooks/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3755 2023-03-17 08:55:41.000000 mercury-2.2.7/mercury/apps/notebooks/views.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.281583 mercury-2.2.7/mercury/apps/storage/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.7/mercury/apps/storage/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-02-13 14:05:12.000000 mercury-2.2.7/mercury/apps/storage/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-02-13 14:05:12.000000 mercury-2.2.7/mercury/apps/storage/apps.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.281583 mercury-2.2.7/mercury/apps/storage/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2949 2023-03-29 09:06:05.000000 mercury-2.2.7/mercury/apps/storage/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1404 2023-03-31 09:54:03.000000 mercury-2.2.7/mercury/apps/storage/migrations/0002_useruploadedfile.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.7/mercury/apps/storage/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1787 2023-03-29 09:06:05.000000 mercury-2.2.7/mercury/apps/storage/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3540 2023-03-31 09:54:03.000000 mercury-2.2.7/mercury/apps/storage/s3utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      469 2023-03-31 14:19:15.000000 mercury-2.2.7/mercury/apps/storage/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11397 2023-03-31 09:54:03.000000 mercury-2.2.7/mercury/apps/storage/storage.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3158 2023-03-17 08:55:41.000000 mercury-2.2.7/mercury/apps/storage/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2132 2023-03-29 09:56:45.000000 mercury-2.2.7/mercury/apps/storage/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      445 2023-03-31 09:54:03.000000 mercury-2.2.7/mercury/apps/storage/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.285583 mercury-2.2.7/mercury/apps/storage/views/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-31 12:45:08.000000 mercury-2.2.7/mercury/apps/storage/views/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6182 2023-03-31 11:42:07.000000 mercury-2.2.7/mercury/apps/storage/views/dashboardfiles.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4935 2023-03-31 11:42:07.000000 mercury-2.2.7/mercury/apps/storage/views/notebookfiles.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3737 2023-03-31 11:42:07.000000 mercury-2.2.7/mercury/apps/storage/views/workerfiles.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.285583 mercury-2.2.7/mercury/apps/tasks/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.7/mercury/apps/tasks/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      287 2022-03-09 11:04:20.000000 mercury-2.2.7/mercury/apps/tasks/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2022-03-09 11:04:20.000000 mercury-2.2.7/mercury/apps/tasks/apps.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      412 2022-03-09 11:06:47.000000 mercury-2.2.7/mercury/apps/tasks/clean_service.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3840 2023-04-03 14:18:32.000000 mercury-2.2.7/mercury/apps/tasks/export_pdf.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3805 2023-04-06 13:49:54.000000 mercury-2.2.7/mercury/apps/tasks/export_png.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.285583 mercury-2.2.7/mercury/apps/tasks/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1328 2023-03-29 09:06:05.000000 mercury-2.2.7/mercury/apps/tasks/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.7/mercury/apps/tasks/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      762 2022-05-18 10:19:32.000000 mercury-2.2.7/mercury/apps/tasks/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3659 2023-02-13 14:05:12.000000 mercury-2.2.7/mercury/apps/tasks/notify.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      433 2022-03-09 11:06:47.000000 mercury-2.2.7/mercury/apps/tasks/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    15223 2023-02-23 14:52:12.000000 mercury-2.2.7/mercury/apps/tasks/tasks.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1314 2023-02-13 14:05:12.000000 mercury-2.2.7/mercury/apps/tasks/tasks_export.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      571 2023-03-14 07:49:44.000000 mercury-2.2.7/mercury/apps/tasks/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1401 2023-03-17 12:41:34.000000 mercury-2.2.7/mercury/apps/tasks/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8619 2023-03-17 08:55:41.000000 mercury-2.2.7/mercury/apps/tasks/views.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.289584 mercury-2.2.7/mercury/apps/workers/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.2.7/mercury/apps/workers/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-03-14 07:49:44.000000 mercury-2.2.7/mercury/apps/workers/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-03-14 07:49:44.000000 mercury-2.2.7/mercury/apps/workers/apps.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.289584 mercury-2.2.7/mercury/apps/workers/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1286 2023-03-29 09:06:05.000000 mercury-2.2.7/mercury/apps/workers/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.2.7/mercury/apps/workers/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      798 2023-03-29 09:06:05.000000 mercury-2.2.7/mercury/apps/workers/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      296 2023-03-14 07:49:44.000000 mercury-2.2.7/mercury/apps/workers/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       60 2023-03-14 07:49:44.000000 mercury-2.2.7/mercury/apps/workers/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1053 2023-03-17 12:41:34.000000 mercury-2.2.7/mercury/apps/workers/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3881 2023-03-31 09:54:03.000000 mercury-2.2.7/mercury/apps/workers/views.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.289584 mercury-2.2.7/mercury/apps/ws/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.7/mercury/apps/ws/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      141 2023-02-13 14:05:12.000000 mercury-2.2.7/mercury/apps/ws/apps.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6162 2023-04-20 13:43:38.000000 mercury-2.2.7/mercury/apps/ws/client.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      947 2023-03-14 07:49:44.000000 mercury-2.2.7/mercury/apps/ws/middleware.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.289584 mercury-2.2.7/mercury/apps/ws/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.7/mercury/apps/ws/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      386 2023-02-28 13:59:46.000000 mercury-2.2.7/mercury/apps/ws/routing.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2495 2023-04-06 13:49:54.000000 mercury-2.2.7/mercury/apps/ws/tasks.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      137 2023-03-01 11:07:38.000000 mercury-2.2.7/mercury/apps/ws/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5106 2023-04-06 13:49:54.000000 mercury-2.2.7/mercury/apps/ws/utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1754 2023-03-14 07:49:44.000000 mercury-2.2.7/mercury/apps/ws/worker.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7191 2023-03-31 14:11:10.000000 mercury-2.2.7/mercury/demo.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.289584 mercury-2.2.7/mercury/frontend-dist/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1158 2023-04-25 12:23:22.000000 mercury-2.2.7/mercury/frontend-dist/asset-manifest.json
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    15406 2023-04-25 12:23:06.000000 mercury-2.2.7/mercury/frontend-dist/favicon-old.ico
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    15086 2023-04-25 12:23:06.000000 mercury-2.2.7/mercury/frontend-dist/favicon.ico
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3086 2023-04-25 12:23:22.000000 mercury-2.2.7/mercury/frontend-dist/index.html
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    17406 2023-04-25 12:23:06.000000 mercury-2.2.7/mercury/frontend-dist/jupyter-additional.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4539 2023-04-25 12:23:06.000000 mercury-2.2.7/mercury/frontend-dist/jupyter-syntax.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   580386 2023-04-25 12:23:06.000000 mercury-2.2.7/mercury/frontend-dist/jupyter-theme-light.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      324 2023-04-25 12:23:06.000000 mercury-2.2.7/mercury/frontend-dist/manifest.json
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6237 2023-04-25 12:23:06.000000 mercury-2.2.7/mercury/frontend-dist/mercury_black_logo.svg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6997 2023-04-25 12:23:06.000000 mercury-2.2.7/mercury/frontend-dist/mercury_logo.svg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       67 2023-04-25 12:23:06.000000 mercury-2.2.7/mercury/frontend-dist/robots.txt
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.269583 mercury-2.2.7/mercury/frontend-dist/static/
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.293583 mercury-2.2.7/mercury/frontend-dist/static/css/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   229115 2023-04-25 12:23:22.000000 mercury-2.2.7/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   612316 2023-04-25 12:23:22.000000 mercury-2.2.7/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2831 2023-04-25 12:23:22.000000 mercury-2.2.7/mercury/frontend-dist/static/css/main.26f96620.chunk.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5260 2023-04-25 12:23:22.000000 mercury-2.2.7/mercury/frontend-dist/static/css/main.26f96620.chunk.css.map
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.297583 mercury-2.2.7/mercury/frontend-dist/static/js/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)  1311795 2023-04-25 12:23:22.000000 mercury-2.2.7/mercury/frontend-dist/static/js/2.6305b467.chunk.js
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3383 2023-04-25 12:23:22.000000 mercury-2.2.7/mercury/frontend-dist/static/js/2.6305b467.chunk.js.LICENSE.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)  4973509 2023-04-25 12:23:22.000000 mercury-2.2.7/mercury/frontend-dist/static/js/2.6305b467.chunk.js.map
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    84339 2023-04-25 12:23:22.000000 mercury-2.2.7/mercury/frontend-dist/static/js/main.68931b96.chunk.js
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   260680 2023-04-25 12:23:22.000000 mercury-2.2.7/mercury/frontend-dist/static/js/main.68931b96.chunk.js.map
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1557 2023-04-25 12:23:22.000000 mercury-2.2.7/mercury/frontend-dist/static/js/runtime-main.248907bc.js
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8276 2023-04-25 12:23:22.000000 mercury-2.2.7/mercury/frontend-dist/static/js/runtime-main.248907bc.js.map
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.297583 mercury-2.2.7/mercury/frontend-dist/static/media/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   165548 2023-04-25 12:23:22.000000 mercury-2.2.7/mercury/frontend-dist/static/media/fontawesome-webfont.1e59d233.ttf
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    77160 2023-04-25 12:23:22.000000 mercury-2.2.7/mercury/frontend-dist/static/media/fontawesome-webfont.20fd1704.woff2
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   165742 2023-04-25 12:23:22.000000 mercury-2.2.7/mercury/frontend-dist/static/media/fontawesome-webfont.8b43027f.eot
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   444379 2023-04-25 12:23:22.000000 mercury-2.2.7/mercury/frontend-dist/static/media/fontawesome-webfont.c1e38fd9.svg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    98024 2023-04-25 12:23:22.000000 mercury-2.2.7/mercury/frontend-dist/static/media/fontawesome-webfont.f691f37e.woff
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      684 2022-03-09 11:04:20.000000 mercury-2.2.7/mercury/manage.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8376 2023-04-07 10:38:38.000000 mercury-2.2.7/mercury/mercury.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      543 2023-03-30 08:36:26.000000 mercury-2.2.7/mercury/requirements.txt
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.301584 mercury-2.2.7/mercury/server/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       68 2022-03-09 11:04:20.000000 mercury-2.2.7/mercury/server/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      837 2023-03-14 07:49:44.000000 mercury-2.2.7/mercury/server/asgi.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2771 2023-03-24 08:43:00.000000 mercury-2.2.7/mercury/server/celery.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9844 2023-04-05 13:16:51.000000 mercury-2.2.7/mercury/server/settings.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1572 2023-03-14 07:49:44.000000 mercury-2.2.7/mercury/server/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1645 2023-03-01 12:07:40.000000 mercury-2.2.7/mercury/server/views.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      405 2022-05-18 11:03:41.000000 mercury-2.2.7/mercury/server/wsgi.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.301584 mercury-2.2.7/mercury/widgets/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.7/mercury/widgets/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2029 2023-03-17 11:39:55.000000 mercury-2.2.7/mercury/widgets/app.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2294 2023-04-07 10:30:37.000000 mercury-2.2.7/mercury/widgets/button.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      826 2023-04-07 10:43:02.000000 mercury-2.2.7/mercury/widgets/chat.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2127 2023-04-07 10:30:37.000000 mercury-2.2.7/mercury/widgets/checkbox.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      408 2023-04-07 10:32:14.000000 mercury-2.2.7/mercury/widgets/confetti.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3393 2023-04-07 10:30:37.000000 mercury-2.2.7/mercury/widgets/file.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4828 2023-02-21 07:28:26.000000 mercury-2.2.7/mercury/widgets/json.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6894 2023-04-07 10:30:37.000000 mercury-2.2.7/mercury/widgets/manager.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      104 2023-02-21 07:28:26.000000 mercury-2.2.7/mercury/widgets/md.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2690 2023-04-07 10:30:37.000000 mercury-2.2.7/mercury/widgets/multiselect.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1219 2023-02-21 07:48:36.000000 mercury-2.2.7/mercury/widgets/note.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3016 2023-04-07 10:30:37.000000 mercury-2.2.7/mercury/widgets/numeric.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1255 2023-02-21 07:48:36.000000 mercury-2.2.7/mercury/widgets/outputdir.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3025 2023-04-07 10:30:37.000000 mercury-2.2.7/mercury/widgets/range.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2403 2023-04-07 10:30:37.000000 mercury-2.2.7/mercury/widgets/select.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2949 2023-04-07 10:30:37.000000 mercury-2.2.7/mercury/widgets/slider.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      222 2023-02-21 07:28:26.000000 mercury-2.2.7/mercury/widgets/stop.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2039 2023-04-07 10:30:37.000000 mercury-2.2.7/mercury/widgets/text.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-25 12:23:23.269583 mercury-2.2.7/mercury.egg-info/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5674 2023-04-25 12:23:23.000000 mercury-2.2.7/mercury.egg-info/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6285 2023-04-25 12:23:23.000000 mercury-2.2.7/mercury.egg-info/SOURCES.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-04-25 12:23:23.000000 mercury-2.2.7/mercury.egg-info/dependency_links.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       50 2023-04-25 12:23:23.000000 mercury-2.2.7/mercury.egg-info/entry_points.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      491 2023-04-25 12:23:23.000000 mercury-2.2.7/mercury.egg-info/requires.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        8 2023-04-25 12:23:23.000000 mercury-2.2.7/mercury.egg-info/top_level.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      106 2022-03-09 11:04:20.000000 mercury-2.2.7/pyproject.toml
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2023-04-25 12:23:23.301584 mercury-2.2.7/setup.cfg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1163 2023-04-25 12:22:08.000000 mercury-2.2.7/setup.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.683245 mercury-2.2.8/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      149 2022-04-19 12:37:24.000000 mercury-2.2.8/MANIFEST.in
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5674 2023-04-27 15:44:08.683245 mercury-2.2.8/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4214 2023-02-15 10:26:45.000000 mercury-2.2.8/README.md
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.671245 mercury-2.2.8/mercury/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       54 2023-04-27 15:43:19.000000 mercury-2.2.8/mercury/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.671245 mercury-2.2.8/mercury/apps/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.8/mercury/apps/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.671245 mercury-2.2.8/mercury/apps/accounts/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.2.8/mercury/apps/accounts/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      459 2023-03-17 11:37:23.000000 mercury-2.2.8/mercury/apps/accounts/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2023-03-01 11:11:00.000000 mercury-2.2.8/mercury/apps/accounts/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      801 2023-03-01 11:11:00.000000 mercury-2.2.8/mercury/apps/accounts/fields.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.671245 mercury-2.2.8/mercury/apps/accounts/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9132 2023-03-29 09:06:05.000000 mercury-2.2.8/mercury/apps/accounts/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.2.8/mercury/apps/accounts/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4715 2023-03-28 08:49:03.000000 mercury-2.2.8/mercury/apps/accounts/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2086 2023-04-06 13:33:42.000000 mercury-2.2.8/mercury/apps/accounts/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2937 2023-03-27 12:26:01.000000 mercury-2.2.8/mercury/apps/accounts/tasks.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.671245 mercury-2.2.8/mercury/apps/accounts/tests/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-16 13:27:44.000000 mercury-2.2.8/mercury/apps/accounts/tests/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7289 2023-03-29 09:06:05.000000 mercury-2.2.8/mercury/apps/accounts/tests/test_accounts.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5543 2023-03-31 10:36:11.000000 mercury-2.2.8/mercury/apps/accounts/tests/test_invitations.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6078 2023-04-06 13:49:54.000000 mercury-2.2.8/mercury/apps/accounts/tests/test_secrets.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11402 2023-03-31 10:52:58.000000 mercury-2.2.8/mercury/apps/accounts/tests/test_sites.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3426 2023-03-29 09:06:05.000000 mercury-2.2.8/mercury/apps/accounts/tests/test_subscription.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2645 2023-04-25 12:36:08.000000 mercury-2.2.8/mercury/apps/accounts/urls.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.671245 mercury-2.2.8/mercury/apps/accounts/views/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-17 08:20:29.000000 mercury-2.2.8/mercury/apps/accounts/views/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2006 2023-03-27 08:34:35.000000 mercury-2.2.8/mercury/apps/accounts/views/accounts.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4308 2023-03-31 10:36:11.000000 mercury-2.2.8/mercury/apps/accounts/views/invitations.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      789 2023-03-24 08:45:58.000000 mercury-2.2.8/mercury/apps/accounts/views/permissions.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2922 2023-04-06 14:49:43.000000 mercury-2.2.8/mercury/apps/accounts/views/secrets.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6576 2023-04-27 14:55:46.000000 mercury-2.2.8/mercury/apps/accounts/views/sites.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4152 2023-03-29 09:06:05.000000 mercury-2.2.8/mercury/apps/accounts/views/subscription.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      436 2023-03-24 08:45:58.000000 mercury-2.2.8/mercury/apps/accounts/views/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.671245 mercury-2.2.8/mercury/apps/nb/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.8/mercury/apps/nb/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5845 2023-04-06 13:49:54.000000 mercury-2.2.8/mercury/apps/nb/exporter.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4086 2023-04-06 13:49:54.000000 mercury-2.2.8/mercury/apps/nb/nbrun.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.671245 mercury-2.2.8/mercury/apps/nb/tests/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-04-05 08:19:32.000000 mercury-2.2.8/mercury/apps/nb/tests/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      854 2023-04-06 13:49:54.000000 mercury-2.2.8/mercury/apps/nb/tests/test_nbrun.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1265 2023-03-17 12:41:34.000000 mercury-2.2.8/mercury/apps/nb/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      403 2023-02-13 14:05:12.000000 mercury-2.2.8/mercury/apps/nb/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.671245 mercury-2.2.8/mercury/apps/nbworker/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.8/mercury/apps/nbworker/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1950 2023-04-27 15:29:23.000000 mercury-2.2.8/mercury/apps/nbworker/__main__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    17411 2023-04-12 08:48:16.000000 mercury-2.2.8/mercury/apps/nbworker/nb.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7485 2023-04-06 14:49:56.000000 mercury-2.2.8/mercury/apps/nbworker/rest.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4864 2023-03-17 08:55:41.000000 mercury-2.2.8/mercury/apps/nbworker/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      701 2023-03-14 07:49:44.000000 mercury-2.2.8/mercury/apps/nbworker/utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2927 2023-04-20 13:08:01.000000 mercury-2.2.8/mercury/apps/nbworker/ws.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.675245 mercury-2.2.8/mercury/apps/notebooks/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.8/mercury/apps/notebooks/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      277 2022-03-09 11:04:20.000000 mercury-2.2.8/mercury/apps/notebooks/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      155 2022-03-09 11:04:20.000000 mercury-2.2.8/mercury/apps/notebooks/apps.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.675245 mercury-2.2.8/mercury/apps/notebooks/management/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.8/mercury/apps/notebooks/management/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.675245 mercury-2.2.8/mercury/apps/notebooks/management/commands/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.8/mercury/apps/notebooks/management/commands/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1279 2022-03-09 11:06:47.000000 mercury-2.2.8/mercury/apps/notebooks/management/commands/add.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      864 2022-03-09 11:06:47.000000 mercury-2.2.8/mercury/apps/notebooks/management/commands/delete.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      545 2022-03-09 11:06:47.000000 mercury-2.2.8/mercury/apps/notebooks/management/commands/list.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3702 2023-02-13 14:05:12.000000 mercury-2.2.8/mercury/apps/notebooks/management/commands/watch.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.675245 mercury-2.2.8/mercury/apps/notebooks/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2300 2023-03-29 09:06:05.000000 mercury-2.2.8/mercury/apps/notebooks/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.8/mercury/apps/notebooks/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1067 2023-03-27 08:29:11.000000 mercury-2.2.8/mercury/apps/notebooks/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      617 2023-03-17 11:38:01.000000 mercury-2.2.8/mercury/apps/notebooks/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4093 2022-05-18 10:19:32.000000 mercury-2.2.8/mercury/apps/notebooks/slides_themes.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11689 2023-04-03 14:44:43.000000 mercury-2.2.8/mercury/apps/notebooks/tasks.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-03-01 11:11:00.000000 mercury-2.2.8/mercury/apps/notebooks/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      582 2023-04-25 12:40:05.000000 mercury-2.2.8/mercury/apps/notebooks/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3798 2023-04-27 15:18:53.000000 mercury-2.2.8/mercury/apps/notebooks/views.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.675245 mercury-2.2.8/mercury/apps/storage/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.8/mercury/apps/storage/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-02-13 14:05:12.000000 mercury-2.2.8/mercury/apps/storage/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-02-13 14:05:12.000000 mercury-2.2.8/mercury/apps/storage/apps.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.675245 mercury-2.2.8/mercury/apps/storage/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2949 2023-03-29 09:06:05.000000 mercury-2.2.8/mercury/apps/storage/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1404 2023-03-31 09:54:03.000000 mercury-2.2.8/mercury/apps/storage/migrations/0002_useruploadedfile.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.8/mercury/apps/storage/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1787 2023-03-29 09:06:05.000000 mercury-2.2.8/mercury/apps/storage/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3540 2023-03-31 09:54:03.000000 mercury-2.2.8/mercury/apps/storage/s3utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      469 2023-03-31 14:19:15.000000 mercury-2.2.8/mercury/apps/storage/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11397 2023-03-31 09:54:03.000000 mercury-2.2.8/mercury/apps/storage/storage.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3158 2023-03-17 08:55:41.000000 mercury-2.2.8/mercury/apps/storage/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2132 2023-03-29 09:56:45.000000 mercury-2.2.8/mercury/apps/storage/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      445 2023-03-31 09:54:03.000000 mercury-2.2.8/mercury/apps/storage/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.675245 mercury-2.2.8/mercury/apps/storage/views/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-31 12:45:08.000000 mercury-2.2.8/mercury/apps/storage/views/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6182 2023-03-31 11:42:07.000000 mercury-2.2.8/mercury/apps/storage/views/dashboardfiles.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4935 2023-03-31 11:42:07.000000 mercury-2.2.8/mercury/apps/storage/views/notebookfiles.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3737 2023-03-31 11:42:07.000000 mercury-2.2.8/mercury/apps/storage/views/workerfiles.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.675245 mercury-2.2.8/mercury/apps/tasks/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.8/mercury/apps/tasks/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      287 2022-03-09 11:04:20.000000 mercury-2.2.8/mercury/apps/tasks/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2022-03-09 11:04:20.000000 mercury-2.2.8/mercury/apps/tasks/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      412 2022-03-09 11:06:47.000000 mercury-2.2.8/mercury/apps/tasks/clean_service.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3840 2023-04-03 14:18:32.000000 mercury-2.2.8/mercury/apps/tasks/export_pdf.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3805 2023-04-06 13:49:54.000000 mercury-2.2.8/mercury/apps/tasks/export_png.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.675245 mercury-2.2.8/mercury/apps/tasks/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1328 2023-03-29 09:06:05.000000 mercury-2.2.8/mercury/apps/tasks/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.8/mercury/apps/tasks/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      762 2022-05-18 10:19:32.000000 mercury-2.2.8/mercury/apps/tasks/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3659 2023-02-13 14:05:12.000000 mercury-2.2.8/mercury/apps/tasks/notify.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      433 2022-03-09 11:06:47.000000 mercury-2.2.8/mercury/apps/tasks/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15223 2023-02-23 14:52:12.000000 mercury-2.2.8/mercury/apps/tasks/tasks.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1314 2023-02-13 14:05:12.000000 mercury-2.2.8/mercury/apps/tasks/tasks_export.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      571 2023-03-14 07:49:44.000000 mercury-2.2.8/mercury/apps/tasks/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1431 2023-04-25 12:37:36.000000 mercury-2.2.8/mercury/apps/tasks/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8619 2023-03-17 08:55:41.000000 mercury-2.2.8/mercury/apps/tasks/views.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.675245 mercury-2.2.8/mercury/apps/workers/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.2.8/mercury/apps/workers/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-03-14 07:49:44.000000 mercury-2.2.8/mercury/apps/workers/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-03-14 07:49:44.000000 mercury-2.2.8/mercury/apps/workers/apps.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.675245 mercury-2.2.8/mercury/apps/workers/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1286 2023-03-29 09:06:05.000000 mercury-2.2.8/mercury/apps/workers/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.2.8/mercury/apps/workers/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      798 2023-03-29 09:06:05.000000 mercury-2.2.8/mercury/apps/workers/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      296 2023-03-14 07:49:44.000000 mercury-2.2.8/mercury/apps/workers/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       60 2023-03-14 07:49:44.000000 mercury-2.2.8/mercury/apps/workers/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1076 2023-04-25 12:37:59.000000 mercury-2.2.8/mercury/apps/workers/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3881 2023-03-31 09:54:03.000000 mercury-2.2.8/mercury/apps/workers/views.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.675245 mercury-2.2.8/mercury/apps/ws/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.8/mercury/apps/ws/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      141 2023-02-13 14:05:12.000000 mercury-2.2.8/mercury/apps/ws/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6162 2023-04-20 13:43:38.000000 mercury-2.2.8/mercury/apps/ws/client.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      947 2023-03-14 07:49:44.000000 mercury-2.2.8/mercury/apps/ws/middleware.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.675245 mercury-2.2.8/mercury/apps/ws/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.8/mercury/apps/ws/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      386 2023-02-28 13:59:46.000000 mercury-2.2.8/mercury/apps/ws/routing.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2495 2023-04-06 13:49:54.000000 mercury-2.2.8/mercury/apps/ws/tasks.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      137 2023-03-01 11:07:38.000000 mercury-2.2.8/mercury/apps/ws/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5106 2023-04-06 13:49:54.000000 mercury-2.2.8/mercury/apps/ws/utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1754 2023-03-14 07:49:44.000000 mercury-2.2.8/mercury/apps/ws/worker.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7191 2023-03-31 14:11:10.000000 mercury-2.2.8/mercury/demo.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.679245 mercury-2.2.8/mercury/frontend-dist/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1158 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury/frontend-dist/asset-manifest.json
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15406 2023-04-27 15:43:53.000000 mercury-2.2.8/mercury/frontend-dist/favicon-old.ico
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15086 2023-04-27 15:43:53.000000 mercury-2.2.8/mercury/frontend-dist/favicon.ico
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3086 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury/frontend-dist/index.html
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    17406 2023-04-27 15:43:53.000000 mercury-2.2.8/mercury/frontend-dist/jupyter-additional.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4539 2023-04-27 15:43:53.000000 mercury-2.2.8/mercury/frontend-dist/jupyter-syntax.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   580386 2023-04-27 15:43:53.000000 mercury-2.2.8/mercury/frontend-dist/jupyter-theme-light.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      324 2023-04-27 15:43:53.000000 mercury-2.2.8/mercury/frontend-dist/manifest.json
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6237 2023-04-27 15:43:53.000000 mercury-2.2.8/mercury/frontend-dist/mercury_black_logo.svg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6997 2023-04-27 15:43:53.000000 mercury-2.2.8/mercury/frontend-dist/mercury_logo.svg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       67 2023-04-27 15:43:53.000000 mercury-2.2.8/mercury/frontend-dist/robots.txt
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.671245 mercury-2.2.8/mercury/frontend-dist/static/
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.679245 mercury-2.2.8/mercury/frontend-dist/static/css/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   229115 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   612316 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2831 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury/frontend-dist/static/css/main.26f96620.chunk.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5260 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury/frontend-dist/static/css/main.26f96620.chunk.css.map
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.683245 mercury-2.2.8/mercury/frontend-dist/static/js/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)  1311795 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury/frontend-dist/static/js/2.6305b467.chunk.js
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3383 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury/frontend-dist/static/js/2.6305b467.chunk.js.LICENSE.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)  4973509 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury/frontend-dist/static/js/2.6305b467.chunk.js.map
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    85726 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury/frontend-dist/static/js/main.c4e40c36.chunk.js
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   262033 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury/frontend-dist/static/js/main.c4e40c36.chunk.js.map
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1557 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury/frontend-dist/static/js/runtime-main.248907bc.js
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8276 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury/frontend-dist/static/js/runtime-main.248907bc.js.map
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.683245 mercury-2.2.8/mercury/frontend-dist/static/media/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   165548 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury/frontend-dist/static/media/fontawesome-webfont.1e59d233.ttf
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    77160 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury/frontend-dist/static/media/fontawesome-webfont.20fd1704.woff2
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   165742 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury/frontend-dist/static/media/fontawesome-webfont.8b43027f.eot
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   444379 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury/frontend-dist/static/media/fontawesome-webfont.c1e38fd9.svg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    98024 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury/frontend-dist/static/media/fontawesome-webfont.f691f37e.woff
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      684 2022-03-09 11:04:20.000000 mercury-2.2.8/mercury/manage.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8556 2023-04-27 14:42:46.000000 mercury-2.2.8/mercury/mercury.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      545 2023-04-25 12:41:47.000000 mercury-2.2.8/mercury/requirements.txt
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.683245 mercury-2.2.8/mercury/server/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       68 2022-03-09 11:04:20.000000 mercury-2.2.8/mercury/server/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      837 2023-03-14 07:49:44.000000 mercury-2.2.8/mercury/server/asgi.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2771 2023-03-24 08:43:00.000000 mercury-2.2.8/mercury/server/celery.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9844 2023-04-05 13:16:51.000000 mercury-2.2.8/mercury/server/settings.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1575 2023-04-25 12:38:18.000000 mercury-2.2.8/mercury/server/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1645 2023-03-01 12:07:40.000000 mercury-2.2.8/mercury/server/views.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      405 2022-05-18 11:03:41.000000 mercury-2.2.8/mercury/server/wsgi.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.683245 mercury-2.2.8/mercury/widgets/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.8/mercury/widgets/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2029 2023-03-17 11:39:55.000000 mercury-2.2.8/mercury/widgets/app.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2294 2023-04-07 10:30:37.000000 mercury-2.2.8/mercury/widgets/button.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      826 2023-04-07 10:43:02.000000 mercury-2.2.8/mercury/widgets/chat.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2127 2023-04-07 10:30:37.000000 mercury-2.2.8/mercury/widgets/checkbox.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      408 2023-04-07 10:32:14.000000 mercury-2.2.8/mercury/widgets/confetti.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3393 2023-04-07 10:30:37.000000 mercury-2.2.8/mercury/widgets/file.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4828 2023-02-21 07:28:26.000000 mercury-2.2.8/mercury/widgets/json.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6894 2023-04-07 10:30:37.000000 mercury-2.2.8/mercury/widgets/manager.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      104 2023-02-21 07:28:26.000000 mercury-2.2.8/mercury/widgets/md.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2690 2023-04-07 10:30:37.000000 mercury-2.2.8/mercury/widgets/multiselect.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1219 2023-02-21 07:48:36.000000 mercury-2.2.8/mercury/widgets/note.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3016 2023-04-07 10:30:37.000000 mercury-2.2.8/mercury/widgets/numeric.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1255 2023-02-21 07:48:36.000000 mercury-2.2.8/mercury/widgets/outputdir.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3025 2023-04-07 10:30:37.000000 mercury-2.2.8/mercury/widgets/range.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2403 2023-04-07 10:30:37.000000 mercury-2.2.8/mercury/widgets/select.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2949 2023-04-07 10:30:37.000000 mercury-2.2.8/mercury/widgets/slider.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      222 2023-02-21 07:28:26.000000 mercury-2.2.8/mercury/widgets/stop.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2039 2023-04-07 10:30:37.000000 mercury-2.2.8/mercury/widgets/text.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-27 15:44:08.671245 mercury-2.2.8/mercury.egg-info/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5674 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury.egg-info/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6285 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury.egg-info/SOURCES.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury.egg-info/dependency_links.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       50 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury.egg-info/entry_points.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      489 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury.egg-info/requires.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        8 2023-04-27 15:44:08.000000 mercury-2.2.8/mercury.egg-info/top_level.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      106 2022-03-09 11:04:20.000000 mercury-2.2.8/pyproject.toml
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2023-04-27 15:44:08.683245 mercury-2.2.8/setup.cfg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1163 2023-04-27 15:43:25.000000 mercury-2.2.8/setup.py
```

### Comparing `mercury-2.2.7/PKG-INFO` & `mercury-2.2.8/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury
-Version: 2.2.7
+Version: 2.2.8
 Summary: Turn Jupyter Notebook to Web App and share with non-technical users
 Home-page: https://github.com/mljar/mercury
 Maintainer: MLJAR Sp. z o.o.
 Maintainer-email: contact@mljar.com
 License: UNKNOWN
 Description:
```

### Comparing `mercury-2.2.7/README.md` & `mercury-2.2.8/README.md`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/accounts/fields.py` & `mercury-2.2.8/mercury/apps/accounts/fields.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/accounts/migrations/0001_initial.py` & `mercury-2.2.8/mercury/apps/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/accounts/models.py` & `mercury-2.2.8/mercury/apps/accounts/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/accounts/serializers.py` & `mercury-2.2.8/mercury/apps/accounts/serializers.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/accounts/tasks.py` & `mercury-2.2.8/mercury/apps/accounts/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/accounts/tests/test_accounts.py` & `mercury-2.2.8/mercury/apps/accounts/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/accounts/tests/test_invitations.py` & `mercury-2.2.8/mercury/apps/accounts/tests/test_invitations.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/accounts/tests/test_secrets.py` & `mercury-2.2.8/mercury/apps/accounts/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/accounts/tests/test_sites.py` & `mercury-2.2.8/mercury/apps/accounts/tests/test_sites.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/accounts/tests/test_subscription.py` & `mercury-2.2.8/mercury/apps/accounts/tests/test_subscription.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/accounts/urls.py` & `mercury-2.2.8/mercury/apps/accounts/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.conf.urls import include, url
+from django.conf.urls import include
 from django.urls import path, re_path
 from django.views.generic.base import TemplateView
 from rest_framework.routers import DefaultRouter
 
 from apps.accounts.views.sites import GetSiteView, InitializeSite, SiteViewSet
 
 from apps.accounts.views.accounts import MembershipViewSet, DeleteAccount
```

### Comparing `mercury-2.2.7/mercury/apps/accounts/views/accounts.py` & `mercury-2.2.8/mercury/apps/accounts/views/accounts.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/accounts/views/invitations.py` & `mercury-2.2.8/mercury/apps/accounts/views/invitations.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/accounts/views/permissions.py` & `mercury-2.2.8/mercury/apps/accounts/views/permissions.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/accounts/views/secrets.py` & `mercury-2.2.8/mercury/apps/accounts/views/secrets.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/accounts/views/sites.py` & `mercury-2.2.8/mercury/apps/accounts/views/sites.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,25 +139,29 @@
 
 class GetSiteView(APIView):
     def get(self, request, site_slug, format=None):
         url = site_slug
         # this can be a custom domain
         custom_domain = url
         # or subdomain with domain
-        subdomain, domain = "", "runmercury.com"
+        subdomain, domain = "single-site", "runmercury.com"
 
         if len(url.split(".")) > 1:
             subdomain = url.split(".")[0]
             domain = ".".join(url.split(".")[1:])
 
         if site_slug in ["127.0.0.1", "localhost"]:
             subdomain = "single-site"
             domain = "runmercury.com"
 
-        print(subdomain, domain, custom_domain)
+        if request.build_absolute_uri().startswith("http://127.0.0.1"):
+            subdomain = "single-site"
+            domain = "runmercury.com"
+
+        print(f"{url}|{request.build_absolute_uri()}|{subdomain}|{domain}|{custom_domain}")
 
         sites = Site.objects.filter(
             Q(custom_domain=custom_domain) | Q(slug=subdomain, domain=domain)
         )
         if not sites:
             return Response(status=status.HTTP_404_NOT_FOUND)
```

### Comparing `mercury-2.2.7/mercury/apps/accounts/views/subscription.py` & `mercury-2.2.8/mercury/apps/accounts/views/subscription.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/nb/exporter.py` & `mercury-2.2.8/mercury/apps/nb/exporter.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/nb/nbrun.py` & `mercury-2.2.8/mercury/apps/nb/nbrun.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/nb/tests/test_nbrun.py` & `mercury-2.2.8/mercury/apps/nb/tests/test_nbrun.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/nb/tests.py` & `mercury-2.2.8/mercury/apps/nb/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/nbworker/__main__.py` & `mercury-2.2.8/mercury/apps/nbworker/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 logging.basicConfig(
     # filename="nbworker.log", filemode="w",
     format="NB %(asctime)s %(message)s",
     level=LOG_LEVEL,
 )
 log = logging.getLogger(__name__)
+logging.getLogger('matplotlib.font_manager').setLevel(logging.ERROR)
 
 from apps.nbworker.nb import NBWorker
 from apps.nbworker.rest import RESTClient
 from apps.nbworker.utils import stop_event
 
 if len(sys.argv) != 5:
     log.error("Wrong number of input parameters")
```

### Comparing `mercury-2.2.7/mercury/apps/nbworker/nb.py` & `mercury-2.2.8/mercury/apps/nbworker/nb.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/nbworker/rest.py` & `mercury-2.2.8/mercury/apps/nbworker/rest.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/nbworker/tests.py` & `mercury-2.2.8/mercury/apps/nbworker/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/nbworker/utils.py` & `mercury-2.2.8/mercury/apps/nbworker/utils.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/nbworker/ws.py` & `mercury-2.2.8/mercury/apps/nbworker/ws.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/notebooks/management/commands/add.py` & `mercury-2.2.8/mercury/apps/notebooks/management/commands/add.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/notebooks/management/commands/delete.py` & `mercury-2.2.8/mercury/apps/notebooks/management/commands/delete.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/notebooks/management/commands/list.py` & `mercury-2.2.8/mercury/apps/notebooks/management/commands/list.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/notebooks/management/commands/watch.py` & `mercury-2.2.8/mercury/apps/notebooks/management/commands/watch.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/notebooks/migrations/0001_initial.py` & `mercury-2.2.8/mercury/apps/notebooks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/notebooks/models.py` & `mercury-2.2.8/mercury/apps/notebooks/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/notebooks/serializers.py` & `mercury-2.2.8/mercury/apps/notebooks/serializers.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/notebooks/slides_themes.py` & `mercury-2.2.8/mercury/apps/notebooks/slides_themes.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/notebooks/tasks.py` & `mercury-2.2.8/mercury/apps/notebooks/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/notebooks/urls.py` & `mercury-2.2.8/mercury/apps/notebooks/urls.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from django.conf.urls import url
+from django.urls import re_path
 
 from apps.notebooks.views import (
     GetNbIframes,
     ListNotebooks,
     RetrieveNotebook,
     RetrieveNotebookWithSlug,
 )
 
 notebooks_urlpatterns = [
-    url(
+    re_path(
         "api/v1/(?P<site_id>.+)/notebooks/(?P<notebook_id>.+)",
         RetrieveNotebook.as_view(),
     ),
-    url(
+    re_path(
         "api/v1/(?P<site_id>.+)/getnb/(?P<notebook_slug>.+)",
         RetrieveNotebookWithSlug.as_view(),
     ),
-    url("api/v1/(?P<site_id>.+)/notebooks", ListNotebooks.as_view()),
-    url("api/v1/(?P<site_id>.+)/nb-iframes", GetNbIframes.as_view()),
+    re_path("api/v1/(?P<site_id>.+)/notebooks", ListNotebooks.as_view()),
+    re_path("api/v1/(?P<site_id>.+)/nb-iframes", GetNbIframes.as_view()),
 ]
```

### Comparing `mercury-2.2.7/mercury/apps/notebooks/views.py` & `mercury-2.2.8/mercury/apps/notebooks/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,17 @@
         return Notebook.objects.filter(hosted_on=site)
     return Notebook.objects.filter(hosted_on=site, created_by=user)
 
 
 def nb_iframe_url(request, iframe_db_address):
     iframe_url = ""
     if settings.STORAGE == settings.STORAGE_MEDIA:
-        host = request.build_absolute_uri("/")[:-1]
-        iframe_url = f"{host}{iframe_db_address}"
+        # host = request.build_absolute_uri("/")[:-1]
+        # iframe_url = f"{host}{iframe_db_address}"
+        iframe_url = iframe_db_address
     elif settings.STORAGE == settings.STORAGE_S3:
         s3 = S3()
         url = s3.get_presigned_url(iframe_db_address, "get_object")
         iframe_url = url
     return iframe_url
```

### Comparing `mercury-2.2.7/mercury/apps/storage/migrations/0001_initial.py` & `mercury-2.2.8/mercury/apps/storage/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/storage/migrations/0002_useruploadedfile.py` & `mercury-2.2.8/mercury/apps/storage/migrations/0002_useruploadedfile.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/storage/models.py` & `mercury-2.2.8/mercury/apps/storage/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/storage/s3utils.py` & `mercury-2.2.8/mercury/apps/storage/s3utils.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/storage/storage.py` & `mercury-2.2.8/mercury/apps/storage/storage.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/storage/tests.py` & `mercury-2.2.8/mercury/apps/storage/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/storage/urls.py` & `mercury-2.2.8/mercury/apps/storage/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/storage/views/dashboardfiles.py` & `mercury-2.2.8/mercury/apps/storage/views/dashboardfiles.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/storage/views/notebookfiles.py` & `mercury-2.2.8/mercury/apps/storage/views/notebookfiles.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/storage/views/workerfiles.py` & `mercury-2.2.8/mercury/apps/storage/views/workerfiles.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/tasks/export_pdf.py` & `mercury-2.2.8/mercury/apps/tasks/export_pdf.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/tasks/export_png.py` & `mercury-2.2.8/mercury/apps/tasks/export_png.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/tasks/migrations/0001_initial.py` & `mercury-2.2.8/mercury/apps/tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/tasks/models.py` & `mercury-2.2.8/mercury/apps/tasks/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/tasks/notify.py` & `mercury-2.2.8/mercury/apps/tasks/notify.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/tasks/tasks.py` & `mercury-2.2.8/mercury/apps/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/tasks/tasks_export.py` & `mercury-2.2.8/mercury/apps/tasks/tasks_export.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/tasks/tests.py` & `mercury-2.2.8/mercury/apps/tasks/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/tasks/views.py` & `mercury-2.2.8/mercury/apps/tasks/views.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/workers/migrations/0001_initial.py` & `mercury-2.2.8/mercury/apps/workers/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/workers/models.py` & `mercury-2.2.8/mercury/apps/workers/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/workers/urls.py` & `mercury-2.2.8/mercury/apps/workers/urls.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from django.conf.urls import url
+from django.urls import re_path
 
 from apps.workers.views import (
     DeleteWorker,
     GetWorker,
     IsWorkerStale,
     SetWorkerState,
     WorkerGetNb,
     WorkerUpdateNb,
 )
 
 workers_urlpatterns = [
-    url(
+    re_path(
         "api/v1/worker/(?P<session_id>.+)/(?P<worker_id>.+)/(?P<notebook_id>.+)/nb",
         WorkerGetNb.as_view(),
     ),
-    url(
+    re_path(
         "api/v1/worker/(?P<session_id>.+)/(?P<worker_id>.+)/(?P<notebook_id>.+)/update-nb",
         WorkerUpdateNb.as_view(),
     ),
-    url(
+    re_path(
         "api/v1/worker/(?P<session_id>.+)/(?P<worker_id>.+)/(?P<notebook_id>.+)/worker",
         GetWorker.as_view(),
     ),
-    url(
+    re_path(
         "api/v1/worker/(?P<session_id>.+)/(?P<worker_id>.+)/(?P<notebook_id>.+)/is-worker-stale",
         IsWorkerStale.as_view(),
     ),
-    url(
+    re_path(
         "api/v1/worker/(?P<session_id>.+)/(?P<worker_id>.+)/(?P<notebook_id>.+)/set-worker-state",
         SetWorkerState.as_view(),
     ),
-    url(
+    re_path(
         "api/v1/worker/(?P<session_id>.+)/(?P<worker_id>.+)/(?P<notebook_id>.+)/delete-worker",
         DeleteWorker.as_view(),
     ),
 ]
```

### Comparing `mercury-2.2.7/mercury/apps/workers/views.py` & `mercury-2.2.8/mercury/apps/workers/views.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/ws/client.py` & `mercury-2.2.8/mercury/apps/ws/client.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/ws/middleware.py` & `mercury-2.2.8/mercury/apps/ws/middleware.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/ws/tasks.py` & `mercury-2.2.8/mercury/apps/ws/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/ws/utils.py` & `mercury-2.2.8/mercury/apps/ws/utils.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/apps/ws/worker.py` & `mercury-2.2.8/mercury/apps/ws/worker.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/demo.py` & `mercury-2.2.8/mercury/demo.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/frontend-dist/asset-manifest.json` & `mercury-2.2.8/mercury/frontend-dist/asset-manifest.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8974358974358974%*

 * *Differences: {"'entrypoints'": "{insert: [(4, 'static/js/main.c4e40c36.chunk.js')], delete: [4]}",*

 * * "'files'": "{'main.js': '/static/js/main.c4e40c36.chunk.js', 'main.js.map': "*

 * *            "'/static/js/main.c4e40c36.chunk.js.map'}"}*

```diff
@@ -1,20 +1,20 @@
 {
     "entrypoints": [
         "static/js/runtime-main.248907bc.js",
         "static/css/2.c6cf5ff9.chunk.css",
         "static/js/2.6305b467.chunk.js",
         "static/css/main.26f96620.chunk.css",
-        "static/js/main.68931b96.chunk.js"
+        "static/js/main.c4e40c36.chunk.js"
     ],
     "files": {
         "index.html": "/index.html",
         "main.css": "/static/css/main.26f96620.chunk.css",
-        "main.js": "/static/js/main.68931b96.chunk.js",
-        "main.js.map": "/static/js/main.68931b96.chunk.js.map",
+        "main.js": "/static/js/main.c4e40c36.chunk.js",
+        "main.js.map": "/static/js/main.c4e40c36.chunk.js.map",
         "runtime-main.js": "/static/js/runtime-main.248907bc.js",
         "runtime-main.js.map": "/static/js/runtime-main.248907bc.js.map",
         "static/css/2.c6cf5ff9.chunk.css": "/static/css/2.c6cf5ff9.chunk.css",
         "static/css/2.c6cf5ff9.chunk.css.map": "/static/css/2.c6cf5ff9.chunk.css.map",
         "static/css/main.26f96620.chunk.css.map": "/static/css/main.26f96620.chunk.css.map",
         "static/js/2.6305b467.chunk.js": "/static/js/2.6305b467.chunk.js",
         "static/js/2.6305b467.chunk.js.LICENSE.txt": "/static/js/2.6305b467.chunk.js.LICENSE.txt",
```

### Comparing `mercury-2.2.7/mercury/frontend-dist/favicon-old.ico` & `mercury-2.2.8/mercury/frontend-dist/favicon-old.ico`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/frontend-dist/favicon.ico` & `mercury-2.2.8/mercury/frontend-dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/frontend-dist/index.html` & `mercury-2.2.8/mercury/frontend-dist/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/static/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Mercury: Easily share your Python notebooks"/><link rel="manifest" href="/static/manifest.json"/><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script><link rel="stylesheet" href="/static/jupyter-syntax.css"/><link rel="stylesheet" href="/static/jupyter-additional.css"/><link rel="stylesheet" href="/static/jupyter-theme-light.css"/><title>Mercury - Turn Jupyter Notebook to Web App</title><script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/latest.js?config=TeX-AMS_CHTML-full,Safe"></script><script>init_mathjax=function(){window.MathJax&&(MathJax.Hub.Config({showProcessingMessages:!1,TeX:{equationNumbers:{autoNumber:"AMS",useLabelIds:!0}},tex2jax:{inlineMath:[["$","$"],["\\(","\\)"]],displayMath:[["$$","$$"],["\\[","\\]"]],processEscapes:!0,processEnvironments:!0},displayAlign:"center",CommonHTML:{linebreaks:{automatic:!0}}}),MathJax.Hub.Queue(["Typeset",MathJax.Hub]))},init_mathjax()</script><link href="/static/css/2.c6cf5ff9.chunk.css" rel="stylesheet"><link href="/static/css/main.26f96620.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function r(r){for(var n,f,l=r[0],i=r[1],a=r[2],c=0,s=[];c<l.length;c++)f=l[c],Object.prototype.hasOwnProperty.call(o,f)&&o[f]&&s.push(o[f][0]),o[f]=0;for(n in i)Object.prototype.hasOwnProperty.call(i,n)&&(e[n]=i[n]);for(p&&p(r);s.length;)s.shift()();return u.push.apply(u,a||[]),t()}function t(){for(var e,r=0;r<u.length;r++){for(var t=u[r],n=!0,l=1;l<t.length;l++){var i=t[l];0!==o[i]&&(n=!1)}n&&(u.splice(r--,1),e=f(f.s=t[0]))}return e}var n={},o={1:0},u=[];function f(r){if(n[r])return n[r].exports;var t=n[r]={i:r,l:!1,exports:{}};return e[r].call(t.exports,t,t.exports,f),t.l=!0,t.exports}f.m=e,f.c=n,f.d=function(e,r,t){f.o(e,r)||Object.defineProperty(e,r,{enumerable:!0,get:t})},f.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},f.t=function(e,r){if(1&r&&(e=f(e)),8&r)return e;if(4&r&&"object"==typeof e&&e&&e.__esModule)return e;var t=Object.create(null);if(f.r(t),Object.defineProperty(t,"default",{enumerable:!0,value:e}),2&r&&"string"!=typeof e)for(var n in e)f.d(t,n,function(r){return e[r]}.bind(null,n));return t},f.n=function(e){var r=e&&e.__esModule?function(){return e.default}:function(){return e};return f.d(r,"a",r),r},f.o=function(e,r){return Object.prototype.hasOwnProperty.call(e,r)},f.p="/";var l=this.webpackJsonpfrontend=this.webpackJsonpfrontend||[],i=l.push.bind(l);l.push=r,l=l.slice();for(var a=0;a<l.length;a++)r(l[a]);var p=i;t()}([])</script><script src="/static/js/2.6305b467.chunk.js"></script><script src="/static/js/main.68931b96.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/static/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Mercury: Easily share your Python notebooks"/><link rel="manifest" href="/static/manifest.json"/><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script><link rel="stylesheet" href="/static/jupyter-syntax.css"/><link rel="stylesheet" href="/static/jupyter-additional.css"/><link rel="stylesheet" href="/static/jupyter-theme-light.css"/><title>Mercury - Turn Jupyter Notebook to Web App</title><script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/latest.js?config=TeX-AMS_CHTML-full,Safe"></script><script>init_mathjax=function(){window.MathJax&&(MathJax.Hub.Config({showProcessingMessages:!1,TeX:{equationNumbers:{autoNumber:"AMS",useLabelIds:!0}},tex2jax:{inlineMath:[["$","$"],["\\(","\\)"]],displayMath:[["$$","$$"],["\\[","\\]"]],processEscapes:!0,processEnvironments:!0},displayAlign:"center",CommonHTML:{linebreaks:{automatic:!0}}}),MathJax.Hub.Queue(["Typeset",MathJax.Hub]))},init_mathjax()</script><link href="/static/css/2.c6cf5ff9.chunk.css" rel="stylesheet"><link href="/static/css/main.26f96620.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function r(r){for(var n,f,l=r[0],i=r[1],a=r[2],c=0,s=[];c<l.length;c++)f=l[c],Object.prototype.hasOwnProperty.call(o,f)&&o[f]&&s.push(o[f][0]),o[f]=0;for(n in i)Object.prototype.hasOwnProperty.call(i,n)&&(e[n]=i[n]);for(p&&p(r);s.length;)s.shift()();return u.push.apply(u,a||[]),t()}function t(){for(var e,r=0;r<u.length;r++){for(var t=u[r],n=!0,l=1;l<t.length;l++){var i=t[l];0!==o[i]&&(n=!1)}n&&(u.splice(r--,1),e=f(f.s=t[0]))}return e}var n={},o={1:0},u=[];function f(r){if(n[r])return n[r].exports;var t=n[r]={i:r,l:!1,exports:{}};return e[r].call(t.exports,t,t.exports,f),t.l=!0,t.exports}f.m=e,f.c=n,f.d=function(e,r,t){f.o(e,r)||Object.defineProperty(e,r,{enumerable:!0,get:t})},f.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},f.t=function(e,r){if(1&r&&(e=f(e)),8&r)return e;if(4&r&&"object"==typeof e&&e&&e.__esModule)return e;var t=Object.create(null);if(f.r(t),Object.defineProperty(t,"default",{enumerable:!0,value:e}),2&r&&"string"!=typeof e)for(var n in e)f.d(t,n,function(r){return e[r]}.bind(null,n));return t},f.n=function(e){var r=e&&e.__esModule?function(){return e.default}:function(){return e};return f.d(r,"a",r),r},f.o=function(e,r){return Object.prototype.hasOwnProperty.call(e,r)},f.p="/";var l=this.webpackJsonpfrontend=this.webpackJsonpfrontend||[],i=l.push.bind(l);l.push=r,l=l.slice();for(var a=0;a<l.length;a++)r(l[a]);var p=i;t()}([])</script><script src="/static/js/2.6305b467.chunk.js"></script><script src="/static/js/main.c4e40c36.chunk.js"></script></body></html>
```

### Comparing `mercury-2.2.7/mercury/frontend-dist/jupyter-additional.css` & `mercury-2.2.8/mercury/frontend-dist/jupyter-additional.css`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/frontend-dist/jupyter-syntax.css` & `mercury-2.2.8/mercury/frontend-dist/jupyter-syntax.css`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/frontend-dist/jupyter-theme-light.css` & `mercury-2.2.8/mercury/frontend-dist/jupyter-theme-light.css`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/frontend-dist/mercury_black_logo.svg` & `mercury-2.2.8/mercury/frontend-dist/mercury_black_logo.svg`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/frontend-dist/mercury_logo.svg` & `mercury-2.2.8/mercury/frontend-dist/mercury_logo.svg`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css` & `mercury-2.2.8/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map` & `mercury-2.2.8/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/frontend-dist/static/css/main.26f96620.chunk.css` & `mercury-2.2.8/mercury/frontend-dist/static/css/main.26f96620.chunk.css`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/frontend-dist/static/css/main.26f96620.chunk.css.map` & `mercury-2.2.8/mercury/frontend-dist/static/css/main.26f96620.chunk.css.map`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/frontend-dist/static/js/2.6305b467.chunk.js` & `mercury-2.2.8/mercury/frontend-dist/static/js/2.6305b467.chunk.js`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/frontend-dist/static/js/2.6305b467.chunk.js.LICENSE.txt` & `mercury-2.2.8/mercury/frontend-dist/static/js/2.6305b467.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/frontend-dist/static/js/2.6305b467.chunk.js.map` & `mercury-2.2.8/mercury/frontend-dist/static/js/2.6305b467.chunk.js.map`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/frontend-dist/static/js/main.68931b96.chunk.js` & `mercury-2.2.8/mercury/frontend-dist/static/js/main.c4e40c36.chunk.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -63,27 +63,27 @@
                     }
                 }),
                 w = y.reducer,
                 k = y.actions,
                 N = k.setToken,
                 S = k.setUsername,
                 P = k.setUserInfo,
-                C = function(e) {
+                T = function(e) {
                     return e.auth.token
                 },
-                T = function(e) {
+                _ = function(e) {
                     return e.auth.username
                 },
-                R = function(e) {
+                C = function(e) {
                     return e.auth.user
                 },
-                _ = a(9),
+                R = a(9),
                 E = (a(193), a(0));
 
-            function F() {
+            function A() {
                 return Object(E.jsx)("div", {
                     style: {
                         color: "white",
                         padding: "5px",
                         float: "right"
                     },
                     children: Object(E.jsxs)(c.b, {
@@ -93,15 +93,15 @@
                             className: "fa fa-sign-in",
                             "aria-hidden": "true"
                         }), " Log in"]
                     })
                 })
             }
 
-            function A(e) {
+            function L(e) {
                 var t = e.username,
                     a = Object(i.b)(),
                     n = Object(r.o)();
                 return Object(E.jsx)("div", {
                     children: Object(E.jsxs)("div", {
                         className: "dropdown",
                         style: {
@@ -171,15 +171,15 @@
                                 })
                             })]
                         })]
                     })
                 })
             }
 
-            function M(e) {
+            function D(e) {
                 var t = e.isSitePublic,
                     a = e.username;
                 return Object(E.jsxs)("header", {
                     className: "navbar navbar-dark sticky-top bg-dark flex-md-nowrap p-0",
                     children: [Object(E.jsx)(c.b, {
                         className: "navbar-brand col-md-3 col-lg-3 me-0 px-3",
                         to: "/",
@@ -187,22 +187,22 @@
                             alt: "Mercury",
                             src: "/static/mercury_logo.svg",
                             style: {
                                 height: "28px",
                                 paddingLeft: "10px"
                             }
                         })
-                    }), !t && "" === a && Object(E.jsx)(F, {}), "" !== a && Object(E.jsx)(A, {
+                    }), !t && "" === a && Object(E.jsx)(A, {}), "" !== a && Object(E.jsx)(L, {
                         username: a
                     })]
                 })
             }
-            var D = a(14),
-                I = a(27),
-                L = Object(b.b)({
+            var U = a(14),
+                F = a(27),
+                W = Object(b.b)({
                     name: "app",
                     initialState: {
                         view: "app",
                         files: [],
                         filesState: "unknown",
                         showSideBar: !0,
                         storageType: "media"
@@ -224,22 +224,22 @@
                             e.showSideBar = !e.showSideBar
                         },
                         setStorageType: function(e, t) {
                             e.storageType = t.payload
                         }
                     }
                 }),
-                U = L.reducer,
-                W = L.actions,
-                H = W.setView,
-                z = W.setFilesState,
-                B = W.setFiles,
-                V = W.setShowSideBar,
-                J = (W.toggleShowSideBar, W.setStorageType),
-                K = function(e) {
+                I = W.reducer,
+                M = W.actions,
+                H = M.setView,
+                B = M.setFilesState,
+                V = M.setFiles,
+                z = M.setShowSideBar,
+                K = (M.toggleShowSideBar, M.setStorageType),
+                J = function(e) {
                     return e.app.view
                 },
                 q = function(e) {
                     return e.app.filesState
                 },
                 Y = function(e) {
                     return e.app.files
@@ -380,38 +380,38 @@
                             e.slidesHash = t.payload
                         },
                         updateWidgetsParams: function(e, t) {
                             for (var a = t.payload.widgetKey, n = !1, o = !0, s = 0, i = Object.keys(e.selectedNotebook.params.params); s < i.length; s++) {
                                 var r = i[s];
                                 if (r === a) {
                                     o = !1;
-                                    var c = Object(D.a)({}, e.selectedNotebook.params.params[a]);
+                                    var c = Object(U.a)({}, e.selectedNotebook.params.params[a]);
                                     ae(c) ? (c.disabled !== t.payload.disabled && (c.disabled = t.payload.disabled, e.widgets[r] = t.payload.value, n = !0), c.hidden !== t.payload.hidden && (c.hidden = t.payload.hidden, e.widgets[r] = t.payload.value, n = !0), c.min !== t.payload.min && (c.min = t.payload.min, e.widgets[r] = t.payload.value, n = !0), c.max !== t.payload.max && (c.max = t.payload.max, e.widgets[r] = t.payload.value, n = !0), c.step !== t.payload.step && (c.step = t.payload.step, e.widgets[r] = t.payload.value, n = !0), c.label !== t.payload.label && (c.label = t.payload.label, n = !0)) : oe(c) ? (c.disabled !== t.payload.disabled && (c.disabled = t.payload.disabled, e.widgets[r] = t.payload.value, n = !0), c.hidden !== t.payload.hidden && (c.hidden = t.payload.hidden, e.widgets[r] = t.payload.value, n = !0), c.rows !== t.payload.rows && (c.rows = t.payload.rows, n = !0), c.label !== t.payload.label && (c.label = t.payload.label, n = !0)) : te(c) ? (c.disabled !== t.payload.disabled && (c.disabled = t.payload.disabled, e.widgets[r] = t.payload.value, n = !0), c.hidden !== t.payload.hidden && (c.hidden = t.payload.hidden, e.widgets[r] = t.payload.value, n = !0), c.min !== t.payload.min && (c.min = t.payload.min, e.widgets[r] = t.payload.value, n = !0), c.max !== t.payload.max && (c.max = t.payload.max, e.widgets[r] = t.payload.value, n = !0), c.step !== t.payload.step && (c.step = t.payload.step, e.widgets[r] = t.payload.value, n = !0), c.label !== t.payload.label && (c.label = t.payload.label, n = !0)) : X(c) ? (c.disabled !== t.payload.disabled && (c.disabled = t.payload.disabled, e.widgets[r] = t.payload.value, n = !0), c.hidden !== t.payload.hidden && (c.hidden = t.payload.hidden, e.widgets[r] = t.payload.value, n = !0), c.choices.toString() !== t.payload.choices.toString() && (c.choices = t.payload.choices, e.widgets[r] = t.payload.value, n = !0), c.label !== t.payload.label && (c.label = t.payload.label, n = !0)) : $(c) ? (c.disabled !== t.payload.disabled && (c.disabled = t.payload.disabled, e.widgets[r] = t.payload.value, n = !0), c.hidden !== t.payload.hidden && (c.hidden = t.payload.hidden, e.widgets[r] = t.payload.value, n = !0), c.label !== t.payload.label && (c.label = t.payload.label, n = !0)) : ee(c) ? (c.disabled !== t.payload.disabled && (c.disabled = t.payload.disabled, e.widgets[r] = t.payload.value, n = !0), c.hidden !== t.payload.hidden && (c.hidden = t.payload.hidden, e.widgets[r] = t.payload.value, n = !0), c.min !== t.payload.min && (c.min = t.payload.min, e.widgets[r] = t.payload.value, n = !0), c.max !== t.payload.max && (c.max = t.payload.max, e.widgets[r] = t.payload.value, n = !0), c.step !== t.payload.step && (c.step = t.payload.step, e.widgets[r] = t.payload.value, n = !0), c.label !== t.payload.label && (c.label = t.payload.label, n = !0)) : ie(c) ? c.value !== t.payload.value && (c.value = t.payload.value, n = !0) : re(c) ? (e.widgets[r] = t.payload.value, c.disabled !== t.payload.disabled && (c.disabled = t.payload.disabled, e.widgets[r] = t.payload.value, n = !0), c.hidden !== t.payload.hidden && (c.hidden = t.payload.hidden, e.widgets[r] = t.payload.value, n = !0), c.label !== t.payload.label && (c.label = t.payload.label, n = !0), c.style !== t.payload.style && (c.style = t.payload.style, n = !0)) : ne(c) && (e.widgets[r] = t.payload.value, c.disabled !== t.payload.disabled && (c.disabled = t.payload.disabled, e.widgets[r] = t.payload.value, n = !0), c.hidden !== t.payload.hidden && (c.hidden = t.payload.hidden, e.widgets[r] = t.payload.value, n = !0), c.label !== t.payload.label && (c.label = t.payload.label, n = !0)), n && (e.selectedNotebook.params.params[a] = c)
                                 }
                             }
                             o && (e.selectedNotebook.params.params[a] = t.payload)
                         },
                         hideWidgets: function(e, t) {
                             var a, n = t.payload.keys,
-                                o = Object(I.a)(n);
+                                o = Object(F.a)(n);
                             try {
                                 for (o.s(); !(a = o.n()).done;) {
                                     var s = a.value;
                                     s in e.selectedNotebook.params.params && delete e.selectedNotebook.params.params[s]
                                 }
                             } catch (i) {
                                 o.e(i)
                             } finally {
                                 o.f()
                             }
                         },
                         initWidgets: function(e, t) {
                             var a = t.payload.widgets;
                             e.selectedNotebook.params.params = {}, e.widgets = {};
-                            var n, o = Object(I.a)(a);
+                            var n, o = Object(F.a)(a);
                             try {
                                 for (o.s(); !(n = o.n()).done;) {
                                     var s = n.value;
                                     e.selectedNotebook.params.params[s.widgetKey] = s, e.widgets[s.widgetKey] = s.value
                                 }
                             } catch (i) {
                                 o.e(i)
@@ -449,49 +449,49 @@
                 ge = be.setWidgetUrlValue,
                 ye = (be.clearWidgets, be.clearWidgetsUrlValues),
                 we = be.initWidgets,
                 ke = be.updateTitle,
                 Ne = be.updateShowCode,
                 Se = (be.setNbIframes, be.setWidgetsInitialized),
                 Pe = be.setUrlValuesUsed,
-                Ce = function(e) {
+                Te = function(e) {
                     return e.notebooks.notebooks
                 },
-                Te = function(e) {
+                _e = function(e) {
                     return e.notebooks.loadingState
                 },
-                Re = function(e) {
+                Ce = function(e) {
                     return e.notebooks.selectedNotebook
                 },
-                _e = function(e) {
+                Re = function(e) {
                     return e.notebooks.selectedNotebookId
                 },
                 Ee = function(e) {
                     var t, a, n = null === (t = e.notebooks.selectedNotebook) || void 0 === t || null === (a = t.params) || void 0 === a ? void 0 : a.static_notebook;
                     return void 0 !== n && n
                 },
-                Fe = function(e) {
+                Ae = function(e) {
                     return e.notebooks.loadingStateSelected
                 },
-                Ae = function(e) {
+                Le = function(e) {
                     return e.notebooks.slidesHash
                 },
-                Me = function(e) {
+                De = function(e) {
                     return e.notebooks.widgets
                 },
-                De = function(e) {
+                Ue = function(e) {
                     return e.notebooks.widgetsUrlValues
                 },
-                Ie = function(e) {
+                Fe = function(e) {
                     return e.notebooks.widgetsInitialized
                 },
-                Le = function(e) {
+                We = function(e) {
                     return e.notebooks.urlValuesUsed
                 },
-                Ue = Object(b.b)({
+                Ie = Object(b.b)({
                     name: "tasks",
                     initialState: {
                         currentTask: {},
                         historicTask: {},
                         showCurrent: !0,
                         previousTask: {},
                         exportingToPDF: !1,
@@ -534,21 +534,21 @@
                             e.executionHistory = t.payload
                         },
                         clearExecutionHistory: function(e) {
                             e.executionHistory = []
                         }
                     }
                 }),
-                We = Ue.reducer,
-                He = Ue.actions,
-                ze = (He.setShowCurrent, He.setCurrentTask, He.setHistoricTask, He.setPreviousTask, He.copyCurrentToPreviousTask, He.setExportingToPDF),
-                Be = He.setExportToPDFJobId,
-                Ve = He.resetExportToPDFCounter,
-                Je = He.increaseExportToPDFCounter,
-                Ke = He.stopPDFExport,
+                Me = Ie.reducer,
+                He = Ie.actions,
+                Be = (He.setShowCurrent, He.setCurrentTask, He.setHistoricTask, He.setPreviousTask, He.copyCurrentToPreviousTask, He.setExportingToPDF),
+                Ve = He.setExportToPDFJobId,
+                ze = He.resetExportToPDFCounter,
+                Ke = He.increaseExportToPDFCounter,
+                Je = He.stopPDFExport,
                 qe = (He.setExecutionHistory, He.clearExecutionHistory),
                 Ye = function(e) {
                     return e.tasks.currentTask
                 },
                 Ge = function(e) {
                     return e.tasks.historicTask
                 },
@@ -579,19 +579,19 @@
                     o = e.value,
                     s = e.disabled,
                     r = e.hidden,
                     l = e.runNb,
                     d = e.url_key,
                     u = Object(i.b)(),
                     b = Object(n.useState)(!1),
-                    p = Object(_.a)(b, 2),
+                    p = Object(R.a)(b, 2),
                     j = p[0],
                     h = p[1],
                     v = Object(c.c)(),
-                    f = Object(_.a)(v, 1)[0];
+                    f = Object(R.a)(v, 1)[0];
                 return Object(n.useEffect)((function() {
                     if (void 0 !== d && "" !== d) {
                         var e, a = null === (e = f.get(d)) || void 0 === e ? void 0 : e.toLowerCase();
                         j || void 0 === a || "true" !== a && "false" !== a || (u(ge({
                             key: t,
                             value: "true" === a
                         })), u(Pe(!0)))
@@ -636,38 +636,38 @@
                     d = e.disabled,
                     u = e.hidden,
                     b = e.runNb,
                     p = e.continuousUpdate,
                     j = e.url_key,
                     h = Object(i.b)(),
                     v = Object(n.useState)(!1),
-                    f = Object(_.a)(v, 2),
+                    f = Object(R.a)(v, 2),
                     m = f[0],
                     x = f[1],
                     O = Object(n.useState)(!1),
-                    g = Object(_.a)(O, 2),
+                    g = Object(R.a)(O, 2),
                     y = g[0],
                     w = g[1],
                     k = 0,
                     N = 10,
                     S = 1;
                 null !== s && (k = s), null !== r && (N = r), null !== l && (S = l);
                 var P = null !== o && void 0 !== o ? o : 0,
-                    C = Object(c.c)(),
-                    T = Object(_.a)(C, 1)[0];
+                    T = Object(c.c)(),
+                    _ = Object(R.a)(T, 1)[0];
                 Object(n.useEffect)((function() {
                     if (void 0 !== j && "" !== j) {
-                        var e = T.get(j);
+                        var e = _.get(j);
                         !y && void 0 !== e && null !== e && !isNaN(parseFloat(e)) && parseFloat(e) >= k && parseFloat(e) <= N && (h(ge({
                             key: t,
                             value: parseFloat(e)
                         })), h(Pe(!0)))
                     }
-                }), [h, N, k, T, y, j, t]);
-                var R = function() {
+                }), [h, N, k, _, y, j, t]);
+                var C = function() {
                     null !== s && null !== o && o < s && h(Oe({
                         key: t,
                         value: s
                     })), null !== r && null !== o && o > r && h(Oe({
                         key: t,
                         value: r
                     }))
@@ -690,18 +690,18 @@
                         onChange: function(e) {
                             w(!0), x(!0), h(Oe({
                                 key: t,
                                 value: e.target.value
                             }))
                         },
                         onBlur: function(e) {
-                            R()
+                            C()
                         },
                         onKeyPress: function(e) {
-                            "Enter" === e.key && (R(), b(), x(!1), e.preventDefault())
+                            "Enter" === e.key && (C(), b(), x(!1), e.preventDefault())
                         },
                         min: k,
                         max: N,
                         step: S,
                         disabled: d
                     }), m && p && Object(E.jsx)("div", {
                         style: {
@@ -709,15 +709,15 @@
                             position: "relative",
                             top: "0px",
                             left: "0px"
                         },
                         children: Object(E.jsx)("button", {
                             className: "btn btn-sm btn-outline-primary",
                             onClick: function(e) {
-                                R(), b(), x(!1), e.preventDefault()
+                                C(), b(), x(!1), e.preventDefault()
                             },
                             style: {
                                 fontSize: "0.7em",
                                 border: "none"
                             },
                             children: "Press enter or click to apply"
                         })
@@ -739,19 +739,19 @@
                     p = e.url_key,
                     j = 0,
                     h = 100,
                     v = 1;
                 s && (j = s), r && (h = r), l && (v = l);
                 var f = Object(i.b)(),
                     m = Object(n.useState)(!1),
-                    x = Object(_.a)(m, 2),
+                    x = Object(R.a)(m, 2),
                     O = x[0],
                     g = x[1],
                     y = Object(c.c)(),
-                    w = Object(_.a)(y, 1)[0];
+                    w = Object(R.a)(y, 1)[0];
                 Object(n.useEffect)((function() {
                     if (void 0 !== p && "" !== p) {
                         var e, a = null === (e = w.get(p)) || void 0 === e ? void 0 : e.split(",").map((function(e) {
                             return parseFloat(e)
                         }));
                         !O && void 0 !== a && 2 === a.length && void 0 !== a[0] && !isNaN(a[0]) && void 0 !== a[1] && !isNaN(a[1]) && a[0] <= a[1] && a[0] >= j && a[1] <= h && (f(ge({
                             key: t,
@@ -795,15 +795,15 @@
                             },
                             renderTrack: function(e) {
                                 var t = e.props,
                                     a = e.children;
                                 return Object(E.jsx)("div", {
                                     onMouseDown: t.onMouseDown,
                                     onTouchStart: t.onTouchStart,
-                                    style: Object(D.a)(Object(D.a)({}, t.style), {}, {
+                                    style: Object(U.a)(Object(U.a)({}, t.style), {}, {
                                         height: "36px",
                                         display: "flex",
                                         width: "100%"
                                     }),
                                     children: Object(E.jsxs)("div", {
                                         ref: t.ref,
                                         style: {
@@ -840,16 +840,16 @@
                                     })
                                 })
                             },
                             renderThumb: function(e) {
                                 var t = e.index,
                                     a = e.props,
                                     n = e.isDragged;
-                                return Object(E.jsxs)("div", Object(D.a)(Object(D.a)({}, a), {}, {
-                                    style: Object(D.a)(Object(D.a)({}, a.style), {}, {
+                                return Object(E.jsxs)("div", Object(U.a)(Object(U.a)({}, a), {}, {
+                                    style: Object(U.a)(Object(U.a)({}, a.style), {}, {
                                         height: "18px",
                                         width: "18px",
                                         border: "None !important",
                                         borderRadius: "4px",
                                         backgroundColor: "#FFF",
                                         display: "flex",
                                         justifyContent: "center",
@@ -893,26 +893,26 @@
                     r = e.multi,
                     l = e.disabled,
                     d = e.hidden,
                     u = e.runNb,
                     b = e.url_key,
                     p = Object(i.b)(),
                     j = Object(n.useState)(!1),
-                    h = Object(_.a)(j, 2),
+                    h = Object(R.a)(j, 2),
                     v = h[0],
                     f = h[1],
                     m = {
                         menu: function(e) {
-                            return Object(D.a)(Object(D.a)({}, e), {}, {
+                            return Object(U.a)(Object(U.a)({}, e), {}, {
                                 zIndex: 100
                             })
                         }
                     },
                     x = Object(c.c)(),
-                    O = Object(_.a)(x, 1)[0];
+                    O = Object(R.a)(x, 1)[0];
                 Object(n.useEffect)((function() {
                     if (void 0 !== b && "" !== b) {
                         var e = O.get(b);
                         if (!v && void 0 !== e && null !== e)
                             if (r) {
                                 var a = e.split(",");
                                 a && (p(ge({
@@ -1006,23 +1006,23 @@
                     l = e.step,
                     d = (e.vertical, e.disabled),
                     u = e.hidden,
                     b = e.runNb,
                     p = e.url_key,
                     j = Object(i.b)(),
                     h = Object(n.useState)(!1),
-                    v = Object(_.a)(h, 2),
+                    v = Object(R.a)(h, 2),
                     f = v[0],
                     m = v[1],
                     x = 0,
                     O = 100,
                     g = 1;
                 s && (x = s), r && (O = r), l && (g = l);
                 var y = Object(c.c)(),
-                    w = Object(_.a)(y, 1)[0];
+                    w = Object(R.a)(y, 1)[0];
                 Object(n.useEffect)((function() {
                     if (void 0 !== p && "" !== p) {
                         var e = w.get(p);
                         !f && void 0 !== e && null !== e && !isNaN(parseFloat(e)) && parseFloat(e) >= x && parseFloat(e) <= O && (j(ge({
                             key: t,
                             value: parseFloat(e)
                         })), j(Pe(!0)))
@@ -1064,15 +1064,15 @@
                             },
                             renderTrack: function(e) {
                                 var t = e.props,
                                     a = e.children;
                                 return Object(E.jsx)("div", {
                                     onMouseDown: t.onMouseDown,
                                     onTouchStart: t.onTouchStart,
-                                    style: Object(D.a)(Object(D.a)({}, t.style), {}, {
+                                    style: Object(U.a)(Object(U.a)({}, t.style), {}, {
                                         height: "36px",
                                         display: "flex",
                                         width: "100%"
                                     }),
                                     children: Object(E.jsxs)("div", {
                                         ref: t.ref,
                                         style: {
@@ -1108,16 +1108,16 @@
                                         })]
                                     })
                                 })
                             },
                             renderThumb: function(e) {
                                 var t = e.props,
                                     a = e.isDragged;
-                                return Object(E.jsxs)("div", Object(D.a)(Object(D.a)({}, t), {}, {
-                                    style: Object(D.a)(Object(D.a)({}, t.style), {}, {
+                                return Object(E.jsxs)("div", Object(U.a)(Object(U.a)({}, t), {}, {
+                                    style: Object(U.a)(Object(U.a)({}, t.style), {}, {
                                         height: "18px",
                                         width: "18px",
                                         border: "None",
                                         borderRadius: "4px",
                                         backgroundColor: "#FFF",
                                         display: "flex",
                                         justifyContent: "center",
@@ -1196,15 +1196,23 @@
                 St = function() {
                     return function() {
                         var e = Object(u.a)(d.a.mark((function e(t) {
                             var a, n, o, i, r;
                             return d.a.wrap((function(e) {
                                 for (;;) switch (e.prev = e.next) {
                                     case 0:
-                                        return e.prev = 0, t(Ot({})), t(gt(ct.Unknown)), a = "single-site", a = window.location.host.split(":")[0], window.location.origin.endsWith("hf.space") && (a = "localhost"), n = "/api/v1/get-site/".concat(a, "/"), e.next = 9, s.a.get(n);
+                                        return e.prev = 0, t(Ot({})), t(gt(ct.Unknown)), a = "single-site", Object({
+                                            NODE_ENV: "production",
+                                            PUBLIC_URL: "",
+                                            WDS_SOCKET_HOST: void 0,
+                                            WDS_SOCKET_PATH: void 0,
+                                            WDS_SOCKET_PORT: void 0,
+                                            FAST_REFRESH: !0,
+                                            REACT_APP_LOCAL_URL: "/static"
+                                        }).REACT_APP_SERVER_URL && (a = window.location.host.split(":")[0]), window.location.origin.endsWith("hf.space") && (a = "localhost"), n = "/api/v1/get-site/".concat(a, "/"), e.next = 9, s.a.get(n);
                                     case 9:
                                         o = e.sent, i = o.data, t(Ot(i)), "Ready" !== (null === i || void 0 === i ? void 0 : i.status) ? t(gt(ct.NotReady)) : t(gt(ct.Loaded)), e.next = 20;
                                         break;
                                     case 15:
                                         e.prev = 15, e.t0 = e.catch(0), r = e.t0, console.log(r.message), "Network Error" === (null === r || void 0 === r ? void 0 : r.message) ? t(gt(ct.NetworkError)) : 403 === r.response.status ? t(gt(ct.AccessForbidden)) : 404 === r.response.status ? t(gt(ct.NotFound)) : 401 === r.response.status ? (t(N("")), t(S("")), t(gt(ct.PleaseRefresh))) : console.error("Problem during loading site information. ".concat(e.t0));
                                     case 20:
                                     case "end":
@@ -1226,15 +1234,15 @@
                     o = e.maxFileSize,
                     r = e.disabled,
                     c = e.hidden,
                     l = e.value,
                     b = e.runNb,
                     j = Object(i.b)(),
                     h = Object(n.useState)(!1),
-                    v = Object(_.a)(h, 2),
+                    v = Object(R.a)(h, 2),
                     m = v[0],
                     x = v[1],
                     O = Object(i.c)(Q),
                     g = Object(i.c)(wt),
                     y = Object(i.c)(f),
                     w = "100MB";
                 o && (w = o), Object(n.useEffect)((function() {
@@ -1244,15 +1252,15 @@
                         var e = Object(u.a)(d.a.mark((function e(t) {
                             var a, n;
                             return d.a.wrap((function(e) {
                                 for (;;) switch (e.prev = e.next) {
                                     case 0:
                                         return e.prev = 0, e.next = 4, s.a.get("/api/v1/storage-type");
                                     case 4:
-                                        a = e.sent, n = a.data, t(J(n.storage_type)), e.next = 12;
+                                        a = e.sent, n = a.data, t(K(n.storage_type)), e.next = 12;
                                         break;
                                     case 9:
                                         e.prev = 9, e.t0 = e.catch(0), console.error("Get storage type error. ".concat(e.t0));
                                     case 12:
                                     case "end":
                                         return e.stop()
                                 }
@@ -1402,39 +1410,39 @@
                             server: "media" === O ? k : N,
                             labelIdle: 'Drag & Drop your file or <span class="filepond--label-action">Browse</span>'
                         })
                     })]
                 })
             }
 
-            function Ct(e) {
+            function Tt(e) {
                 var t = e.widgetKey,
                     a = e.label,
                     o = e.value,
                     s = e.rows,
                     r = e.disabled,
                     l = e.hidden,
                     d = e.runNb,
                     u = e.continuousUpdate,
                     b = e.url_key,
                     p = Object(i.b)(),
                     j = Object(n.useState)(!1),
-                    h = Object(_.a)(j, 2),
+                    h = Object(R.a)(j, 2),
                     v = h[0],
                     f = h[1],
                     m = Object(n.useState)(!1),
-                    x = Object(_.a)(m, 2),
+                    x = Object(R.a)(m, 2),
                     O = x[0],
                     g = x[1],
                     y = s || 1,
                     w = function(e) {
                         return e.replace(/["'(){}[\]`^]/gim, "")
                     },
                     k = Object(c.c)(),
-                    N = Object(_.a)(k, 1)[0];
+                    N = Object(R.a)(k, 1)[0];
                 return Object(n.useEffect)((function() {
                     if (void 0 !== b && "" !== b) {
                         var e = N.get(b);
                         O || void 0 === e || null === e || (p(ge({
                             key: t,
                             value: e
                         })), p(Pe(!0)))
@@ -1513,49 +1521,49 @@
                             },
                             children: "Apply"
                         })
                     })]
                 })
             }
             Object(lt.registerPlugin)(ut.a, pt.a, ht.a);
-            var Tt, Rt, _t = a(312),
+            var _t, Ct, Rt = a(312),
                 Et = a(314),
-                Ft = a(87),
-                At = a(90),
-                Mt = a(88);
+                At = a(87),
+                Lt = a(90),
+                Dt = a(88);
 
-            function Dt(e) {
+            function Ut(e) {
                 var t = e.value,
                     a = e.disabled;
                 return Object(E.jsx)("div", {
                     className: "form-group mb-3",
                     style: {
                         color: a ? "#555" : "#212529"
                     },
-                    children: Object(E.jsx)(_t.a, {
-                        rehypePlugins: [Ft.a, Et.a, At.a, Mt.a],
+                    children: Object(E.jsx)(Rt.a, {
+                        rehypePlugins: [At.a, Et.a, Lt.a, Dt.a],
                         children: t
                     })
                 })
             }! function(e) {
                 e.Connecting = "Connecting", e.Connected = "Connected", e.Unknown = "Unknown", e.Disconnected = "Disconnected"
-            }(Tt || (Tt = {})),
+            }(_t || (_t = {})),
             function(e) {
                 e.Unknown = "Unknown", e.Starting = "Starting", e.Running = "Running", e.Missing = "Missing", e.Busy = "Busy", e.Queued = "Queued", e.MaxRunTimeReached = "MaxRunTimeReached", e.MaxIdleTimeReached = "MaxIdleTimeReached", e.UsageLimitReached = "UsageLimitReached"
-            }(Rt || (Rt = {}));
-            var It = {
-                    webSocketState: Tt.Unknown,
-                    workerState: Rt.Unknown,
+            }(Ct || (Ct = {}));
+            var Ft = {
+                    webSocketState: _t.Unknown,
+                    workerState: Ct.Unknown,
                     workerId: void 0,
                     notebookSrc: "",
                     tryConnectCount: 0
                 },
-                Lt = Object(b.b)({
+                Wt = Object(b.b)({
                     name: "ws",
-                    initialState: It,
+                    initialState: Ft,
                     reducers: {
                         setWebSocketState: function(e, t) {
                             e.webSocketState = t.payload
                         },
                         setWorkerState: function(e, t) {
                             e.workerState = t.payload
                         },
@@ -1569,22 +1577,22 @@
                             e.tryConnectCount += 1
                         },
                         resetTryConnectCount: function(e) {
                             e.tryConnectCount = 0
                         }
                     }
                 }),
-                Ut = Lt.reducer,
-                Wt = Lt.actions,
-                Ht = Wt.setWebSocketState,
-                zt = Wt.setWorkerState,
-                Bt = Wt.setWorkerId,
-                Vt = Wt.setNotebookSrc,
-                Jt = Wt.increaseTryConnectCount,
-                Kt = Wt.resetTryConnectCount,
+                It = Wt.reducer,
+                Mt = Wt.actions,
+                Ht = Mt.setWebSocketState,
+                Bt = Mt.setWorkerState,
+                Vt = Mt.setWorkerId,
+                zt = Mt.setNotebookSrc,
+                Kt = Mt.increaseTryConnectCount,
+                Jt = Mt.resetTryConnectCount,
                 qt = function(e) {
                     return e.ws.webSocketState
                 },
                 Yt = function(e) {
                     return e.ws.workerState
                 },
                 Gt = function(e) {
@@ -1601,25 +1609,41 @@
                         purpose: "run-notebook",
                         widgets: e
                     }
                 },
                 $t = Object(n.createContext)(void 0),
                 ea = "ws://127.0.0.1:8000",
                 ta = !0;
-            ea = "ws://localhost:8000", ta = !1, window.location.origin.endsWith("hf.space") && (ea = window.location.origin.replace("http://", "ws://").replace("https://", "wss://"), ta = !1);
+            Object({
+                NODE_ENV: "production",
+                PUBLIC_URL: "",
+                WDS_SOCKET_HOST: void 0,
+                WDS_SOCKET_PATH: void 0,
+                WDS_SOCKET_PORT: void 0,
+                FAST_REFRESH: !0,
+                REACT_APP_LOCAL_URL: "/static"
+            }).REACT_APP_SERVER_WS ? (ea = Object({
+                NODE_ENV: "production",
+                PUBLIC_URL: "",
+                WDS_SOCKET_HOST: void 0,
+                WDS_SOCKET_PATH: void 0,
+                WDS_SOCKET_PORT: void 0,
+                FAST_REFRESH: !0,
+                REACT_APP_LOCAL_URL: "/static"
+            }).REACT_APP_SERVER_WS, ta = !1) : "http://localhost:3000" === window.location.origin ? (ea = "ws://127.0.0.1:8000", ta = !0) : (ea = window.location.origin.replace("http://", "ws://").replace("https://", "wss://"), ta = !1), window.location.origin.endsWith("hf.space") && (ea = window.location.origin.replace("http://", "ws://").replace("https://", "wss://"), ta = !1);
             var aa = 0,
                 na = void 0;
 
             function oa(e) {
                 var t = e.children;
                 console.log("WebSocketProvider");
                 var a = Object(i.b)(),
                     o = Object(i.c)(wt),
-                    r = Object(i.c)(_e),
-                    c = Object(i.c)(C),
+                    r = Object(i.c)(Re),
+                    c = Object(i.c)(T),
                     l = Object(i.c)(Ee),
                     b = void 0,
                     p = "Unknown";
                 Object(n.useEffect)((function() {
                     return aa = 0,
                         function() {
                             var e;
@@ -1627,35 +1651,35 @@
                         }
                 }), []);
                 var j = function(e) {
                     void 0 !== b && b.readyState === b.OPEN && b.send(e)
                 };
 
                 function h(e) {
-                    a(Kt()), j(JSON.stringify({
+                    a(Jt()), j(JSON.stringify({
                         purpose: "server-address",
                         address: ea
-                    })), a(Ht(Tt.Connected)), g()
+                    })), a(Ht(_t.Connected)), g()
                 }
 
                 function v(e) {
                     var t, n = JSON.parse(e.data);
-                    "purpose" in n && ("worker-state" === n.purpose ? (console.log("worker-state", n.state), p = n.state, a(zt(n.state)), a(Bt(n.workerId)), (p === Rt.MaxIdleTimeReached || p === Rt.MaxRunTimeReached) && (null === (t = b) || void 0 === t || t.close())) : "executed-notebook" === n.purpose ? ((null === n || void 0 === n ? void 0 : n.reloadNotebook) && void 0 !== r && a(function(e, t) {
+                    "purpose" in n && ("worker-state" === n.purpose ? (console.log("worker-state", n.state), p = n.state, a(Bt(n.state)), a(Vt(n.workerId)), (p === Ct.MaxIdleTimeReached || p === Ct.MaxRunTimeReached) && (null === (t = b) || void 0 === t || t.close())) : "executed-notebook" === n.purpose ? ((null === n || void 0 === n ? void 0 : n.reloadNotebook) && void 0 !== r && a(function(e, t) {
                         var a = arguments.length > 2 && void 0 !== arguments[2] && arguments[2];
                         return function() {
                             var n = Object(u.a)(d.a.mark((function n(o) {
                                 var i, r, c, l, u, b;
                                 return d.a.wrap((function(n) {
                                     for (;;) switch (n.prev = n.next) {
                                         case 0:
-                                            return n.prev = 0, a || (o(fe("")), o(qe())), i = ce(), r = i.width, o(V(r > 992)), a || o(ve("loading")), c = "/api/v1/".concat(e, "/notebooks/").concat(t, "/"), n.next = 8, s.a.get(c);
+                                            return n.prev = 0, a || (o(fe("")), o(qe())), i = ce(), r = i.width, o(z(r > 992)), a || o(ve("loading")), c = "/api/v1/".concat(e, "/notebooks/").concat(t, "/"), n.next = 8, s.a.get(c);
                                         case 8:
-                                            l = n.sent, u = l.data, b = JSON.parse(u.params), o(he(Object(D.a)(Object(D.a)({}, u), {}, {
+                                            l = n.sent, u = l.data, b = JSON.parse(u.params), o(he(Object(U.a)(Object(U.a)({}, u), {}, {
                                                 params: b
-                                            }))), a || o(ve("loaded")), null !== (null === b || void 0 === b ? void 0 : b.show_sidebar) && void 0 !== (null === b || void 0 === b ? void 0 : b.show_sidebar) && o(V(null === b || void 0 === b ? void 0 : b.show_sidebar)), n.next = 20;
+                                            }))), a || o(ve("loaded")), null !== (null === b || void 0 === b ? void 0 : b.show_sidebar) && void 0 !== (null === b || void 0 === b ? void 0 : b.show_sidebar) && o(z(null === b || void 0 === b ? void 0 : b.show_sidebar)), n.next = 20;
                                             break;
                                         case 16:
                                             n.prev = 16, n.t0 = n.catch(0), a || o(ve("error")), console.error("Problem during loading selected notebook (".concat(t, "). ").concat(n.t0));
                                         case 20:
                                         case "end":
                                             return n.stop()
                                     }
@@ -1663,38 +1687,38 @@
                                     [0, 16]
                                 ])
                             })));
                             return function(e) {
                                 return n.apply(this, arguments)
                             }
                         }()
-                    }(o, r)), a(Vt(n.body))) : "update-widgets" === n.purpose ? a(me(n)) : "hide-widgets" === n.purpose ? a(xe(n)) : "init-widgets" === n.purpose ? (a(we(n)), a(Se(!0))) : "update-title" === n.purpose ? a(ke(n.title)) : "update-show-code" === n.purpose ? a(Ne(n.showCode)) : "download-html" !== n.purpose && "download-pdf" !== n.purpose || n.url && n.filename && (a(ze(!1)), x(n.url, n.filename)))
+                    }(o, r)), a(zt(n.body))) : "update-widgets" === n.purpose ? a(me(n)) : "hide-widgets" === n.purpose ? a(xe(n)) : "init-widgets" === n.purpose ? (a(we(n)), a(Se(!0))) : "update-title" === n.purpose ? a(ke(n.title)) : "update-show-code" === n.purpose ? a(Ne(n.showCode)) : "download-html" !== n.purpose && "download-pdf" !== n.purpose || n.url && n.filename && (a(Be(!1)), x(n.url, n.filename)))
                 }
 
                 function m(e) {
-                    a(Ht(Tt.Disconnected)), a(zt(Rt.Unknown))
+                    a(Ht(_t.Disconnected)), a(Bt(Ct.Unknown))
                 }
 
                 function O(e) {
-                    a(Ht(Tt.Disconnected)), b = void 0, p !== Rt.MaxIdleTimeReached && p !== Rt.MaxRunTimeReached && (a(zt(Rt.Unknown)), a(Bt(void 0)), aa < 5 && setTimeout((function() {
+                    a(Ht(_t.Disconnected)), b = void 0, p !== Ct.MaxIdleTimeReached && p !== Ct.MaxRunTimeReached && (a(Bt(Ct.Unknown)), a(Vt(void 0)), aa < 5 && setTimeout((function() {
                         return y()
                     }), 5e3))
                 }
 
                 function g() {
                     j(JSON.stringify({
                         purpose: "worker-ping"
                     })), void 0 !== b && b.readyState === b.OPEN && setTimeout((function() {
                         return g()
                     }), 1e4)
                 }
 
                 function y() {
-                    if ((ta || !l) && void 0 !== r && void 0 === b && p !== Rt.MaxIdleTimeReached && p !== Rt.MaxRunTimeReached && aa < 5) {
-                        console.log("WS connect ..." + p + " " + aa), a(Jt());
+                    if ((ta || !l) && void 0 !== r && void 0 === b && p !== Ct.MaxIdleTimeReached && p !== Ct.MaxRunTimeReached && aa < 5) {
+                        console.log("WS connect ..." + p + " " + aa), a(Kt());
                         var e = "".concat(ea, "/ws/client/").concat(r, "/").concat(f(), "/");
                         void 0 !== c && null !== c && "" !== c && (e += "?token=".concat(c)), (b = new WebSocket(e)).onopen = h, b.onmessage = v, b.onerror = m, b.onclose = O, na = b, (aa += 1) >= 5 && a(gt(ct.NetworkError))
                     }
                 }
                 y();
                 var w = {
                     sendMessage: j
@@ -1714,50 +1738,50 @@
                     l = e.notebookTitle,
                     b = e.runDownloadHTML,
                     j = e.runDownloadPDF,
                     h = e.widgetsValues,
                     v = e.widgetsParams,
                     m = Object(i.b)(),
                     O = Object(n.useState)(!1),
-                    g = Object(_.a)(O, 2),
+                    g = Object(R.a)(O, 2),
                     y = g[0],
                     w = g[1],
                     k = Object(i.c)(qt),
                     N = Object(i.c)(Yt),
                     S = Object(i.c)(Zt);
                 Object(n.useEffect)((function() {
                     S >= 5 && m(gt(ct.LostConnection))
                 }), [m, S]);
                 var P = "orange";
-                k === Tt.Connected ? P = "green" : k !== Tt.Disconnected && k !== Tt.Unknown || (P = "red");
-                var C = "orange";
-                N === Rt.Running || N === Rt.Busy ? C = "green" : N !== Rt.Missing && N !== Rt.Unknown || (C = "red");
-                var T = !0,
-                    R = "?";
+                k === _t.Connected ? P = "green" : k !== _t.Disconnected && k !== _t.Unknown || (P = "red");
+                var T = "orange";
+                N === Ct.Running || N === Ct.Busy ? T = "green" : N !== Ct.Missing && N !== Ct.Unknown || (T = "red");
+                var _ = !0,
+                    C = "?";
                 if (void 0 !== v && null !== v && void 0 !== h && null !== h) {
-                    for (var F = 0, A = Object.entries(v); F < A.length; F++) {
-                        var M = Object(_.a)(A[F], 2),
-                            D = M[0],
-                            I = M[1];
-                        if (void 0 !== h[D]) {
-                            if (($(I) || ee(I) || ae(I) || X(I) || te(I) || oe(I)) && null !== (null === I || void 0 === I ? void 0 : I.url_key) && "" !== (null === I || void 0 === I ? void 0 : I.url_key) && (T = !1), ($(I) || ee(I) || te(I) || oe(I)) && null !== (null === I || void 0 === I ? void 0 : I.url_key) && "" !== (null === I || void 0 === I ? void 0 : I.url_key) && (R += "".concat(null === I || void 0 === I ? void 0 : I.url_key, "=").concat(h[D], "&")), ae(I) && null !== (null === I || void 0 === I ? void 0 : I.url_key) && "" !== (null === I || void 0 === I ? void 0 : I.url_key)) {
-                                var L = h[D];
-                                R += "".concat(null === I || void 0 === I ? void 0 : I.url_key, "=").concat(L[0], ",").concat(L[1], "&")
+                    for (var A = 0, L = Object.entries(v); A < L.length; A++) {
+                        var D = Object(R.a)(L[A], 2),
+                            U = D[0],
+                            F = D[1];
+                        if (void 0 !== h[U]) {
+                            if (($(F) || ee(F) || ae(F) || X(F) || te(F) || oe(F)) && null !== (null === F || void 0 === F ? void 0 : F.url_key) && "" !== (null === F || void 0 === F ? void 0 : F.url_key) && (_ = !1), ($(F) || ee(F) || te(F) || oe(F)) && null !== (null === F || void 0 === F ? void 0 : F.url_key) && "" !== (null === F || void 0 === F ? void 0 : F.url_key) && (C += "".concat(null === F || void 0 === F ? void 0 : F.url_key, "=").concat(h[U], "&")), ae(F) && null !== (null === F || void 0 === F ? void 0 : F.url_key) && "" !== (null === F || void 0 === F ? void 0 : F.url_key)) {
+                                var W = h[U];
+                                C += "".concat(null === F || void 0 === F ? void 0 : F.url_key, "=").concat(W[0], ",").concat(W[1], "&")
                             }
-                            if (X(I) && null !== (null === I || void 0 === I ? void 0 : I.url_key) && "" !== (null === I || void 0 === I ? void 0 : I.url_key))
-                                if (null === I || void 0 === I ? void 0 : I.multi) {
-                                    var U = h[D];
-                                    R += "".concat(null === I || void 0 === I ? void 0 : I.url_key, "=").concat(U.join(","), "&")
+                            if (X(F) && null !== (null === F || void 0 === F ? void 0 : F.url_key) && "" !== (null === F || void 0 === F ? void 0 : F.url_key))
+                                if (null === F || void 0 === F ? void 0 : F.multi) {
+                                    var I = h[U];
+                                    C += "".concat(null === F || void 0 === F ? void 0 : F.url_key, "=").concat(I.join(","), "&")
                                 } else {
-                                    var W = h[D];
-                                    R += "".concat(null === I || void 0 === I ? void 0 : I.url_key, "=").concat(W, "&")
+                                    var M = h[U];
+                                    C += "".concat(null === F || void 0 === F ? void 0 : F.url_key, "=").concat(M, "&")
                                 }
                         }
                     }
-                    "?" !== R && (R = R.slice(0, R.length - 1))
+                    "?" !== C && (C = C.slice(0, C.length - 1))
                 }
                 return Object(E.jsxs)("div", {
                     style: {
                         paddingBottom: "25px"
                     },
                     children: [void 0 !== r && !o && Object(E.jsxs)(E.Fragment, {
                         children: [Object(E.jsx)("span", {
@@ -1777,23 +1801,23 @@
                             })
                         }), " ", Object(E.jsx)("span", {
                             title: "Worker: ".concat(N, "\nSession Id: ").concat(f()),
                             children: Object(E.jsx)("svg", {
                                 xmlns: "http://www.w3.org/2000/svg",
                                 width: "16",
                                 height: "16",
-                                fill: C,
+                                fill: T,
                                 className: "bi bi-cpu",
                                 viewBox: "0 0 16 16",
                                 children: Object(E.jsx)("path", {
                                     d: "M5 0a.5.5 0 0 1 .5.5V2h1V.5a.5.5 0 0 1 1 0V2h1V.5a.5.5 0 0 1 1 0V2h1V.5a.5.5 0 0 1 1 0V2A2.5 2.5 0 0 1 14 4.5h1.5a.5.5 0 0 1 0 1H14v1h1.5a.5.5 0 0 1 0 1H14v1h1.5a.5.5 0 0 1 0 1H14v1h1.5a.5.5 0 0 1 0 1H14a2.5 2.5 0 0 1-2.5 2.5v1.5a.5.5 0 0 1-1 0V14h-1v1.5a.5.5 0 0 1-1 0V14h-1v1.5a.5.5 0 0 1-1 0V14h-1v1.5a.5.5 0 0 1-1 0V14A2.5 2.5 0 0 1 2 11.5H.5a.5.5 0 0 1 0-1H2v-1H.5a.5.5 0 0 1 0-1H2v-1H.5a.5.5 0 0 1 0-1H2v-1H.5a.5.5 0 0 1 0-1H2A2.5 2.5 0 0 1 4.5 2V.5A.5.5 0 0 1 5 0zm-.5 3A1.5 1.5 0 0 0 3 4.5v7A1.5 1.5 0 0 0 4.5 13h7a1.5 1.5 0 0 0 1.5-1.5v-7A1.5 1.5 0 0 0 11.5 3h-7zM5 6.5A1.5 1.5 0 0 1 6.5 5h3A1.5 1.5 0 0 1 11 6.5v3A1.5 1.5 0 0 1 9.5 11h-3A1.5 1.5 0 0 1 5 9.5v-3zM6.5 6a.5.5 0 0 0-.5.5v3a.5.5 0 0 0 .5.5h3a.5.5 0 0 0 .5-.5v-3a.5.5 0 0 0-.5-.5h-3z"
                                 })
                             })
                         })]
-                    }), N === Rt.Busy && Object(E.jsxs)("span", {
+                    }), N === Ct.Busy && Object(E.jsxs)("span", {
                         title: "Worker is busy",
                         children: [" ", Object(E.jsx)("svg", {
                             xmlns: "http://www.w3.org/2000/svg",
                             width: "16",
                             height: "16",
                             fill: "green",
                             className: "bi bi-activity",
@@ -1871,37 +1895,37 @@
                                             o ? m(function(e, t) {
                                                 return function() {
                                                     var a = Object(u.a)(d.a.mark((function a(n) {
                                                         var o, i, r, c;
                                                         return d.a.wrap((function(a) {
                                                             for (;;) switch (a.prev = a.next) {
                                                                 case 0:
-                                                                    return a.prev = 0, n(ze(!0)), n(Ve()), n(Be("")), o = f(), i = {
+                                                                    return a.prev = 0, n(Be(!0)), n(ze()), n(Ve("")), o = f(), i = {
                                                                         session_id: o,
                                                                         notebook_id: e,
                                                                         notebook_path: t
                                                                     }, a.next = 9, s.a.post("/api/v1/export_pdf/", i);
                                                                 case 9:
-                                                                    r = a.sent, c = r.data, n(Be(c.job_id)), a.next = 18;
+                                                                    r = a.sent, c = r.data, n(Ve(c.job_id)), a.next = 18;
                                                                     break;
                                                                 case 14:
-                                                                    a.prev = 14, a.t0 = a.catch(0), p.b.error("The error occured during PDF export. ".concat(a.t0)), n(Ke());
+                                                                    a.prev = 14, a.t0 = a.catch(0), p.b.error("The error occured during PDF export. ".concat(a.t0)), n(Je());
                                                                 case 18:
                                                                 case "end":
                                                                     return a.stop()
                                                             }
                                                         }), a, null, [
                                                             [0, 14]
                                                         ])
                                                     })));
                                                     return function(e) {
                                                         return a.apply(this, arguments)
                                                     }
                                                 }()
-                                            }(r, c)) : (m(ze(!0)), j())
+                                            }(r, c)) : (m(Be(!0)), j())
                                         },
                                         children: [Object(E.jsx)("i", {
                                             className: "fa fa-file-pdf-o",
                                             "aria-hidden": "true"
                                         }), " ", "Download as PDF"]
                                     })
                                 })]
@@ -2010,25 +2034,25 @@
                                                 children: "App address"
                                             }), Object(E.jsx)("input", {
                                                 type: "text",
                                                 className: "form-control",
                                                 disabled: !0,
                                                 value: window.location.href
                                             })]
-                                        }), !T && Object(E.jsxs)("div", {
+                                        }), !_ && Object(E.jsxs)("div", {
                                             className: "py-2",
                                             children: [Object(E.jsx)("label", {
                                                 children: "App address with current paramters"
                                             }), Object(E.jsx)("textarea", {
                                                 rows: 5,
                                                 className: "form-control",
                                                 disabled: !0,
-                                                value: window.location.href + R
+                                                value: window.location.href + C
                                             })]
-                                        }), T && Object(E.jsxs)("div", {
+                                        }), _ && Object(E.jsxs)("div", {
                                             className: "py-2",
                                             children: ["There are no ", Object(E.jsx)("code", {
                                                 children: "url_key"
                                             }), " defined for any widget. You can easily share URL to your notebook with preset values by using ", Object(E.jsx)("code", {
                                                 children: "url_key"
                                             }), " in the widget. Please check", " ", Object(E.jsx)("a", {
                                                 href: "https://runmercury.com/docs/input-widgets/",
@@ -2103,34 +2127,34 @@
                     style: {
                         marginRight: "10px",
                         width: "100%"
                     },
                     onClick: function() {
                         t()
                     },
-                    disabled: a || n !== Rt.Running,
-                    children: [n === Rt.Running && Object(E.jsxs)("span", {
+                    disabled: a || n !== Ct.Running,
+                    children: [n === Ct.Running && Object(E.jsxs)("span", {
                         children: [Object(E.jsx)("i", {
                             className: "fa fa-play",
                             "aria-hidden": "true"
                         }), " Run"]
-                    }), n === Rt.Busy && Object(E.jsxs)("span", {
+                    }), n === Ct.Busy && Object(E.jsxs)("span", {
                         children: [Object(E.jsx)("svg", {
                             xmlns: "http://www.w3.org/2000/svg",
                             width: "16",
                             height: "16",
                             fill: "white",
                             className: "bi bi-activity",
                             viewBox: "0 0 16 16",
                             children: Object(E.jsx)("path", {
                                 fillRule: "evenodd",
                                 d: "M6 2a.5.5 0 0 1 .47.33L10 12.036l1.53-4.208A.5.5 0 0 1 12 7.5h3.5a.5.5 0 0 1 0 1h-3.15l-1.88 5.17a.5.5 0 0 1-.94 0L6 3.964 4.47 8.171A.5.5 0 0 1 4 8.5H.5a.5.5 0 0 1 0-1h3.15l1.88-5.17A.5.5 0 0 1 6 2Z"
                             })
                         }), " ", "Busy"]
-                    }), n !== Rt.Busy && n !== Rt.Running && Object(E.jsx)("span", {
+                    }), n !== Ct.Busy && n !== Ct.Running && Object(E.jsx)("span", {
                         children: "Waiting ..."
                     })]
                 })
             }
             var ca = a(49);
 
             function la(e) {
@@ -2143,28 +2167,28 @@
                     l = e.displayEmbed,
                     d = e.showFiles,
                     u = e.isPresentation,
                     b = (e.notebookParseErrors, e.continuousUpdate),
                     p = e.staticNotebook,
                     j = e.allowDownload,
                     h = Object(i.b)(),
-                    v = Object(i.c)(Me),
-                    f = Object(i.c)(De),
+                    v = Object(i.c)(De),
+                    f = Object(i.c)(Ue),
                     m = Object(i.c)(Yt),
-                    x = Object(i.c)(Ie),
-                    O = Object(i.c)(Le),
+                    x = Object(i.c)(Fe),
+                    O = Object(i.c)(We),
                     g = Object(n.useContext)($t),
                     y = function() {
                         b && w()
                     },
                     w = function() {
                         var e = et();
                         if (h(fe(e)), f) {
                             for (var t = {}, a = 0, n = Object.entries(s); a < n.length; a++) {
-                                var o = Object(_.a)(n[a], 2),
+                                var o = Object(R.a)(n[a], 2),
                                     i = o[0];
                                 o[1];
                                 i in f ? (t[i] = f[i], h(Oe({
                                     key: i,
                                     value: t[i]
                                 }))) : i in v && (t[i] = v[i])
                             }
@@ -2173,15 +2197,15 @@
                     };
                 Object(n.useEffect)((function() {
                     x && O && (w(), h(Pe(!1)), h(Se(!1)))
                 }), [x, O]);
                 Object(n.useEffect)((function() {
                     if (s)
                         for (var e = 0, t = Object.entries(s); e < t.length; e++) {
-                            var a = Object(_.a)(t[e], 2),
+                            var a = Object(R.a)(t[e], 2),
                                 n = a[0],
                                 o = a[1];
                             n in v || ("file" === o.input ? h(Oe({
                                 key: n,
                                 value: []
                             })) : "text" === o.input ? h(Oe({
                                 key: n,
@@ -2194,120 +2218,120 @@
                                 value: o.value
                             }))))
                         }
                 }), [h, s, v]);
                 var k = [],
                     N = [];
                 if (s && !p) {
-                    for (var S = [], P = 0, C = Object.keys(s); P < C.length; P++) {
-                        var T = C[P],
-                            R = T.split(".");
-                        S.push([T, parseFloat("".concat(R[1], ".").concat(R[2]))])
+                    for (var S = [], P = 0, T = Object.keys(s); P < T.length; P++) {
+                        var _ = T[P],
+                            C = _.split(".");
+                        S.push([_, parseFloat("".concat(C[1], ".").concat(C[2]))])
                     }
                     S.sort((function(e, t) {
                         return e[1] - t[1]
                     }));
-                    for (var F = 0, A = S; F < A.length; F++) {
-                        var M = A[F][0],
-                            I = s[M];
-                        X(I) ? k.push(Object(E.jsx)(it, {
-                            widgetKey: M,
-                            disabled: o || (null === I || void 0 === I ? void 0 : I.disabled),
-                            hidden: null === I || void 0 === I ? void 0 : I.hidden,
-                            label: null === I || void 0 === I ? void 0 : I.label,
-                            value: v[M],
-                            choices: null === I || void 0 === I ? void 0 : I.choices,
-                            multi: null === I || void 0 === I ? void 0 : I.multi,
+                    for (var A = 0, L = S; A < L.length; A++) {
+                        var D = L[A][0],
+                            F = s[D];
+                        X(F) ? k.push(Object(E.jsx)(it, {
+                            widgetKey: D,
+                            disabled: o || (null === F || void 0 === F ? void 0 : F.disabled),
+                            hidden: null === F || void 0 === F ? void 0 : F.hidden,
+                            label: null === F || void 0 === F ? void 0 : F.label,
+                            value: v[D],
+                            choices: null === F || void 0 === F ? void 0 : F.choices,
+                            multi: null === F || void 0 === F ? void 0 : F.multi,
                             runNb: y,
-                            url_key: null === I || void 0 === I ? void 0 : I.url_key
-                        }, M)) : $(I) ? k.push(Object(E.jsx)(tt, {
-                            widgetKey: M,
-                            disabled: o || (null === I || void 0 === I ? void 0 : I.disabled),
-                            hidden: null === I || void 0 === I ? void 0 : I.hidden,
-                            label: null === I || void 0 === I ? void 0 : I.label,
-                            value: v[M],
+                            url_key: null === F || void 0 === F ? void 0 : F.url_key
+                        }, D)) : $(F) ? k.push(Object(E.jsx)(tt, {
+                            widgetKey: D,
+                            disabled: o || (null === F || void 0 === F ? void 0 : F.disabled),
+                            hidden: null === F || void 0 === F ? void 0 : F.hidden,
+                            label: null === F || void 0 === F ? void 0 : F.label,
+                            value: v[D],
                             runNb: y,
-                            url_key: null === I || void 0 === I ? void 0 : I.url_key
-                        }, M)) : ee(I) ? k.push(Object(E.jsx)(at, {
-                            widgetKey: M,
-                            disabled: o || (null === I || void 0 === I ? void 0 : I.disabled),
-                            hidden: null === I || void 0 === I ? void 0 : I.hidden,
-                            label: null === I || void 0 === I ? void 0 : I.label,
-                            value: v[M],
-                            min: null === I || void 0 === I ? void 0 : I.min,
-                            max: null === I || void 0 === I ? void 0 : I.max,
-                            step: null === I || void 0 === I ? void 0 : I.step,
+                            url_key: null === F || void 0 === F ? void 0 : F.url_key
+                        }, D)) : ee(F) ? k.push(Object(E.jsx)(at, {
+                            widgetKey: D,
+                            disabled: o || (null === F || void 0 === F ? void 0 : F.disabled),
+                            hidden: null === F || void 0 === F ? void 0 : F.hidden,
+                            label: null === F || void 0 === F ? void 0 : F.label,
+                            value: v[D],
+                            min: null === F || void 0 === F ? void 0 : F.min,
+                            max: null === F || void 0 === F ? void 0 : F.max,
+                            step: null === F || void 0 === F ? void 0 : F.step,
                             runNb: y,
                             continuousUpdate: b,
-                            url_key: null === I || void 0 === I ? void 0 : I.url_key
-                        }, M)) : te(I) ? k.push(Object(E.jsx)(rt, {
-                            widgetKey: M,
-                            disabled: o || (null === I || void 0 === I ? void 0 : I.disabled),
-                            hidden: null === I || void 0 === I ? void 0 : I.hidden,
-                            label: null === I || void 0 === I ? void 0 : I.label,
-                            value: v[M],
-                            min: null === I || void 0 === I ? void 0 : I.min,
-                            max: null === I || void 0 === I ? void 0 : I.max,
-                            step: null === I || void 0 === I ? void 0 : I.step,
-                            vertical: null === I || void 0 === I ? void 0 : I.vertical,
+                            url_key: null === F || void 0 === F ? void 0 : F.url_key
+                        }, D)) : te(F) ? k.push(Object(E.jsx)(rt, {
+                            widgetKey: D,
+                            disabled: o || (null === F || void 0 === F ? void 0 : F.disabled),
+                            hidden: null === F || void 0 === F ? void 0 : F.hidden,
+                            label: null === F || void 0 === F ? void 0 : F.label,
+                            value: v[D],
+                            min: null === F || void 0 === F ? void 0 : F.min,
+                            max: null === F || void 0 === F ? void 0 : F.max,
+                            step: null === F || void 0 === F ? void 0 : F.step,
+                            vertical: null === F || void 0 === F ? void 0 : F.vertical,
                             runNb: y,
-                            url_key: null === I || void 0 === I ? void 0 : I.url_key
-                        }, M)) : ae(I) ? k.push(Object(E.jsx)(ot, {
-                            widgetKey: M,
-                            disabled: o || (null === I || void 0 === I ? void 0 : I.disabled),
-                            hidden: null === I || void 0 === I ? void 0 : I.hidden,
-                            label: null === I || void 0 === I ? void 0 : I.label,
-                            value: v[M],
-                            min: null === I || void 0 === I ? void 0 : I.min,
-                            max: null === I || void 0 === I ? void 0 : I.max,
-                            step: null === I || void 0 === I ? void 0 : I.step,
-                            vertical: null === I || void 0 === I ? void 0 : I.vertical,
+                            url_key: null === F || void 0 === F ? void 0 : F.url_key
+                        }, D)) : ae(F) ? k.push(Object(E.jsx)(ot, {
+                            widgetKey: D,
+                            disabled: o || (null === F || void 0 === F ? void 0 : F.disabled),
+                            hidden: null === F || void 0 === F ? void 0 : F.hidden,
+                            label: null === F || void 0 === F ? void 0 : F.label,
+                            value: v[D],
+                            min: null === F || void 0 === F ? void 0 : F.min,
+                            max: null === F || void 0 === F ? void 0 : F.max,
+                            step: null === F || void 0 === F ? void 0 : F.step,
+                            vertical: null === F || void 0 === F ? void 0 : F.vertical,
                             runNb: y,
-                            url_key: I.url_key
-                        }, M)) : ne(I) ? (k.push(Object(E.jsx)(Pt, {
-                            widgetKey: M,
-                            disabled: o || (null === I || void 0 === I ? void 0 : I.disabled),
-                            hidden: null === I || void 0 === I ? void 0 : I.hidden,
-                            label: null === I || void 0 === I ? void 0 : I.label,
-                            maxFileSize: null === I || void 0 === I ? void 0 : I.maxFileSize,
-                            value: v[M],
+                            url_key: F.url_key
+                        }, D)) : ne(F) ? (k.push(Object(E.jsx)(Pt, {
+                            widgetKey: D,
+                            disabled: o || (null === F || void 0 === F ? void 0 : F.disabled),
+                            hidden: null === F || void 0 === F ? void 0 : F.hidden,
+                            label: null === F || void 0 === F ? void 0 : F.label,
+                            maxFileSize: null === F || void 0 === F ? void 0 : F.maxFileSize,
+                            value: v[D],
                             runNb: y
-                        }, M)), N.push(M)) : oe(I) ? k.push(Object(E.jsx)(Ct, {
-                            widgetKey: M,
-                            disabled: o || (null === I || void 0 === I ? void 0 : I.disabled),
-                            hidden: null === I || void 0 === I ? void 0 : I.hidden,
-                            label: null === I || void 0 === I ? void 0 : I.label,
-                            value: v[M],
-                            rows: null === I || void 0 === I ? void 0 : I.rows,
+                        }, D)), N.push(D)) : oe(F) ? k.push(Object(E.jsx)(Tt, {
+                            widgetKey: D,
+                            disabled: o || (null === F || void 0 === F ? void 0 : F.disabled),
+                            hidden: null === F || void 0 === F ? void 0 : F.hidden,
+                            label: null === F || void 0 === F ? void 0 : F.label,
+                            value: v[D],
+                            rows: null === F || void 0 === F ? void 0 : F.rows,
                             runNb: y,
                             continuousUpdate: b,
-                            url_key: null === I || void 0 === I ? void 0 : I.url_key
-                        }, M)) : ie(I) ? k.push(Object(E.jsx)(Dt, {
-                            value: I.value,
+                            url_key: null === F || void 0 === F ? void 0 : F.url_key
+                        }, D)) : ie(F) ? k.push(Object(E.jsx)(Ut, {
+                            value: F.value,
                             disabled: o
-                        }, M)) : re(I) ? k.push(Object(E.jsx)(ia, {
-                            widgetKey: M,
-                            disabled: o || (null === I || void 0 === I ? void 0 : I.disabled),
-                            hidden: null === I || void 0 === I ? void 0 : I.hidden,
-                            label: null === I || void 0 === I ? void 0 : I.label,
-                            value: v[M],
-                            style: null === I || void 0 === I ? void 0 : I.style,
+                        }, D)) : re(F) ? k.push(Object(E.jsx)(ia, {
+                            widgetKey: D,
+                            disabled: o || (null === F || void 0 === F ? void 0 : F.disabled),
+                            hidden: null === F || void 0 === F ? void 0 : F.hidden,
+                            label: null === F || void 0 === F ? void 0 : F.label,
+                            value: v[D],
+                            style: null === F || void 0 === F ? void 0 : F.style,
                             runNb: y
-                        }, M)) : se(I) || console.log("Unknown widget type", I)
+                        }, D)) : se(F) || console.log("Unknown widget type", F)
                     }
                 }
-                var L = {};
-                l && (L = {
+                var W = {};
+                l && (W = {
                     padding: "0px"
                 });
-                var U = void 0 === t || null === t || "" === t;
+                var I = void 0 === t || null === t || "" === t;
                 return Object(E.jsx)("nav", {
                     id: "sidebarMenu",
                     className: "col-lg-3 d-md-block bg-light sidebar",
-                    style: Object(D.a)(Object(D.a)({}, L), {}, {
+                    style: Object(U.a)(Object(U.a)({}, W), {}, {
                         overflowY: "auto"
                     }),
                     children: Object(E.jsx)(ca.a, {
                         blocking: !1,
                         message: "",
                         children: Object(E.jsxs)("div", {
                             className: "position-sticky p-3",
@@ -2316,81 +2340,81 @@
                                     className: "btn btn-sm  btn-outline-primary",
                                     type: "button",
                                     style: {
                                         float: "right",
                                         zIndex: "101"
                                     },
                                     onClick: function() {
-                                        return h(V(!1))
+                                        return h(z(!1))
                                     },
                                     "data-toggle": "tooltip",
                                     "data-placement": "right",
                                     title: "Hide sidebar",
                                     children: Object(E.jsx)("i", {
                                         className: "fa fa-chevron-left",
                                         "aria-hidden": "true"
                                     })
                                 })]
                             }), Object(E.jsx)("div", {
                                 style: {
                                     padding: "0px"
                                 },
                                 children: Object(E.jsxs)("form", {
-                                    children: [k, U && Object(E.jsx)("div", {
+                                    children: [k, I && Object(E.jsx)("div", {
                                         style: {
                                             padding: "15px"
                                         }
                                     }), Object(E.jsx)("div", {
                                         className: "form-group mb-3 pb-1 pt-2",
                                         children: !b && Object(E.jsx)(ra, {
                                             runNb: w,
                                             waiting: o,
                                             workerState: m
                                         })
-                                    }), m === Rt.UsageLimitReached && Object(E.jsxs)("div", {
+                                    }), m === Ct.UsageLimitReached && Object(E.jsxs)("div", {
                                         className: "alert alert-info mb-3 mt-3",
                                         role: "alert",
                                         children: [Object(E.jsx)("i", {
                                             className: "fa fa-info-circle",
                                             "aria-hidden": "true"
                                         }), " Usage limit was reached. Please upgrade the plan."]
-                                    }), m === Rt.MaxIdleTimeReached && Object(E.jsxs)("div", {
+                                    }), m === Ct.MaxIdleTimeReached && Object(E.jsxs)("div", {
                                         className: "alert alert-info mb-3 mt-3",
                                         role: "alert",
                                         children: [Object(E.jsx)("i", {
                                             className: "fa fa-info-circle",
                                             "aria-hidden": "true"
                                         }), " Your worker was idle for too long, that's why we have stopped it. Do you need a worker?", Object(E.jsx)("br", {}), Object(E.jsx)("button", {
                                             className: "btn btn-sm btn-primary my-2",
                                             onClick: function() {
                                                 return window.location.reload()
                                             },
                                             children: "Restart worker"
                                         })]
-                                    }), m === Rt.MaxRunTimeReached && Object(E.jsxs)("div", {
+                                    }), m === Ct.MaxRunTimeReached && Object(E.jsxs)("div", {
                                         className: "alert alert-info mb-3 mt-3",
                                         role: "alert",
                                         children: [Object(E.jsx)("i", {
                                             className: "fa fa-info-circle",
                                             "aria-hidden": "true"
                                         }), " Your worker was running for too long, that's why we have stopped it. Do you need a worker?", Object(E.jsx)("br", {}), Object(E.jsx)("button", {
                                             className: "btn btn-sm btn-primary my-2",
                                             onClick: function() {
                                                 return window.location.reload()
                                             },
                                             children: "Restart worker"
                                         })]
-                                    }), o && (m === Rt.Unknown || m === Rt.Queued) && Object(E.jsxs)("div", {
+                                    }), o && (m === Ct.Unknown || m === Ct.Queued) && Object(E.jsxs)("div", {
                                         className: "alert alert-warning mb-3 mt-3",
                                         role: "alert",
                                         children: [Object(E.jsx)("i", {
                                             className: "fa fa-cogs",
                                             "aria-hidden": "true"
                                         }), " Waiting for worker ..."]
-                                    }), o && m === Rt.Starting && Object(E.jsxs)("div", {
+                                    }), o && m === Ct.Starting && Object(E.jsxs)("div", {
                                         className: "alert alert-success mb-3 mt-3",
                                         role: "alert",
                                         children: [Object(E.jsx)("i", {
                                             className: "fa fa-cogs",
                                             "aria-hidden": "true"
                                         }), " Initializing worker ..."]
                                     }), r && Object(E.jsxs)("div", {
@@ -2489,46 +2513,46 @@
                     u = e.username,
                     b = e.slidesHash,
                     p = e.columnsWidth,
                     j = e.isPresentation,
                     h = e.fullScreen,
                     v = function() {
                         var e = Object(n.useState)(ce()),
-                            t = Object(_.a)(e, 2),
+                            t = Object(R.a)(e, 2),
                             a = t[0],
                             o = t[1];
                         return Object(n.useEffect)((function() {
                             function e() {
                                 o(ce())
                             }
                             return window.addEventListener("resize", e),
                                 function() {
                                     return window.removeEventListener("resize", e)
                                 }
                         }), []), a
                     }().height,
                     f = d ? v - 10 : v - 58,
                     m = Object(i.b)(),
-                    x = Object(i.c)(Re),
+                    x = Object(i.c)(Ce),
                     O = Object(i.c)(Qt),
                     g = !1;
                 if (void 0 !== x && void 0 !== x.params && void 0 !== x.params["show-code"] && null !== x.params["show-code"] && (g = x.params["show-code"]), "" !== O && !j && (O = "<script>init_mathjax();<\/script>" + O, !g)) {
                     O = '<style type="text/css">\n      .jp-mod-noOutputs {\n          padding: 0px; \n      }\n      .jp-mod-noInput {\n        padding-top: 0px;\n        padding-bottom: 0px;\n      }\n      </style>' + O
                 }
                 if ("" !== O && j && "" !== b && -1 === O.indexOf("Reveal.slide(")) {
                     var y = b.split("/"),
                         w = "";
                     4 === y.length ? w = "Reveal.slide(".concat(y[1], ", ").concat(y[2], ", ").concat(y[3], ");") : 3 === y.length ? w = "Reveal.slide(".concat(y[1], ", ").concat(y[2], ");") : 2 === y.length && (w = "Reveal.slide(".concat(y[1], ");")), "" !== w && (O = O.replace("setScrollingSlide);", "setScrollingSlide); try{ ".concat(w, " } catch(error) {}")))
                 }
                 Object(n.useEffect)((function() {
                     if (void 0 !== o) {
                         var e = o;
-                        window.location.origin.startsWith("https") && (e = e.replace("http://", "https://")), s.a.get("".concat(e).concat(b)).then((function(e) {
+                        window.location.origin.startsWith("https") && (e = e.replace("http://", "https://")), "http://localhost:3000" === window.location.origin && e.startsWith("/media") && (e = "https://127.0.0.1:8000" + e), s.a.get("".concat(e).concat(b)).then((function(e) {
                             var t = e.data;
-                            j || (t = (t = (t = (t = (t = (t = t.replace(/<head>[\s\S]*?<\/head>/, "")).replace("<html>", "")).replace("</html>", "")).replace("<body", "<div")).replace("</body>", "</div>")).replace("<!DOCTYPE html>", "")), m(Vt(t))
+                            j || (t = (t = (t = (t = (t = (t = t.replace(/<head>[\s\S]*?<\/head>/, "")).replace("<html>", "")).replace("</html>", "")).replace("<body", "<div")).replace("</body>", "</div>")).replace("<!DOCTYPE html>", "")), m(zt(t))
                         }))
                     }
                 }), [m, o, b, j]);
                 var k = {
                         paddingTop: "0px",
                         paddingRight: "0px",
                         paddingLeft: h ? "12px" : "0px",
@@ -2597,15 +2621,15 @@
             function ba(e) {
                 var t = e.files,
                     a = e.filesState,
                     n = e.waiting,
                     o = Object(i.b)();
                 console.log(t);
                 var r, c = [],
-                    l = Object(I.a)(t);
+                    l = Object(F.a)(t);
                 try {
                     var d = function() {
                         var e, t = r.value,
                             a = t.split("/").pop();
                         if (a = null === (e = a) || void 0 === e ? void 0 : e.split("?")[0], t && a) {
                             var n = "".concat(s.a.defaults.baseURL).concat(t);
                             t.includes("s3.amazonaws.com") && (n = t), c.push(Object(E.jsxs)("div", {
@@ -2715,16 +2739,16 @@
                     })
                 })
             }
 
             function ja(e) {
                 for (var t = e.slug, a = e.widgetsParams, o = e.notebookPath, r = e.columnsWidth, c = e.taskSessionId, l = Object(n.useState)(JSON.stringify({
                         msg: "Example output"
-                    })), b = Object(_.a)(l, 2), p = b[0], j = b[1], h = Object(i.c)(Me), v = {}, f = 0, m = Object.entries(a); f < m.length; f++) {
-                    var x = Object(_.a)(m[f], 2),
+                    })), b = Object(R.a)(l, 2), p = b[0], j = b[1], h = Object(i.c)(De), v = {}, f = 0, m = Object.entries(a); f < m.length; f++) {
+                    var x = Object(R.a)(m[f], 2),
                         O = x[0];
                     x[1].input && (v[O] = h[O])
                 }
 
                 function g() {
                     return (g = Object(u.a)(d.a.mark((function e() {
                         var t, a;
@@ -2819,79 +2843,79 @@
                                 var t = Object(u.a)(d.a.mark((function t(a) {
                                     var n, o, i;
                                     return d.a.wrap((function(t) {
                                         for (;;) switch (t.prev = t.next) {
                                             case 0:
                                                 return t.prev = 0, n = "/api/v1/get_pdf/".concat(e, "/"), t.next = 4, s.a.get(n);
                                             case 4:
-                                                o = t.sent, (i = o.data).ready ? (a(Ke()), "" !== i.error ? p.b.error(i.error) : x("".concat(s.a.defaults.baseURL).concat(i.url), "".concat(i.title))) : a(Je()), t.next = 13;
+                                                o = t.sent, (i = o.data).ready ? (a(Je()), "" !== i.error ? p.b.error(i.error) : x("".concat(s.a.defaults.baseURL).concat(i.url), "".concat(i.title))) : a(Ke()), t.next = 13;
                                                 break;
                                             case 9:
-                                                t.prev = 9, t.t0 = t.catch(0), p.b.error("The error occured during PDF export. ".concat(t.t0)), a(Ke());
+                                                t.prev = 9, t.t0 = t.catch(0), p.b.error("The error occured during PDF export. ".concat(t.t0)), a(Je());
                                             case 13:
                                             case "end":
                                                 return t.stop()
                                         }
                                     }), t, null, [
                                         [0, 9]
                                     ])
                                 })));
                                 return function(e) {
                                     return t.apply(this, arguments)
                                 }
                             }()
                         }(a))
-                    }), 1e3) : (e(Ke()), p.b.error("Problem with PDF export. Please try again later or ask your admin for help.", {
+                    }), 1e3) : (e(Je()), p.b.error("Problem with PDF export. Please try again later or ask your admin for help.", {
                         autoClose: 6e3
                     })))
                 }), [e, t, a, o]), Object(E.jsx)("div", {})
             }
             var va = function(e) {
                 e.isSingleApp;
                 var t, a, o, r, c, l = e.notebookSlug,
                     b = e.displayEmbed,
                     p = Object(i.b)(),
-                    j = Object(i.c)(Re),
-                    h = Object(i.c)(Fe),
+                    j = Object(i.c)(Ce),
+                    h = Object(i.c)(Ae),
                     v = Object(i.c)(Ye),
                     m = Object(i.c)(Ge),
                     x = Object(i.c)(Qe),
-                    O = Object(i.c)(K),
+                    O = Object(i.c)(J),
                     g = Object(i.c)(Y),
                     y = Object(i.c)(q),
-                    w = Object(i.c)(T),
-                    k = Object(i.c)(C),
-                    N = Object(i.c)(Ae),
+                    w = Object(i.c)(_),
+                    k = Object(i.c)(T),
+                    N = Object(i.c)(Le),
                     S = Object(i.c)(G),
                     P = Object(i.c)(Ze),
-                    R = Object(i.c)(Gt),
-                    F = Object(i.c)(Yt),
-                    A = Object(i.c)(wt),
-                    I = Object(i.c)(Nt),
-                    L = function() {
+                    C = Object(i.c)(Gt),
+                    A = Object(i.c)(Yt),
+                    L = Object(i.c)(wt),
+                    F = Object(i.c)(Nt),
+                    W = function() {
                         var e;
-                        return !(null === j || void 0 === j || null === (e = j.params) || void 0 === e ? void 0 : e.static_notebook) && (F !== Rt.UsageLimitReached && F !== Rt.MaxIdleTimeReached && F !== Rt.MaxRunTimeReached && F !== Rt.Running)
+                        return !(null === j || void 0 === j || null === (e = j.params) || void 0 === e ? void 0 : e.static_notebook) && (A !== Ct.UsageLimitReached && A !== Ct.MaxIdleTimeReached && A !== Ct.MaxRunTimeReached && A !== Ct.Running)
                     },
-                    U = function() {
+                    I = function() {
                         return "WATCH_READY" === j.state || "WATCH_WAIT" === j.state || "WATCH_ERROR" === j.state
                     };
                 Object(n.useEffect)((function() {
-                    void 0 !== A && p(function(e, t) {
+                    void 0 !== L && p(function(e, t) {
                         var a = arguments.length > 2 && void 0 !== arguments[2] && arguments[2];
                         return function() {
                             var n = Object(u.a)(d.a.mark((function n(o) {
                                 var i, r, c, l, u, b;
                                 return d.a.wrap((function(n) {
                                     for (;;) switch (n.prev = n.next) {
                                         case 0:
-                                            return n.prev = 0, a || (o(fe("")), o(qe())), i = ce(), r = i.width, o(V(r > 992)), a || o(ve("loading")), c = "/api/v1/".concat(e, "/getnb/").concat(t, "/"), n.next = 8, s.a.get(c);
+                                            return n.prev = 0, a || (o(fe("")), o(qe())), i = ce(), r = i.width, o(z(r > 992)), a || o(ve("loading")), c = "/api/v1/".concat(e, "/getnb/").concat(t, "/"), n.next = 8, s.a.get(c);
                                         case 8:
-                                            l = n.sent, u = l.data, b = JSON.parse(u.params), o(he(Object(D.a)(Object(D.a)({}, u), {}, {
+                                            l = n.sent, u = l.data, b = JSON.parse(u.params), o(he(Object(U.a)(Object(U.a)({}, u), {}, {
                                                 params: b
-                                            }))), a || o(ve("loaded")), null !== (null === b || void 0 === b ? void 0 : b.show_sidebar) && void 0 !== (null === b || void 0 === b ? void 0 : b.show_sidebar) && o(V(null === b || void 0 === b ? void 0 : b.show_sidebar)), n.next = 20;
+                                            }))), a || o(ve("loaded")), null !== (null === b || void 0 === b ? void 0 : b.show_sidebar) && void 0 !== (null === b || void 0 === b ? void 0 : b.show_sidebar) && o(z(null === b || void 0 === b ? void 0 : b.show_sidebar)), n.next = 20;
                                             break;
                                         case 16:
                                             n.prev = 16, n.t0 = n.catch(0), a || o(ve("error")), console.error("Problem during loading selected notebook (".concat(t, "). ").concat(n.t0));
                                         case 20:
                                         case "end":
                                             return n.stop()
                                     }
@@ -2899,76 +2923,76 @@
                                     [0, 16]
                                 ])
                             })));
                             return function(e) {
                                 return n.apply(this, arguments)
                             }
                         }()
-                    }(A, l))
-                }), [p, A, l, k]), Object(n.useEffect)((function() {
+                    }(L, l))
+                }), [p, L, l, k]), Object(n.useEffect)((function() {
                     var e;
-                    "files" === O && "2" === (null === j || void 0 === j || null === (e = j.params) || void 0 === e ? void 0 : e.version) && void 0 !== R && void 0 !== j.id && p(function(e, t) {
+                    "files" === O && "2" === (null === j || void 0 === j || null === (e = j.params) || void 0 === e ? void 0 : e.version) && void 0 !== C && void 0 !== j.id && p(function(e, t) {
                         return function() {
                             var a = Object(u.a)(d.a.mark((function a(n) {
                                 var o, i, r, c;
                                 return d.a.wrap((function(a) {
                                     for (;;) switch (a.prev = a.next) {
                                         case 0:
-                                            return a.prev = 0, n(z("loading")), n(B([])), o = f(), i = "/api/v1/worker-output-files/".concat(o, "/").concat(e, "/").concat(t, "/"), a.next = 7, s.a.get(i);
+                                            return a.prev = 0, n(B("loading")), n(V([])), o = f(), i = "/api/v1/worker-output-files/".concat(o, "/").concat(e, "/").concat(t, "/"), a.next = 7, s.a.get(i);
                                         case 7:
-                                            r = a.sent, c = r.data, n(B(c)), n(z("loaded")), a.next = 17;
+                                            r = a.sent, c = r.data, n(V(c)), n(B("loaded")), a.next = 17;
                                             break;
                                         case 13:
-                                            a.prev = 13, a.t0 = a.catch(0), n(z("error")), console.error("Problem during loading worker output files. ".concat(a.t0));
+                                            a.prev = 13, a.t0 = a.catch(0), n(B("error")), console.error("Problem during loading worker output files. ".concat(a.t0));
                                         case 17:
                                         case "end":
                                             return a.stop()
                                     }
                                 }), a, null, [
                                     [0, 13]
                                 ])
                             })));
                             return function(e) {
                                 return a.apply(this, arguments)
                             }
                         }()
-                    }(R, j.id))
-                }), [p, O, j, R]);
-                var W = j.default_view_path;
-                v.state && "DONE" === v.state && v.result && (W = v.result);
+                    }(C, j.id))
+                }), [p, O, j, C]);
+                var M = j.default_view_path;
+                v.state && "DONE" === v.state && v.result && (M = v.result);
                 var H = "";
-                v.state && v.result && "ERROR" === v.state && (H = v.result), m.state && "DONE" === m.state && m.result && (W = m.result), m.state && m.result && "ERROR" === m.state && (H = m.result), W === j.default_view_path && x.state && "DONE" === x.state && x.result && (W = x.result);
-                var J = !1;
-                return j.output && j.output.toLowerCase().startsWith("rest") && (J = !0), Object(E.jsxs)("div", {
+                v.state && v.result && "ERROR" === v.state && (H = v.result), m.state && "DONE" === m.state && m.result && (M = m.result), m.state && m.result && "ERROR" === m.state && (H = m.result), M === j.default_view_path && x.state && "DONE" === x.state && x.result && (M = x.result);
+                var K = !1;
+                return j.output && j.output.toLowerCase().startsWith("rest") && (K = !0), Object(E.jsxs)("div", {
                     className: "App",
-                    children: [!b && Object(E.jsx)(M, {
-                        isSitePublic: I,
+                    children: [!b && Object(E.jsx)(D, {
+                        isSitePublic: F,
                         username: w
                     }), Object(E.jsxs)(ca.a, {
                         blocking: P,
                         message: "Exporting to PDF. Please wait ...",
                         children: [P && Object(E.jsx)(ha, {}), Object(E.jsx)("div", {
                             className: "container-fluid",
                             children: Object(E.jsxs)("div", {
                                 className: "row",
                                 children: [S && Object(E.jsx)(la, {
                                     notebookTitle: j.title,
                                     notebookId: j.id,
                                     notebookSchedule: j.schedule,
                                     taskCreatedAt: v.created_at,
                                     loadingState: h,
-                                    waiting: L(),
+                                    waiting: W(),
                                     widgetsParams: null === j || void 0 === j || null === (t = j.params) || void 0 === t ? void 0 : t.params,
-                                    watchMode: U(),
-                                    notebookPath: W,
+                                    watchMode: I(),
+                                    notebookPath: M,
                                     displayEmbed: b,
                                     showFiles: function(e) {
                                         if (e)
                                             for (var t = 0, a = Object.entries(e); t < a.length; t++) {
-                                                if (se(Object(_.a)(a[t], 2)[1])) return !0
+                                                if (se(Object(R.a)(a[t], 2)[1])) return !0
                                             }
                                         return !1
                                     }(null === j || void 0 === j || null === (a = j.params) || void 0 === a ? void 0 : a.params),
                                     isPresentation: void 0 !== j.output && "slides" === j.output,
                                     notebookParseErrors: j.errors,
                                     continuousUpdate: null === j || void 0 === j || null === (o = j.params) || void 0 === o ? void 0 : o.continuous_update,
                                     staticNotebook: null === j || void 0 === j || null === (r = j.params) || void 0 === r ? void 0 : r.static_notebook,
@@ -2983,50 +3007,50 @@
                                         style: {
                                             position: "absolute",
                                             top: b ? "5px" : "50px",
                                             left: "5px",
                                             zIndex: "2000"
                                         },
                                         onClick: function() {
-                                            return p(V(!0))
+                                            return p(z(!0))
                                         },
                                         "data-toggle": "tooltip",
                                         "data-placement": "right",
                                         title: "Show sidebar",
                                         children: Object(E.jsx)("i", {
                                             className: "fa fa-chevron-right",
                                             "aria-hidden": "true"
                                         })
                                     })
-                                }), J && Object(E.jsx)(ja, {
+                                }), K && Object(E.jsx)(ja, {
                                     slug: j.slug,
                                     widgetsParams: null === j || void 0 === j || null === (c = j.params) || void 0 === c ? void 0 : c.params,
-                                    notebookPath: W,
+                                    notebookPath: M,
                                     columnsWidth: S ? 9 : 12,
                                     taskSessionId: v.session_id
                                 }), Object(E.jsx)(ua, {
                                     appView: O,
                                     loadingState: h,
-                                    notebookPath: W,
+                                    notebookPath: M,
                                     errorMsg: H,
-                                    waiting: L(),
-                                    watchMode: U(),
+                                    waiting: W(),
+                                    watchMode: I(),
                                     displayEmbed: b,
                                     username: w,
                                     slidesHash: N,
                                     columnsWidth: S ? 9 : 12,
                                     isPresentation: void 0 !== j.output && "slides" === j.output,
                                     fullScreen: function() {
                                         var e, t;
                                         return void 0 === j || null === j || (void 0 === (null === j || void 0 === j || null === (e = j.params) || void 0 === e ? void 0 : e.full_screen) || null === (null === j || void 0 === j || null === (t = j.params) || void 0 === t ? void 0 : t.full_screen) || j.params.full_screen)
                                     }()
                                 }), "files" === O && Object(E.jsx)(ba, {
                                     files: g,
                                     filesState: y,
-                                    waiting: L()
+                                    waiting: W()
                                 })]
                             })
                         })]
                     }), b && Object(E.jsx)(pa, {})]
                 })
             };
 
@@ -3120,38 +3144,38 @@
                             })
                         }), Object(E.jsxs)("div", {
                             className: "col-4",
                             style: {
                                 marginRight: "0px",
                                 paddingRight: "0px"
                             },
-                            children: [!t && "" === a && Object(E.jsx)(F, {}), "" !== a && Object(E.jsx)(A, {
+                            children: [!t && "" === a && Object(E.jsx)(A, {}), "" !== a && Object(E.jsx)(L, {
                                 username: a
                             })]
                         })]
                     })
                 })
             }
 
             function Oa() {
                 var e = Object(i.b)(),
                     t = Object(n.useState)(""),
-                    a = Object(_.a)(t, 2),
+                    a = Object(R.a)(t, 2),
                     o = a[0],
                     r = a[1],
                     c = Object(n.useState)(""),
-                    l = Object(_.a)(c, 2),
+                    l = Object(R.a)(c, 2),
                     b = l[0],
                     j = l[1],
                     h = Object(n.useState)(""),
-                    v = Object(_.a)(h, 2),
+                    v = Object(R.a)(h, 2),
                     f = v[0],
                     m = v[1],
-                    x = Object(i.c)(T),
-                    O = Object(i.c)(R),
+                    x = Object(i.c)(_),
+                    O = Object(i.c)(C),
                     g = Object(i.c)(Nt);
                 return document.body.style.backgroundColor = "white", Object(n.useEffect)((function() {
                     e(function() {
                         var e = Object(u.a)(d.a.mark((function e(t) {
                             var a, n;
                             return d.a.wrap((function(e) {
                                 for (;;) switch (e.prev = e.next) {
@@ -3356,21 +3380,21 @@
                 ka = (wa.setVersion, wa.setWelcome),
                 Na = function(e) {
                     return e.version.welcome
                 };
 
             function Sa() {
                 var e = Object(i.b)(),
-                    t = Object(i.c)(Ce),
-                    a = Object(i.c)(Te),
+                    t = Object(i.c)(Te),
+                    a = Object(i.c)(_e),
                     o = Object(i.c)(Na),
-                    r = Object(i.c)(T),
-                    c = Object(i.c)(C),
+                    r = Object(i.c)(_),
+                    c = Object(i.c)(T),
                     l = Object(n.useState)(""),
-                    b = Object(_.a)(l, 2),
+                    b = Object(R.a)(l, 2),
                     p = b[0],
                     j = b[1],
                     h = Object(i.c)(wt),
                     v = Object(i.c)(Nt),
                     f = Object(i.c)(kt);
                 Object(n.useEffect)((function() {
                     void 0 !== h && (e(function(e) {
@@ -3380,15 +3404,15 @@
                                 return d.a.wrap((function(t) {
                                     for (;;) switch (t.prev = t.next) {
                                         case 0:
                                             return t.prev = 0, a(fe("")), a(je("loading")), a(qe()), n = "/api/v1/".concat(e, "/notebooks/"), t.next = 7, s.a.get(n);
                                         case 7:
                                             o = t.sent, i = o.data, r = i.map((function(e) {
                                                 var t = JSON.parse(e.params);
-                                                return Object(D.a)(Object(D.a)({}, e), {}, {
+                                                return Object(U.a)(Object(U.a)({}, e), {}, {
                                                     params: t
                                                 })
                                             })), a(pe(r)), a(je("loaded")), t.next = 18;
                                             break;
                                         case 14:
                                             t.prev = 14, t.t0 = t.catch(0), a(je("error")), console.error("Problem during loading recent notebooks. ".concat(t.t0));
                                         case 18:
@@ -3431,15 +3455,15 @@
                     }(h)))
                 }), [e, h, c, f]);
                 var m = function(e, t) {
                         return null !== e && void 0 !== e ? e.slice(0, t) + (e.length > t ? " ..." : "") : ""
                     },
                     x = t.map((function(e, t) {
                         var a = e.default_view_path;
-                        return window.location.origin.startsWith("https") && (a = a.replace("http://", "https://")), Object(E.jsx)("div", {
+                        return window.location.origin.startsWith("https") && (a = a.replace("http://", "https://")), "http://localhost:3000" === window.location.origin && a.startsWith("/media") && (a = "https://127.0.0.1:8000" + a), Object(E.jsx)("div", {
                             className: "col-md-4",
                             style: {
                                 paddingBottom: "20px"
                             },
                             children: Object(E.jsxs)("div", {
                                 className: "card",
                                 children: [Object(E.jsx)("div", {
@@ -3525,16 +3549,16 @@
                             },
                             children: "Welcome!"
                         }), "" !== O && Object(E.jsx)("div", {
                             style: {
                                 paddingTop: "20px",
                                 paddingBottom: "10px"
                             },
-                            children: Object(E.jsx)(_t.a, {
-                                rehypePlugins: [Ft.a, Et.a, At.a, Mt.a],
+                            children: Object(E.jsx)(Rt.a, {
+                                rehypePlugins: [At.a, Et.a, Lt.a, Dt.a],
                                 children: O
                             })
                         }), Object(E.jsxs)("div", {
                             className: "row",
                             children: ["loading" === a && Object(E.jsx)("p", {
                                 children: "Loading notebooks. Please wait ..."
                             }), "loaded" === a && 0 === t.length && Object(E.jsx)("div", {
@@ -3549,19 +3573,19 @@
                 })
             }
 
             function Pa() {
                 var e = Object(i.b)(),
                     t = Object(r.o)(),
                     a = Object(n.useState)(""),
-                    o = Object(_.a)(a, 2),
+                    o = Object(R.a)(a, 2),
                     c = o[0],
                     l = o[1],
                     b = Object(n.useState)(""),
-                    j = Object(_.a)(b, 2),
+                    j = Object(R.a)(b, 2),
                     h = j[0],
                     v = j[1],
                     f = Object(i.c)(Nt);
                 document.body.style.backgroundColor = "#f5f5f5";
                 var m = "/",
                     x = Object(r.m)();
                 if (x && x.state) {
@@ -3660,15 +3684,15 @@
                                 children: ["No account? ", Object(E.jsx)("br", {}), " Please contact administrator to create account for you."]
                             })
                         })]
                     }), Object(E.jsx)(ma, {})]
                 })
             }
 
-            function Ca() {
+            function Ta() {
                 return Object(E.jsxs)("div", {
                     className: "App",
                     children: [Object(E.jsx)(xa, {
                         isSitePublic: !0,
                         username: ""
                     }), Object(E.jsxs)("div", {
                         style: {
@@ -3682,15 +3706,15 @@
                         }), Object(E.jsx)("p", {
                             children: "App lost connection to the server. Please try again in a moment or contact administrator."
                         })]
                     }), Object(E.jsx)(ma, {})]
                 })
             }
 
-            function Ta() {
+            function _a() {
                 return Object(E.jsxs)("div", {
                     className: "App",
                     children: [Object(E.jsx)(xa, {
                         isSitePublic: !0,
                         username: ""
                     }), Object(E.jsxs)("div", {
                         style: {
@@ -3707,15 +3731,15 @@
                                 children: "login"
                             }), " to access site."]
                         })]
                     }), Object(E.jsx)(ma, {})]
                 })
             }
 
-            function Ra() {
+            function Ca() {
                 return Object(E.jsxs)("div", {
                     className: "App",
                     children: [Object(E.jsx)(xa, {
                         isSitePublic: !0,
                         username: ""
                     }), Object(E.jsx)("div", {
                         style: {
@@ -3730,15 +3754,15 @@
                             },
                             children: "Please wait. Loading site ..."
                         })
                     }), Object(E.jsx)(ma, {})]
                 })
             }
 
-            function _a() {
+            function Ra() {
                 return Object(E.jsxs)("div", {
                     className: "App",
                     children: [Object(E.jsx)(xa, {
                         isSitePublic: !0,
                         username: ""
                     }), Object(E.jsxs)("div", {
                         style: {
@@ -3774,15 +3798,15 @@
                         }), Object(E.jsx)("p", {
                             children: "We can't find site you are looking for. Please make sure that URL address is correct."
                         })]
                     }), Object(E.jsx)(ma, {})]
                 })
             }
 
-            function Fa() {
+            function Aa() {
                 return Object(E.jsxs)("div", {
                     className: "App",
                     children: [Object(E.jsx)(xa, {
                         isSitePublic: !0,
                         username: ""
                     }), Object(E.jsxs)("div", {
                         style: {
@@ -3796,15 +3820,15 @@
                         }), Object(E.jsx)("p", {
                             children: "Please try to refresh the website ..."
                         })]
                     }), Object(E.jsx)(ma, {})]
                 })
             }
 
-            function Aa() {
+            function La() {
                 return Object(E.jsxs)("div", {
                     className: "App",
                     children: [Object(E.jsx)(xa, {
                         isSitePublic: !0,
                         username: ""
                     }), Object(E.jsxs)("div", {
                         style: {
@@ -3824,57 +3848,57 @@
                             },
                             children: "Refresh"
                         })]
                     }), Object(E.jsx)(ma, {})]
                 })
             }
 
-            function Ma(e) {
+            function Da(e) {
                 var t = e.children,
-                    a = Object(i.c)(C),
+                    a = Object(i.c)(T),
                     o = Object(i.c)(Nt),
                     s = Object(r.m)(),
                     c = Object(i.b)(),
                     l = Object(i.c)(yt);
                 return Object(n.useEffect)((function() {
                     c(St())
-                }), [c]), l === ct.Unknown ? Object(E.jsx)(Ra, {}) : l === ct.NotFound ? Object(E.jsx)(Ea, {}) : l === ct.NotReady ? Object(E.jsx)(Aa, {}) : l === ct.AccessForbidden ? Object(E.jsx)(Ta, {}) : l === ct.NetworkError ? Object(E.jsx)(_a, {}) : l === ct.PleaseRefresh ? Object(E.jsx)(Fa, {}) : l === ct.LostConnection ? (window.location.reload(), Object(E.jsx)(Ca, {})) : o || a ? t : Object(E.jsx)(r.a, {
+                }), [c]), l === ct.Unknown ? Object(E.jsx)(Ca, {}) : l === ct.NotFound ? Object(E.jsx)(Ea, {}) : l === ct.NotReady ? Object(E.jsx)(La, {}) : l === ct.AccessForbidden ? Object(E.jsx)(_a, {}) : l === ct.NetworkError ? Object(E.jsx)(Ra, {}) : l === ct.PleaseRefresh ? Object(E.jsx)(Aa, {}) : l === ct.LostConnection ? (window.location.reload(), Object(E.jsx)(Ta, {})) : o || a ? t : Object(E.jsx)(r.a, {
                     to: "/login",
                     state: {
                         from: s
                     },
                     replace: !0
                 })
             }
 
-            function Da(e) {
+            function Ua(e) {
                 var t = e.children;
                 return Object(E.jsx)(E.Fragment, {
                     children: t
                 })
             }
 
-            function Ia() {
-                return Object(E.jsx)(Ma, {
+            function Fa() {
+                return Object(E.jsx)(Da, {
                     children: Object(E.jsx)(E.Fragment, {
                         children: Object(E.jsx)(r.b, {})
                     })
                 })
             }
 
-            function La() {
+            function Wa() {
                 var e = Object(i.b)();
                 return Object(n.useEffect)((function() {
                     f(!0), localStorage.getItem("token") && e(N(localStorage.getItem("token"))), localStorage.getItem("username") && e(S(localStorage.getItem("username"))), e(St())
                 }), []), Object(E.jsx)(c.a, {
-                    children: Object(E.jsx)(Da, {
+                    children: Object(E.jsx)(Ua, {
                         children: Object(E.jsxs)(r.e, {
                             children: [Object(E.jsxs)(r.c, {
                                 path: "/",
-                                element: Object(E.jsx)(Ia, {}),
+                                element: Object(E.jsx)(Fa, {}),
                                 children: [Object(E.jsx)(r.c, {
                                     path: "/",
                                     element: Object(E.jsx)(Sa, {})
                                 }), Object(E.jsx)(r.c, {
                                     path: "/app/:slug/:embed?",
                                     element: Object(E.jsx)(oa, {
                                         children: Object(E.jsx)(fa, {})
@@ -3887,46 +3911,62 @@
                                 path: "/login",
                                 element: Object(E.jsx)(Pa, {})
                             })]
                         })
                     })
                 })
             }
-            var Ua = function(e) {
+            var Ia = function(e) {
                     var t = e.store;
                     e.history;
                     return Object(E.jsx)(i.a, {
                         store: t,
-                        children: Object(E.jsx)(La, {})
+                        children: Object(E.jsx)(Wa, {})
                     })
                 },
-                Wa = a(15),
+                Ma = a(15),
                 Ha = a(171),
-                za = a(32);
-            var Ba, Va = Object(Ha.a)(),
-                Ja = Object(za.b)({
+                Ba = a(32);
+            var Va, za = Object(Ha.a)(),
+                Ka = Object(Ba.b)({
                     notebooks: ue,
-                    tasks: We,
+                    tasks: Me,
                     version: ya,
-                    app: U,
+                    app: I,
                     auth: w,
-                    ws: Ut,
+                    ws: It,
                     sites: mt
                 }),
-                Ka = Object(Wa.a)(Object(b.c)()),
+                Ja = Object(Ma.a)(Object(b.c)()),
                 qa = (a(285), a(286), a(288), a(289), a(290), a(291), a(292), a(293), Object(b.a)({
-                    reducer: Ja,
-                    middleware: Ka,
-                    preloadedState: Ba
+                    reducer: Ka,
+                    middleware: Ja,
+                    preloadedState: Va
                 }));
-            s.a.defaults.baseURL = "http://127.0.0.1:8000", window.location.origin.endsWith("hf.space") && (s.a.defaults.baseURL = window.location.origin), s.a.defaults.baseURL = s.a.defaults.baseURL.split("+")[0], s.a.defaults.baseURL = s.a.defaults.baseURL.split("?")[0], s.a.defaults.baseURL = s.a.defaults.baseURL.split("#")[0], document.addEventListener("DOMContentLoaded", (function() {
+            Object({
+                NODE_ENV: "production",
+                PUBLIC_URL: "",
+                WDS_SOCKET_HOST: void 0,
+                WDS_SOCKET_PATH: void 0,
+                WDS_SOCKET_PORT: void 0,
+                FAST_REFRESH: !0,
+                REACT_APP_LOCAL_URL: "/static"
+            }).REACT_APP_SERVER_URL ? s.a.defaults.baseURL = Object({
+                NODE_ENV: "production",
+                PUBLIC_URL: "",
+                WDS_SOCKET_HOST: void 0,
+                WDS_SOCKET_PATH: void 0,
+                WDS_SOCKET_PORT: void 0,
+                FAST_REFRESH: !0,
+                REACT_APP_LOCAL_URL: "/static"
+            }).REACT_APP_SERVER_URL : "http://localhost:3000" === window.location.origin ? s.a.defaults.baseURL = "http://127.0.0.1:8000" : s.a.defaults.baseURL = window.location.origin, window.location.origin.endsWith("hf.space") && (s.a.defaults.baseURL = window.location.origin), s.a.defaults.baseURL = s.a.defaults.baseURL.split("+")[0], s.a.defaults.baseURL = s.a.defaults.baseURL.split("?")[0], s.a.defaults.baseURL = s.a.defaults.baseURL.split("#")[0], document.addEventListener("DOMContentLoaded", (function() {
                 return Object(o.render)(Object(E.jsxs)("div", {
-                    children: [Object(E.jsx)(Ua, {
+                    children: [Object(E.jsx)(Ia, {
                         store: qa,
-                        history: Va
+                        history: za
                     }), Object(E.jsx)(p.a, {
                         position: "top-right",
                         autoClose: 3e3,
                         hideProgressBar: !0,
                         newestOnTop: !0,
                         closeOnClick: !0,
                         pauseOnHover: !0
@@ -3935,8 +3975,8 @@
             }))
         }
     },
     [
         [295, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.68931b96.chunk.js.map
+//# sourceMappingURL=main.c4e40c36.chunk.js.map
```

### Comparing `mercury-2.2.7/mercury/frontend-dist/static/js/main.68931b96.chunk.js.map` & `mercury-2.2.8/mercury/frontend-dist/static/js/main.c4e40c36.chunk.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8515476479684108%*

 * *Differences: {"'file'": "'static/js/main.c4e40c36.chunk.js'",*

 * * "'mappings'": "'8QAIaA,EAAe,WAA0B,IAAzBC,EAAwB,wDAC7CC,EAAYC,eAAeC,QAAQ,aAQvC,OAPiB,MAAbF,GAGOD,KAFPC,EAAYG,eACZF,eAAeG,QAAQ,YAAaJ,IAKjCA,GAGEK,EAAoB,SAACC,GACT,qBAAVA,GAAyBA,EAEhCC,IAAMC,SAASC,QAAQC,OAAvB,cAAiD,SAAWJ,SAGrDC,IAAMC,SAASC,QAAQC,OAAvB,eAIFC,EAAiB,SAACC,EAAaC,GACxCN,IACKO,IAAIF,EAAK,CACNG,aAAc,SAEjBC,MAAK,SAACC,GACHC,IAAaD,EAAIE,KAAMN,OClB/BO,EAAY,KACZC,aAAanB,QAAQ,WACvBkB,EAAYC,aAAanB,QAAQ,SACjCG,EAAkBe,IAWpB,IAAME,EAAe,CACnBhB,MAAOc,EACPG,SAAU […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.68931b96.chunk.js",
-    "mappings": "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",
+    "file": "static/js/main.c4e40c36.chunk.js",
+    "mappings": "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",
     "names": [
         "getSessionId",
         "forceReload",
         "sessionId",
         "sessionStorage",
         "getItem",
         "uuidv4",
@@ -325,14 +325,15 @@
         "getSiteId",
         "getSiteWelcome",
         "welcome",
         "isPublic",
         "share",
         "fetchSite",
         "siteSlug",
+        "REACT_APP_SERVER_URL",
         "host",
         "origin",
         "endsWith",
         "status",
         "NotReady",
         "Loaded",
         "err",
@@ -414,14 +415,15 @@
         "runNotebook",
         "widgets_params",
         "purpose",
         "WebSocketContext",
         "createContext",
         "wsServer",
         "localServer",
+        "REACT_APP_SERVER_WS",
         "connectCounter",
         "globalConnection",
         "WebSocketProvider",
         "isStatic",
         "connection",
         "MAX_CONNECT_COUNT",
         "close",
@@ -776,26 +778,26 @@
         "/* eslint-disable import/no-cycle */\nimport { createSlice, PayloadAction } from \"@reduxjs/toolkit\";\nimport { RootState } from \"../store\";\n\nexport enum WebSocketState {\n  Connecting = \"Connecting\",\n  Connected = \"Connected\",\n  Unknown = \"Unknown\",\n  Disconnected = \"Disconnected\",\n}\n\nexport enum WorkerState {\n  Unknown = \"Unknown\",\n  Starting = \"Starting\",\n  Running = \"Running\",\n  Missing = \"Missing\",\n  Busy = \"Busy\",\n  Queued = \"Queued\",\n  MaxRunTimeReached = \"MaxRunTimeReached\",\n  MaxIdleTimeReached = \"MaxIdleTimeReached\",\n  UsageLimitReached = \"UsageLimitReached\",\n  //InstallPackages = \"InstallPackages\",\n}\n\nconst initialState = {\n  webSocketState: WebSocketState.Unknown,\n  workerState: WorkerState.Unknown,\n  workerId: undefined as undefined | number,\n  notebookSrc: \"\",\n  tryConnectCount: 0,\n};\n\nconst wsSlice = createSlice({\n  name: \"ws\",\n  initialState,\n  reducers: {\n    setWebSocketState(state, action: PayloadAction<WebSocketState>) {\n      state.webSocketState = action.payload;\n    },\n    setWorkerState(state, action: PayloadAction<WorkerState>) {\n      state.workerState = action.payload;\n    },\n    setWorkerId(state, action: PayloadAction<undefined | number>) {\n      state.workerId = action.payload;\n    },\n    setNotebookSrc(state, action: PayloadAction<string>) {\n      state.notebookSrc = action.payload;\n    },\n    increaseTryConnectCount(state) {\n      state.tryConnectCount += 1;\n    },\n    resetTryConnectCount(state) {\n      state.tryConnectCount = 0;\n    },\n  },\n});\n\nexport default wsSlice.reducer;\n\nexport const {\n  setWebSocketState,\n  setWorkerState,\n  setWorkerId,\n  setNotebookSrc,\n  increaseTryConnectCount,\n  resetTryConnectCount,\n} = wsSlice.actions;\n\nexport const getWebSocketState = (state: RootState) => state.ws.webSocketState;\nexport const getWorkerState = (state: RootState) => state.ws.workerState;\nexport const getWorkerId = (state: RootState) => state.ws.workerId;\nexport const getNotebookSrc = (state: RootState) => state.ws.notebookSrc;\nexport const getTryConnectCount = (state: RootState) =>\n  state.ws.tryConnectCount;\n\nexport const runNotebook = (widgets_params: string) => {\n  return {\n    purpose: \"run-notebook\",\n    widgets: widgets_params,\n  };\n};\n\nexport const saveNotebook = () => {\n  return {\n    purpose: \"save-notebook\",\n  };\n};\n\nexport const displayNotebook = (taskId: number) => {\n  return {\n    purpose: \"display-notebook\",\n    taskId,\n  };\n};\n\nexport const downloadHTML = () => {\n  return {\n    purpose: \"download-html\",\n  };\n};\n\nexport const downloadPDF = () => {\n  return {\n    purpose: \"download-pdf\",\n  };\n};\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\n\nimport ReactMarkdown from \"react-markdown\";\nimport rehypeHighlight from \"rehype-highlight\";\nimport remarkGfm from \"remark-gfm\";\nimport emoji from \"remark-emoji\";\nimport rehypeRaw from \"rehype-raw\";\n\ntype MarkdownProps = {\n  value: string;\n  disabled: boolean;\n};\n\nexport default function MarkdownWidget({ value, disabled }: MarkdownProps) {\n  return (\n    <div\n      className=\"form-group mb-3\"\n      style={{ color: disabled ? \"#555\" : \"#212529\" }}\n    >\n      <ReactMarkdown\n        rehypePlugins={[remarkGfm, rehypeHighlight, emoji, rehypeRaw]}\n      >\n        {value}\n      </ReactMarkdown>\n    </div>\n  );\n}\n",
         "import React, { createContext, useEffect } from \"react\";\nimport { useDispatch } from \"react-redux\";\nimport {\n  getSelectedNotebookId,\n  hideWidgets,\n  isStaticNotebook,\n  updateWidgetsParams,\n  initWidgets,\n  fetchNotebook,\n  updateTitle,\n  updateShowCode,\n  setWidgetsInitialized,\n} from \"../slices/notebooksSlice\";\nimport {\n  setNotebookSrc,\n  setWebSocketState,\n  setWorkerState,\n  setWorkerId,\n  WebSocketState,\n  WorkerState,\n  resetTryConnectCount,\n  increaseTryConnectCount,\n} from \"../slices/wsSlice\";\n\nimport { useSelector } from \"react-redux\";\nimport { getSessionId, handleDownload } from \"../utils\";\nimport { setExportingToPDF } from \"../slices/tasksSlice\";\nimport { getSiteId, setSiteStatus, SiteStatus } from \"../slices/sitesSlice\";\nimport { getToken } from \"../slices/authSlice\";\n\nconst WebSocketContext = createContext(undefined as any);\n\nexport { WebSocketContext };\n\nlet wsServer = \"ws://127.0.0.1:8000\";\nlet localServer = true;\nif (process.env.REACT_APP_SERVER_WS) {\n  wsServer = process.env.REACT_APP_SERVER_WS;\n  localServer = false;\n} else {\n  if (window.location.origin === \"http://localhost:3000\") {\n    wsServer = \"ws://127.0.0.1:8000\";\n    localServer = true;\n  } else {\n    wsServer = window.location.origin\n      .replace(\"http://\", \"ws://\")\n      .replace(\"https://\", \"wss://\");\n    localServer = false;\n  }\n}\n\nif (window.location.origin.endsWith(\"hf.space\")) {\n  wsServer = window.location.origin\n    .replace(\"http://\", \"ws://\")\n    .replace(\"https://\", \"wss://\");\n  localServer = false;\n}\n\nconst MAX_CONNECT_COUNT = 5;\nlet connectCounter = 0;\nlet globalConnection: WebSocket | undefined = undefined;\n\nexport default function WebSocketProvider({\n  children,\n}: {\n  children: JSX.Element;\n}) {\n  console.log(\"WebSocketProvider\");\n\n  const dispatch = useDispatch();\n  const siteId = useSelector(getSiteId);\n  const selectedNotebookId = useSelector(getSelectedNotebookId);\n  const token = useSelector(getToken);\n  const isStatic = useSelector(isStaticNotebook);\n\n  let connection: WebSocket | undefined = undefined;\n  let workerState = \"Unknown\" as WorkerState;\n\n  useEffect(() => {\n    connectCounter = 0;\n    // returned function will be called on component unmount\n    return () => {\n      connectCounter = MAX_CONNECT_COUNT + 1;\n      globalConnection?.close();\n    };\n    // eslint-disable-next-line react-hooks/exhaustive-deps\n  }, []);\n\n  const sendMessage = (payload: string) => {\n    if (connection !== undefined && connection.readyState === connection.OPEN) {\n      connection.send(payload);\n    }\n  };\n\n  function onOpen(event: any): void {\n    dispatch(resetTryConnectCount());\n    sendMessage(\n      JSON.stringify({\n        purpose: \"server-address\",\n        address: wsServer,\n      })\n    );\n    dispatch(setWebSocketState(WebSocketState.Connected));\n    ping();\n  }\n\n  function onMessage(event: any): void {\n    // console.log(\"reveived from server\", event.data);\n\n    const response = JSON.parse(event.data);\n    if (\"purpose\" in response) {\n      if (response.purpose === \"worker-state\") {\n        console.log(\"worker-state\", response.state);\n        workerState = response.state;\n\n        dispatch(setWorkerState(response.state));\n        dispatch(setWorkerId(response.workerId));\n\n        if (\n          workerState === WorkerState.MaxIdleTimeReached ||\n          workerState === WorkerState.MaxRunTimeReached\n        ) {\n          connection?.close();\n        }\n      } else if (response.purpose === \"executed-notebook\") {\n        //console.log(response?.reloadNotebook, selectedNotebookId);\n        if (response?.reloadNotebook && selectedNotebookId !== undefined) {\n          //console.log(\"reload notebook ...........................\");\n          dispatch(fetchNotebook(siteId, selectedNotebookId));\n        }\n        dispatch(setNotebookSrc(response.body));\n        // } else if (response.purpose === \"saved-notebook\") {\n        //   if (selectedNotebookId !== undefined) {\n        //     dispatch(fetchExecutionHistory(selectedNotebookId, false));\n        //   }\n      } else if (response.purpose === \"update-widgets\") {\n        dispatch(updateWidgetsParams(response));\n      } else if (response.purpose === \"hide-widgets\") {\n        dispatch(hideWidgets(response));\n      } else if (response.purpose === \"init-widgets\") {\n        dispatch(initWidgets(response));\n        dispatch(setWidgetsInitialized(true));\n      } else if (response.purpose === \"update-title\") {\n        dispatch(updateTitle(response.title));\n      } else if (response.purpose === \"update-show-code\") {\n        dispatch(updateShowCode(response.showCode));\n      } else if (\n        response.purpose === \"download-html\" ||\n        response.purpose === \"download-pdf\"\n      ) {\n        if (response.url && response.filename) {\n          dispatch(setExportingToPDF(false));\n          handleDownload(response.url, response.filename);\n        }\n      }\n    }\n  }\n\n  function onError(event: any): void {\n    dispatch(setWebSocketState(WebSocketState.Disconnected));\n    dispatch(setWorkerState(WorkerState.Unknown));\n  }\n\n  function onClose(event: any): void {\n    dispatch(setWebSocketState(WebSocketState.Disconnected));\n    connection = undefined;\n    if (\n      workerState !== WorkerState.MaxIdleTimeReached &&\n      workerState !== WorkerState.MaxRunTimeReached\n    ) {\n      dispatch(setWorkerState(WorkerState.Unknown));\n      dispatch(setWorkerId(undefined));\n      if (connectCounter < MAX_CONNECT_COUNT) {\n        setTimeout(() => connect(), 5000);\n      }\n    }\n  }\n\n  function ping(): void {\n    sendMessage(\n      JSON.stringify({\n        purpose: \"worker-ping\",\n      })\n    );\n    if (connection !== undefined && connection.readyState === connection.OPEN) {\n      setTimeout(() => ping(), 10000);\n    }\n  }\n\n  function connect() {\n    if (\n      (localServer || !isStatic) &&\n      selectedNotebookId !== undefined &&\n      connection === undefined &&\n      workerState !== WorkerState.MaxIdleTimeReached &&\n      workerState !== WorkerState.MaxRunTimeReached &&\n      connectCounter < MAX_CONNECT_COUNT\n    ) {\n      console.log(\"WS connect ...\" + workerState + \" \" + connectCounter);\n      dispatch(increaseTryConnectCount());\n      let url = `${wsServer}/ws/client/${selectedNotebookId}/${getSessionId()}/`;\n      if (token !== undefined && token !== null && token !== \"\") {\n        url += `?token=${token}`;\n      }\n      connection = new WebSocket(url);\n      connection.onopen = onOpen;\n      connection.onmessage = onMessage;\n      connection.onerror = onError;\n      connection.onclose = onClose;\n      connectCounter += 1;\n\n      globalConnection = connection;\n      if (connectCounter >= MAX_CONNECT_COUNT) {\n        dispatch(setSiteStatus(SiteStatus.NetworkError));\n      }\n    }\n  }\n  connect();\n\n  const ws = {\n    sendMessage,\n  };\n\n  return (\n    <WebSocketContext.Provider value={ws}>{children}</WebSocketContext.Provider>\n  );\n}\n",
         "import React, { useEffect, useState } from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\nimport { getSessionId, handleDownload } from \"../utils\";\nimport {\n  WorkerState,\n  WebSocketState,\n  getWebSocketState,\n  getWorkerState,\n  getTryConnectCount,\n} from \"../slices/wsSlice\";\nimport { setSiteStatus, SiteStatus } from \"../slices/sitesSlice\";\nimport axios from \"axios\";\nimport { exportToPDF, setExportingToPDF } from \"../slices/tasksSlice\";\nimport {\n  isCheckboxWidget,\n  isNumericWidget,\n  isRangeWidget,\n  isSelectWidget,\n  isSliderWidget,\n  isTextWidget,\n  IWidget,\n} from \"../widgets/Types\";\nimport { WidgetValueType } from \"../slices/notebooksSlice\";\n\ntype Props = {\n  allowDownload: boolean;\n  waiting: boolean;\n  continuousUpdate: boolean;\n  staticNotebook: boolean;\n  notebookId: number;\n  notebookPath: string;\n  notebookTitle: string;\n  runDownloadHTML: () => void;\n  runDownloadPDF: () => void;\n  widgetsValues: Record<string, WidgetValueType>;\n  widgetsParams: Record<string, IWidget>;\n};\n\nexport default function StatusBar({\n  allowDownload,\n  waiting,\n  continuousUpdate,\n  staticNotebook,\n  notebookId,\n  notebookPath,\n  notebookTitle,\n  runDownloadHTML,\n  runDownloadPDF,\n  widgetsValues,\n  widgetsParams,\n}: Props) {\n  const dispatch = useDispatch();\n  const [showShareModal, setShowShareModal] = useState(false);\n  const wsStatus = useSelector(getWebSocketState);\n  const workerState = useSelector(getWorkerState);\n  const tryConnectCount = useSelector(getTryConnectCount);\n\n  useEffect(() => {\n    if (tryConnectCount >= 5) {\n      dispatch(setSiteStatus(SiteStatus.LostConnection));\n    }\n  }, [dispatch, tryConnectCount]);\n\n  let wifiColor = \"orange\";\n  if (wsStatus === WebSocketState.Connected) {\n    wifiColor = \"green\";\n  } else if (\n    wsStatus === WebSocketState.Disconnected ||\n    wsStatus === WebSocketState.Unknown\n  ) {\n    wifiColor = \"red\";\n  }\n\n  let workerColor = \"orange\";\n  if (workerState === WorkerState.Running || workerState === WorkerState.Busy) {\n    workerColor = \"green\";\n  } else if (\n    workerState === WorkerState.Missing ||\n    workerState === WorkerState.Unknown\n  ) {\n    workerColor = \"red\";\n  }\n\n  let noUrlKeys = true;\n  let urlParams = \"?\";\n  if (\n    widgetsParams !== undefined &&\n    widgetsParams !== null &&\n    widgetsValues !== undefined &&\n    widgetsValues !== null\n  ) {\n    for (let [key, widgetParams] of Object.entries(widgetsParams)) {\n      if (widgetsValues[key] === undefined) {\n        continue;\n      }\n\n      if (\n        isCheckboxWidget(widgetParams) ||\n        isNumericWidget(widgetParams) ||\n        isRangeWidget(widgetParams) ||\n        isSelectWidget(widgetParams) ||\n        isSliderWidget(widgetParams) ||\n        isTextWidget(widgetParams)\n      ) {\n        if (widgetParams?.url_key !== null && widgetParams?.url_key !== \"\") {\n          noUrlKeys = false;\n        }\n      }\n\n      if (\n        isCheckboxWidget(widgetParams) ||\n        isNumericWidget(widgetParams) ||\n        isSliderWidget(widgetParams) ||\n        isTextWidget(widgetParams)\n      ) {\n        if (widgetParams?.url_key !== null && widgetParams?.url_key !== \"\") {\n          urlParams += `${widgetParams?.url_key}=${widgetsValues[key]}&`;\n        }\n      }\n\n      if (isRangeWidget(widgetParams)) {\n        if (widgetParams?.url_key !== null && widgetParams?.url_key !== \"\") {\n          const v = widgetsValues[key] as [number, number];\n\n          urlParams += `${widgetParams?.url_key}=${v[0]},${v[1]}&`;\n        }\n      }\n      if (isSelectWidget(widgetParams)) {\n        if (widgetParams?.url_key !== null && widgetParams?.url_key !== \"\") {\n          if (widgetParams?.multi) {\n            const v = widgetsValues[key] as string[];\n\n            urlParams += `${widgetParams?.url_key}=${v.join(\",\")}&`;\n          } else {\n            const v = widgetsValues[key] as string;\n            urlParams += `${widgetParams?.url_key}=${v}&`;\n          }\n        }\n      }\n    }\n    if (urlParams !== \"?\") {\n      urlParams = urlParams.slice(0, urlParams.length - 1);\n    }\n  }\n\n  return (\n    <div style={{ paddingBottom: \"25px\" }}>\n      {notebookId !== undefined && !staticNotebook && (\n        <>\n          <span title={`WebSocket: ${wsStatus}`}>\n            <svg\n              xmlns=\"http://www.w3.org/2000/svg\"\n              width=\"16\"\n              height=\"16\"\n              fill={wifiColor}\n              className=\"bi bi-wifi\"\n              viewBox=\"0 0 16 16\"\n            >\n              <path d=\"M15.384 6.115a.485.485 0 0 0-.047-.736A12.444 12.444 0 0 0 8 3C5.259 3 2.723 3.882.663 5.379a.485.485 0 0 0-.048.736.518.518 0 0 0 .668.05A11.448 11.448 0 0 1 8 4c2.507 0 4.827.802 6.716 2.164.205.148.49.13.668-.049z\" />\n              <path d=\"M13.229 8.271a.482.482 0 0 0-.063-.745A9.455 9.455 0 0 0 8 6c-1.905 0-3.68.56-5.166 1.526a.48.48 0 0 0-.063.745.525.525 0 0 0 .652.065A8.46 8.46 0 0 1 8 7a8.46 8.46 0 0 1 4.576 1.336c.206.132.48.108.653-.065zm-2.183 2.183c.226-.226.185-.605-.1-.75A6.473 6.473 0 0 0 8 9c-1.06 0-2.062.254-2.946.704-.285.145-.326.524-.1.75l.015.015c.16.16.407.19.611.09A5.478 5.478 0 0 1 8 10c.868 0 1.69.201 2.42.56.203.1.45.07.61-.091l.016-.015zM9.06 12.44c.196-.196.198-.52-.04-.66A1.99 1.99 0 0 0 8 11.5a1.99 1.99 0 0 0-1.02.28c-.238.14-.236.464-.04.66l.706.706a.5.5 0 0 0 .707 0l.707-.707z\" />\n            </svg>\n          </span>{\" \"}\n          <span title={`Worker: ${workerState}\\nSession Id: ${getSessionId()}`}>\n            <svg\n              xmlns=\"http://www.w3.org/2000/svg\"\n              width=\"16\"\n              height=\"16\"\n              fill={workerColor}\n              className=\"bi bi-cpu\"\n              viewBox=\"0 0 16 16\"\n            >\n              <path d=\"M5 0a.5.5 0 0 1 .5.5V2h1V.5a.5.5 0 0 1 1 0V2h1V.5a.5.5 0 0 1 1 0V2h1V.5a.5.5 0 0 1 1 0V2A2.5 2.5 0 0 1 14 4.5h1.5a.5.5 0 0 1 0 1H14v1h1.5a.5.5 0 0 1 0 1H14v1h1.5a.5.5 0 0 1 0 1H14v1h1.5a.5.5 0 0 1 0 1H14a2.5 2.5 0 0 1-2.5 2.5v1.5a.5.5 0 0 1-1 0V14h-1v1.5a.5.5 0 0 1-1 0V14h-1v1.5a.5.5 0 0 1-1 0V14h-1v1.5a.5.5 0 0 1-1 0V14A2.5 2.5 0 0 1 2 11.5H.5a.5.5 0 0 1 0-1H2v-1H.5a.5.5 0 0 1 0-1H2v-1H.5a.5.5 0 0 1 0-1H2v-1H.5a.5.5 0 0 1 0-1H2A2.5 2.5 0 0 1 4.5 2V.5A.5.5 0 0 1 5 0zm-.5 3A1.5 1.5 0 0 0 3 4.5v7A1.5 1.5 0 0 0 4.5 13h7a1.5 1.5 0 0 0 1.5-1.5v-7A1.5 1.5 0 0 0 11.5 3h-7zM5 6.5A1.5 1.5 0 0 1 6.5 5h3A1.5 1.5 0 0 1 11 6.5v3A1.5 1.5 0 0 1 9.5 11h-3A1.5 1.5 0 0 1 5 9.5v-3zM6.5 6a.5.5 0 0 0-.5.5v3a.5.5 0 0 0 .5.5h3a.5.5 0 0 0 .5-.5v-3a.5.5 0 0 0-.5-.5h-3z\" />\n            </svg>\n          </span>\n        </>\n      )}\n      {workerState === WorkerState.Busy && (\n        <span title=\"Worker is busy\">\n          {\" \"}\n          <svg\n            xmlns=\"http://www.w3.org/2000/svg\"\n            width=\"16\"\n            height=\"16\"\n            fill=\"green\"\n            className=\"bi bi-activity\"\n            viewBox=\"0 0 16 16\"\n          >\n            <path\n              fillRule=\"evenodd\"\n              d=\"M6 2a.5.5 0 0 1 .47.33L10 12.036l1.53-4.208A.5.5 0 0 1 12 7.5h3.5a.5.5 0 0 1 0 1h-3.15l-1.88 5.17a.5.5 0 0 1-.94 0L6 3.964 4.47 8.171A.5.5 0 0 1 4 8.5H.5a.5.5 0 0 1 0-1h3.15l1.88-5.17A.5.5 0 0 1 6 2Z\"\n            />\n          </svg>\n        </span>\n      )}\n      <div style={{ float: \"right\" }}>\n        {allowDownload && (\n          <div\n            className=\"dropdown mx-2 btn-group\"\n            style={{\n              display: \"inline\",\n              // width: \"47%\",\n              // float: continuousUpdate ? \"left\" : \"right\",\n            }}\n          >\n            <button\n              className=\"btn btn-sm btn-primary dropdown-toggle\"\n              // style={{ margin: \"0px\", width: \"100%\" }}\n              type=\"button\"\n              data-bs-toggle=\"dropdown\"\n              disabled={waiting}\n            >\n              <svg\n                xmlns=\"http://www.w3.org/2000/svg\"\n                width=\"14\"\n                height=\"14\"\n                viewBox=\"0 0 24 24\"\n                strokeWidth=\"2\"\n                stroke=\"currentColor\"\n                fill=\"none\"\n                strokeLinecap=\"round\"\n                strokeLinejoin=\"round\"\n                style={{ paddingBottom: \"1px\" }}\n              >\n                <path stroke=\"none\" d=\"M0 0h24v24H0z\" fill=\"none\"></path>\n                <path d=\"M4 17v2a2 2 0 0 0 2 2h12a2 2 0 0 0 2 -2v-2\"></path>\n                <path d=\"M7 11l5 5l5 -5\"></path>\n                <path d=\"M12 4l0 12\"></path>\n              </svg>{\" \"}\n              Download\n            </button>\n\n            {/* dropdown-menu-end */}\n            <ul className=\"dropdown-menu my-2\">\n              <li>\n                <button\n                  type=\"button\"\n                  style={{ cursor: \"pointer\" }}\n                  className=\"dropdown-item\"\n                  onClick={() => {\n                    if (staticNotebook) {\n                      handleDownload(\n                        `${axios.defaults.baseURL}${notebookPath}`,\n                        `${notebookTitle}.html`\n                      );\n                    } else {\n                      runDownloadHTML();\n                    }\n                  }}\n                >\n                  <i className=\"fa fa-file-code-o\" aria-hidden=\"true\"></i>{\" \"}\n                  Download as HTML\n                </button>\n              </li>\n              <li>\n                <hr className=\"dropdown-divider\" />\n              </li>\n              <li>\n                <button\n                  type=\"button\"\n                  className=\"dropdown-item\"\n                  onClick={() => {\n                    if (staticNotebook) {\n                      dispatch(exportToPDF(notebookId, notebookPath));\n                    } else {\n                      dispatch(setExportingToPDF(true));\n                      runDownloadPDF();\n                    }\n                  }}\n                >\n                  <i className=\"fa fa-file-pdf-o\" aria-hidden=\"true\"></i>{\" \"}\n                  Download as PDF\n                </button>\n              </li>\n            </ul>\n          </div>\n        )}\n        <button\n          className=\"btn btn-sm btn-primary\"\n          onClick={() => setShowShareModal(!showShareModal)}\n          disabled={waiting}\n        >\n          <svg\n            xmlns=\"http://www.w3.org/2000/svg\"\n            width=\"14\"\n            height=\"14\"\n            viewBox=\"0 0 24 24\"\n            strokeWidth=\"2\"\n            stroke=\"currentColor\"\n            fill=\"none\"\n            strokeLinecap=\"round\"\n            strokeLinejoin=\"round\"\n          >\n            <path stroke=\"none\" d=\"M0 0h24v24H0z\" fill=\"none\"></path>\n            <path d=\"M6 12m-3 0a3 3 0 1 0 6 0a3 3 0 1 0 -6 0\"></path>\n            <path d=\"M18 6m-3 0a3 3 0 1 0 6 0a3 3 0 1 0 -6 0\"></path>\n            <path d=\"M18 18m-3 0a3 3 0 1 0 6 0a3 3 0 1 0 -6 0\"></path>\n            <path d=\"M8.7 10.7l6.6 -3.4\"></path>\n            <path d=\"M8.7 13.3l6.6 3.4\"></path>\n          </svg>{\" \"}\n          Share\n        </button>\n      </div>\n\n      <div\n        className=\"\"\n        style={{\n          position: \"fixed\",\n          top: \"0\",\n          left: \"0\",\n          width: \"100%\",\n          height: \"100%\",\n          background: \"rgba(0, 0, 0, 0.6)\",\n          display: showShareModal ? \"block\" : \"none\",\n        }}\n      >\n        <section\n          className=\"\"\n          style={{\n            position: \"fixed\",\n            width: \"100%\",\n            height: \"auto\",\n            top: \"50%\",\n            left: \"50%\",\n            transform: \"translate(-50%,-50%)\",\n          }}\n        >\n          <div className=\"modal-dialog\">\n            <div className=\"modal-content\">\n              <div className=\"modal-header\">\n                <h3 className=\"modal-title\">\n                  <svg\n                    xmlns=\"http://www.w3.org/2000/svg\"\n                    width=\"24\"\n                    height=\"24\"\n                    viewBox=\"0 0 24 24\"\n                    strokeWidth=\"2\"\n                    stroke=\"currentColor\"\n                    fill=\"none\"\n                    strokeLinecap=\"round\"\n                    strokeLinejoin=\"round\"\n                  >\n                    <path stroke=\"none\" d=\"M0 0h24v24H0z\" fill=\"none\"></path>\n                    <path d=\"M6 12m-3 0a3 3 0 1 0 6 0a3 3 0 1 0 -6 0\"></path>\n                    <path d=\"M18 6m-3 0a3 3 0 1 0 6 0a3 3 0 1 0 -6 0\"></path>\n                    <path d=\"M18 18m-3 0a3 3 0 1 0 6 0a3 3 0 1 0 -6 0\"></path>\n                    <path d=\"M8.7 10.7l6.6 -3.4\"></path>\n                    <path d=\"M8.7 13.3l6.6 3.4\"></path>\n                  </svg>{\" \"}\n                  Share\n                </h3>\n                <button\n                  type=\"button\"\n                  className=\"btn-close\"\n                  aria-label=\"Close\"\n                  onClick={() => setShowShareModal(false)}\n                ></button>\n              </div>\n              <div className=\"modal-body\">\n                <div className=\"py-2\">\n                  <label>App address</label>\n                  <input\n                    type=\"text\"\n                    className=\"form-control\"\n                    disabled={true}\n                    value={window.location.href}\n                  ></input>\n                </div>\n\n                {!noUrlKeys && (\n                  <div className=\"py-2\">\n                    <label>App address with current paramters</label>\n                    <textarea\n                      rows={5}\n                      className=\"form-control\"\n                      disabled={true}\n                      value={window.location.href + urlParams}\n                    />\n                  </div>\n                )}\n                {noUrlKeys && (\n                  <div className=\"py-2\">\n                    There are no <code>url_key</code> defined for any widget.\n                    You can easily share URL to your notebook with preset values\n                    by using <code>url_key</code> in the widget. Please check{\" \"}\n                    <a\n                      href=\"https://runmercury.com/docs/input-widgets/\"\n                      target=\"_blank\"\n                      rel=\"noreferrer\"\n                    >\n                      documentation\n                    </a>\n                    .\n                  </div>\n                )}\n                <div className=\"py-2\"></div>\n              </div>\n              <div className=\"modal-footer\">\n                <button\n                  type=\"button\"\n                  className=\"btn btn-secondary\"\n                  onClick={() => setShowShareModal(false)}\n                >\n                  Close\n                </button>\n              </div>\n            </div>\n          </div>\n        </section>\n      </div>\n    </div>\n  );\n}\n",
         "import React, { useEffect } from \"react\";\nimport { useDispatch } from \"react-redux\";\nimport { setWidgetValue } from \"../slices/notebooksSlice\";\n\ntype ButtonProps = {\n  widgetKey: string;\n  label: string | null;\n  style: string;\n  value: string | boolean | null;\n  disabled: boolean;\n  hidden: boolean;\n  runNb: () => void;\n};\n\nexport default function ButtonWidget({\n  widgetKey,\n  label,\n  style,\n  value,\n  disabled,\n  hidden,\n  runNb,\n}: ButtonProps) {\n  const dispatch = useDispatch();\n\n  let selectedClass = \"btn-primary\";\n  if (style === \"success\") {\n    selectedClass = \"btn-success\";\n  } else if (style === \"danger\") {\n    selectedClass = \"btn-danger\";\n  } else if (style === \"info\") {\n    selectedClass = \"btn-info\";\n  } else if (style === \"warning\") {\n    selectedClass = \"btn-warning\";\n  }\n\n  useEffect(() => {\n    if (value) {\n      runNb();\n    }\n    // eslint-disable-next-line react-hooks/exhaustive-deps\n  }, [value]);\n\n  return (\n    <div className=\"form-group mb-3\" style={{ display: hidden ? \"none\" : \"\" }}>\n      <button\n        type=\"button\"\n        className={`btn ${selectedClass}`}\n        style={{ marginRight: \"10px\", width: \"47%\" }}\n        onClick={() => {\n          dispatch(\n            setWidgetValue({\n              key: widgetKey,\n              value: true,\n            })\n          );\n        }}\n        disabled={disabled}\n      >\n        {label}\n      </button>\n    </div>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\nimport { WorkerState } from \"../slices/wsSlice\";\n\ntype RunButtonProps = {\n  runNb: () => void;\n  waiting: boolean;\n  workerState: WorkerState;\n};\n\nexport default function RunButton({\n  runNb,\n  waiting,\n  workerState,\n}: RunButtonProps) {\n  return (\n    <button\n      type=\"button\"\n      className=\"btn btn-success\"\n      style={{ marginRight: \"10px\", width: \"100%\" }}\n      onClick={() => {\n        runNb();\n      }}\n      disabled={\n        waiting ||\n        // !allFilesUploaded() ||\n        workerState !== WorkerState.Running\n      }\n    >\n      {workerState === WorkerState.Running && (\n        <span>\n          <i className=\"fa fa-play\" aria-hidden=\"true\"></i> Run\n        </span>\n      )}\n      {workerState === WorkerState.Busy && (\n        <span>\n          <svg\n            xmlns=\"http://www.w3.org/2000/svg\"\n            width=\"16\"\n            height=\"16\"\n            fill=\"white\"\n            className=\"bi bi-activity\"\n            viewBox=\"0 0 16 16\"\n          >\n            <path\n              fillRule=\"evenodd\"\n              d=\"M6 2a.5.5 0 0 1 .47.33L10 12.036l1.53-4.208A.5.5 0 0 1 12 7.5h3.5a.5.5 0 0 1 0 1h-3.15l-1.88 5.17a.5.5 0 0 1-.94 0L6 3.964 4.47 8.171A.5.5 0 0 1 4 8.5H.5a.5.5 0 0 1 0-1h3.15l1.88-5.17A.5.5 0 0 1 6 2Z\"\n            />\n          </svg>{\" \"}\n          Busy\n        </span>\n      )}\n      {workerState !== WorkerState.Busy &&\n        workerState !== WorkerState.Running && <span>Waiting ...</span>}\n    </button>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React, { useContext } from \"react\";\nimport { useEffect } from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\nimport {\n  scrapeSlidesHash,\n} from \"../slices/tasksSlice\";\nimport CheckboxWidget from \"../widgets/Checkbox\";\nimport NumericWidget from \"../widgets/Numeric\";\nimport RangeWidget from \"../widgets/Range\";\nimport SelectWidget from \"../widgets/Select\";\nimport SliderWidget from \"../widgets/Slider\";\n\nimport {\n  isCheckboxWidget,\n  isFileWidget,\n  isNumericWidget,\n  isRangeWidget,\n  isSelectWidget,\n  isSliderWidget,\n  isTextWidget,\n  isMarkdownWidget,\n  IWidget,\n  isOutputFilesWidget,\n  isButtonWidget,\n} from \"../widgets/Types\";\n\nimport {\n  clearWidgetsUrlValues,\n  getUrlValuesUsed,\n  getWidgetsInitialized,\n  getWidgetsUrlValues,\n  getWidgetsValues,\n  setSlidesHash,\n  setUrlValuesUsed,\n  setWidgetsInitialized,\n  setWidgetValue,\n  WidgetValueType,\n} from \"../slices/notebooksSlice\";\nimport FileWidget from \"../widgets/File\";\nimport TextWidget from \"../widgets/Text\";\nimport { setShowSideBar, setView } from \"../slices/appSlice\";\nimport MarkdownWidget from \"../widgets/Markdown\";\n\nimport { WebSocketContext } from \"../websocket/Provider\";\nimport WebSocketStateBar from \"./StatusBar\";\nimport {\n  downloadHTML,\n  downloadPDF,\n  getWorkerState,\n  runNotebook,\n  WorkerState,\n} from \"../slices/wsSlice\";\nimport ButtonWidget from \"../widgets/Button\";\nimport RunButton from \"./RunButton\";\nimport BlockUi from \"react-block-ui\";\n\ntype SideBarProps = {\n  notebookTitle: string;\n  notebookId: number;\n  notebookSchedule: string;\n  taskCreatedAt: Date;\n  loadingState: string;\n  waiting: boolean;\n  widgetsParams: Record<string, IWidget>;\n  watchMode: boolean;\n  notebookPath: string;\n  displayEmbed: boolean;\n  showFiles: boolean;\n  isPresentation: boolean;\n  notebookParseErrors: string;\n  continuousUpdate: boolean;\n  staticNotebook: boolean;\n  allowDownload: boolean;\n};\n\nexport default function SideBar({\n  notebookTitle,\n  notebookId,\n  notebookSchedule,\n  taskCreatedAt,\n  loadingState,\n  waiting,\n  widgetsParams,\n  watchMode,\n  notebookPath,\n  displayEmbed,\n  showFiles,\n  isPresentation,\n  notebookParseErrors,\n  continuousUpdate,\n  staticNotebook,\n  allowDownload,\n}: SideBarProps) {\n  const dispatch = useDispatch();\n  const widgetsValues: Record<string, WidgetValueType> = useSelector(\n    getWidgetsValues\n  ) as Record<string, WidgetValueType>;\n  const widgetsUrlValues = useSelector(getWidgetsUrlValues);\n  const workerState = useSelector(getWorkerState);\n  const widgetsInitialized = useSelector(getWidgetsInitialized);\n  const urlValuesUsed = useSelector(getUrlValuesUsed);\n\n  const ws = useContext(WebSocketContext);\n\n  const runNb = () => {\n    if (continuousUpdate) {\n      execNb();\n    }\n  };\n\n  const execNb = () => {\n    const slidesHash = scrapeSlidesHash();\n    dispatch(setSlidesHash(slidesHash));\n\n    if (widgetsUrlValues) {\n      let params = {} as Record<string, WidgetValueType>;\n      // eslint-disable-next-line @typescript-eslint/no-unused-vars\n      for (let [key, widgetParams] of Object.entries(widgetsParams)) {\n        if (key in widgetsUrlValues) {\n          params[key] = widgetsUrlValues[key];\n          dispatch(setWidgetValue({ key, value: params[key] }));\n        } else if (key in widgetsValues) {\n          params[key] = widgetsValues[key];\n        }\n      }\n      ws.sendMessage(JSON.stringify(runNotebook(JSON.stringify(params))));\n      dispatch(clearWidgetsUrlValues());\n    } else {\n      ws.sendMessage(\n        JSON.stringify(runNotebook(JSON.stringify(widgetsValues)))\n      );\n    }\n  };\n\n  useEffect(() => {\n    if (widgetsInitialized && urlValuesUsed) {\n      execNb();\n      dispatch(setUrlValuesUsed(false));\n      dispatch(setWidgetsInitialized(false));\n    }\n    // eslint-disable-next-line react-hooks/exhaustive-deps\n  }, [widgetsInitialized, urlValuesUsed]);\n\n  const runDownloadHTML = () => {\n    if (!staticNotebook) {\n      ws.sendMessage(JSON.stringify(downloadHTML()));\n    }\n  };\n\n  const runDownloadPDF = () => {\n    if (!staticNotebook) {\n      ws.sendMessage(JSON.stringify(downloadPDF()));\n    }\n  };\n\n  useEffect(() => {\n    if (widgetsParams) {\n      for (let [key, widgetParams] of Object.entries(widgetsParams)) {\n        if (key in widgetsValues) {\n          continue;\n        }\n\n        if (widgetParams.input === \"file\") {\n          dispatch(setWidgetValue({ key, value: [] as string[] }));\n        } else if (widgetParams.input === \"text\") {\n          dispatch(\n            setWidgetValue({\n              key,\n              value: widgetParams.value ? widgetParams.value : \"\",\n            })\n          );\n        } else if (isMarkdownWidget(widgetParams)) {\n          // do nothing\n          // dont put value into store\n        } else if (isOutputFilesWidget(widgetParams)) {\n          dispatch(setWidgetValue({ key, value: \"output-dir\" }));\n        } else {\n          dispatch(setWidgetValue({ key, value: widgetParams.value }));\n        }\n      }\n    }\n  }, [dispatch, widgetsParams, widgetsValues]);\n\n  let widgets = [];\n  let fileKeys = [] as string[]; // keys to file widgets, all need to be selected to enable RUN button\n\n  if (widgetsParams && !staticNotebook) {\n    // sort widgets keys based on cell index and code line number\n    let widgetKeys = [];\n    for (let key of Object.keys(widgetsParams)) {\n      const parts = key.split(\".\");\n      widgetKeys.push([key, parseFloat(`${parts[1]}.${parts[2]}`)]);\n    }\n    widgetKeys.sort(function (a, b) {\n      const a1 = a[1] as number;\n      const b1 = b[1] as number;\n      return a1 - b1;\n    });\n\n    for (let wKey of widgetKeys) {\n      const key = wKey[0] as string;\n      const widgetParams = widgetsParams[key];\n\n      if (isSelectWidget(widgetParams)) {\n        widgets.push(\n          <SelectWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            value={widgetsValues[key] as string}\n            choices={widgetParams?.choices}\n            multi={widgetParams?.multi}\n            key={key}\n            runNb={runNb}\n            url_key={widgetParams?.url_key}\n          />\n        );\n      } else if (isCheckboxWidget(widgetParams)) {\n        widgets.push(\n          <CheckboxWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            value={widgetsValues[key] as boolean}\n            key={key}\n            runNb={runNb}\n            url_key={widgetParams?.url_key}\n          />\n        );\n      } else if (isNumericWidget(widgetParams)) {\n        widgets.push(\n          <NumericWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            value={widgetsValues[key] as number}\n            min={widgetParams?.min}\n            max={widgetParams?.max}\n            step={widgetParams?.step}\n            key={key}\n            runNb={runNb}\n            continuousUpdate={continuousUpdate}\n            url_key={widgetParams?.url_key}\n          />\n        );\n      } else if (isSliderWidget(widgetParams)) {\n        widgets.push(\n          <SliderWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            value={widgetsValues[key] as number}\n            min={widgetParams?.min}\n            max={widgetParams?.max}\n            step={widgetParams?.step}\n            vertical={widgetParams?.vertical}\n            key={key}\n            runNb={runNb}\n            url_key={widgetParams?.url_key}\n          />\n        );\n      } else if (isRangeWidget(widgetParams)) {\n        widgets.push(\n          <RangeWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            value={widgetsValues[key] as [number, number]}\n            min={widgetParams?.min}\n            max={widgetParams?.max}\n            step={widgetParams?.step}\n            vertical={widgetParams?.vertical}\n            key={key}\n            runNb={runNb}\n            url_key={widgetParams.url_key}\n          />\n        );\n      } else if (isFileWidget(widgetParams)) {\n        widgets.push(\n          <FileWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            maxFileSize={widgetParams?.maxFileSize}\n            key={key}\n            value={widgetsValues[key] as string[]}\n            runNb={runNb}\n          />\n        );\n        fileKeys.push(key);\n      } else if (isTextWidget(widgetParams)) {\n        widgets.push(\n          <TextWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            value={widgetsValues[key] as string}\n            rows={widgetParams?.rows}\n            key={key}\n            runNb={runNb}\n            continuousUpdate={continuousUpdate}\n            url_key={widgetParams?.url_key}\n          />\n        );\n      } else if (isMarkdownWidget(widgetParams)) {\n        widgets.push(\n          <MarkdownWidget\n            value={widgetParams.value as string}\n            disabled={waiting}\n            key={key}\n          />\n        );\n      } else if (isButtonWidget(widgetParams)) {\n        widgets.push(\n          <ButtonWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            value={widgetsValues[key] as boolean}\n            style={widgetParams?.style}\n            key={key}\n            runNb={runNb}\n          />\n        );\n      } else if (isOutputFilesWidget(widgetParams)) {\n        // do nothing\n      } else {\n        console.log(\"Unknown widget type\", widgetParams);\n      }\n    }\n  }\n\n  let additionalStyle = {};\n  if (displayEmbed) {\n    additionalStyle = { padding: \"0px\" };\n  }\n\n  const addSpaceInsteadTitle =\n    notebookTitle === undefined ||\n    notebookTitle === null ||\n    notebookTitle === \"\";\n\n  return (\n    <nav\n      id=\"sidebarMenu\"\n      className=\"col-lg-3 d-md-block bg-light sidebar\"\n      style={{ ...additionalStyle, overflowY: \"auto\" }}\n    >\n      <BlockUi blocking={false} message=\"\">\n        <div className=\"position-sticky p-3\">\n          <h4>\n            {notebookTitle}\n            <button\n              className=\"btn btn-sm  btn-outline-primary\"\n              type=\"button\"\n              style={{\n                float: \"right\",\n                zIndex: \"101\",\n              }}\n              onClick={() => dispatch(setShowSideBar(false))}\n              data-toggle=\"tooltip\"\n              data-placement=\"right\"\n              title=\"Hide sidebar\"\n            >\n              <i className=\"fa fa-chevron-left\" aria-hidden=\"true\" />\n            </button>\n          </h4>\n\n          <div style={{ padding: \"0px\" }}>\n            <form>\n              {widgets}\n\n              {addSpaceInsteadTitle && <div style={{ padding: \"15px\" }}></div>}\n\n              <div className=\"form-group mb-3 pb-1 pt-2\">\n                {!continuousUpdate && (\n                  <RunButton\n                    runNb={execNb}\n                    waiting={waiting}\n                    workerState={workerState}\n                  />\n                )}\n              </div>\n\n              {workerState === WorkerState.UsageLimitReached && (\n                <div className=\"alert alert-info mb-3 mt-3\" role=\"alert\">\n                  <i className=\"fa fa-info-circle\" aria-hidden=\"true\"></i> Usage\n                  limit was reached. Please upgrade the plan.\n                </div>\n              )}\n\n              {workerState === WorkerState.MaxIdleTimeReached && (\n                <div className=\"alert alert-info mb-3 mt-3\" role=\"alert\">\n                  <i className=\"fa fa-info-circle\" aria-hidden=\"true\"></i> Your\n                  worker was idle for too long, that's why we have stopped it.\n                  Do you need a worker?\n                  <br />\n                  <button\n                    className=\"btn btn-sm btn-primary my-2\"\n                    onClick={() => window.location.reload()}\n                  >\n                    Restart worker\n                  </button>\n                </div>\n              )}\n              {workerState === WorkerState.MaxRunTimeReached && (\n                <div className=\"alert alert-info mb-3 mt-3\" role=\"alert\">\n                  <i className=\"fa fa-info-circle\" aria-hidden=\"true\"></i> Your\n                  worker was running for too long, that's why we have stopped\n                  it. Do you need a worker?\n                  <br />\n                  <button\n                    className=\"btn btn-sm btn-primary my-2\"\n                    onClick={() => window.location.reload()}\n                  >\n                    Restart worker\n                  </button>\n                </div>\n              )}\n              {waiting &&\n                (workerState === WorkerState.Unknown ||\n                  workerState === WorkerState.Queued) && (\n                  <div className=\"alert alert-warning mb-3 mt-3\" role=\"alert\">\n                    <i className=\"fa fa-cogs\" aria-hidden=\"true\"></i> Waiting\n                    for worker ...\n                  </div>\n                )}\n              {waiting && workerState === WorkerState.Starting && (\n                <div className=\"alert alert-success mb-3 mt-3\" role=\"alert\">\n                  <i className=\"fa fa-cogs\" aria-hidden=\"true\"></i> Initializing\n                  worker ...\n                </div>\n              )}\n              {watchMode && (\n                <div className=\"alert alert-secondary mb-3 mt-3\" role=\"alert\">\n                  <i className=\"fa fa-refresh\" aria-hidden=\"true\"></i> Notebook\n                  in watch mode. All changes to Notebook will be automatically\n                  visible in Mercury.\n                </div>\n              )}\n\n              {isPresentation && (\n                <div className=\"alert alert-primary mb-3\" role=\"alert\">\n                  <i className=\"fa fa-television\" aria-hidden=\"true\"></i> Click\n                  on presentation and press <b>F</b> for full screen. Press{\" \"}\n                  <b>Esc</b> to quit.\n                  <br />\n                  <br />\n                  <i className=\"fa fa-arrows\" aria-hidden=\"true\"></i> Click on\n                  presentation and press <b>Esc</b> to navigate slides.\n                </div>\n              )}\n\n              {/* {notebookParseErrors && (\n                <div className=\"alert alert-danger mb-3\" role=\"alert\">\n                  <i\n                    className=\"fa fa-exclamation-circle\"\n                    aria-hidden=\"true\"\n                  ></i>{\" \"}\n                  <b>Errors in the YAML</b>\n                  <br />\n                  {notebookParseErrors}\n                </div>\n              )} */}\n            </form>\n          </div>\n\n          {showFiles && (\n            <div>\n              <hr />\n              <button\n                className=\"btn btn-sm btn-outline-secondary\"\n                style={{\n                  border: \"none\",\n                  //fontWeight: 500,\n                }}\n                onClick={() => {\n                  dispatch(setView(\"app\"));\n                }}\n              >\n                <i className=\"fa fa-laptop\" aria-hidden=\"true\"></i> App\n              </button>\n\n              <button\n                className=\"btn btn-sm btn-outline-secondary\"\n                style={{\n                  border: \"none\",\n                  //fontWeight: 500,\n                }}\n                onClick={() => {\n                  dispatch(setView(\"files\"));\n                }}\n              >\n                <i className=\"fa fa-folder-open-o\" aria-hidden=\"true\"></i>{\" \"}\n                Output Files\n              </button>\n            </div>\n          )}\n\n          <div>\n            <hr />\n            <div style={{ paddingLeft: \"10px\" }}>\n              <WebSocketStateBar\n                notebookId={notebookId}\n                notebookPath={notebookPath}\n                notebookTitle={notebookTitle}\n                staticNotebook={staticNotebook}\n                allowDownload={allowDownload}\n                waiting={waiting}\n                continuousUpdate={continuousUpdate}\n                runDownloadHTML={runDownloadHTML}\n                runDownloadPDF={runDownloadPDF}\n                widgetsValues={widgetsValues}\n                widgetsParams={widgetsParams}\n              />{\" \"}\n            </div>\n          </div>\n        </div>\n      </BlockUi>\n    </nav>\n  );\n}\n",
-        "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React, { useEffect } from \"react\";\nimport axios from \"axios\";\nimport useWindowDimensions from \"./WindowDimensions\";\n\nimport BlockUi from \"react-block-ui\";\nimport { useDispatch, useSelector } from \"react-redux\";\nimport { getNotebookSrc, setNotebookSrc } from \"../slices/wsSlice\";\n\nimport InnerHTML from \"dangerously-set-html-content\";\nimport { getSelectedNotebook } from \"../slices/notebooksSlice\";\n\ntype MainViewProps = {\n  appView: string;\n  loadingState: string;\n  notebookPath: string;\n  waiting: boolean;\n  errorMsg: string;\n  watchMode: boolean;\n  displayEmbed: boolean;\n  username: string;\n  slidesHash: string;\n  columnsWidth: number;\n  isPresentation: boolean;\n  fullScreen: boolean;\n};\n\nexport default function MainView({\n  appView,\n  loadingState,\n  notebookPath,\n  waiting,\n  errorMsg,\n  watchMode,\n  displayEmbed,\n  username,\n  slidesHash,\n  columnsWidth,\n  isPresentation,\n  fullScreen,\n}: MainViewProps) {\n  const { height } = useWindowDimensions();\n\n  const iframeHeight = displayEmbed ? height - 10 : height - 58;\n  const dispatch = useDispatch();\n  let nb = useSelector(getSelectedNotebook);\n  let notebookSrc = useSelector(getNotebookSrc);\n\n  let showCode = false;\n  if (nb !== undefined && nb.params !== undefined) {\n    if (\n      nb.params[\"show-code\"] !== undefined &&\n      nb.params[\"show-code\"] !== null\n    ) {\n      showCode = nb.params[\"show-code\"];\n    }\n  }\n\n  if (notebookSrc !== \"\" && !isPresentation) {\n    notebookSrc = \"<script>init_mathjax();</script>\" + notebookSrc;\n\n    if (!showCode) {\n      const hideCodeStyle = `<style type=\"text/css\">\n      .jp-mod-noOutputs {\n          padding: 0px; \n      }\n      .jp-mod-noInput {\n        padding-top: 0px;\n        padding-bottom: 0px;\n      }\n      </style>`;\n      notebookSrc = hideCodeStyle + notebookSrc;\n    }\n  }\n\n  if (notebookSrc !== \"\" && isPresentation && slidesHash !== \"\") {\n    if (notebookSrc.indexOf(\"Reveal.slide(\") === -1) {\n      const splitted = slidesHash.split(\"/\");\n      let injectCode = \"\";\n      if (splitted.length === 4) {\n        injectCode = `Reveal.slide(${splitted[1]}, ${splitted[2]}, ${splitted[3]});`;\n      } else if (splitted.length === 3) {\n        injectCode = `Reveal.slide(${splitted[1]}, ${splitted[2]});`;\n      } else if (splitted.length === 2) {\n        injectCode = `Reveal.slide(${splitted[1]});`;\n      }\n\n      if (injectCode !== \"\") {\n        notebookSrc = notebookSrc.replace(\n          \"setScrollingSlide);\",\n          `setScrollingSlide); try{ ${injectCode} } catch(error) {}`\n        );\n      }\n    }\n  }\n\n  useEffect(() => {\n    if (notebookPath !== undefined) {\n      \n      let nbPath = notebookPath;\n      if (window.location.origin.startsWith(\"https\")) {\n        nbPath = nbPath.replace(\"http://\", \"https://\");\n      }\n\n      axios.get(`${nbPath}${slidesHash}`).then((response) => {\n        let nbSrc = response.data;\n        if (!isPresentation) {\n          nbSrc = nbSrc.replace(/<head>[\\s\\S]*?<\\/head>/, \"\");\n          nbSrc = nbSrc.replace(\"<html>\", \"\");\n          nbSrc = nbSrc.replace(\"</html>\", \"\");\n          nbSrc = nbSrc.replace(\"<body\", \"<div\");\n          nbSrc = nbSrc.replace(\"</body>\", \"</div>\");\n          nbSrc = nbSrc.replace(\"<!DOCTYPE html>\", \"\");\n        }\n        dispatch(setNotebookSrc(nbSrc));\n      });\n    }\n  }, [dispatch, notebookPath, slidesHash, isPresentation]);\n\n  let mainStyle = {\n    paddingTop: \"0px\",\n    paddingRight: \"0px\",\n    paddingLeft: fullScreen ? \"12px\" : \"0px\",\n    display: appView === \"files\" ? \"none\" : \"block\",\n  };\n\n  let divStyle = {};\n  if (!fullScreen) {\n    divStyle = { maxWidth: \"1140px\", margin: \"auto\" };\n  }\n\n  // hide blocking for small screens when sidebar is only showed\n  // because it causes some strange shadow\n  // see https://github.com/mljar/mercury/issues/250\n  let hideBlockUi = false;\n  if (columnsWidth < 12 && window.innerWidth < 992) {\n    hideBlockUi = true;\n  }\n\n  return (\n    <main className={`ms-sm-auto col-${columnsWidth}`} style={mainStyle}>\n      <BlockUi tag=\"div\" blocking={!hideBlockUi && waiting}>\n        <div style={divStyle}>\n          {loadingState === \"loading\" && !watchMode && (\n            <p>Loading notebook. Please wait ...</p>\n          )}\n          {loadingState === \"error\" && (\n            <p style={{ margin: \"20px\" }}>\n              Problem while loading notebook. Please try again later or contact\n              Mercury administrator.\n            </p>\n          )}\n\n          {loadingState === \"error\" && username === \"\" && (\n            <p style={{ margin: \"20px\" }}>\n              <h5>Please log in to see the notebook</h5>\n              <a href=\"/login\" className=\"btn btn-primary btn-sm \">\n                <i className=\"fa fa-sign-in\" aria-hidden=\"true\"></i> Log in\n              </a>\n            </p>\n          )}\n\n          {errorMsg && (\n            <div className=\"alert alert-danger mb-3\" role=\"alert\">\n              <b>Notebook is executed with errors.</b>\n              <p>{errorMsg}</p>\n            </div>\n          )}\n\n          {errorMsg === \"\" &&\n            loadingState !== \"loading\" &&\n            isPresentation &&\n            notebookSrc !== \"\" && (\n              <iframe\n                width=\"100%\"\n                height={iframeHeight}\n                key={notebookPath}\n                srcDoc={notebookSrc}\n                title=\"display\"\n                id=\"main-iframe\"\n                onError={() => {\n                  console.log(\"iframe error\");\n                }}\n              ></iframe>\n            )}\n\n          {notebookSrc !== \"\" && !isPresentation && (\n            <InnerHTML html={notebookSrc} />\n          )}\n        </div>\n      </BlockUi>\n    </main>\n  );\n}\n",
+        "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React, { useEffect } from \"react\";\nimport axios from \"axios\";\nimport useWindowDimensions from \"./WindowDimensions\";\n\nimport BlockUi from \"react-block-ui\";\nimport { useDispatch, useSelector } from \"react-redux\";\nimport { getNotebookSrc, setNotebookSrc } from \"../slices/wsSlice\";\n\nimport InnerHTML from \"dangerously-set-html-content\";\nimport { getSelectedNotebook } from \"../slices/notebooksSlice\";\n\ntype MainViewProps = {\n  appView: string;\n  loadingState: string;\n  notebookPath: string;\n  waiting: boolean;\n  errorMsg: string;\n  watchMode: boolean;\n  displayEmbed: boolean;\n  username: string;\n  slidesHash: string;\n  columnsWidth: number;\n  isPresentation: boolean;\n  fullScreen: boolean;\n};\n\nexport default function MainView({\n  appView,\n  loadingState,\n  notebookPath,\n  waiting,\n  errorMsg,\n  watchMode,\n  displayEmbed,\n  username,\n  slidesHash,\n  columnsWidth,\n  isPresentation,\n  fullScreen,\n}: MainViewProps) {\n  const { height } = useWindowDimensions();\n\n  const iframeHeight = displayEmbed ? height - 10 : height - 58;\n  const dispatch = useDispatch();\n  let nb = useSelector(getSelectedNotebook);\n  let notebookSrc = useSelector(getNotebookSrc);\n\n  let showCode = false;\n  if (nb !== undefined && nb.params !== undefined) {\n    if (\n      nb.params[\"show-code\"] !== undefined &&\n      nb.params[\"show-code\"] !== null\n    ) {\n      showCode = nb.params[\"show-code\"];\n    }\n  }\n\n  if (notebookSrc !== \"\" && !isPresentation) {\n    notebookSrc = \"<script>init_mathjax();</script>\" + notebookSrc;\n\n    if (!showCode) {\n      const hideCodeStyle = `<style type=\"text/css\">\n      .jp-mod-noOutputs {\n          padding: 0px; \n      }\n      .jp-mod-noInput {\n        padding-top: 0px;\n        padding-bottom: 0px;\n      }\n      </style>`;\n      notebookSrc = hideCodeStyle + notebookSrc;\n    }\n  }\n\n  if (notebookSrc !== \"\" && isPresentation && slidesHash !== \"\") {\n    if (notebookSrc.indexOf(\"Reveal.slide(\") === -1) {\n      const splitted = slidesHash.split(\"/\");\n      let injectCode = \"\";\n      if (splitted.length === 4) {\n        injectCode = `Reveal.slide(${splitted[1]}, ${splitted[2]}, ${splitted[3]});`;\n      } else if (splitted.length === 3) {\n        injectCode = `Reveal.slide(${splitted[1]}, ${splitted[2]});`;\n      } else if (splitted.length === 2) {\n        injectCode = `Reveal.slide(${splitted[1]});`;\n      }\n\n      if (injectCode !== \"\") {\n        notebookSrc = notebookSrc.replace(\n          \"setScrollingSlide);\",\n          `setScrollingSlide); try{ ${injectCode} } catch(error) {}`\n        );\n      }\n    }\n  }\n\n  useEffect(() => {\n    if (notebookPath !== undefined) {\n      \n      let nbPath = notebookPath;\n      \n      if (window.location.origin.startsWith(\"https\")) {\n        nbPath = nbPath.replace(\"http://\", \"https://\");\n      }\n      if (window.location.origin === \"http://localhost:3000\") {\n        if (nbPath.startsWith(\"/media\")) {\n          nbPath = \"https://127.0.0.1:8000\" + nbPath;\n        }\n      }\n\n      axios.get(`${nbPath}${slidesHash}`).then((response) => {\n        let nbSrc = response.data;\n        if (!isPresentation) {\n          nbSrc = nbSrc.replace(/<head>[\\s\\S]*?<\\/head>/, \"\");\n          nbSrc = nbSrc.replace(\"<html>\", \"\");\n          nbSrc = nbSrc.replace(\"</html>\", \"\");\n          nbSrc = nbSrc.replace(\"<body\", \"<div\");\n          nbSrc = nbSrc.replace(\"</body>\", \"</div>\");\n          nbSrc = nbSrc.replace(\"<!DOCTYPE html>\", \"\");\n        }\n        dispatch(setNotebookSrc(nbSrc));\n      });\n    }\n  }, [dispatch, notebookPath, slidesHash, isPresentation]);\n\n  let mainStyle = {\n    paddingTop: \"0px\",\n    paddingRight: \"0px\",\n    paddingLeft: fullScreen ? \"12px\" : \"0px\",\n    display: appView === \"files\" ? \"none\" : \"block\",\n  };\n\n  let divStyle = {};\n  if (!fullScreen) {\n    divStyle = { maxWidth: \"1140px\", margin: \"auto\" };\n  }\n\n  // hide blocking for small screens when sidebar is only showed\n  // because it causes some strange shadow\n  // see https://github.com/mljar/mercury/issues/250\n  let hideBlockUi = false;\n  if (columnsWidth < 12 && window.innerWidth < 992) {\n    hideBlockUi = true;\n  }\n\n  return (\n    <main className={`ms-sm-auto col-${columnsWidth}`} style={mainStyle}>\n      <BlockUi tag=\"div\" blocking={!hideBlockUi && waiting}>\n        <div style={divStyle}>\n          {loadingState === \"loading\" && !watchMode && (\n            <p>Loading notebook. Please wait ...</p>\n          )}\n          {loadingState === \"error\" && (\n            <p style={{ margin: \"20px\" }}>\n              Problem while loading notebook. Please try again later or contact\n              Mercury administrator.\n            </p>\n          )}\n\n          {loadingState === \"error\" && username === \"\" && (\n            <p style={{ margin: \"20px\" }}>\n              <h5>Please log in to see the notebook</h5>\n              <a href=\"/login\" className=\"btn btn-primary btn-sm \">\n                <i className=\"fa fa-sign-in\" aria-hidden=\"true\"></i> Log in\n              </a>\n            </p>\n          )}\n\n          {errorMsg && (\n            <div className=\"alert alert-danger mb-3\" role=\"alert\">\n              <b>Notebook is executed with errors.</b>\n              <p>{errorMsg}</p>\n            </div>\n          )}\n\n          {errorMsg === \"\" &&\n            loadingState !== \"loading\" &&\n            isPresentation &&\n            notebookSrc !== \"\" && (\n              <iframe\n                width=\"100%\"\n                height={iframeHeight}\n                key={notebookPath}\n                srcDoc={notebookSrc}\n                title=\"display\"\n                id=\"main-iframe\"\n                onError={() => {\n                  console.log(\"iframe error\");\n                }}\n              ></iframe>\n            )}\n\n          {notebookSrc !== \"\" && !isPresentation && (\n            <InnerHTML html={notebookSrc} />\n          )}\n        </div>\n      </BlockUi>\n    </main>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\nimport { useDispatch } from \"react-redux\";\nimport axios from \"axios\";\nimport fileDownload from \"js-file-download\";\nimport BlockUi from \"react-block-ui\";\nimport { setView } from \"../slices/appSlice\";\n\ntype FilesViewProps = {\n  files: string[];\n  filesState: string;\n  waiting: boolean;\n};\n\nexport default function FilesView({\n  files,\n  filesState,\n  waiting,\n}: FilesViewProps) {\n  const dispatch = useDispatch();\n\n  const handleDownload = (url: string, filename: string) => {\n    axios\n      .get(url, {\n        responseType: \"blob\",\n      })\n      .then((res) => {\n        fileDownload(res.data, filename);\n      });\n  };\n\n  console.log(files)\n\n  let filesLinks = [];\n\n  for (let f of files) {\n    let fname = f.split(\"/\").pop()\n    fname = fname?.split(\"?\")[0];\n\n    if (f && fname) {\n      let downloadLink = `${axios.defaults.baseURL}${f}`\n      if(f.includes(\"s3.amazonaws.com\")) {\n        downloadLink = f;\n      }\n      filesLinks.push(\n        <div key={f}>\n          <i\n            className=\"fa fa-file-text-o\"\n            aria-hidden=\"true\"\n            style={{ paddingRight: \"5px\" }}\n          ></i>{\" \"}\n          <b>{fname}</b>\n          <button\n            style={{ float: \"right\" }}\n            type=\"button\"\n            className=\"btn btn-primary\"\n            onClick={() =>\n\n              handleDownload(downloadLink, fname!)\n\n            }\n          >\n            <i className=\"fa fa-download\" aria-hidden=\"true\"></i> Download\n          </button>\n          <hr />\n        </div>\n      );\n    }\n  }\n\n  return (\n    <main className=\"col-md-9 ms-sm-auto col-lg-9\" style={{ padding: \"20px\" }}>\n      <div className=\"col-8\">\n        <h3 style={{ paddingBottom: \"10px\" }}>\n          <i className=\"fa fa-folder-open-o\" aria-hidden=\"true\"></i> Output Files\n        </h3>\n        <BlockUi tag=\"div\" blocking={waiting}>\n          <div>\n            {filesState === \"loaded\" && filesLinks}\n            {filesState === \"unknown\" && (\n              <p>Please run the notebook to produce output files ...</p>\n            )}\n            {filesState === \"loading\" && <p>Loading files please wait ...</p>}\n            {filesState === \"error\" && (\n              <div className=\"alert alert-danger mb-3\" role=\"alert\">\n                There was an error during loading files. Please try to run the\n                app again or contact the administrator.\n              </div>\n            )}\n          </div>\n        </BlockUi>\n      </div>\n\n      <button\n        className=\"btn btn-secondary btn-sm\"\n        // style={{ background: \"transparent\", border: \"none\", fontSize: \"0.9em\" }}\n        onClick={() => {\n          dispatch(setView(\"app\"));\n        }}\n      >\n        <i className=\"fa fa-arrow-left\" aria-hidden=\"true\"></i> Back to App\n      </button>\n    </main>\n  );\n}\n",
         "import React from \"react\";\n\nexport default function MadeWithDiv() {\n  return (\n    <a href=\"https://runmercury.com\" target=\"_blank\" rel=\"noreferrer\">\n      <div className=\"poweredby\">\n        <div className=\"text-center\">\n          {\" \"}\n          <b style={{ fontSize: \"0.9em\" }}>created with</b>{\" \"}\n        </div>\n        <div>\n          <img\n            alt=\"Mercury\"\n            src={\n              process.env.PUBLIC_URL +\n              process.env.REACT_APP_LOCAL_URL +\n              \"/mercury_black_logo.svg\"\n            }\n            style={{ height: \"27px\" }}\n          />\n        </div>\n      </div>\n    </a>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React, { useEffect, useState } from \"react\";\nimport axios from \"axios\";\nimport { IWidget } from \"../widgets/Types\";\nimport { useSelector } from \"react-redux\";\nimport { getWidgetsValues } from \"../slices/notebooksSlice\";\n\ntype Props = {\n  slug: string;\n  widgetsParams: Record<string, IWidget>;  \n  notebookPath: string;\n  columnsWidth: number;\n  taskSessionId: string | undefined;\n};\n\nexport default function RestAPIView({\n  slug,\n  widgetsParams,\n  notebookPath,\n  columnsWidth,\n  taskSessionId,\n}: Props) {\n  const [response, setResponse] = useState(\n    JSON.stringify({ msg: \"Example output\" })\n  );\n  const widgetsValues = useSelector(getWidgetsValues);\n\n  let examplePostData = {} as Record<\n    string,\n    | string\n    | number\n    | null\n    | undefined\n    | boolean\n    | [number, number]\n    | string[]\n    | unknown\n  >;\n  for (let [key, widgetParams] of Object.entries(widgetsParams)) {\n    if (widgetParams.input) {\n      examplePostData[key] = widgetsValues[key];\n    }\n  }\n\n  async function fetchResponse() {\n    try {\n      const { data } = await axios.get(`get/${taskSessionId}`);\n      setResponse(JSON.stringify(data));\n    } catch (error) {}\n  }\n\n  useEffect(() => {\n    if (taskSessionId) {\n      fetchResponse();\n    }\n    // eslint-disable-next-line react-hooks/exhaustive-deps\n  }, [taskSessionId, notebookPath]);\n\n  let sessionId = \"id-with-some-random-string\";\n  if (taskSessionId) {\n    sessionId = taskSessionId;\n  }\n\n  let postRequest = `curl -X POST -H \"Content-Type: application/json\" -d '${JSON.stringify(\n    examplePostData\n  )}' ${axios.defaults.baseURL}/run/${slug}`;\n  return (\n    <div\n      className={`ms-sm-auto col-lg-${columnsWidth}`}\n      style={{\n        border: \"none\",\n        paddingTop: \"0px\",\n        paddingRight: \"0px\",\n        paddingLeft: \"0px\",\n        padding: \"10px\",\n      }}\n    >\n      <h4>Notebook as REST API</h4>\n      <p>\n        This notebook can be executed as REST API. Please see the examples below\n        on how to access the notebook.\n      </p>\n\n      <div className=\"alert alert-secondary\" role=\"alert\">\n        <h5>POST request to execute the notebook</h5>\n        <textarea\n          disabled\n          style={{ width: \"100%\" }}\n          rows={3}\n          value={postRequest}\n        ></textarea>\n        The above request should return a JSON with `id`. The `id` should be\n        used in the GET request to fetch the result.\n        <br />\n        Example response:\n        <pre>{`{\"id\": \"${sessionId}\"}`}</pre>\n      </div>\n      <div className=\"alert alert-secondary\" role=\"alert\">\n        <h5>GET request to get execution result in JSON</h5>\n        <textarea\n          disabled\n          style={{ width: \"100%\" }}\n          rows={1}\n          value={`curl ${axios.defaults.baseURL}/get/${sessionId}`}\n        ></textarea>\n      </div>\n\n      <div className=\"alert alert-primary\" role=\"alert\">\n        <h5>Response</h5>\n        <pre>{response}</pre>\n      </div>\n    </div>\n  );\n}\n",
         "import React, { useEffect } from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\nimport { toast } from \"react-toastify\";\nimport { getExportingToPDF, getExportToPDFCounter, getExportToPDFJobId, getPDF, stopPDFExport } from \"../slices/tasksSlice\";\n\nexport default function WaitPDFExport() {\n  const dispatch = useDispatch();\n  const counter = useSelector(getExportToPDFCounter);\n  const jobId = useSelector(getExportToPDFJobId);\n  const exportingPDF = useSelector(getExportingToPDF);\n\n  useEffect(() => {\n    if(jobId === '') {\n      return;\n    } \n    if(!exportingPDF) {\n      return;\n    }\n    // raise error after 2 minutes of waiting ...\n    if (counter < 120) {\n      setTimeout(() => {\n        dispatch(getPDF(jobId));\n      }, 1000); // every 1 second\n    } else {\n      dispatch(stopPDFExport());\n      toast.error(\"Problem with PDF export. Please try again later or ask your admin for help.\", { autoClose: 6000 })\n    }\n  }, [dispatch, counter, jobId, exportingPDF]);\n\n  return <div></div>;\n}\n",
         "import React, { useEffect } from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\nimport \"./App.css\";\nimport NavBar from \"../components/NavBar\";\nimport SideBar from \"../components/SideBar\";\nimport MainView from \"../components/MainView\";\n\nimport {\n  fetchNotebookWithSlug,\n  getLoadingStateSelected,\n  getSelectedNotebook,\n  getSlidesHash,\n  // getWatchModeCounter,\n} from \"../slices/notebooksSlice\";\nimport {\n  //fetchCurrentTask,\n  //fetchExecutionHistory,\n  getCurrentTask,\n  getExportingToPDF,\n  getHistoricTask,\n  getPreviousTask,\n  //ITask,\n  //setPreviousTask,\n} from \"../slices/tasksSlice\";\nimport { isOutputFilesWidget, IWidget } from \"../widgets/Types\";\nimport {\n  fetchWorkerOutputFiles,\n  getOutputFiles,\n  getOutputFilesState,\n  getShowSideBar,\n  getView,\n  setShowSideBar,\n} from \"../slices/appSlice\";\nimport FilesView from \"../components/FilesView\";\nimport { getToken, getUsername } from \"../slices/authSlice\";\nimport MadeWithDiv from \"../components/MadeWithDiv\";\nimport RestAPIView from \"../components/RestAPIView\";\nimport BlockUi from \"react-block-ui\";\nimport WaitPDFExport from \"../components/WaitPDFExport\";\nimport { getWorkerId, getWorkerState, WorkerState } from \"../slices/wsSlice\";\nimport { getSiteId, isPublic } from \"../slices/sitesSlice\";\n\ntype AppProps = {\n  isSingleApp: boolean;\n  notebookSlug: string;\n  displayEmbed: boolean;\n};\n\nfunction App({ isSingleApp, notebookSlug, displayEmbed }: AppProps) {\n  const dispatch = useDispatch();\n  const notebook = useSelector(getSelectedNotebook);\n  const loadingState = useSelector(getLoadingStateSelected);\n  const task = useSelector(getCurrentTask);\n  const historicTask = useSelector(getHistoricTask);\n  const previousTask = useSelector(getPreviousTask);\n  const appView = useSelector(getView);\n  const outputFiles = useSelector(getOutputFiles);\n  const outputFilesState = useSelector(getOutputFilesState);\n  const username = useSelector(getUsername);\n  const token = useSelector(getToken);\n  const slidesHash = useSelector(getSlidesHash);\n  const showSideBar = useSelector(getShowSideBar);\n  const exportingToPDF = useSelector(getExportingToPDF);\n  const workerId = useSelector(getWorkerId);\n  const workerState = useSelector(getWorkerState);\n  const siteId = useSelector(getSiteId);\n  const isSitePublic = useSelector(isPublic);\n\n  const pleaseWait = () => {\n    if (notebook?.params?.static_notebook) {\n      return false;\n    }\n    if (\n      workerState === WorkerState.UsageLimitReached ||\n      workerState === WorkerState.MaxIdleTimeReached ||\n      workerState === WorkerState.MaxRunTimeReached\n    ) {\n      return false;\n    }\n    return workerState !== WorkerState.Running;\n  };\n\n  const isWatchMode = () => {\n    return (\n      notebook.state === \"WATCH_READY\" ||\n      notebook.state === \"WATCH_WAIT\" ||\n      notebook.state === \"WATCH_ERROR\"\n    );\n  };\n\n  useEffect(() => {\n    if (siteId !== undefined) {\n      dispatch(fetchNotebookWithSlug(siteId, notebookSlug));\n    }\n  }, [dispatch, siteId, notebookSlug, token]);\n\n  useEffect(() => {\n    if (\n      appView === \"files\" &&\n      notebook?.params?.version === \"2\" &&\n      workerId !== undefined &&\n      notebook.id !== undefined\n    ) {\n      dispatch(fetchWorkerOutputFiles(workerId, notebook.id));\n    }\n  }, [dispatch, appView, notebook, workerId]);\n\n  let notebookPath = notebook.default_view_path;\n  if (task.state && task.state === \"DONE\" && task.result) {\n    notebookPath = task.result;\n  }\n  let errorMsg = \"\";\n  if (task.state && task.result && task.state === \"ERROR\") {\n    errorMsg = task.result;\n  }\n\n  // set historic task to display if available\n  if (\n    historicTask.state &&\n    historicTask.state === \"DONE\" &&\n    historicTask.result\n  ) {\n    notebookPath = historicTask.result;\n  }\n  if (\n    historicTask.state &&\n    historicTask.result &&\n    historicTask.state === \"ERROR\"\n  ) {\n    errorMsg = historicTask.result;\n  }\n\n  // if we have previous task to show, just show it\n  if (\n    notebookPath === notebook.default_view_path &&\n    previousTask.state &&\n    previousTask.state === \"DONE\" &&\n    previousTask.result\n  ) {\n    notebookPath = previousTask.result;\n  }\n\n  const areOutputFilesAvailable = (\n    widgetsParams: Record<string, IWidget>\n  ): boolean => {\n    if (widgetsParams) {\n      for (let [, widgetParams] of Object.entries(widgetsParams)) {\n        if (isOutputFilesWidget(widgetParams)) {\n          return true;\n        }\n      }\n    }\n    return false;\n  };\n\n  let showRestApi = false;\n  if (notebook.output && notebook.output.toLowerCase().startsWith(\"rest\")) {\n    showRestApi = true;\n  }\n\n  const isFullScreen = () => {\n    if (notebook !== undefined && notebook !== null) {\n      return notebook?.params?.full_screen !== undefined &&\n        notebook?.params?.full_screen !== null\n        ? notebook.params.full_screen\n        : true;\n    }\n    return true;\n  };\n\n  const doAllowDownload = () => {\n    if (notebook !== undefined && notebook !== null) {\n      return notebook?.params?.allow_download !== undefined &&\n        notebook?.params?.allow_download !== null\n        ? notebook.params.allow_download\n        : true;\n    }\n    return true;\n  };\n\n  return (\n    <div className=\"App\">\n      {!displayEmbed && (\n        <NavBar isSitePublic={isSitePublic} username={username} />\n      )}\n      <BlockUi\n        blocking={exportingToPDF}\n        message=\"Exporting to PDF. Please wait ...\"\n      >\n        {exportingToPDF && <WaitPDFExport />}\n        <div className=\"container-fluid\">\n          <div className=\"row\">\n            {/* {notebook.schedule !== undefined && notebook.schedule !== \"\" && (\n              <AutoRefresh notebookId={notebookId} />\n            )} */}\n\n            {showSideBar && (\n              <SideBar\n                notebookTitle={notebook.title}\n                notebookId={notebook.id}\n                notebookSchedule={notebook.schedule}\n                taskCreatedAt={task.created_at}\n                loadingState={loadingState}\n                waiting={pleaseWait()}\n                widgetsParams={notebook?.params?.params}\n                watchMode={isWatchMode()}\n                notebookPath={notebookPath}\n                displayEmbed={displayEmbed}\n                showFiles={areOutputFilesAvailable(notebook?.params?.params)}\n                isPresentation={\n                  notebook.output !== undefined && notebook.output === \"slides\"\n                }\n                notebookParseErrors={notebook.errors}\n                continuousUpdate={notebook?.params?.continuous_update}\n                staticNotebook={notebook?.params?.static_notebook}\n                allowDownload={doAllowDownload()}\n              />\n            )}\n\n            {!showSideBar && (\n              <div>\n                <button\n                  className=\"btn btn-sm  btn-outline-primary\"\n                  type=\"button\"\n                  style={{\n                    position: \"absolute\",\n                    top: displayEmbed ? \"5px\" : \"50px\",\n                    left: \"5px\",\n                    zIndex: \"2000\",\n                  }}\n                  onClick={() => dispatch(setShowSideBar(true))}\n                  data-toggle=\"tooltip\"\n                  data-placement=\"right\"\n                  title=\"Show sidebar\"\n                >\n                  <i className=\"fa fa-chevron-right\" aria-hidden=\"true\" />\n                </button>\n              </div>\n            )}\n\n            {showRestApi && (\n              <RestAPIView\n                slug={notebook.slug}\n                widgetsParams={notebook?.params?.params}\n                notebookPath={notebookPath}\n                columnsWidth={showSideBar ? 9 : 12}\n                taskSessionId={task.session_id}\n              />\n            )}\n\n            <MainView\n              appView={appView}\n              loadingState={loadingState}\n              notebookPath={notebookPath}\n              errorMsg={errorMsg}\n              waiting={pleaseWait()}\n              watchMode={isWatchMode()}\n              displayEmbed={displayEmbed}\n              username={username}\n              slidesHash={slidesHash}\n              columnsWidth={showSideBar ? 9 : 12}\n              isPresentation={\n                notebook.output !== undefined && notebook.output === \"slides\"\n              }\n              fullScreen={isFullScreen()}\n            />\n\n            {appView === \"files\" && (\n              <FilesView\n                files={outputFiles}\n                filesState={outputFilesState}\n                waiting={pleaseWait()}\n              />\n            )}\n          </div>\n        </div>\n      </BlockUi>\n      {displayEmbed && <MadeWithDiv />}\n    </div>\n  );\n}\n\nconst AppView = App;\nexport default AppView;\n",
         "import { useParams } from \"react-router-dom\";\nimport AppView from \"./AppView\";\n\nexport default function MyApp() {\n  const { slug } = useParams<{ slug: string }>();\n  const { embed } = useParams<{ embed: string }>();\n  const displayEmbed = !!(embed && embed === \"embed\");\n\n  return (\n    <AppView\n      isSingleApp={false}\n      notebookSlug={slug as string}\n      displayEmbed={displayEmbed}\n    />\n  );\n}\n",
         "import React from \"react\";\n\nexport default function Footer() {\n  return (\n    <footer\n      className=\"footer\"\n      style={{\n        position: \"absolute\",\n        bottom: \"0\",\n        width: \"100%\",\n        height: \"40px\",\n        lineHeight: \"40px\",\n        backgroundColor: \"#f5f5f5\",\n        borderTop: \"1px solid #e5e5e5\",\n      }}\n    >\n      <div className=\"container\">\n        <span className=\"text-muted\" style={{ color: \"gray\" }}>\n          Mercury \u00a9{\" \"}\n          <a\n            style={{ textDecoration: \"none\", color: \"gray\" }}\n            href=\"https://mljar.com\"\n            target=\"_blank\"\n            rel=\"noreferrer\"\n          >\n            MLJAR\n          </a>\n        </span>\n        <span className=\"text-muted\" style={{ float: \"right\" }}>\n          \n          <a\n            style={{ textDecoration: \"none\", color: \"gray\" }}\n            href=\"https://github.com/mljar/mercury\"\n            target=\"_blank\"\n            rel=\"noreferrer\"\n          >\n            Mercury\n          </a>\n          {\" \"}\n          <i className=\"fa fa-github\" aria-hidden=\"true\"></i>\n        </span>\n      </div>\n    </footer>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\nimport LoginButton from \"./LoginButton\";\nimport UserButton from \"./UserButton\";\n\ntype NavBarProps = {\n  isSitePublic: boolean;\n  username: string;\n};\n\nexport default function NavBar({ isSitePublic, username }: NavBarProps) {\n  return (\n    <header\n      className=\"navbar navbar-dark sticky-top bg-dark p-0\"\n    >\n      <div className=\"row\" style={{ width: \"100%\", paddingRight: \"0px\" }}>\n        <div className=\"col-4\"></div>\n        <div className=\"col-4 text-center\">\n          <a href=\"/\">\n            <img\n              alt=\"Mercury\"\n              src={\n                process.env.PUBLIC_URL +\n                process.env.REACT_APP_LOCAL_URL +\n                \"/mercury_logo.svg\"\n              }\n              style={{ height: \"40px\" }}\n            />\n          </a>\n        </div>\n        <div\n          className=\"col-4\"\n          style={{ marginRight: \"0px\", paddingRight: \"0px\" }}\n        >\n          {!isSitePublic && username === \"\" && <LoginButton />}\n          {username !== \"\" && <UserButton username={username} />}\n        </div>\n      </div>\n    </header>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React, { useEffect, useState } from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\nimport {\n  changePassword,\n  fetchUserInfo,\n  getUserInfo,\n  getUsername,\n} from \"../slices/authSlice\";\nimport Footer from \"../components/Footer\";\nimport HomeNavBar from \"../components/HomeNavBar\";\nimport { isPublic } from \"../slices/sitesSlice\";\n\nexport default function AccountView() {\n  const dispatch = useDispatch();\n  const [oldPassword, setOldPassword] = useState(\"\");\n  const [newPassword1, setNewPassword1] = useState(\"\");\n  const [newPassword2, setNewPassword2] = useState(\"\");\n  const username = useSelector(getUsername);\n  const user = useSelector(getUserInfo);\n  const isSitePublic = useSelector(isPublic);\n\n  document.body.style.backgroundColor = \"white\";\n\n  useEffect(() => {\n    dispatch(fetchUserInfo());\n  }, [dispatch]);\n\n  return (\n    <div className=\"App\">\n      <HomeNavBar isSitePublic={isSitePublic} username={username} />\n\n      <div className=\"container\">\n        <div className=\"mx-auto\" style={{ width: \"700px\" }}>\n          <div className=\"row\" style={{ marginTop: \"40px\" }}>\n            <h2>\n              <i className=\"fa fa-user\" aria-hidden=\"true\"></i> Account\n            </h2>\n            <form>\n              <div className=\"mb-3\">\n                <label className=\"form-label\">Username</label>\n                <input\n                  className=\"form-control\"\n                  value={user.username}\n                  disabled\n                />\n              </div>\n              <div className=\"mb-3\">\n                <label className=\"form-label\">First name</label>\n                <input\n                  className=\"form-control\"\n                  value={user.first_name}\n                  disabled\n                />\n              </div>\n              <div className=\"mb-3\">\n                <label className=\"form-label\">Last name</label>\n                <input\n                  className=\"form-control\"\n                  value={user.last_name}\n                  disabled\n                />\n              </div>\n\n              <div className=\"mb-3\">\n                <label className=\"form-label\">Email address</label>\n                <input className=\"form-control\" value={user.email} disabled />\n              </div>\n            </form>\n          </div>\n          <hr />\n          <div className=\"row\">\n            <h2>\n              <i className=\"fa fa-key\" aria-hidden=\"true\"></i> Change password\n            </h2>\n            <div>\n              <div className=\"mb-3\">\n                <label className=\"form-label\">Old password</label>\n                <input\n                  type=\"password\"\n                  className=\"form-control\"\n                  value={oldPassword}\n                  onChange={(e) => setOldPassword(e.target.value)}\n                />\n              </div>\n              <div className=\"mb-3\">\n                <label className=\"form-label\">New password</label>\n                <input\n                  type=\"password\"\n                  className=\"form-control\"\n                  value={newPassword1}\n                  onChange={(e) => setNewPassword1(e.target.value)}\n                />\n              </div>\n              <div className=\"mb-3\">\n                <label className=\"form-label\">Repeat new password</label>\n                <input\n                  type=\"password\"\n                  className=\"form-control\"\n                  value={newPassword2}\n                  onChange={(e) => setNewPassword2(e.target.value)}\n                />\n              </div>\n              <div className=\"mb-3\" style={{ paddingBottom: \"50px\" }}>\n                <button\n                  className=\"btn btn-primary\"\n                  onClick={() =>\n                    dispatch(\n                      changePassword(oldPassword, newPassword1, newPassword2)\n                    )\n                  }\n                  disabled={\n                    oldPassword === \"\" ||\n                    newPassword1 === \"\" ||\n                    newPassword2 === \"\"\n                  }\n                >\n                  Change password\n                </button>\n              </div>\n            </div>\n          </div>\n        </div>\n      </div>\n\n      <Footer />\n    </div>\n  );\n}\n",
         "/* eslint-disable import/no-cycle */\r\nimport {\r\n  createSlice,\r\n  PayloadAction,\r\n  AnyAction,\r\n  Dispatch,\r\n} from '@reduxjs/toolkit';\r\nimport axios from 'axios';\r\n\r\nimport { RootState } from '../store';\r\nimport { setToken, setUsername } from './authSlice';\r\n\r\n\r\nconst initialState = {\r\n  fetchingIsPro: true,\r\n  isPro: false,\r\n  welcome: \"\"\r\n};\r\n\r\nconst versionSlice = createSlice({\r\n  name: 'version',\r\n  initialState,\r\n  reducers: {\r\n    setVersion(state, action: PayloadAction<{ isPro: boolean }>) {\r\n      const { isPro } = action.payload;\r\n      state.isPro = isPro;\r\n      state.fetchingIsPro = false;\r\n    },\r\n    setWelcome(state, action: PayloadAction<string>) {\r\n      state.welcome = action.payload;\r\n    }\r\n  },\r\n});\r\n\r\nexport default versionSlice.reducer;\r\n\r\nexport const {\r\n  setVersion,\r\n  setWelcome,\r\n} = versionSlice.actions;\r\n\r\nexport const getIsPro = (state: RootState) => state.version.isPro;\r\nexport const getFetchingIsPro = (state: RootState) => state.version.fetchingIsPro;\r\nexport const getWelcome = (state: RootState) => state.version.welcome;\r\n\r\nexport const fetchVersion =\r\n  () =>\r\n    async (dispatch: Dispatch<AnyAction>) => {\r\n\r\n      try {\r\n        const url = '/api/v1/version/';\r\n        const { data } = await axios.get(url);\r\n        dispatch(setVersion(data));\r\n      } catch (error) {\r\n        console.log(`Problem during loading Mercury version. ${error}`);\r\n        if (axios.isAxiosError(error)) {\r\n          if (error.response?.status === 401) {\r\n            // clear auth data \r\n            dispatch(setToken(null));\r\n            dispatch(setUsername(null));\r\n            window.location.reload();\r\n          }\r\n        }\r\n      }\r\n    };\r\n\r\n\r\nexport const fetchWelcome =\r\n  (siteId: number) =>\r\n    async (dispatch: Dispatch<AnyAction>) => {\r\n\r\n      try {\r\n        const url = `/api/v1/${siteId}/welcome/`;\r\n        const { data } = await axios.get(url);\r\n        dispatch(setWelcome(data.msg));\r\n      } catch (error) {\r\n        console.log(`Problem during loading Mercury welcome message. ${error}`);\r\n      }\r\n\r\n    };\r\n\r\n",
-        "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React, { useEffect, useState } from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\n\nimport HomeNavBar from \"../components/HomeNavBar\";\nimport Footer from \"../components/Footer\";\nimport {\n  // fetchNbIframes,\n  fetchNotebooks,\n  getLoadingState,\n  // getNbIframes,\n  getNotebooks,\n} from \"../slices/notebooksSlice\";\nimport { fetchWelcome, getWelcome } from \"../slices/versionSlice\";\n\nimport ReactMarkdown from \"react-markdown\";\nimport rehypeHighlight from \"rehype-highlight\";\nimport remarkGfm from \"remark-gfm\";\nimport emoji from \"remark-emoji\";\nimport rehypeRaw from \"rehype-raw\";\nimport { getToken, getUsername } from \"../slices/authSlice\";\nimport { getSiteId, getSiteWelcome, isPublic } from \"../slices/sitesSlice\";\n\nexport default function HomeView() {\n  const dispatch = useDispatch();\n  const notebooks = useSelector(getNotebooks);\n  const loadingState = useSelector(getLoadingState);\n  const welcome = useSelector(getWelcome);\n  const username = useSelector(getUsername);\n  const token = useSelector(getToken);\n  const [showButton, setShowButton] = useState(\"\");\n  const siteId = useSelector(getSiteId);\n  const isSitePublic = useSelector(isPublic);\n  const siteWelcome = useSelector(getSiteWelcome);\n\n  useEffect(() => {\n    if (siteId !== undefined) {\n      dispatch(fetchNotebooks(siteId));\n      if (siteWelcome === undefined || siteWelcome === \"\") {\n        dispatch(fetchWelcome(siteId));\n      }\n    }\n    // fetchNotebooks depends on token\n    // if token is set then private notebooks are returned\n  }, [dispatch, siteId, token, siteWelcome]);\n\n  const firstLetters = (text: string | null, count: number): string => {\n    if (text !== null && text !== undefined) {\n      return text.slice(0, count) + (text.length > count ? \" ...\" : \"\");\n    }\n    return \"\";\n  };\n\n  const notebookItems = notebooks.map((notebook, index) => {\n    let nbPath = notebook.default_view_path;\n    if (window.location.origin.startsWith(\"https\")) {\n      nbPath = nbPath.replace(\"http://\", \"https://\");\n    }\n\n    return (\n      <div\n        className=\"col-md-4\"\n        style={{ paddingBottom: \"20px\" }}\n        key={`notebook-${notebook.id}}`}\n      >\n        <div className=\"card\">\n          <div\n            style={{\n              height: \"200px\",\n              width: \"100%\",\n              padding: \"1px\",\n              overflow: \"hidden\",\n            }}\n          >\n            <iframe\n              className=\"thumbnailIframe\"\n              width=\"200%\"\n              height={800}\n              src={nbPath}\n              title=\"display\"\n              scrolling=\"no\"\n            ></iframe>\n\n            {/* <img\n              alt=\"some alt\" \n              \n              width=\"100%\"\n              src={`${notebook.default_view_path.replace(\".html\", \".png\")}`}\n            ></img> */}\n          </div>\n          <a\n            href={`/app/${notebook.slug}`}\n            style={{ textDecoration: \"none\", color: \"black\" }}\n            className=\"title-card\"\n            onMouseEnter={() => {\n              setShowButton(notebook.slug);\n            }}\n            onMouseLeave={() => {\n              setShowButton(\"\");\n            }}\n          >\n            <div\n              className=\"card-body\"\n              style={{\n                borderTop: \"1px solid rgba(0,0,0,0.1)\",\n                height: \"110px\",\n              }}\n            >\n              <h5 className=\"card-title\">{firstLetters(notebook.title, 40)}</h5>\n\n              <p className=\"card-text\">\n                {firstLetters(notebook.params.description, 100)}\n              </p>\n\n              {/* <a href={`/app/${notebook.id}`} className=\"btn btn-primary\">\n              Open <i className=\"fa fa-arrow-right\" aria-hidden=\"true\"></i>\n            </a> */}\n            </div>\n            {showButton === notebook.slug && (\n              <button\n                className=\"btn btn-outline-primary\"\n                type=\"button\"\n                style={{\n                  zIndex: \"101\",\n                  border: \"none\",\n                  margin: \"5px\",\n                  position: \"absolute\",\n                  right: \"0px\",\n                  bottom: \"0px\",\n                }}\n                data-toggle=\"tooltip\"\n                data-placement=\"right\"\n                title={`Open ${notebook.title}`}\n              >\n                <i className=\"fa fa-chevron-right\" aria-hidden=\"true\" />\n              </button>\n            )}\n          </a>\n        </div>\n      </div>\n    );\n  });\n\n  document.body.style.backgroundColor = \"white\";\n\n  let welcomeMd = siteWelcome;\n  if (welcomeMd === undefined || welcomeMd === \"\") {\n    welcomeMd = welcome;\n  }\n\n  return (\n    <div className=\"App\">\n      <HomeNavBar isSitePublic={isSitePublic} username={username} />\n      <div className=\"container\" style={{ paddingBottom: \"50px\" }}>\n        {welcomeMd === \"\" && (\n          <h1 style={{ padding: \"30px\", textAlign: \"center\" }}>Welcome!</h1>\n        )}\n        {welcomeMd !== \"\" && (\n          <div style={{ paddingTop: \"20px\", paddingBottom: \"10px\" }}>\n            <ReactMarkdown\n              rehypePlugins={[remarkGfm, rehypeHighlight, emoji, rehypeRaw]}\n            >\n              {welcomeMd}\n            </ReactMarkdown>\n          </div>\n        )}\n\n        <div className=\"row\">\n          {loadingState === \"loading\" && (\n            <p>Loading notebooks. Please wait ...</p>\n          )}\n\n          {loadingState === \"loaded\" && notebooks.length === 0 && (\n            <div>\n              <p>There are no notebooks available.</p>\n            </div>\n          )}\n          {loadingState === \"error\" && (\n            <p>\n              Problem while loading notebooks. Please try again later or contact\n              Mercury administrator.\n            </p>\n          )}\n          {notebookItems}\n        </div>\n      </div>\n      <Footer />\n    </div>\n  );\n}\n",
+        "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React, { useEffect, useState } from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\n\nimport HomeNavBar from \"../components/HomeNavBar\";\nimport Footer from \"../components/Footer\";\nimport {\n  // fetchNbIframes,\n  fetchNotebooks,\n  getLoadingState,\n  // getNbIframes,\n  getNotebooks,\n} from \"../slices/notebooksSlice\";\nimport { fetchWelcome, getWelcome } from \"../slices/versionSlice\";\n\nimport ReactMarkdown from \"react-markdown\";\nimport rehypeHighlight from \"rehype-highlight\";\nimport remarkGfm from \"remark-gfm\";\nimport emoji from \"remark-emoji\";\nimport rehypeRaw from \"rehype-raw\";\nimport { getToken, getUsername } from \"../slices/authSlice\";\nimport { getSiteId, getSiteWelcome, isPublic } from \"../slices/sitesSlice\";\n\nexport default function HomeView() {\n  const dispatch = useDispatch();\n  const notebooks = useSelector(getNotebooks);\n  const loadingState = useSelector(getLoadingState);\n  const welcome = useSelector(getWelcome);\n  const username = useSelector(getUsername);\n  const token = useSelector(getToken);\n  const [showButton, setShowButton] = useState(\"\");\n  const siteId = useSelector(getSiteId);\n  const isSitePublic = useSelector(isPublic);\n  const siteWelcome = useSelector(getSiteWelcome);\n\n  useEffect(() => {\n    if (siteId !== undefined) {\n      dispatch(fetchNotebooks(siteId));\n      if (siteWelcome === undefined || siteWelcome === \"\") {\n        dispatch(fetchWelcome(siteId));\n      }\n    }\n    // fetchNotebooks depends on token\n    // if token is set then private notebooks are returned\n  }, [dispatch, siteId, token, siteWelcome]);\n\n  const firstLetters = (text: string | null, count: number): string => {\n    if (text !== null && text !== undefined) {\n      return text.slice(0, count) + (text.length > count ? \" ...\" : \"\");\n    }\n    return \"\";\n  };\n\n  const notebookItems = notebooks.map((notebook, index) => {\n    let nbPath = notebook.default_view_path;\n\n    if (window.location.origin.startsWith(\"https\")) {\n      nbPath = nbPath.replace(\"http://\", \"https://\");\n    }\n\n    if (window.location.origin === \"http://localhost:3000\") {\n      if (nbPath.startsWith(\"/media\")) {\n        nbPath = \"https://127.0.0.1:8000\" + nbPath;\n      }\n    }\n\n    // if (window.location.origin !== \"http://localhost:3000\") {\n    //   if (nbPath.startsWith(\"https://127.0.0.1:8000\")) {\n    //     nbPath = nbPath.replace(\n    //       \"https://127.0.0.1:8000\",\n    //       window.location.origin\n    //     );\n    //   }\n    //   if (nbPath.startsWith(\"http://127.0.0.1:8000\")) {\n    //     nbPath = nbPath.replace(\n    //       \"http://127.0.0.1:8000\",\n    //       window.location.origin\n    //     );\n    //   }\n    // }\n\n    return (\n      <div\n        className=\"col-md-4\"\n        style={{ paddingBottom: \"20px\" }}\n        key={`notebook-${notebook.id}}`}\n      >\n        <div className=\"card\">\n          <div\n            style={{\n              height: \"200px\",\n              width: \"100%\",\n              padding: \"1px\",\n              overflow: \"hidden\",\n            }}\n          >\n            <iframe\n              className=\"thumbnailIframe\"\n              width=\"200%\"\n              height={800}\n              src={nbPath}\n              title=\"display\"\n              scrolling=\"no\"\n            ></iframe>\n\n            {/* <img\n              alt=\"some alt\" \n              \n              width=\"100%\"\n              src={`${notebook.default_view_path.replace(\".html\", \".png\")}`}\n            ></img> */}\n          </div>\n          <a\n            href={`/app/${notebook.slug}`}\n            style={{ textDecoration: \"none\", color: \"black\" }}\n            className=\"title-card\"\n            onMouseEnter={() => {\n              setShowButton(notebook.slug);\n            }}\n            onMouseLeave={() => {\n              setShowButton(\"\");\n            }}\n          >\n            <div\n              className=\"card-body\"\n              style={{\n                borderTop: \"1px solid rgba(0,0,0,0.1)\",\n                height: \"110px\",\n              }}\n            >\n              <h5 className=\"card-title\">{firstLetters(notebook.title, 40)}</h5>\n\n              <p className=\"card-text\">\n                {firstLetters(notebook.params.description, 100)}\n              </p>\n\n              {/* <a href={`/app/${notebook.id}`} className=\"btn btn-primary\">\n              Open <i className=\"fa fa-arrow-right\" aria-hidden=\"true\"></i>\n            </a> */}\n            </div>\n            {showButton === notebook.slug && (\n              <button\n                className=\"btn btn-outline-primary\"\n                type=\"button\"\n                style={{\n                  zIndex: \"101\",\n                  border: \"none\",\n                  margin: \"5px\",\n                  position: \"absolute\",\n                  right: \"0px\",\n                  bottom: \"0px\",\n                }}\n                data-toggle=\"tooltip\"\n                data-placement=\"right\"\n                title={`Open ${notebook.title}`}\n              >\n                <i className=\"fa fa-chevron-right\" aria-hidden=\"true\" />\n              </button>\n            )}\n          </a>\n        </div>\n      </div>\n    );\n  });\n\n  document.body.style.backgroundColor = \"white\";\n\n  let welcomeMd = siteWelcome;\n  if (welcomeMd === undefined || welcomeMd === \"\") {\n    welcomeMd = welcome;\n  }\n\n  return (\n    <div className=\"App\">\n      <HomeNavBar isSitePublic={isSitePublic} username={username} />\n      <div className=\"container\" style={{ paddingBottom: \"50px\" }}>\n        {welcomeMd === \"\" && (\n          <h1 style={{ padding: \"30px\", textAlign: \"center\" }}>Welcome!</h1>\n        )}\n        {welcomeMd !== \"\" && (\n          <div style={{ paddingTop: \"20px\", paddingBottom: \"10px\" }}>\n            <ReactMarkdown\n              rehypePlugins={[remarkGfm, rehypeHighlight, emoji, rehypeRaw]}\n            >\n              {welcomeMd}\n            </ReactMarkdown>\n          </div>\n        )}\n\n        <div className=\"row\">\n          {loadingState === \"loading\" && (\n            <p>Loading notebooks. Please wait ...</p>\n          )}\n\n          {loadingState === \"loaded\" && notebooks.length === 0 && (\n            <div>\n              <p>There are no notebooks available.</p>\n            </div>\n          )}\n          {loadingState === \"error\" && (\n            <p>\n              Problem while loading notebooks. Please try again later or contact\n              Mercury administrator.\n            </p>\n          )}\n          {notebookItems}\n        </div>\n      </div>\n      <Footer />\n    </div>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React, { useState } from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\nimport { fetchToken } from \"../slices/authSlice\";\nimport Footer from \"../components/Footer\";\nimport HomeNavBar from \"../components/HomeNavBar\";\n\nimport { useLocation, useNavigate } from \"react-router-dom\";\nimport { isPublic } from \"../slices/sitesSlice\";\n\ntype LocationState = {\n  from: {\n    pathname: string;\n  };\n};\n\nexport default function LoginView() {\n  const dispatch = useDispatch();\n  const navigate = useNavigate();\n  const [email, setEmail] = useState(\"\");\n  const [password, setPassword] = useState(\"\");\n  const isSitePublic = useSelector(isPublic);\n\n  document.body.style.backgroundColor = \"#f5f5f5\";\n\n  let redirectPath = \"/\";\n  let location = useLocation();\n  if (location && location.state) {\n    // redirect from ...\n    const { from } = location.state as LocationState;\n    redirectPath = from.pathname;\n  }\n\n  return (\n    <div className=\"App\">\n      <HomeNavBar isSitePublic={isSitePublic} username={\"\"} />\n\n      <div className=\"div-signin text-center\">\n        <form\n          className=\"form-signin\"\n          onSubmit={(e) => {\n            e.preventDefault();\n            e.stopPropagation();\n            dispatch(fetchToken(email, password, redirectPath, navigate));\n          }}\n        >\n          <h3 className=\"h3 mb-3 font-weight-normal\">Please sign in</h3>\n          <label className=\"sr-only\">Email</label>\n          <input\n            type=\"email\"\n            id=\"inputEmail\"\n            className=\"form-control\"\n            placeholder=\"Email\"\n            value={email}\n            onChange={(e) => {\n              setEmail(e.target.value);\n            }}\n            required\n          />\n          <label className=\"sr-only\">Password</label>\n          <input\n            type=\"password\"\n            id=\"inputPassword\"\n            className=\"form-control\"\n            placeholder=\"Password\"\n            value={password}\n            onChange={(e) => {\n              setPassword(e.target.value);\n            }}\n            required\n          />\n          <button\n            className=\"btn btn-lg btn-primary btn-block\"\n            type=\"submit\"\n            style={{ margin: \"5px\" }}\n            disabled={email === \"\" || password === \"\"}\n          >\n            <i className=\"fa fa-sign-in\" aria-hidden=\"true\"></i> Log in\n          </button>\n        </form>\n        <div className=\"mx-auto\" style={{ width: \"400px\", marginTop: \"40px\" }}>\n          <p className=\"text-muted\">\n            No account? <br /> Please contact administrator to create account\n            for you.\n          </p>\n        </div>\n      </div>\n\n      <Footer />\n    </div>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\"; \nimport Footer from \"../components/Footer\";\nimport HomeNavBar from \"../components/HomeNavBar\";\n\nexport default function LostConnection() {\n  return (\n    <div className=\"App\">\n      <HomeNavBar isSitePublic={true} username={\"\"} />\n      <div\n        style={{\n          width: \"100%\",\n          maxWidth: \"500px\",\n          padding: \"15px\",\n          margin: \"0 auto\",\n        }}\n      >\n        <h3>Lost connection</h3>\n        <p>\n          App lost connection to the server. Please try again in a moment or contact administrator.\n        </p>\n      </div>\n      <Footer />\n    </div>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\nimport { Link } from \"react-router-dom\";\nimport Footer from \"../components/Footer\";\nimport HomeNavBar from \"../components/HomeNavBar\";\n\nexport default function SiteAccessForbiddenView() {\n  return (\n    <div className=\"App\">\n      <HomeNavBar isSitePublic={true} username={\"\"} />\n      <div\n        style={{\n          width: \"100%\",\n          maxWidth: \"500px\",\n          padding: \"15px\",\n          margin: \"0 auto\",\n        }}\n      >\n        <h3>Access forbidden</h3>\n        <p>\n          Please <Link to=\"/login\">login</Link> to access site.\n        </p>\n      </div>\n      <Footer />\n    </div>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\nimport Footer from \"../components/Footer\";\nimport HomeNavBar from \"../components/HomeNavBar\";\n\nexport default function SiteLoadingView() {\n  return (\n    <div className=\"App\">\n      <HomeNavBar isSitePublic={true} username={\"\"} />\n      <div\n        style={{\n          width: \"100%\",\n          maxWidth: \"500px\",\n          padding: \"15px\",\n          margin: \"0 auto\",\n        }}\n      >\n        <p style={{ color: \"gray\" }}>Please wait. Loading site ...</p>\n      </div>\n      <Footer />\n    </div>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\nimport Footer from \"../components/Footer\";\nimport HomeNavBar from \"../components/HomeNavBar\";\n\nexport default function SiteNetworkErrorView() {\n  return (\n    <div className=\"App\">\n      <HomeNavBar isSitePublic={true} username={\"\"} />\n      <div\n        style={{\n          width: \"100%\",\n          maxWidth: \"500px\",\n          padding: \"15px\",\n          margin: \"0 auto\",\n        }}\n      >\n        <h3>Network Error</h3>\n        <p>\n          Please check if you have internet connection and server is running. In\n          case of problems, please contact administrator.\n        </p>\n      </div>\n      <Footer />\n    </div>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\nimport Footer from \"../components/Footer\";\nimport HomeNavBar from \"../components/HomeNavBar\";\n\nexport default function SiteNotFoundView() {\n  return (\n    <div className=\"App\">\n      <HomeNavBar isSitePublic={true} username={\"\"} />\n      <div\n        style={{\n          width: \"100%\",\n          maxWidth: \"500px\",\n          padding: \"15px\",\n          margin: \"0 auto\",\n        }}\n      >\n        <h3>Site does not exist</h3>\n        <p>\n          We can't find site you are looking for. Please make sure that URL\n          address is correct.\n        </p>\n      </div>\n      <Footer />\n    </div>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\nimport Footer from \"../components/Footer\";\nimport HomeNavBar from \"../components/HomeNavBar\";\n\nexport default function SitePleaseRefreshView() {\n  return (\n    <div className=\"App\">\n      <HomeNavBar isSitePublic={true} username={\"\"} />\n      <div\n        style={{\n          width: \"100%\",\n          maxWidth: \"500px\",\n          padding: \"15px\",\n          margin: \"0 auto\",\n        }}\n      >\n        <h3>Please refresh</h3>\n        <p>\n          Please try to refresh the website ...\n        </p>\n      </div>\n      <Footer />\n    </div>\n  );\n}\n",
```

### Comparing `mercury-2.2.7/mercury/frontend-dist/static/js/runtime-main.248907bc.js` & `mercury-2.2.8/mercury/frontend-dist/static/js/runtime-main.248907bc.js`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/frontend-dist/static/js/runtime-main.248907bc.js.map` & `mercury-2.2.8/mercury/frontend-dist/static/js/runtime-main.248907bc.js.map`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/frontend-dist/static/media/fontawesome-webfont.1e59d233.ttf` & `mercury-2.2.8/mercury/frontend-dist/static/media/fontawesome-webfont.1e59d233.ttf`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/frontend-dist/static/media/fontawesome-webfont.20fd1704.woff2` & `mercury-2.2.8/mercury/frontend-dist/static/media/fontawesome-webfont.20fd1704.woff2`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/frontend-dist/static/media/fontawesome-webfont.8b43027f.eot` & `mercury-2.2.8/mercury/frontend-dist/static/media/fontawesome-webfont.8b43027f.eot`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/frontend-dist/static/media/fontawesome-webfont.c1e38fd9.svg` & `mercury-2.2.8/mercury/frontend-dist/static/media/fontawesome-webfont.c1e38fd9.svg`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/frontend-dist/static/media/fontawesome-webfont.f691f37e.woff` & `mercury-2.2.8/mercury/frontend-dist/static/media/fontawesome-webfont.f691f37e.woff`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/manage.py` & `mercury-2.2.8/mercury/manage.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/mercury.py` & `mercury-2.2.8/mercury/mercury.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,17 +211,23 @@
         ):
             arguments += ["--noreload"]
             try:
                 running_local = True
                 for i in sys.argv:
                     if "0.0.0.0" in i:
                         running_local = False
+                        
                 if running_local:
                     # open web browser if we are running a server
                     url = "http://127.0.0.1:8000"
+
+                    for arg in arguments:
+                        if arg.count(".") == 3 and arg.count(":"):
+                            url = arg
+
                     webbrowser.open(url)
             except Exception as e:
                 pass
 
         execute_from_command_line(arguments)
 
     except KeyboardInterrupt:
```

### Comparing `mercury-2.2.7/mercury/requirements.txt` & `mercury-2.2.8/mercury/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-django==3.2.5
-djangorestframework==3.12.4
+django==4.2
+djangorestframework==3.14.0
 django-filter==21.1
 markdown==3.3.6
 celery>=5.1.2
 sqlalchemy==1.4.27
 gevent
 nbconvert>=6.5.0
 ipython_genutils
@@ -20,8 +20,9 @@
 channels[daphne]>=4.0.0
 websocket-client>=1.4.2
 execnb
 ipywidgets==8.0.3 # cant update ipywidgets!
 dj-rest-auth[with_social]==3.0.0
 boto3==1.26.83
 cryptography
-pyopenssl>=23.1.1
+pyopenssl>=23.1.1
+
```

### Comparing `mercury-2.2.7/mercury/server/asgi.py` & `mercury-2.2.8/mercury/server/asgi.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/server/celery.py` & `mercury-2.2.8/mercury/server/celery.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/server/settings.py` & `mercury-2.2.8/mercury/server/settings.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/server/urls.py` & `mercury-2.2.8/mercury/server/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.conf import settings
-from django.conf.urls import include, url
+from django.conf.urls import include
 from django.conf.urls.static import static
 from django.contrib import admin
 from django.shortcuts import render
 from django.urls import path, re_path
 
 from apps.notebooks.urls import notebooks_urlpatterns
 from apps.tasks.urls import tasks_urlpatterns
@@ -27,19 +27,19 @@
         re_path(r"^account", index),
     ]
     urlpatterns += static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)
 
 
 urlpatterns += [
     path("admin/", admin.site.urls),
-    url(
+    re_path(
         "api/v1/version",
         VersionInfo.as_view(),
     ),
-    url(
+    re_path(
         "api/v1/(?P<site_id>.+)/welcome",
         WelcomeMessage.as_view(),
     ),
     re_path(r"^api/v1/fp/", include("django_drf_filepond.urls")),
 ]
 
 urlpatterns += tasks_urlpatterns
```

### Comparing `mercury-2.2.7/mercury/server/views.py` & `mercury-2.2.8/mercury/server/views.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/widgets/app.py` & `mercury-2.2.8/mercury/widgets/app.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/widgets/button.py` & `mercury-2.2.8/mercury/widgets/button.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/widgets/chat.py` & `mercury-2.2.8/mercury/widgets/chat.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/widgets/checkbox.py` & `mercury-2.2.8/mercury/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/widgets/file.py` & `mercury-2.2.8/mercury/widgets/file.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/widgets/json.py` & `mercury-2.2.8/mercury/widgets/json.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/widgets/manager.py` & `mercury-2.2.8/mercury/widgets/manager.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/widgets/multiselect.py` & `mercury-2.2.8/mercury/widgets/multiselect.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/widgets/note.py` & `mercury-2.2.8/mercury/widgets/note.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/widgets/numeric.py` & `mercury-2.2.8/mercury/widgets/numeric.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/widgets/outputdir.py` & `mercury-2.2.8/mercury/widgets/outputdir.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/widgets/range.py` & `mercury-2.2.8/mercury/widgets/range.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/widgets/select.py` & `mercury-2.2.8/mercury/widgets/select.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/widgets/slider.py` & `mercury-2.2.8/mercury/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury/widgets/text.py` & `mercury-2.2.8/mercury/widgets/text.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.7/mercury.egg-info/PKG-INFO` & `mercury-2.2.8/mercury.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury
-Version: 2.2.7
+Version: 2.2.8
 Summary: Turn Jupyter Notebook to Web App and share with non-technical users
 Home-page: https://github.com/mljar/mercury
 Maintainer: MLJAR Sp. z o.o.
 Maintainer-email: contact@mljar.com
 License: UNKNOWN
 Description:
```

### Comparing `mercury-2.2.7/mercury.egg-info/SOURCES.txt` & `mercury-2.2.8/mercury.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -137,16 +137,16 @@
 mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css
 mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map
 mercury/frontend-dist/static/css/main.26f96620.chunk.css
 mercury/frontend-dist/static/css/main.26f96620.chunk.css.map
 mercury/frontend-dist/static/js/2.6305b467.chunk.js
 mercury/frontend-dist/static/js/2.6305b467.chunk.js.LICENSE.txt
 mercury/frontend-dist/static/js/2.6305b467.chunk.js.map
-mercury/frontend-dist/static/js/main.68931b96.chunk.js
-mercury/frontend-dist/static/js/main.68931b96.chunk.js.map
+mercury/frontend-dist/static/js/main.c4e40c36.chunk.js
+mercury/frontend-dist/static/js/main.c4e40c36.chunk.js.map
 mercury/frontend-dist/static/js/runtime-main.248907bc.js
 mercury/frontend-dist/static/js/runtime-main.248907bc.js.map
 mercury/frontend-dist/static/media/fontawesome-webfont.1e59d233.ttf
 mercury/frontend-dist/static/media/fontawesome-webfont.20fd1704.woff2
 mercury/frontend-dist/static/media/fontawesome-webfont.8b43027f.eot
 mercury/frontend-dist/static/media/fontawesome-webfont.c1e38fd9.svg
 mercury/frontend-dist/static/media/fontawesome-webfont.f691f37e.woff
```

### Comparing `mercury-2.2.7/setup.py` & `mercury-2.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     for (path, directories, filenames) in os.walk(directory):
         for filename in filenames:
             paths.append(os.path.join(path, filename))
     return paths
 
 setup(
     name="mercury",
-    version="2.2.7",
+    version="2.2.8",
     maintainer="MLJAR Sp. z o.o.",
     maintainer_email="contact@mljar.com",
     description="Turn Jupyter Notebook to Web App and share with non-technical users",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=open("mercury/requirements.txt").readlines(),
     url="https://github.com/mljar/mercury",
```

