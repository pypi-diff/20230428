# Comparing `tmp/django-bulk-signals-0.2.1.tar.gz` & `tmp/django-bulk-signals-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-bulk-signals-0.2.1.tar", last modified: Wed Dec  7 22:06:21 2022, max compression
+gzip compressed data, was "django-bulk-signals-0.3.0.tar", last modified: Fri Apr 28 11:51:32 2023, max compression
```

## Comparing `django-bulk-signals-0.2.1.tar` & `django-bulk-signals-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 22:06:21.225988 django-bulk-signals-0.2.1/
--rw-r--r--   0 root         (0) root         (0)     1053 2022-12-07 22:06:18.000000 django-bulk-signals-0.2.1/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1063 2022-12-07 22:06:18.000000 django-bulk-signals-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       33 2022-12-07 22:06:18.000000 django-bulk-signals-0.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2468 2022-12-07 22:06:21.225988 django-bulk-signals-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1324 2022-12-07 22:06:18.000000 django-bulk-signals-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 22:06:21.221988 django-bulk-signals-0.2.1/bulk_signals/
--rw-r--r--   0 root         (0) root         (0)       46 2022-12-07 22:06:18.000000 django-bulk-signals-0.2.1/bulk_signals/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2244 2022-12-07 22:06:18.000000 django-bulk-signals-0.2.1/bulk_signals/apps.py
--rw-r--r--   0 root         (0) root         (0)      227 2022-12-07 22:06:18.000000 django-bulk-signals-0.2.1/bulk_signals/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 22:06:21.225988 django-bulk-signals-0.2.1/bulk_signals/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-07 22:06:18.000000 django-bulk-signals-0.2.1/bulk_signals/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      218 2022-12-07 22:06:18.000000 django-bulk-signals-0.2.1/bulk_signals/tests/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 22:06:21.225988 django-bulk-signals-0.2.1/bulk_signals/tests/migrations/
--rw-r--r--   0 root         (0) root         (0)      762 2022-12-07 22:06:18.000000 django-bulk-signals-0.2.1/bulk_signals/tests/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-07 22:06:18.000000 django-bulk-signals-0.2.1/bulk_signals/tests/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      722 2022-12-07 22:06:18.000000 django-bulk-signals-0.2.1/bulk_signals/tests/models.py
--rw-r--r--   0 root         (0) root         (0)      322 2022-12-07 22:06:18.000000 django-bulk-signals-0.2.1/bulk_signals/tests/settings.py
--rw-r--r--   0 root         (0) root         (0)     3104 2022-12-07 22:06:18.000000 django-bulk-signals-0.2.1/bulk_signals/tests/tests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 22:06:21.225988 django-bulk-signals-0.2.1/django_bulk_signals.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2468 2022-12-07 22:06:21.000000 django-bulk-signals-0.2.1/django_bulk_signals.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2022-12-07 22:06:21.000000 django-bulk-signals-0.2.1/django_bulk_signals.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-07 22:06:21.000000 django-bulk-signals-0.2.1/django_bulk_signals.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-12-07 22:06:21.000000 django-bulk-signals-0.2.1/django_bulk_signals.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-12-07 22:06:21.000000 django-bulk-signals-0.2.1/django_bulk_signals.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      593 2022-12-07 22:06:21.225988 django-bulk-signals-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2370 2022-12-07 22:06:18.000000 django-bulk-signals-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:51:32.715282 django-bulk-signals-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1253 2023-04-28 11:51:29.000000 django-bulk-signals-0.3.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       33 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-04-28 11:51:32.715282 django-bulk-signals-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1324 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:51:32.711282 django-bulk-signals-0.3.0/bulk_signals/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 11:51:29.000000 django-bulk-signals-0.3.0/bulk_signals/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2294 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/bulk_signals/apps.py
+-rw-r--r--   0 root         (0) root         (0)      203 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/bulk_signals/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:51:32.711282 django-bulk-signals-0.3.0/bulk_signals/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/bulk_signals/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      194 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/bulk_signals/tests/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:51:32.711282 django-bulk-signals-0.3.0/bulk_signals/tests/migrations/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/bulk_signals/tests/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/bulk_signals/tests/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      887 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/bulk_signals/tests/models.py
+-rw-r--r--   0 root         (0) root         (0)      298 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/bulk_signals/tests/settings.py
+-rw-r--r--   0 root         (0) root         (0)     3512 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/bulk_signals/tests/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:51:32.715282 django-bulk-signals-0.3.0/django_bulk_signals.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-04-28 11:51:32.000000 django-bulk-signals-0.3.0/django_bulk_signals.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-04-28 11:51:32.000000 django-bulk-signals-0.3.0/django_bulk_signals.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 11:51:32.000000 django-bulk-signals-0.3.0/django_bulk_signals.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-28 11:51:32.000000 django-bulk-signals-0.3.0/django_bulk_signals.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 11:51:32.000000 django-bulk-signals-0.3.0/django_bulk_signals.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      593 2023-04-28 11:51:32.715282 django-bulk-signals-0.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-04-28 11:51:28.000000 django-bulk-signals-0.3.0/setup.py
```

### Comparing `django-bulk-signals-0.2.1/CHANGELOG.md` & `django-bulk-signals-0.3.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.3.0 (2023-04-28)
+### Feature
+* Post query update signal now passed the update count ([`e2424c9`](https://github.com/awmath/django-bulk-signals/commit/e2424c9a6033aab0164e94ff32c6699658291555))
+
 ## v0.2.1 (2022-12-07)
 ### Fix
 * Added missing tests module ([`9d4581c`](https://github.com/awmath/django-bulk-signals/commit/9d4581cbd0bc5a6f6d212e1ca796a1349dad2f79))
 * Bulk_update no longer triggers the pre_update signal ([`809c86a`](https://github.com/awmath/django-bulk-signals/commit/809c86adcbe92d485ca0c1c48b59792ec26efdd4))
 
 ## v0.2.0 (2022-12-07)
 ### Feature
```

### Comparing `django-bulk-signals-0.2.1/LICENSE` & `django-bulk-signals-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-bulk-signals-0.2.1/PKG-INFO` & `django-bulk-signals-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bulk-signals
-Version: 0.2.1
+Version: 0.3.0
 Summary: A product aggregation function to a postgres database and makes it available with django
 Home-page: https://github.com/awmath/django-bulk-signals
 Download-URL: https://github.com/awmath/django-bulk-signals
 Author: Axel Wegener
 Author-email: pypi@sparse-space.de
 License: MIT
 Keywords: django
```

### Comparing `django-bulk-signals-0.2.1/README.md` & `django-bulk-signals-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `django-bulk-signals-0.2.1/bulk_signals/apps.py` & `django-bulk-signals-0.3.0/bulk_signals/apps.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from django.apps import AppConfig, apps
 
 from bulk_signals import signals
 
 
 class BulkSignalsConfig(AppConfig):
     default_auto_field = "django.db.models.BigAutoField"
@@ -54,13 +53,16 @@
                 return base_update(queryset, **kwargs)
 
             signals.pre_query_update.send(
                 sender=model, queryset=queryset, update_kwargs=kwargs
             )
             return_val = base_update(queryset, **kwargs)
             signals.post_query_update.send(
-                sender=model, queryset=queryset, update_kwargs=kwargs
+                sender=model,
+                queryset=queryset,
+                update_kwargs=kwargs,
+                update_count=return_val,
             )
 
             return return_val
 
         QuerySet.update = update
```

### Comparing `django-bulk-signals-0.2.1/bulk_signals/tests/models.py` & `django-bulk-signals-0.3.0/bulk_signals/tests/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from django.db import models
 from django.dispatch import receiver
 
 from bulk_signals import signals
 
 
 def create_stub(*args, **kwargs):
@@ -29,9 +28,18 @@
 
 @receiver(signals.pre_query_update)
 @receiver(signals.post_query_update)
 def call_query_update_stub(*args, **kwargs):
     query_update_stub(*args, **kwargs)
 
 
+def query_update_post_stub(*args, **kwargs):
+    pass
+
+
+@receiver(signals.post_query_update)
+def call_post_query_update_stub(*args, **kwargs):
+    query_update_post_stub(*args, **kwargs)
+
+
 class BulkTestModel(models.Model):
     num = models.IntegerField(default=0)
```

### Comparing `django-bulk-signals-0.2.1/bulk_signals/tests/tests.py` & `django-bulk-signals-0.3.0/bulk_signals/tests/tests.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 import pytest
 from django.db.models import Sum
 from django.dispatch import receiver
 
 from bulk_signals import signals
 
 from .models import BulkTestModel
@@ -97,7 +96,24 @@
     @receiver(signal=signals.pre_query_update)
     def half(sender, queryset, update_kwargs, **kwargs):
         update_kwargs["num"] /= 2
 
     BulkTestModel.objects.update(num=8)
 
     assert BulkTestModel.objects.get().num == 4
+
+
+def query_update_count_test(*args, **kwargs):
+    assert kwargs["update_count"] == 2
+
+
+def test_query_update_return_count(mocker):
+    BulkTestModel.objects.create(num=1)
+    BulkTestModel.objects.create(num=1)
+    BulkTestModel.objects.create(num=2)
+
+    mocker.patch(
+        "bulk_signals.tests.models.query_update_post_stub",
+        wraps=query_update_count_test,
+    )
+
+    BulkTestModel.objects.filter(num=1).update(num=3)
```

### Comparing `django-bulk-signals-0.2.1/django_bulk_signals.egg-info/PKG-INFO` & `django-bulk-signals-0.3.0/django_bulk_signals.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bulk-signals
-Version: 0.2.1
+Version: 0.3.0
 Summary: A product aggregation function to a postgres database and makes it available with django
 Home-page: https://github.com/awmath/django-bulk-signals
 Download-URL: https://github.com/awmath/django-bulk-signals
 Author: Axel Wegener
 Author-email: pypi@sparse-space.de
 License: MIT
 Keywords: django
```

### Comparing `django-bulk-signals-0.2.1/django_bulk_signals.egg-info/SOURCES.txt` & `django-bulk-signals-0.3.0/django_bulk_signals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-bulk-signals-0.2.1/setup.cfg` & `django-bulk-signals-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-bulk-signals-0.2.1/setup.py` & `django-bulk-signals-0.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 import os
 from distutils.core import setup
 
 from setuptools import find_packages
 
 from bulk_signals import __version__
```

