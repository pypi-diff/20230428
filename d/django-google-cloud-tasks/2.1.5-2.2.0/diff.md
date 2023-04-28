# Comparing `tmp/django_google_cloud_tasks-2.1.5.tar.gz` & `tmp/django_google_cloud_tasks-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_google_cloud_tasks-2.1.5.tar", max compression
+gzip compressed data, was "django_google_cloud_tasks-2.2.0.tar", max compression
```

## Comparing `django_google_cloud_tasks-2.1.5.tar` & `django_google_cloud_tasks-2.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    11358 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/LICENSE.md
--rw-r--r--   0        0        0      153 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/__init__.py
--rw-r--r--   0        0        0     6245 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/apps.py
--rw-r--r--   0        0        0      446 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/context.py
--rw-r--r--   0        0        0      373 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/exceptions.py
--rw-r--r--   0        0        0     1389 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/field.py
--rw-r--r--   0        0        0        0 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/management/__init__.py
--rw-r--r--   0        0        0      860 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/management/commands/__init__.py
--rw-r--r--   0        0        0      490 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/management/commands/initialize_subscribers.py
--rw-r--r--   0        0        0      394 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/management/commands/initialize_tasks.py
--rw-r--r--   0        0        0      501 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/management/commands/schedule_tasks.py
--rw-r--r--   0        0        0      252 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/middleware/__init__.py
--rw-r--r--   0        0        0     1179 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/middleware/headers_context_middlware.py
--rw-r--r--   0        0        0     1870 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/middleware/pubsub_headers_middleware.py
--rw-r--r--   0        0        0     3888 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/migrations/0001_initial.py
--rw-r--r--   0        0        0     1024 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py
--rw-r--r--   0        0        0        0 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/migrations/__init__.py
--rw-r--r--   0        0        0     4364 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/models.py
--rw-r--r--   0        0        0      925 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/serializers.py
--rw-r--r--   0        0        0     2704 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/signals.py
--rw-r--r--   0        0        0      667 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/__init__.py
--rw-r--r--   0        0        0     1118 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/periodic_task.py
--rw-r--r--   0        0        0     4775 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/publisher_task.py
--rw-r--r--   0        0        0     2522 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/routine_task.py
--rw-r--r--   0        0        0     2610 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/subscriber_task.py
--rw-r--r--   0        0        0     8812 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/task.py
--rw-r--r--   0        0        0        0 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/tests/__init__.py
--rw-r--r--   0        0        0      985 2023-04-12 23:18:32.989646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/tests/factories.py
--rw-r--r--   0        0        0      871 2023-04-12 23:18:32.993646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/tests/tests_base.py
--rw-r--r--   0        0        0      291 2023-04-12 23:18:32.993646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/urls.py
--rw-r--r--   0        0        0     3014 2023-04-12 23:18:32.993646 django_google_cloud_tasks-2.1.5/django_cloud_tasks/views.py
--rw-r--r--   0        0        0      772 2023-04-12 23:18:32.993646 django_google_cloud_tasks-2.1.5/pyproject.toml
--rw-r--r--   0        0        0      357 1970-01-01 00:00:00.000000 django_google_cloud_tasks-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/LICENSE.md
+-rw-r--r--   0        0        0      153 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/__init__.py
+-rw-r--r--   0        0        0     6245 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/apps.py
+-rw-r--r--   0        0        0      446 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/context.py
+-rw-r--r--   0        0        0      373 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/exceptions.py
+-rw-r--r--   0        0        0     1389 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/field.py
+-rw-r--r--   0        0        0        0 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/management/__init__.py
+-rw-r--r--   0        0        0      860 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/management/commands/__init__.py
+-rw-r--r--   0        0        0      490 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/management/commands/initialize_subscribers.py
+-rw-r--r--   0        0        0      394 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/management/commands/initialize_tasks.py
+-rw-r--r--   0        0        0      501 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/management/commands/schedule_tasks.py
+-rw-r--r--   0        0        0      252 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/middleware/__init__.py
+-rw-r--r--   0        0        0     1179 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/middleware/headers_context_middlware.py
+-rw-r--r--   0        0        0     1870 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/middleware/pubsub_headers_middleware.py
+-rw-r--r--   0        0        0     3888 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1024 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py
+-rw-r--r--   0        0        0        0 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/migrations/__init__.py
+-rw-r--r--   0        0        0     4364 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/models.py
+-rw-r--r--   0        0        0      925 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/serializers.py
+-rw-r--r--   0        0        0     2704 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/signals.py
+-rw-r--r--   0        0        0      667 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/tasks/__init__.py
+-rw-r--r--   0        0        0     1118 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/tasks/periodic_task.py
+-rw-r--r--   0        0        0     4775 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/tasks/publisher_task.py
+-rw-r--r--   0        0        0     2522 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/tasks/routine_task.py
+-rw-r--r--   0        0        0     2610 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/tasks/subscriber_task.py
+-rw-r--r--   0        0        0     9166 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/tasks/task.py
+-rw-r--r--   0        0        0        0 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/tests/__init__.py
+-rw-r--r--   0        0        0      985 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/tests/factories.py
+-rw-r--r--   0        0        0      871 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/tests/tests_base.py
+-rw-r--r--   0        0        0      291 2023-04-28 13:30:34.404838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/urls.py
+-rw-r--r--   0        0        0     3014 2023-04-28 13:30:34.408838 django_google_cloud_tasks-2.2.0/django_cloud_tasks/views.py
+-rw-r--r--   0        0        0      772 2023-04-28 13:30:34.408838 django_google_cloud_tasks-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      357 1970-01-01 00:00:00.000000 django_google_cloud_tasks-2.2.0/PKG-INFO
```

### Comparing `django_google_cloud_tasks-2.1.5/LICENSE.md` & `django_google_cloud_tasks-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.5/django_cloud_tasks/apps.py` & `django_google_cloud_tasks-2.2.0/django_cloud_tasks/apps.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.5/django_cloud_tasks/field.py` & `django_google_cloud_tasks-2.2.0/django_cloud_tasks/field.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.5/django_cloud_tasks/management/commands/__init__.py` & `django_google_cloud_tasks-2.2.0/django_cloud_tasks/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.5/django_cloud_tasks/middleware/headers_context_middlware.py` & `django_google_cloud_tasks-2.2.0/django_cloud_tasks/middleware/headers_context_middlware.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.5/django_cloud_tasks/middleware/pubsub_headers_middleware.py` & `django_google_cloud_tasks-2.2.0/django_cloud_tasks/middleware/pubsub_headers_middleware.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.5/django_cloud_tasks/migrations/0001_initial.py` & `django_google_cloud_tasks-2.2.0/django_cloud_tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.5/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py` & `django_google_cloud_tasks-2.2.0/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.5/django_cloud_tasks/models.py` & `django_google_cloud_tasks-2.2.0/django_cloud_tasks/models.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.5/django_cloud_tasks/serializers.py` & `django_google_cloud_tasks-2.2.0/django_cloud_tasks/serializers.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.5/django_cloud_tasks/signals.py` & `django_google_cloud_tasks-2.2.0/django_cloud_tasks/signals.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/__init__.py` & `django_google_cloud_tasks-2.2.0/django_cloud_tasks/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/periodic_task.py` & `django_google_cloud_tasks-2.2.0/django_cloud_tasks/tasks/periodic_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/publisher_task.py` & `django_google_cloud_tasks-2.2.0/django_cloud_tasks/tasks/publisher_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/routine_task.py` & `django_google_cloud_tasks-2.2.0/django_cloud_tasks/tasks/routine_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/subscriber_task.py` & `django_google_cloud_tasks-2.2.0/django_cloud_tasks/tasks/subscriber_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.5/django_cloud_tasks/tasks/task.py` & `django_google_cloud_tasks-2.2.0/django_cloud_tasks/tasks/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -241,14 +241,22 @@
 
             api_kwargs["queue_name"] = backup_queue_name
             outcome = cls._get_tasks_client().push(**api_kwargs)
 
         return TaskMetadata.from_task_obj(task_obj=outcome)
 
     @classmethod
