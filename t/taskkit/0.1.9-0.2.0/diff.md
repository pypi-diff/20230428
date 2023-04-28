# Comparing `tmp/taskkit-0.1.9.tar.gz` & `tmp/taskkit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskkit-0.1.9.tar", last modified: Tue Dec 20 00:21:26 2022, max compression
+gzip compressed data, was "taskkit-0.2.0.tar", last modified: Fri Apr 28 12:44:03 2023, max compression
```

## Comparing `taskkit-0.1.9.tar` & `taskkit-0.2.0.tar`

### file list

```diff
@@ -1,42 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 00:21:26.080677 taskkit-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2022-12-20 00:21:15.000000 taskkit-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2022-12-20 00:21:26.080677 taskkit-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2022-12-20 00:21:15.000000 taskkit-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-20 00:21:15.000000 taskkit-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 00:21:26.080677 taskkit-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2022-12-20 00:21:15.000000 taskkit-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 00:21:26.076677 taskkit-0.1.9/taskkit/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 00:21:26.080677 taskkit-0.1.9/taskkit/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 00:21:26.080677 taskkit-0.1.9/taskkit/contrib/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/contrib/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/contrib/django/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 00:21:26.080677 taskkit-0.1.9/taskkit/contrib/django/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/contrib/django/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/contrib/django/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/contrib/django/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 00:21:26.080677 taskkit-0.1.9/taskkit/impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9942 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/impl/django.py
--rw-r--r--   0 runner    (1001) docker     (123)    10770 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/impl/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/kit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/services.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/threads.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2022-12-20 00:21:15.000000 taskkit-0.1.9/taskkit/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 00:21:26.080677 taskkit-0.1.9/taskkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2022-12-20 00:21:26.000000 taskkit-0.1.9/taskkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      761 2022-12-20 00:21:26.000000 taskkit-0.1.9/taskkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 00:21:26.000000 taskkit-0.1.9/taskkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-20 00:21:26.000000 taskkit-0.1.9/taskkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-20 00:21:26.000000 taskkit-0.1.9/taskkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:44:03.209424 taskkit-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-28 12:43:52.000000 taskkit-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-04-28 12:44:03.209424 taskkit-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-04-28 12:43:52.000000 taskkit-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-28 12:43:52.000000 taskkit-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 12:44:03.209424 taskkit-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-28 12:43:52.000000 taskkit-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:44:03.205424 taskkit-0.2.0/taskkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:44:03.205424 taskkit-0.2.0/taskkit/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:44:03.205424 taskkit-0.2.0/taskkit/contrib/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/contrib/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/contrib/django/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:44:03.209424 taskkit-0.2.0/taskkit/contrib/django/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/contrib/django/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/contrib/django/migrations/0002_taskkittaskqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/contrib/django/migrations/0003_rename_taskkittask_done_began_taskkit_tas_done_e2b997_idx_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/contrib/django/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/contrib/django/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:44:03.209424 taskkit-0.2.0/taskkit/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10827 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/impl/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10867 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/impl/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/kit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-04-28 12:43:52.000000 taskkit-0.2.0/taskkit/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:44:03.205424 taskkit-0.2.0/taskkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-04-28 12:44:03.000000 taskkit-0.2.0/taskkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-28 12:44:03.000000 taskkit-0.2.0/taskkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:44:03.000000 taskkit-0.2.0/taskkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-28 12:44:03.000000 taskkit-0.2.0/taskkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 12:44:03.000000 taskkit-0.2.0/taskkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:44:03.209424 taskkit-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-04-28 12:43:52.000000 taskkit-0.2.0/tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-28 12:43:52.000000 taskkit-0.2.0/tests/test_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-28 12:43:52.000000 taskkit-0.2.0/tests/test_kit.py
```

### Comparing `taskkit-0.1.9/LICENSE` & `taskkit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskkit-0.1.9/PKG-INFO` & `taskkit-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskkit
-Version: 0.1.9
+Version: 0.2.0
 Summary: a distributed task runner
 Home-page: https://github.com/saryou/taskkit
 Author: Ryosuke Sasaki
 Author-email: saryou.ssk@gmail.com
 Project-URL: Bug Tracker, https://github.com/saryou/taskkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `taskkit-0.1.9/README.md` & `taskkit-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `taskkit-0.1.9/setup.py` & `taskkit-0.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,12 +21,13 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(exclude=["tests"]),
     package_dir={"taskkit": "taskkit"},
