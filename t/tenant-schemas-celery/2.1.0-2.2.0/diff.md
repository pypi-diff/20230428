# Comparing `tmp/tenant-schemas-celery-2.1.0.tar.gz` & `tmp/tenant-schemas-celery-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenant-schemas-celery-2.1.0.tar", last modified: Thu Mar 30 19:20:50 2023, max compression
+gzip compressed data, was "tenant-schemas-celery-2.2.0.tar", last modified: Fri Apr 28 11:40:09 2023, max compression
```

## Comparing `tenant-schemas-celery-2.1.0.tar` & `tenant-schemas-celery-2.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 maciejgol  (1000) maciejgol  (1000)        0 2023-03-30 19:20:50.536088 tenant-schemas-celery-2.1.0/
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     1076 2021-01-02 19:05:21.000000 tenant-schemas-celery-2.1.0/LICENSE
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)       34 2021-01-02 19:05:21.000000 tenant-schemas-celery-2.1.0/MANIFEST.in
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     6160 2023-03-30 19:20:50.536088 tenant-schemas-celery-2.1.0/PKG-INFO
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     5681 2023-03-30 19:19:58.000000 tenant-schemas-celery-2.1.0/README.md
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)        6 2023-03-30 19:20:06.000000 tenant-schemas-celery-2.1.0/VERSION
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)       38 2023-03-30 19:20:50.536088 tenant-schemas-celery-2.1.0/setup.cfg
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     1001 2022-02-04 09:43:17.000000 tenant-schemas-celery-2.1.0/setup.py
-drwxrwxr-x   0 maciejgol  (1000) maciejgol  (1000)        0 2023-03-30 19:20:50.536088 tenant-schemas-celery-2.1.0/tenant_schemas_celery/
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)        0 2021-01-02 19:05:21.000000 tenant-schemas-celery-2.1.0/tenant_schemas_celery/__init__.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     3246 2023-03-30 18:49:09.000000 tenant-schemas-celery-2.1.0/tenant_schemas_celery/app.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)      746 2021-01-02 19:05:21.000000 tenant-schemas-celery-2.1.0/tenant_schemas_celery/cache.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     1402 2021-01-02 19:05:21.000000 tenant-schemas-celery-2.1.0/tenant_schemas_celery/cache_test.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)      226 2023-03-30 18:49:09.000000 tenant-schemas-celery-2.1.0/tenant_schemas_celery/compat.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)      439 2022-02-04 09:35:57.000000 tenant-schemas-celery-2.1.0/tenant_schemas_celery/conftest.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     5799 2022-02-04 09:35:57.000000 tenant-schemas-celery-2.1.0/tenant_schemas_celery/integration_test.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)      562 2021-01-02 19:05:21.000000 tenant-schemas-celery-2.1.0/tenant_schemas_celery/registry.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     1234 2021-01-04 22:35:23.000000 tenant-schemas-celery-2.1.0/tenant_schemas_celery/registry_test.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     3440 2023-03-30 19:19:58.000000 tenant-schemas-celery-2.1.0/tenant_schemas_celery/scheduler.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     2462 2022-02-04 09:35:57.000000 tenant-schemas-celery-2.1.0/tenant_schemas_celery/task.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     5624 2022-02-04 09:35:57.000000 tenant-schemas-celery-2.1.0/tenant_schemas_celery/task_test.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)      642 2023-03-30 19:19:58.000000 tenant-schemas-celery-2.1.0/tenant_schemas_celery/test_app.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     4708 2023-03-30 19:19:58.000000 tenant-schemas-celery-2.1.0/tenant_schemas_celery/test_scheduler.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     1442 2023-03-30 19:16:55.000000 tenant-schemas-celery-2.1.0/tenant_schemas_celery/test_tasks.py
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)      460 2021-01-02 19:05:21.000000 tenant-schemas-celery-2.1.0/tenant_schemas_celery/test_utils.py
-drwxrwxr-x   0 maciejgol  (1000) maciejgol  (1000)        0 2023-03-30 19:20:50.536088 tenant-schemas-celery-2.1.0/tenant_schemas_celery.egg-info/
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     6160 2023-03-30 19:20:50.000000 tenant-schemas-celery-2.1.0/tenant_schemas_celery.egg-info/PKG-INFO
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)      827 2023-03-30 19:20:50.000000 tenant-schemas-celery-2.1.0/tenant_schemas_celery.egg-info/SOURCES.txt
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)        1 2023-03-30 19:20:50.000000 tenant-schemas-celery-2.1.0/tenant_schemas_celery.egg-info/dependency_links.txt
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)        7 2023-03-30 19:20:50.000000 tenant-schemas-celery-2.1.0/tenant_schemas_celery.egg-info/requires.txt
--rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)       22 2023-03-30 19:20:50.000000 tenant-schemas-celery-2.1.0/tenant_schemas_celery.egg-info/top_level.txt
+drwxrwxr-x   0 maciejgol  (1000) maciejgol  (1000)        0 2023-04-28 11:40:09.002534 tenant-schemas-celery-2.2.0/
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     1076 2021-01-02 19:05:21.000000 tenant-schemas-celery-2.2.0/LICENSE
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)       34 2021-01-02 19:05:21.000000 tenant-schemas-celery-2.2.0/MANIFEST.in
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     7184 2023-04-28 11:40:09.002534 tenant-schemas-celery-2.2.0/PKG-INFO
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     6705 2023-04-28 11:38:19.000000 tenant-schemas-celery-2.2.0/README.md
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)        6 2023-04-28 11:38:26.000000 tenant-schemas-celery-2.2.0/VERSION
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)       38 2023-04-28 11:40:09.002534 tenant-schemas-celery-2.2.0/setup.cfg
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     1001 2022-02-04 09:43:17.000000 tenant-schemas-celery-2.2.0/setup.py
+drwxrwxr-x   0 maciejgol  (1000) maciejgol  (1000)        0 2023-04-28 11:40:08.998534 tenant-schemas-celery-2.2.0/tenant_schemas_celery/
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)        0 2021-01-02 19:05:21.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/__init__.py
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     3246 2023-03-30 18:49:09.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/app.py
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)      746 2021-01-02 19:05:21.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/cache.py
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     1402 2021-01-02 19:05:21.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/cache_test.py
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)      226 2023-03-30 18:49:09.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/compat.py
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)      439 2022-02-04 09:35:57.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/conftest.py
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     5799 2022-02-04 09:35:57.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/integration_test.py
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)      562 2021-01-02 19:05:21.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/registry.py
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     1234 2021-01-04 22:35:23.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/registry_test.py
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     3585 2023-04-28 11:38:19.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/scheduler.py
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     2462 2022-02-04 09:35:57.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/task.py
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     5624 2022-02-04 09:35:57.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/task_test.py
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)      642 2023-03-30 19:19:58.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/test_app.py
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     5524 2023-04-28 11:38:19.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/test_scheduler.py
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     1442 2023-03-30 19:16:55.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/test_tasks.py
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)      460 2021-01-02 19:05:21.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery/test_utils.py
+drwxrwxr-x   0 maciejgol  (1000) maciejgol  (1000)        0 2023-04-28 11:40:09.002534 tenant-schemas-celery-2.2.0/tenant_schemas_celery.egg-info/
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)     7184 2023-04-28 11:40:08.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery.egg-info/PKG-INFO
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)      827 2023-04-28 11:40:08.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery.egg-info/SOURCES.txt
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)        1 2023-04-28 11:40:08.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery.egg-info/dependency_links.txt
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)        7 2023-04-28 11:40:08.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery.egg-info/requires.txt
+-rw-rw-r--   0 maciejgol  (1000) maciejgol  (1000)       22 2023-04-28 11:40:08.000000 tenant-schemas-celery-2.2.0/tenant_schemas_celery.egg-info/top_level.txt
```

### Comparing `tenant-schemas-celery-2.1.0/LICENSE` & `tenant-schemas-celery-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.1.0/PKG-INFO` & `tenant-schemas-celery-2.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: tenant-schemas-celery
-Version: 2.1.0
-Summary: Celery integration for django-tenant-schemas and django-tenants
-Home-page: https://github.com/maciej-gol/tenant-schemas-celery
-Author: Maciej Gol
-Author-email: 1kroolik1@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Framework :: Django
-Classifier: Programming Language :: Python
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 tenant-schemas-celery 
 =====================
 
 Celery application implementation that allows celery tasks to cooperate with
 multi-tenancy provided by [django-tenant-schemas](https://github.com/bernardopires/django-tenant-schemas) and
 [django-tenants](https://github.com/tomturner/django-tenants) packages.
 
@@ -142,22 +127,39 @@
 
 The `reset_remaining_jobs_in_all_schemas` task (called the dispatch task) should be registered in your celery beat schedule. The `reset_remaining_jobs_in_schema` task should be called from the dispatch task.
 
 That way you have full control over which schemas the task should be scheduled in.
 
 
 ### Custom scheduler
-You are using the standard `Scheduler` or `PersistentScheduler` classes provided by `celery`, you can transition to using this package's `TenantAwareScheduler` or `TenantAwarePersistentScheduler` classes. You should then specify the scheduler you want to use in your invocation to `beat`. i.e:
+If you are using the standard `Scheduler` or `PersistentScheduler` classes provided by `celery`, you can transition to using this package's `TenantAwareScheduler` or `TenantAwarePersistentScheduler` classes. You should then specify the scheduler you want to use in the celery beat config or your invocation to `beat`. i.e:
 
 ```bash
 celery -A proj beat --scheduler=tenant_schemas_celery.scheduler.TenantAwareScheduler
 ```
 
 #### Caveats
-`TenantAwareSchedulerMixin` uses a subclass of `SchedulerEntry` that allows the user to provide specific schemas to run a task on. This might prove useful if you have a task you only want to run in the `public` schema or to a subset of your tenants. In order to use set that, you must configure `tenant_schemas` in the tasks definition as such:
+- There's a chance that celery beat will try to run a task for a newly created tenant before its migrations are ready, which could potentially lead to deadlocks. This is specially true with big projects with a lot of migrations and very frequent tasks (i.e: every minute). In order to mitigate it, one could do the following:
+    1. Subclass any of `TenantAwareScheduler` or `TenantAwarePersistentScheduler` and override the `get_queryset` method to match your definition of "ready" tenants. For example, imagine that you had a `ready` flag in your tenant model. You could do the following:
+
+    ```python
+    # tenants_app/scheduler.py
+    class MyTenantAwareScheduler(TenantAwareScheduler):
+        @classmethod
+        def get_queryset(cls):
+            return super().get_queryset().filter(ready=True)
+    ```
+
+    2. Use the new scheduler in your celery beat config or invocation:
+    
+    ```bash
+    celery -A proj beat --scheduler=tenants_app.scheduler.MyTenantAwareScheduler
+    ```
+
+- `TenantAwareSchedulerMixin` uses a subclass of `SchedulerEntry` that allows the user to provide specific schemas to run a task on. This might prove useful if you have a task you only want to run in the `public` schema or to a subset of your tenants. In order to use set that, you must configure `tenant_schemas` in the tasks definition as such:
 
 ```python
 app.conf.beat_schedule = {
     "my-task": {
         "task": "myapp.tasks.my_task",
         "schedule": schedules.crontab(minute="*/5"),
         "tenant_schemas": ["public"]
```

### Comparing `tenant-schemas-celery-2.1.0/README.md` & `tenant-schemas-celery-2.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: tenant-schemas-celery
+Version: 2.2.0
+Summary: Celery integration for django-tenant-schemas and django-tenants
+Home-page: https://github.com/maciej-gol/tenant-schemas-celery
+Author: Maciej Gol
+Author-email: 1kroolik1@gmail.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Framework :: Django
+Classifier: Programming Language :: Python
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 tenant-schemas-celery 
 =====================
 
 Celery application implementation that allows celery tasks to cooperate with
 multi-tenancy provided by [django-tenant-schemas](https://github.com/bernardopires/django-tenant-schemas) and
 [django-tenants](https://github.com/tomturner/django-tenants) packages.
 
@@ -127,22 +142,39 @@
 
 The `reset_remaining_jobs_in_all_schemas` task (called the dispatch task) should be registered in your celery beat schedule. The `reset_remaining_jobs_in_schema` task should be called from the dispatch task.
 
 That way you have full control over which schemas the task should be scheduled in.
 
 
 ### Custom scheduler
-You are using the standard `Scheduler` or `PersistentScheduler` classes provided by `celery`, you can transition to using this package's `TenantAwareScheduler` or `TenantAwarePersistentScheduler` classes. You should then specify the scheduler you want to use in your invocation to `beat`. i.e:
+If you are using the standard `Scheduler` or `PersistentScheduler` classes provided by `celery`, you can transition to using this package's `TenantAwareScheduler` or `TenantAwarePersistentScheduler` classes. You should then specify the scheduler you want to use in the celery beat config or your invocation to `beat`. i.e:
 
 ```bash
 celery -A proj beat --scheduler=tenant_schemas_celery.scheduler.TenantAwareScheduler
 ```
 
 #### Caveats
-`TenantAwareSchedulerMixin` uses a subclass of `SchedulerEntry` that allows the user to provide specific schemas to run a task on. This might prove useful if you have a task you only want to run in the `public` schema or to a subset of your tenants. In order to use set that, you must configure `tenant_schemas` in the tasks definition as such:
+- There's a chance that celery beat will try to run a task for a newly created tenant before its migrations are ready, which could potentially lead to deadlocks. This is specially true with big projects with a lot of migrations and very frequent tasks (i.e: every minute). In order to mitigate it, one could do the following:
+    1. Subclass any of `TenantAwareScheduler` or `TenantAwarePersistentScheduler` and override the `get_queryset` method to match your definition of "ready" tenants. For example, imagine that you had a `ready` flag in your tenant model. You could do the following:
+
+    ```python
+    # tenants_app/scheduler.py
+    class MyTenantAwareScheduler(TenantAwareScheduler):
+        @classmethod
+        def get_queryset(cls):
+            return super().get_queryset().filter(ready=True)
+    ```
+
+    2. Use the new scheduler in your celery beat config or invocation:
+    
+    ```bash
+    celery -A proj beat --scheduler=tenants_app.scheduler.MyTenantAwareScheduler
+    ```
+
+- `TenantAwareSchedulerMixin` uses a subclass of `SchedulerEntry` that allows the user to provide specific schemas to run a task on. This might prove useful if you have a task you only want to run in the `public` schema or to a subset of your tenants. In order to use set that, you must configure `tenant_schemas` in the tasks definition as such:
 
 ```python
 app.conf.beat_schedule = {
     "my-task": {
         "task": "myapp.tasks.my_task",
         "schedule": schedules.crontab(minute="*/5"),
         "tenant_schemas": ["public"]
```

### Comparing `tenant-schemas-celery-2.1.0/setup.py` & `tenant-schemas-celery-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.1.0/tenant_schemas_celery/app.py` & `tenant-schemas-celery-2.2.0/tenant_schemas_celery/app.py`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.1.0/tenant_schemas_celery/cache.py` & `tenant-schemas-celery-2.2.0/tenant_schemas_celery/cache.py`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.1.0/tenant_schemas_celery/cache_test.py` & `tenant-schemas-celery-2.2.0/tenant_schemas_celery/cache_test.py`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.1.0/tenant_schemas_celery/integration_test.py` & `tenant-schemas-celery-2.2.0/tenant_schemas_celery/integration_test.py`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.1.0/tenant_schemas_celery/registry.py` & `tenant-schemas-celery-2.2.0/tenant_schemas_celery/registry.py`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.1.0/tenant_schemas_celery/registry_test.py` & `tenant-schemas-celery-2.2.0/tenant_schemas_celery/registry_test.py`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.1.0/tenant_schemas_celery/scheduler.py` & `tenant-schemas-celery-2.2.0/tenant_schemas_celery/scheduler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import logging
 from typing import List, Optional
 
 from celery.beat import PersistentScheduler, ScheduleEntry, Scheduler
 from django_tenants.utils import get_tenant_model, tenant_context, get_public_schema_name
+from django.db import models
 
 logger = logging.getLogger(__name__)
 
+Tenant = get_tenant_model()
+
 
 class TenantAwareScheduleEntry(ScheduleEntry):
     tenant_schemas: Optional[List[str]] = None
 
     def __init__(self, *args, **kwargs):
         if args:
             # Unpickled from database
@@ -64,20 +67,24 @@
                 return False
         return True
 
 
 class TenantAwareSchedulerMixin:
     Entry = TenantAwareScheduleEntry
 
+    @classmethod
+    def get_queryset(cls) -> models.QuerySet:
+        return Tenant.objects.all()
+
     def apply_entry(self, entry: TenantAwareScheduleEntry, producer=None):
         """
         See https://github.com/celery/celery/blob/c571848023be732a1a11d46198cf831a522cfb54/celery/beat.py#L277
         """
 
-        tenants = get_tenant_model().objects.all()
+        tenants = self.get_queryset()
 
         if entry.tenant_schemas is None:
             tenants = tenants.exclude(schema_name=get_public_schema_name())
         else:
             tenants = tenants.filter(schema_name__in=entry.tenant_schemas)
 
         logger.info(
```

### Comparing `tenant-schemas-celery-2.1.0/tenant_schemas_celery/task.py` & `tenant-schemas-celery-2.2.0/tenant_schemas_celery/task.py`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.1.0/tenant_schemas_celery/task_test.py` & `tenant-schemas-celery-2.2.0/tenant_schemas_celery/task_test.py`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.1.0/tenant_schemas_celery/test_app.py` & `tenant-schemas-celery-2.2.0/tenant_schemas_celery/test_app.py`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.1.0/tenant_schemas_celery/test_scheduler.py` & `tenant-schemas-celery-2.2.0/tenant_schemas_celery/test_scheduler.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from tenant_schemas_celery.app import CeleryApp
 
 from .scheduler import (
     TenantAwarePersistentScheduler,
     TenantAwareSchedulerMixin,
 )
 
+Tenant = get_tenant_model()
+
 
 class FakeScheduler(TenantAwareSchedulerMixin, Scheduler):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._sent: List[Tuple[str, TenantAwareSchedulerMixin.Entry]] = []
 
     def apply_async(self, entry, producer=None, advance=True, **kwargs):
@@ -89,38 +91,62 @@
             assert entry.task == config["task"]
             assert entry.schedule == schedules.crontab(minute="*")
             assert entry.tenant_schemas == config.get("tenant_schemas", None)
 
     @fixture
     def tenants(self) -> None:
         with schema_context(get_public_schema_name()):
-            get_tenant_model().objects.create(
+            Tenant.objects.create(
                 name="Tenant1", schema_name="tenant1"
             )
-            get_tenant_model().objects.create(
+            Tenant.objects.create(
                 name="Tenant2", schema_name="tenant2"
             )
 
     @mark.django_db
     def test_apply_entry(self, scheduler: FakeScheduler, tenants: None):
         for task_name, entry in scheduler.schedule.items():
             scheduler.apply_entry(entry)
 
             schemas = (
                 entry.tenant_schemas
-                or get_tenant_model().objects.values_list(
+                or Tenant.objects.values_list(
                     "schema_name", flat=True
                 )
             )
 
             for schema_name in schemas:
                 assert (schema_name, entry) in scheduler._sent
 
             scheduler._sent.clear()
 
+    @mark.django_db
+    class TestCustomQuerySet:
+        @fixture
+        def scheduler(self, app: CeleryApp) -> FakeScheduler:
+            class WithCustomQuerySet(FakeScheduler):
+                @classmethod
+                def get_queryset(cls):
+                    return super().get_queryset().filter(ready=True)
+
+            return WithCustomQuerySet(app)
+
+        def test_unready_tenants_are_not_sent(self, scheduler: FakeScheduler):
+            with schema_context(get_public_schema_name()):
+                Tenant.objects.create(
+                    name="Tenant1",
+                    schema_name="tenant1",
+                    ready=False
+                )
+
+            for task_name, entry in scheduler.schedule.items():
+                scheduler.apply_entry(entry)
+
+            assert scheduler._sent == []
+
 
 @COMMON_PARAMETERS
 class TestTenantAwarePersistentScheduler:
     """This is mostly to test that the serialization of `TenantAwareSchedulerEntry`s works
 
     This is because `PersistentScheduler`'s `schedule` property does a dynamic lookup on the `shelve` db,
     which forces pickling/unpickling of the entries.
```

### Comparing `tenant-schemas-celery-2.1.0/tenant_schemas_celery/test_tasks.py` & `tenant-schemas-celery-2.2.0/tenant_schemas_celery/test_tasks.py`

 * *Files identical despite different names*

### Comparing `tenant-schemas-celery-2.1.0/tenant_schemas_celery.egg-info/PKG-INFO` & `tenant-schemas-celery-2.2.0/tenant_schemas_celery.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenant-schemas-celery
-Version: 2.1.0
+Version: 2.2.0
 Summary: Celery integration for django-tenant-schemas and django-tenants
 Home-page: https://github.com/maciej-gol/tenant-schemas-celery
 Author: Maciej Gol
 Author-email: 1kroolik1@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: Django
@@ -142,22 +142,39 @@
 
 The `reset_remaining_jobs_in_all_schemas` task (called the dispatch task) should be registered in your celery beat schedule. The `reset_remaining_jobs_in_schema` task should be called from the dispatch task.
 
 That way you have full control over which schemas the task should be scheduled in.
 
 
 ### Custom scheduler
-You are using the standard `Scheduler` or `PersistentScheduler` classes provided by `celery`, you can transition to using this package's `TenantAwareScheduler` or `TenantAwarePersistentScheduler` classes. You should then specify the scheduler you want to use in your invocation to `beat`. i.e:
+If you are using the standard `Scheduler` or `PersistentScheduler` classes provided by `celery`, you can transition to using this package's `TenantAwareScheduler` or `TenantAwarePersistentScheduler` classes. You should then specify the scheduler you want to use in the celery beat config or your invocation to `beat`. i.e:
 
 ```bash
 celery -A proj beat --scheduler=tenant_schemas_celery.scheduler.TenantAwareScheduler
 ```
 
 #### Caveats
-`TenantAwareSchedulerMixin` uses a subclass of `SchedulerEntry` that allows the user to provide specific schemas to run a task on. This might prove useful if you have a task you only want to run in the `public` schema or to a subset of your tenants. In order to use set that, you must configure `tenant_schemas` in the tasks definition as such:
+- There's a chance that celery beat will try to run a task for a newly created tenant before its migrations are ready, which could potentially lead to deadlocks. This is specially true with big projects with a lot of migrations and very frequent tasks (i.e: every minute). In order to mitigate it, one could do the following:
+    1. Subclass any of `TenantAwareScheduler` or `TenantAwarePersistentScheduler` and override the `get_queryset` method to match your definition of "ready" tenants. For example, imagine that you had a `ready` flag in your tenant model. You could do the following:
+
+    ```python
+    # tenants_app/scheduler.py
+    class MyTenantAwareScheduler(TenantAwareScheduler):
+        @classmethod
+        def get_queryset(cls):
+            return super().get_queryset().filter(ready=True)
+    ```
+
+    2. Use the new scheduler in your celery beat config or invocation:
+    
+    ```bash
+    celery -A proj beat --scheduler=tenants_app.scheduler.MyTenantAwareScheduler
+    ```
+
+- `TenantAwareSchedulerMixin` uses a subclass of `SchedulerEntry` that allows the user to provide specific schemas to run a task on. This might prove useful if you have a task you only want to run in the `public` schema or to a subset of your tenants. In order to use set that, you must configure `tenant_schemas` in the tasks definition as such:
 
 ```python
 app.conf.beat_schedule = {
     "my-task": {
         "task": "myapp.tasks.my_task",
         "schedule": schedules.crontab(minute="*/5"),
         "tenant_schemas": ["public"]
```

### Comparing `tenant-schemas-celery-2.1.0/tenant_schemas_celery.egg-info/SOURCES.txt` & `tenant-schemas-celery-2.2.0/tenant_schemas_celery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