+    def debug(cls, task_id: str):
+        client = cls._get_tasks_client()
+        task_obj = client.get_task(queue_name=cls.queue(), task_name=task_id)
+        task_kwargs = json.loads(task_obj.http_request.body)
+        metadata = TaskMetadata.from_task_obj(task_obj=task_obj)
+        return cls(metadata=metadata).run(**task_kwargs)
+
+    @classmethod
     def name(cls) -> str:
         return str(cls)
 
     @classmethod
     def queue(cls) -> str:
         app_name = get_config(name="app_name")
         return app_name or "tasks"
```

### Comparing `django_google_cloud_tasks-2.1.5/django_cloud_tasks/tests/factories.py` & `django_google_cloud_tasks-2.2.0/django_cloud_tasks/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.5/django_cloud_tasks/tests/tests_base.py` & `django_google_cloud_tasks-2.2.0/django_cloud_tasks/tests/tests_base.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.5/django_cloud_tasks/views.py` & `django_google_cloud_tasks-2.2.0/django_cloud_tasks/views.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.1.5/pyproject.toml` & `django_google_cloud_tasks-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-google-cloud-tasks"
-version = "2.1.5"
+version = "2.2.0"
 description = "Async Tasks with HTTP endpoints"
 authors = ["Joao Daher <joao@daher.dev>"]
 packages = [
     { include = "django_cloud_tasks" },
 ]
 
 [tool.poetry.dependencies]
```