+    package_data={"taskkit": ["py.typed"]},
     python_requires=">=3.9",
     install_requires=[
         'typing-extensions>=4.0.0',
     ]
 )
```

### Comparing `taskkit-0.1.9/taskkit/backend.py` & `taskkit-0.2.0/taskkit/backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,19 +39,19 @@
         ...
 
     def purge_workers(self, worker_ids: set[str]):
         """purge given workers"""
         ...
 
     def put_tasks(self, *tasks: Task):
-        """Put the tasks to the queue
+        """Put the tasks to the queue"""
+        ...
 
-        If there is same task on the stage, it should be removed from the
-        stage first because it will be called when the task should retry.
-        """
+    def retry_task(self, task: Task):
+        """Remove the task from stage and put it to the queue"""
         ...
 
     def get_queued_tasks(self, group: str, limit: int) -> list[Task]:
         """Get tasks in the queue"""
         ...
 
     def lookup_tasks(self, *task_ids: str) -> dict[str, Optional[Task]]:
```

### Comparing `taskkit-0.1.9/taskkit/contrib/django/migrations/0001_initial.py` & `taskkit-0.2.0/taskkit/contrib/django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `taskkit-0.1.9/taskkit/contrib/django/models.py` & `taskkit-0.2.0/taskkit/contrib/django/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     expires: models.FloatField = models.FloatField(db_index=True)
 
 
 class TaskkitTask(models.Model):
     class Meta:
         db_table = 'taskkit_task'
         app_label = 'taskkit'
-        index_together = (
-            ('began', 'group', 'due'),
-            ('done', 'began'),
-            ('name', 'created'),
-        )
+        indexes = [
+            models.Index(fields=['began', 'group', 'due']),
+            models.Index(fields=['done', 'began']),
+            models.Index(fields=['name', 'created']),
+        ]
 
     id: models.CharField = models.CharField(primary_key=True, max_length=255)
     group: models.CharField = models.CharField(max_length=40)
     name: models.CharField = models.CharField(max_length=255)
     data: models.BinaryField = models.BinaryField()
     due: models.FloatField = models.FloatField()
     created: models.FloatField = models.FloatField()
@@ -52,14 +52,27 @@
 
     result: models.BinaryField = models.BinaryField(null=True)
     error_message: models.TextField = models.TextField(null=True)
     done: models.FloatField = models.FloatField(null=True)
     disposable: models.FloatField = models.FloatField(null=True, db_index=True)
 
 
+class TaskkitTaskQueue(models.Model):
+    class Meta:
+        db_table = 'taskkit_task_queue'
+        app_label = 'taskkit'
+        indexes = [
+            models.Index(fields=['group', 'due']),
+        ]
+
+    id: models.CharField = models.CharField(primary_key=True, max_length=255)
+    group: models.CharField = models.CharField(max_length=40)
+    due: models.FloatField = models.FloatField()
+
+
 class TaskkitSchedulerState(models.Model):
     class Meta:
         db_table = 'taskkit_scheduler_state'
         app_label = 'taskkit'
 
     id: models.CharField = models.CharField(primary_key=True, max_length=255)
     data: models.BinaryField = models.BinaryField()
```

### Comparing `taskkit-0.1.9/taskkit/event.py` & `taskkit-0.2.0/taskkit/event.py`

 * *Files identical despite different names*

### Comparing `taskkit-0.1.9/taskkit/impl/django.py` & `taskkit-0.2.0/taskkit/impl/django.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 from typing import Generator, Optional
 
 from django.db.transaction import atomic, Atomic
 from django.db.utils import OperationalError, IntegrityError
 
 from ..backend import Backend, Lock, NotFound, NoResult, Failed
