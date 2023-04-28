# Comparing `tmp/bitmapist-3.98.tar.gz` & `tmp/bitmapist-3.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bitmapist-3.98.tar", last modified: Mon Jul  4 19:20:16 2016, max compression
+gzip compressed data, was "dist/bitmapist-3.99.tar", last modified: Wed Dec  7 15:10:05 2016, max compression
```

## Comparing `bitmapist-3.98.tar` & `bitmapist-3.99.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2016-07-04 19:20:16.000000 bitmapist-3.98/
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2016-07-04 19:20:16.000000 bitmapist-3.98/bitmapist/
--rw-r--r--   0 roman      (501) staff       (20)    19668 2016-04-27 09:41:27.000000 bitmapist-3.98/bitmapist/__init__.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2016-07-04 19:20:16.000000 bitmapist-3.98/bitmapist/cohort/
--rw-r--r--   0 roman      (501) staff       (20)    11143 2016-07-04 19:20:08.000000 bitmapist-3.98/bitmapist/cohort/__init__.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2016-07-04 19:20:16.000000 bitmapist-3.98/bitmapist/cohort/tmpl/
--rw-r--r--   0 roman      (501) staff       (20)     3109 2016-04-20 11:54:43.000000 bitmapist-3.98/bitmapist/cohort/tmpl/form_data.mako
--rw-r--r--   0 roman      (501) staff       (20)     3119 2016-04-19 14:13:48.000000 bitmapist-3.98/bitmapist/cohort/tmpl/table_data.mako
--rw-r--r--   0 roman      (501) staff       (20)      701 2016-04-19 14:13:48.000000 bitmapist-3.98/bitmapist/cohort/tmpl/table_data_csv.mako
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2016-07-04 19:20:16.000000 bitmapist-3.98/bitmapist.egg-info/
--rw-r--r--   0 roman      (501) staff       (20)        1 2016-07-04 19:20:16.000000 bitmapist-3.98/bitmapist.egg-info/dependency_links.txt
--rw-r--r--   0 roman      (501) staff       (20)        1 2016-04-20 11:54:56.000000 bitmapist-3.98/bitmapist.egg-info/not-zip-safe
--rw-r--r--   0 roman      (501) staff       (20)     5143 2016-07-04 19:20:16.000000 bitmapist-3.98/bitmapist.egg-info/PKG-INFO
--rw-r--r--   0 roman      (501) staff       (20)       45 2016-07-04 19:20:16.000000 bitmapist-3.98/bitmapist.egg-info/requires.txt
--rw-r--r--   0 roman      (501) staff       (20)      529 2016-07-04 19:20:16.000000 bitmapist-3.98/bitmapist.egg-info/SOURCES.txt
--rw-r--r--   0 roman      (501) staff       (20)       10 2016-07-04 19:20:16.000000 bitmapist-3.98/bitmapist.egg-info/top_level.txt
--rw-r--r--   0 roman      (501) staff       (20)       42 2016-04-19 14:13:48.000000 bitmapist-3.98/MANIFEST.in
--rw-r--r--   0 roman      (501) staff       (20)     5143 2016-07-04 19:20:16.000000 bitmapist-3.98/PKG-INFO
--rw-r--r--   0 roman      (501) staff       (20)       59 2016-07-04 19:20:16.000000 bitmapist-3.98/setup.cfg
--rwxr-xr-x   0 roman      (501) staff       (20)     5035 2016-07-04 19:20:08.000000 bitmapist-3.98/setup.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2016-07-04 19:20:16.000000 bitmapist-3.98/test/
--rw-r--r--   0 roman      (501) staff       (20)     7240 2016-04-27 09:41:27.000000 bitmapist-3.98/test/test_bitmapist.py
--rw-r--r--   0 roman      (501) staff       (20)     1575 2016-04-27 09:41:27.000000 bitmapist-3.98/test/test_cohort.py
--rw-r--r--   0 roman      (501) staff       (20)     1013 2016-04-19 14:13:48.000000 bitmapist-3.98/test/test_delta_methods.py
--rw-r--r--   0 roman      (501) staff       (20)      216 2016-04-19 14:13:48.000000 bitmapist-3.98/test/test_equality.py
--rw-r--r--   0 roman      (501) staff       (20)      929 2016-04-19 14:13:48.000000 bitmapist-3.98/test/test_from_date.py
--rw-r--r--   0 roman      (501) staff       (20)      449 2016-04-19 14:13:48.000000 bitmapist-3.98/test/test_period_start_end.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2016-12-07 15:10:05.000000 bitmapist-3.99/
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2016-12-07 15:10:05.000000 bitmapist-3.99/bitmapist/
+-rw-r--r--   0 roman      (501) staff       (20)    22064 2016-12-07 14:36:26.000000 bitmapist-3.99/bitmapist/__init__.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2016-12-07 15:10:05.000000 bitmapist-3.99/bitmapist/cohort/
+-rw-r--r--   0 roman      (501) staff       (20)    11143 2016-07-04 19:20:08.000000 bitmapist-3.99/bitmapist/cohort/__init__.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2016-12-07 15:10:05.000000 bitmapist-3.99/bitmapist/cohort/tmpl/
+-rw-r--r--   0 roman      (501) staff       (20)     3109 2016-04-20 11:54:43.000000 bitmapist-3.99/bitmapist/cohort/tmpl/form_data.mako
+-rw-r--r--   0 roman      (501) staff       (20)     3119 2016-04-19 14:13:48.000000 bitmapist-3.99/bitmapist/cohort/tmpl/table_data.mako
+-rw-r--r--   0 roman      (501) staff       (20)      701 2016-04-19 14:13:48.000000 bitmapist-3.99/bitmapist/cohort/tmpl/table_data_csv.mako
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2016-12-07 15:10:05.000000 bitmapist-3.99/bitmapist.egg-info/
+-rw-r--r--   0 roman      (501) staff       (20)        1 2016-12-07 15:10:04.000000 bitmapist-3.99/bitmapist.egg-info/dependency_links.txt
+-rw-r--r--   0 roman      (501) staff       (20)        1 2016-04-20 11:54:56.000000 bitmapist-3.99/bitmapist.egg-info/not-zip-safe
+-rw-r--r--   0 roman      (501) staff       (20)     5143 2016-12-07 15:10:04.000000 bitmapist-3.99/bitmapist.egg-info/PKG-INFO
+-rw-r--r--   0 roman      (501) staff       (20)       57 2016-12-07 15:10:04.000000 bitmapist-3.99/bitmapist.egg-info/requires.txt
+-rw-r--r--   0 roman      (501) staff       (20)      556 2016-12-07 15:10:05.000000 bitmapist-3.99/bitmapist.egg-info/SOURCES.txt
+-rw-r--r--   0 roman      (501) staff       (20)       10 2016-12-07 15:10:04.000000 bitmapist-3.99/bitmapist.egg-info/top_level.txt
+-rw-r--r--   0 roman      (501) staff       (20)       42 2016-04-19 14:13:48.000000 bitmapist-3.99/MANIFEST.in
+-rw-r--r--   0 roman      (501) staff       (20)     5143 2016-12-07 15:10:05.000000 bitmapist-3.99/PKG-INFO
+-rw-r--r--   0 roman      (501) staff       (20)       59 2016-12-07 15:10:05.000000 bitmapist-3.99/setup.cfg
+-rwxr-xr-x   0 roman      (501) staff       (20)     5058 2016-12-07 14:37:28.000000 bitmapist-3.99/setup.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2016-12-07 15:10:05.000000 bitmapist-3.99/test/
+-rw-r--r--   0 roman      (501) staff       (20)     7365 2016-08-03 15:14:58.000000 bitmapist-3.99/test/test_bitmapist.py
+-rw-r--r--   0 roman      (501) staff       (20)     1575 2016-04-27 09:41:27.000000 bitmapist-3.99/test/test_cohort.py
+-rw-r--r--   0 roman      (501) staff       (20)     1013 2016-04-19 14:13:48.000000 bitmapist-3.99/test/test_delta_methods.py
+-rw-r--r--   0 roman      (501) staff       (20)      216 2016-04-19 14:13:48.000000 bitmapist-3.99/test/test_equality.py
+-rw-r--r--   0 roman      (501) staff       (20)      929 2016-04-19 14:13:48.000000 bitmapist-3.99/test/test_from_date.py
+-rw-r--r--   0 roman      (501) staff       (20)      449 2016-04-19 14:13:48.000000 bitmapist-3.99/test/test_period_start_end.py
+-rw-r--r--   0 roman      (501) staff       (20)     1304 2016-12-07 14:36:26.000000 bitmapist-3.99/test/test_unique_events.py
```

### Comparing `bitmapist-3.98/bitmapist/__init__.py` & `bitmapist-3.99/bitmapist/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,14 +96,17 @@
 }
 
 # Should hourly be tracked as default?
 # Note that this can have huge implications in amounts
 # of memory that Redis uses (especially with huge integers)
 TRACK_HOURLY = False
 