-from ..contrib.django.models import TaskkitControlEvent, TaskkitLock, TaskkitWorker, TaskkitTask, TaskkitSchedulerState
+from ..contrib.django.models import TaskkitControlEvent, TaskkitLock, TaskkitWorker, TaskkitTask, TaskkitTaskQueue, TaskkitSchedulerState
 from ..event import EventBridge, ControlEvent, encode_control_event, decode_control_event
 from ..kit import Kit
 from ..stage import StageInfo
 from ..task import Task, TaskHandler
 from ..utils import cur_ts
 
 
@@ -44,29 +44,29 @@
             return True
 
         if not self.ensured:
             self.ensured = True
             try:
                 with atomic():
                     TaskkitLock.objects\
-                        .select_for_update(nowait=True)\
+                        .select_for_update(skip_locked=True)\
                         .get(pk=self.target)
             except TaskkitLock.DoesNotExist:
                 try:
                     TaskkitLock.objects.create(pk=self.target)
                 except IntegrityError:
                     pass
             except Exception:
                 pass
 
         self.atomic = atomic()
         self.atomic.__enter__()
         try:
             TaskkitLock.objects\
-                .select_for_update(nowait=True)\
+                .select_for_update(skip_locked=True)\
                 .get(pk=self.target)
             self.acquired = True
             return True
         except Exception:
             self.atomic.__exit__(*sys.exc_info())
             self.atomic = None
             return False
@@ -101,16 +101,25 @@
         TaskkitWorker.objects.filter(pk__in=worker_ids).delete()
 
     def put_tasks(self, *tasks: Task):
         if not tasks:
             return
         objects = [self._task_to_db(t) for t in tasks]
         with atomic():
-            self.discard_tasks(*[t.pk for t in objects])
             TaskkitTask.objects.bulk_create(objects, ignore_conflicts=True)
+            TaskkitTaskQueue.objects.bulk_create([
+                self._db_task_to_queue(t) for t in objects
+            ], ignore_conflicts=True)
+
+    def retry_task(self, task: Task):
+        with atomic():
+            self.discard_tasks(task.id)
+            db_task = self._task_to_db(task)
+            db_task.save()
+            self._db_task_to_queue(db_task).save()
 
     def get_queued_tasks(self, group: str, limit: int) -> list[Task]:
         return [
             self._db_to_task(t) for t in TaskkitTask.objects
             .filter(began__isnull=True, group=group)
             .order_by('due')[:limit]
         ]
@@ -119,34 +128,47 @@
         tasks = {
             t.pk: self._db_to_task(t)
             for t in TaskkitTask.objects.filter(pk__in=task_ids)
         }
         return {tid: tasks.get(tid) for tid in task_ids}
 
     def assign_task(self, group: str, worker_id: str) -> Optional[Task]:
-        for pk in TaskkitTask.objects\
-                .filter(began__isnull=True, group=group, due__lt=cur_ts())\
-                .values_list('pk', flat=True)\
-                .order_by('due')[:50]:
-            with atomic():
-                try:
-                    db_task = TaskkitTask.objects\
-                        .select_for_update(nowait=True)\
-                        .get(pk=pk)
-                    if db_task.began is None:
-                        db_task.assignee_worker_id = worker_id
-                        db_task.began = cur_ts()
-                        db_task.save()
-                        return self._db_to_task(db_task)
-                except (OperationalError, TaskkitTask.DoesNotExist):
-                    pass
+        n = 8
+        while True:
+            pks = list(
+                TaskkitTaskQueue.objects
+                .filter(group=group, due__lt=cur_ts())
+                .values_list('pk', flat=True)
+                .order_by('due')[:n])
+            for pk in pks:
+                if (task := self._assign(pk, worker_id)):
+                    return task
+            if len(pks) < n:
+                return None
+            n *= 2
+
+    def _assign(self, task_id: str, worker_id: str) -> Optional[Task]:
+        with atomic():
+            try:
+                db_task = TaskkitTask.objects\
+                    .select_for_update(skip_locked=True)\
+                    .get(pk=task_id)
+                TaskkitTaskQueue.objects.filter(id=task_id).delete()
+                if db_task.began is None:
+                    db_task.assignee_worker_id = worker_id
+                    db_task.began = cur_ts()
+                    db_task.save()
+                    return self._db_to_task(db_task)
+            except (OperationalError, TaskkitTask.DoesNotExist):
+                pass
         return None
 
     def discard_tasks(self, *task_ids: str):
         TaskkitTask.objects.filter(pk__in=task_ids).delete()
+        TaskkitTaskQueue.objects.filter(pk__in=task_ids).delete()
 
     def succeed(self, task: Task, result: bytes):
         with atomic():
             try:
                 db_task = TaskkitTask.objects\
                     .select_for_update()\
                     .get(pk=task.id)
@@ -218,16 +240,16 @@
 
     def restore(self, info: StageInfo):
         try:
             task = TaskkitTask.objects\
                 .filter(began__isnull=False)\
                 .get(pk=info.task_id)
             task.began = None
-            task.assignee_worker_id = None
             task.save()
+            self._db_task_to_queue(task).save()
         except TaskkitTask.DoesNotExist:
             pass
 
     def get_lock(self, target: str) -> Lock:
         return DjangoLock(target)
 
     def persist_scheduler_state_and_put_tasks(self,
@@ -282,10 +304,13 @@
             assignee_worker_id=None,
             began=None,
             result=None,
             done=None,
             disposable=None,
         )
 
+    def _db_task_to_queue(self, t: TaskkitTask) -> TaskkitTaskQueue:
+        return TaskkitTaskQueue(id=t.id, group=t.group, due=t.due)
+
 
 def make_kit(handler: TaskHandler) -> Kit:
     return Kit(DjangoBackend(), DjangoEventBridge(), handler)
```

### Comparing `taskkit-0.1.9/taskkit/impl/redis.py` & `taskkit-0.2.0/taskkit/impl/redis.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,22 +110,26 @@
     def put_tasks(self, *tasks: Task):
         if not tasks:
             return
         with self.redis.pipeline() as pipe:
             self._put_tasks(pipe, *tasks)
             pipe.execute()
 
+    def retry_task(self, task: Task):
+        with self.redis.pipeline() as pipe:
+            pipe.zrem(self.stage_queue_key(), task.id)
+            pipe.hdel(self.stage_info_key(), task.id)
+            self._put_tasks(pipe, task)
+            pipe.execute()
+
     def _put_tasks(self, pipe: Pipeline, *_tasks: Task):
         if not _tasks:
             return
+        self._put_task_data(pipe, *_tasks)
         for group, tasks in Task.group_tasks(*_tasks).items():