+# Should unique events be tracked as default?
+TRACK_UNIQUE = False
+
 
 def setup_redis(name, host, port, **kw):
     """
     Setup a redis system.
 
     :param :name The name of the system
     :param :host The host of the redis installation
@@ -131,71 +134,121 @@
     else:
         return SYSTEMS[system]
 
 
 # --- Events marking and deleting
 
 def mark_event(event_name, uuid, system='default', now=None, track_hourly=None,
-               use_pipeline=True):
+               track_unique=None, use_pipeline=True):
     """
     Marks an event for hours, days, weeks and months.
 
     :param :event_name The name of the event, could be "active" or "new_signups"
     :param :uuid An unique id, typically user id. The id should not be huge,
         read Redis documentation why (bitmaps)
     :param :system The Redis system to use (string, Redis instance, or Pipeline
         instance).
     :param :now Which date should be used as a reference point, default is
         `datetime.utcnow()`
     :param :track_hourly Should hourly stats be tracked, defaults to
         bitmapist.TRACK_HOURLY
+    :param :track_unique Should unique stats be tracked, defaults to
+        bitmapist.TRACK_UNIQUE
     :param :use_pipeline Boolean flag indicating if the command should use
         pipelines or not. You may want to avoid using pipeline within the
         command if you provide the pipeline object in `system` argument and
         want to manage the pipe execution yourself.
 
     Examples::
 
         # Mark id 1 as active
         mark_event('active', 1)
 
         # Mark task completed for id 252
         mark_event('tasks:completed', 252)
     """
-    _mark(event_name, uuid, system, now, track_hourly, use_pipeline, value=1)
+    _mark(event_name, uuid, system, now, track_hourly, track_unique, use_pipeline, value=1)
 
 
 def unmark_event(event_name, uuid, system='default', now=None, track_hourly=None,
-                 use_pipeline=True):
-    _mark(event_name, uuid, system, now, track_hourly, use_pipeline, value=0)
+                 track_unique=None, use_pipeline=True):
+    _mark(event_name, uuid, system, now, track_hourly, track_unique, use_pipeline, value=0)
 
 
 def _mark(event_name, uuid, system='default', now=None,
-          track_hourly=None, use_pipeline=True, value=1):
+          track_hourly=None, track_unique=None, use_pipeline=True, value=1):
     if track_hourly is None:
         track_hourly = TRACK_HOURLY
+    if track_unique is None:
+        track_unique = TRACK_UNIQUE
 
     if not now:
         now = datetime.utcnow()
 
     obj_classes = [MonthEvents, WeekEvents, DayEvents]
     if track_hourly:
         obj_classes.append(HourEvents)
+    if track_unique:
+        obj_classes.append(UniqueEvents)
 
     client = get_redis(system)
     if use_pipeline:
         client = client.pipeline()
 
     for obj_class in obj_classes:
         client.setbit(obj_class.from_date(event_name, now).redis_key, uuid, value)
 
     if use_pipeline:
         client.execute()
 
 
+def mark_unique(event_name, uuid, system='default'):
+    """
+    Mark unique event
+
+    Unique event (aka "user flag") is an event which doesn't depend on date.
+    Can be used for storing user properties, A/B testing, extra filtering, etc.
+
+    :param :event_name The name of the event, could be "active" or "new_signups"
+    :param :uuid An unique id, typically user id. The id should not be huge,
+        read Redis documentation why (bitmaps)
+    :param :system The Redis system to use (string, Redis instance, or Pipeline
+
+    Examples::
+
+        # Mark id 42 as premium
+        mark_unique('premium', 42)
+    """
+    _mark_unique(event_name, uuid, system, value=1)
+
+
+def unmark_unique(event_name, uuid, system='default'):
+    """
+    Unmark unique event
+
+    Unique event (aka "user flag") is an event which doesn't depend on date.
+    Can be used for storing user properties, A/B testing, extra filtering, etc.
+
+    :param :event_name The name of the event, could be "active" or "new_signups"
+    :param :uuid An unique id, typically user id. The id should not be huge,
+        read Redis documentation why (bitmaps)
+    :param :system The Redis system to use (string, Redis instance, or Pipeline
+
+    Examples::
+
+        # Mark id 42 as not premium anymore
+        unmark_unique('premium', 42)
+    """
+    _mark_unique(event_name, uuid, system, value=0)
+
+
+def _mark_unique(event_name, uuid, system='default', value=1):
+    get_redis(system).setbit(UniqueEvents(event_name).redis_key, uuid, value)
+
+
 def get_event_names(system='default', prefix='', batch=10000):
     """
     Return the list of all event names, with no particular order. Optional
     `prefix` value is used to filter only subset of keys
     """
     cli = get_redis(system)
     expr = 'trackist_%s*' % prefix
@@ -339,14 +392,33 @@
         cli = get_redis(self.system)
         if cli.getbit(self.redis_key, uuid):
             return True
         else:
             return False
 
 
+class UniqueEvents(MixinIter, MixinCounts, MixinContains,
+                   MixinEventsMisc, MixinBitOperations):
+
+    @classmethod
+    def from_date(cls, event_name, dt=None, system='default'):
+        return cls(event_name, system=system)
+
+    def __init__(self, event_name, system='default'):
+        self.event_name = event_name
+        self.system = system
+        self.redis_key = _prefix_key(event_name, 'u')
+
+    def next(self):
+        return self
+
+    def prev(self):
+        return self
+
+
 class GenericPeriodEvents(MixinIter, MixinCounts, MixinContains,
                           MixinEventsMisc, MixinBitOperations):
 
     def next(self):
         """ next object in a datetime line """
         return self.delta(value=1)
 
@@ -373,15 +445,15 @@
         self.event_name = event_name
         self.year = not_none(year, now.year)
         self.system = system
 
         months = []
         for m in range(1, 13):
             months.append(MonthEvents(event_name, self.year, m, system))
-        or_op = BitOpOr(*months)
+        or_op = BitOpOr(system, *months)
         self.redis_key = or_op.redis_key
 
     def delta(self, value):
         return self.__class__(self.event_name, self.year + value, self.system)
 
     def period_start(self):
         return datetime(self.year, 1, 1)
```

### Comparing `bitmapist-3.98/bitmapist/cohort/__init__.py` & `bitmapist-3.99/bitmapist/cohort/__init__.py`

 * *Files identical despite different names*

### Comparing `bitmapist-3.98/bitmapist/cohort/tmpl/form_data.mako` & `bitmapist-3.99/bitmapist/cohort/tmpl/form_data.mako`

 * *Files identical despite different names*

### Comparing `bitmapist-3.98/bitmapist/cohort/tmpl/table_data.mako` & `bitmapist-3.99/bitmapist/cohort/tmpl/table_data.mako`

 * *Files identical despite different names*

### Comparing `bitmapist-3.98/bitmapist/cohort/tmpl/table_data_csv.mako` & `bitmapist-3.99/bitmapist/cohort/tmpl/table_data_csv.mako`

 * *Files identical despite different names*

### Comparing `bitmapist-3.98/bitmapist.egg-info/PKG-INFO` & `bitmapist-3.99/bitmapist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bitmapist
-Version: 3.98
+Version: 3.99
 Summary: Implements a powerful analytics library using Redis bitmaps.
 Home-page: http://www.amix.dk/
 Author: amix
 Author-email: amix@amix.dk
 License: BSD
 Description: bitmapist
         ---------------
@@ -110,11 +110,11 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `bitmapist-3.98/bitmapist.egg-info/SOURCES.txt` & `bitmapist-3.99/bitmapist.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 bitmapist/cohort/tmpl/table_data.mako
 bitmapist/cohort/tmpl/table_data_csv.mako
 test/test_bitmapist.py
 test/test_cohort.py
 test/test_delta_methods.py
 test/test_equality.py
 test/test_from_date.py
-test/test_period_start_end.py
+test/test_period_start_end.py
+test/test_unique_events.py
```

### Comparing `bitmapist-3.98/PKG-INFO` & `bitmapist-3.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bitmapist
-Version: 3.98
+Version: 3.99
 Summary: Implements a powerful analytics library using Redis bitmaps.
 Home-page: http://www.amix.dk/
 Author: amix
 Author-email: amix@amix.dk
 License: BSD
 Description: bitmapist
         ---------------
@@ -110,11 +110,11 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `bitmapist-3.98/setup.py` & `bitmapist-3.99/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,35 +4,36 @@
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or (at
 # your option) any later version.
 
 from setuptools import setup
 
 setup(name='bitmapist',
-      version = '3.98',
+      version='3.99',
       author="amix",
       author_email="amix@amix.dk",
       url="http://www.amix.dk/",
       install_requires=[
           'redis>=2.10.0',
           'python-dateutil',
-          'future>=0.14.3'
+          'future>=0.14.3',
+          'Mako>=1.0.4'
       ],
       classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.2",
         "Programming Language :: Python :: 3.3",
         "Programming Language :: Python :: 3.4",
+        "Programming Language :: Python :: 3.5",
         "Topic :: Software Development :: Libraries :: Python Modules",
       ],
       packages=['bitmapist', 'bitmapist.cohort'],
       include_package_data=True,
       zip_safe=False,
       platforms=["Any"],
       license="BSD",
```

### Comparing `bitmapist-3.98/test/test_bitmapist.py` & `bitmapist-3.99/test/test_bitmapist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from datetime import datetime, timedelta
 
 from bitmapist import mark_event, unmark_event,\
-                      MonthEvents, WeekEvents, DayEvents, HourEvents,\
+                      YearEvents, MonthEvents, WeekEvents, DayEvents, HourEvents,\
                       BitOpAnd, BitOpOr, get_event_names
 
 
 def test_mark_with_diff_days():
     mark_event('active', 123, track_hourly=True)
 
     now = datetime.utcnow()
@@ -232,7 +232,12 @@
     mark_event('bar', 3)
     foo = DayEvents('foo')
     bar = DayEvents('bar')
     assert list(foo & bar) == [2]
     assert list(foo | bar) == [1, 2, 3]
     assert list(foo ^ bar) == [1, 3]
     assert list(~foo & bar) == [3]
+
+
+def test_year_events():
+    mark_event('foo', 1, system='db1')
+    assert 1 in YearEvents('foo', system='db1')
```

### Comparing `bitmapist-3.98/test/test_cohort.py` & `bitmapist-3.99/test/test_cohort.py`

 * *Files identical despite different names*

### Comparing `bitmapist-3.98/test/test_delta_methods.py` & `bitmapist-3.99/test/test_delta_methods.py`

 * *Files identical despite different names*

### Comparing `bitmapist-3.98/test/test_from_date.py` & `bitmapist-3.99/test/test_from_date.py`

 * *Files identical despite different names*