-            task_ids = [t.id for t in tasks]
-            pipe.zrem(self.stage_queue_key(), *task_ids)
-            pipe.hdel(self.stage_info_key(), *task_ids)
-            self._put_task_data(pipe, *_tasks)
             pipe.zadd(self.queue_key(group), {t.id: t.due for t in tasks})
 
     def _put_task_data(self, pipe: Pipeline, *tasks: Task):
         if not tasks:
             return
         pipe.hset(self.data_store_key(), mapping={
             t.id: t.data for t in tasks
```

### Comparing `taskkit-0.1.9/taskkit/process.py` & `taskkit-0.2.0/taskkit/process.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 from datetime import tzinfo
 from multiprocessing import Process, Event
+from typing import Union
 
 from .backend import Backend
 from .event import EventBridge
 from .scheduler import ScheduleEntry, Scheduler
 from .signal import SignalCaptured, capture_signals, signal
 from .task import TaskHandler
 from .threads import WorkerThread, ServiceThread
@@ -17,51 +18,74 @@
     def __init__(self,
                  num_worker_threads_per_group: dict[str, int],
                  backend: Backend,
                  bridge: EventBridge,
                  handler: TaskHandler,
                  schedule_entries: dict[str, list[ScheduleEntry]],
                  tzinfo: tzinfo,
+                 polling_interval: Union[dict[str, float], float, None] = None,
+                 helper_services: bool = True,
                  **kwargs):
         assert all(n >= 0 for n in num_worker_threads_per_group.values()),\
             'All values for num_worker_threads_per_group must be positive int.'
         self.num_worker_threads = num_worker_threads_per_group
         self.backend = backend
         self.bridge = bridge
         self.handler = handler
         self.schedule_entries = schedule_entries
         self.tzinfo = tzinfo
+
+        if isinstance(polling_interval, float):
+            polling_interval = {
+                group: polling_interval
+                for group in num_worker_threads_per_group.keys()
+            }
+        elif polling_interval is None:
+            polling_interval = dict()
+
+        self.polling_interval = {
+            group: polling_interval.get(group) or _make_polling_interval(n)
+            for group, n in num_worker_threads_per_group.items()
+        }
+
+        self.helper_services = helper_services
+
         self._terminate_event = Event()
         super().__init__(**kwargs)
 
     def is_active(self) -> bool:
         return not self._terminate_event.is_set()
 
     def run(self):
         _id = f'{os.getpid()}'
         logger.info(f'[{_id}] taskkit process started: '
                     f'{self.num_worker_threads}')
 
         backend = self.backend
         workers: list[WorkerThread] = []
         for group, n in self.num_worker_threads.items():
-            for _ in range(n):
-                w = WorkerThread(group, backend, self.handler)
+            interval = self.polling_interval[group]
+            for i in range(n):
+                w = WorkerThread(group, backend, self.handler,
+                                 polling_interval=interval,
+                                 initial_delay=interval / n * i)
                 w.start()
                 workers.append(w)
         refresh_ttl = ServiceThread(
             RefreshWorkerLifetime(backend, workers))
         refresh_ttl.start()
 
         services = [
             *[ServiceThread(Scheduler(name, backend, entries, self.tzinfo))
               for name, entries in self.schedule_entries.items() if entries],
-            ServiceThread(RestoreAbandonedTasks(backend)),
-            ServiceThread(PurgeDeadWorkers(backend)),
-            ServiceThread(DiscardDisposableTasks(backend)),
+            *([
+                ServiceThread(RestoreAbandonedTasks(backend)),
+                ServiceThread(PurgeDeadWorkers(backend)),
+                ServiceThread(DiscardDisposableTasks(backend)),
+            ] if self.helper_services else []),
         ]
         for service in services:
             service.start()
 
         alive = {g for g, n in self.num_worker_threads.items() if n > 0}
 
         try:
@@ -103,7 +127,11 @@
             service.should_stop = True
         for service in services:
             service.join()
         for w in workers:
             w.join()
         refresh_ttl.should_stop = True
         refresh_ttl.join()
+
+
+def _make_polling_interval(num_threads: int) -> float:
+    return max(1, min(4, num_threads * 0.25))
```

### Comparing `taskkit-0.1.9/taskkit/result.py` & `taskkit-0.2.0/taskkit/result.py`

 * *Files identical despite different names*

### Comparing `taskkit-0.1.9/taskkit/scheduler.py` & `taskkit-0.2.0/taskkit/scheduler.py`

 * *Files identical despite different names*

### Comparing `taskkit-0.1.9/taskkit/services.py` & `taskkit-0.2.0/taskkit/services.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import Protocol, Sequence
 
 from .backend import Backend
 from .utils import cur_ts, logger
-from .worker import WORKER_TTL_IN_SEC
+
+
+WORKER_TTL_IN_SEC = 15
 
 
 class Service(Protocol):
     def __call__(self) -> float:
         """Call the service.
 
         It should returns the time interval to wait for next call.
@@ -30,15 +32,15 @@
         self.backend = backend
         self.workers = list(workers)
 
     def __call__(self) -> float:
         self.backend.set_worker_ttl(
             {w.get_id() for w in self.workers if w.is_alive()},
             cur_ts() + WORKER_TTL_IN_SEC)
-        return 1.0
+        return WORKER_TTL_IN_SEC / 3
 
 
 class PurgeDeadWorkers(Service):
     def __init__(self, backend: Backend, **kwargs):
         self.backend = backend
         self.lock = backend.get_lock('purge_workers')
 
@@ -50,38 +52,38 @@
                     wid for (wid, ttl) in self.backend.get_workers()
                     if ttl < now
                 }
                 if to_purge:
                     self.backend.purge_workers(to_purge)
             finally:
                 self.lock.release()
-        return 10.0
+        return WORKER_TTL_IN_SEC
 
 
 class RestoreAbandonedTasks(Service):
     def __init__(self, backend: Backend, **kwargs):
         self.backend = backend
         self.lock = backend.get_lock('restore_abandoned_tasks')
 
     def __call__(self) -> float:
         if self.lock.acquire():
             try:
-                stage_info_list = self.backend.get_stage_info(50)
+                stage_info_list = self.backend.get_stage_info(100)
                 now = cur_ts()
                 active_worker_ids = {
                     wid for (wid, ttl) in self.backend.get_workers()
                     if ttl >= now
                 }
                 for stage_info in stage_info_list:
                     if stage_info.worker_id not in active_worker_ids:
                         logger.info(f'restore task `{stage_info.task_id}`')
                         self.backend.restore(stage_info)
             finally:
                 self.lock.release()
-        return 5.0
+        return 15.0
 
 
 class DiscardDisposableTasks(Service):
     def __init__(self, backend: Backend, **kwargs):
         self.backend = backend
         self.lock = backend.get_lock('discard_disposable_tasks')
```

### Comparing `taskkit-0.1.9/taskkit/signal.py` & `taskkit-0.2.0/taskkit/signal.py`

 * *Files identical despite different names*

### Comparing `taskkit-0.1.9/taskkit/stage.py` & `taskkit-0.2.0/taskkit/stage.py`

 * *Files identical despite different names*

### Comparing `taskkit-0.1.9/taskkit/task.py` & `taskkit-0.2.0/taskkit/task.py`

 * *Files identical despite different names*

### Comparing `taskkit-0.1.9/taskkit/threads.py` & `taskkit-0.2.0/taskkit/threads.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,45 +3,14 @@
 from .backend import Backend
 from .services import Service
 from .task import TaskHandler
 from .utils import logger
 from .worker import Worker
 
 
-class WorkerThread(Thread):
-    def __init__(self,
-                 group: str,
-                 backend: Backend,
-                 handler: TaskHandler,
-                 **kwargs):
-        self.group = group
-        self.worker = Worker(group, backend, handler)
-        self.should_stop = False
-        self.paused = False
-        super().__init__(**kwargs)
-
-    @property
-    def id(self) -> str:
-        return self.worker.id
-
-    def get_id(self) -> str:
-        return self.worker.id
-
-    def run(self):
-        logger.info(f'[{self.id}] worker thread started')
-        while not self.should_stop:
-            if self.paused:
-                time.sleep(1)
-                continue
-
-            if not self.worker():
-                time.sleep(1)
-        logger.info(f'[{self.id}] worker thread stopped')
-
-
 class ServiceThread(Thread):
     def __init__(self,
                  service: Service,
                  **kwargs):
         self.should_stop = False
         self.service = service
         super().__init__(**kwargs)
@@ -56,7 +25,42 @@
                     if self.should_stop:
                         return
             except Exception:
                 logger.exception(
                     'Unexpected exception occurred during service call '
                     f'({self.service.__class__.__qualname__})')
                 time.sleep(1)
+
+
+class WorkerThread(ServiceThread):
+    def __init__(self,
+                 group: str,
+                 backend: Backend,
+                 handler: TaskHandler,
+                 polling_interval: float,
+                 initial_delay: float,
+                 **kwargs):
+        self.group = group
+        self.worker = Worker(group, backend, handler, polling_interval)
+        self.initial_delay = initial_delay
+        super().__init__(service=self.worker, **kwargs)
+
+    @property
+    def id(self) -> str:
+        return self.worker.id
+
+    def get_id(self) -> str:
+        return self.worker.id
+
+    @property
+    def paused(self) -> bool:
+        return self.worker.paused
+
+    @paused.setter
+    def paused(self, paused: bool):
+        self.worker.paused = paused
+
+    def run(self):
+        logger.info(f'[{self.id}] worker thread started')
+        time.sleep(self.initial_delay)
+        super().run()
+        logger.info(f'[{self.id}] worker thread stopped')
```

### Comparing `taskkit-0.1.9/taskkit/utils.py` & `taskkit-0.2.0/taskkit/utils.py`

 * *Files identical despite different names*

### Comparing `taskkit-0.1.9/taskkit/worker.py` & `taskkit-0.2.0/taskkit/worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 from traceback import format_exc
 from typing import Any
 from uuid import uuid4
 
 from .backend import Backend
 from .result import Result, prevent_to_wait_result, ResultGetPrevented
+from .services import Service
 from .task import Task, TaskHandler, DiscardTask
 from .utils import logger
 
 
 REASON_TO_PREVENT_WAIT_RESULT =\
     'You should avoid to wait results of other tasks because it may causes '\
     'deadlock. If you can assure that it is safe you can pass '\
     '`avoid_assertion=True` for the `get` method.'
 
-WORKER_TTL_IN_SEC = 10
 
-
-class Worker:
+class Worker(Service):
     def __init__(self,
                  group: str,
                  backend: Backend,
-                 handler: TaskHandler):
+                 handler: TaskHandler,
+                 polling_interval: float = 1):
         self.id = f'wk_{group}_{uuid4().hex}'
         self.group = group
         self.backend = backend
         self.handler = handler
+        self.polling_interval = polling_interval
+        self.paused = False
 
-    def __call__(self) -> bool:
+    def __call__(self) -> float:
         """Pop a task from the queue and handle the task.
 
-        If there is a task to handle then it returns whether if task finished
-        successfully otherwise returns False.
+        If there is a task to handle then it returns zero to indicate that
+        it's next call should be right away otherwise it returns time to wait.
+        If it is paused, it won't handle task and just return the time to wait.
         """
 
+        if self.paused:
+            return 1
+
         try:
             task = self.backend.assign_task(self.group, self.id)
             if task is None:
-                return False
+                return self.polling_interval
             else:
                 self._handle_task(task)
-                return True
+                return 0
         except Exception:
             logger.exception(f'[{self.id}] unexpected exception')
-            return False
+            return 1
 
     def _handle_task(self, task: Task):
         logger.info(f'[{self.id}] handle task ({task.id}: {task.name})')
         try:
             with prevent_to_wait_result(REASON_TO_PREVENT_WAIT_RESULT):
                 ret = self.handler.encode_result(
                     task, self.handler.handle(task))
@@ -90,15 +96,15 @@
         else:
             self._retry(task, interval)
 
     def _retry(self, task: Task, interval: float):
         clone = task.clone_for_retry(interval)
         logger.info(f'[{self.id}] retry n{clone.retry_count} '
                     f'({task.id}: {task.name})')
-        self.backend.put_tasks(clone)
+        self.backend.retry_task(clone)
 
 
 class EagerWorker(Worker):
     def __init__(self, backend: Backend, handler: TaskHandler):
         super().__init__('_', backend, handler)
 
     def __call__(self) -> bool:
```

### Comparing `taskkit-0.1.9/taskkit.egg-info/PKG-INFO` & `taskkit-0.2.0/taskkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskkit
-Version: 0.1.9
+Version: 0.2.0
 Summary: a distributed task runner
 Home-page: https://github.com/saryou/taskkit
 Author: Ryosuke Sasaki
 Author-email: saryou.ssk@gmail.com
 Project-URL: Bug Tracker, https://github.com/saryou/taskkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

