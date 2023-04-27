# Comparing `tmp/admem-2.0.0.tar.gz` & `tmp/admem-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "admem-2.0.0.tar", last modified: Wed Apr 26 00:03:00 2023, max compression
+gzip compressed data, was "admem-2.1.0.tar", last modified: Thu Apr 27 19:36:59 2023, max compression
```

## Comparing `admem-2.0.0.tar` & `admem-2.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 00:03:00.387689 admem-2.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1059 2023-04-20 07:45:29.000000 admem-2.0.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      351 2023-04-26 00:03:00.387689 admem-2.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-26 00:03:00.387689 admem-2.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 admem-2.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 00:03:00.355688 admem-2.0.0/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 00:03:00.375689 admem-2.0.0/source/admem/
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-25 23:38:34.000000 admem-2.0.0/source/admem/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1212 2023-04-20 07:45:29.000000 admem-2.0.0/source/admem/_backend_manager_proxy.py
--rw-rw-rw-   0 root         (0) root         (0)     6524 2023-04-25 23:57:00.000000 admem-2.0.0/source/admem/_create_django_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1575 2023-04-20 07:45:29.000000 admem-2.0.0/source/admem/_decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     4842 2023-04-25 23:38:34.000000 admem-2.0.0/source/admem/_django_store.py
--rw-rw-rw-   0 root         (0) root         (0)     2350 2023-04-20 07:45:29.000000 admem-2.0.0/source/admem/_inspect_dataclass.py
--rw-rw-rw-   0 root         (0) root         (0)      542 2023-04-20 07:45:29.000000 admem-2.0.0/source/admem/_protocols.py
--rw-rw-rw-   0 root         (0) root         (0)     2798 2023-04-20 07:45:29.000000 admem-2.0.0/source/admem/_store_setup.py
--rw-rw-rw-   0 root         (0) root         (0)     2009 2023-04-20 07:45:29.000000 admem-2.0.0/source/admem/_sync_store.py
--rw-rw-rw-   0 root         (0) root         (0)      498 2023-04-20 07:45:29.000000 admem-2.0.0/source/admem/_util.py
--rw-rw-rw-   0 root         (0) root         (0)     3270 2023-04-25 23:57:00.000000 admem-2.0.0/source/admem/fields.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 07:45:29.000000 admem-2.0.0/source/admem/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 00:03:00.387689 admem-2.0.0/source/admem.egg-info/
--rw-r--r--   0 root         (0) root         (0)      351 2023-04-26 00:03:00.000000 admem-2.0.0/source/admem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      588 2023-04-26 00:03:00.000000 admem-2.0.0/source/admem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 00:03:00.000000 admem-2.0.0/source/admem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 00:02:17.000000 admem-2.0.0/source/admem.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      232 2023-04-26 00:03:00.000000 admem-2.0.0/source/admem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-26 00:03:00.000000 admem-2.0.0/source/admem.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:36:59.445915 admem-2.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2023-04-20 07:45:29.000000 admem-2.1.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      351 2023-04-27 19:36:59.445915 admem-2.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-27 19:36:59.449915 admem-2.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 admem-2.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:36:59.345911 admem-2.1.0/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:36:59.393913 admem-2.1.0/source/admem/
+-rw-rw-rw-   0 root         (0) root         (0)      584 2023-04-26 22:14:31.000000 admem-2.1.0/source/admem/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2023-04-20 07:45:29.000000 admem-2.1.0/source/admem/_backend_manager_proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     6649 2023-04-26 22:14:31.000000 admem-2.1.0/source/admem/_create_django_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1575 2023-04-20 07:45:29.000000 admem-2.1.0/source/admem/_decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     6599 2023-04-26 22:14:31.000000 admem-2.1.0/source/admem/_django_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     2350 2023-04-20 07:45:29.000000 admem-2.1.0/source/admem/_inspect_dataclass.py
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-04-26 22:14:31.000000 admem-2.1.0/source/admem/_path_proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)      542 2023-04-20 07:45:29.000000 admem-2.1.0/source/admem/_protocols.py
+-rw-rw-rw-   0 root         (0) root         (0)     2960 2023-04-26 22:14:31.000000 admem-2.1.0/source/admem/_store_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     2009 2023-04-20 07:45:29.000000 admem-2.1.0/source/admem/_sync_store.py
+-rw-rw-rw-   0 root         (0) root         (0)      498 2023-04-20 07:45:29.000000 admem-2.1.0/source/admem/_util.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 07:45:29.000000 admem-2.1.0/source/admem/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:36:59.445915 admem-2.1.0/source/admem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-04-27 19:36:59.000000 admem-2.1.0/source/admem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      593 2023-04-27 19:36:59.000000 admem-2.1.0/source/admem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:36:59.000000 admem-2.1.0/source/admem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:36:28.000000 admem-2.1.0/source/admem.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      232 2023-04-27 19:36:59.000000 admem-2.1.0/source/admem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-27 19:36:59.000000 admem-2.1.0/source/admem.egg-info/top_level.txt
```

### Comparing `admem-2.0.0/LICENSE.txt` & `admem-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `admem-2.0.0/setup.cfg` & `admem-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `admem-2.0.0/source/admem/__init__.py` & `admem-2.1.0/source/admem/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,27 +3,24 @@
 from django.conf import settings
 
 from . import _create_django_model
 from . import _decorator
 from . import _inspect_dataclass
 from . import _store_setup
 from . import _sync_store
-from . import fields
 from ._create_django_model import *
 from ._decorator import *
 from ._inspect_dataclass import *
 from ._store_setup import *
 from ._sync_store import *
-from .fields import *
 
 
 __all__ = (
     _decorator.__all__
     + _sync_store.__all__
     + _store_setup.__all__
     + _create_django_model.__all__
     + _inspect_dataclass.__all__
-    + fields.__all__
 )
 
 
-__version__ = "2.0.0"
+__version__ = "2.1.0"
```

### Comparing `admem-2.0.0/source/admem/_backend_manager_proxy.py` & `admem-2.1.0/source/admem/_backend_manager_proxy.py`

 * *Files identical despite different names*

### Comparing `admem-2.0.0/source/admem/_create_django_model.py` & `admem-2.1.0/source/admem/_create_django_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import django.db  # pylint: disable=unused-import
 from django.db import models
 
 from ._decorator import BACKEND_LINKER
 from ._decorator import django_model
 from ._inspect_dataclass import InspectDataclass
 from ._util import public_name
-from .fields import DjangoPathField
 
 # 2023-Q1: sphinx has a bug regarding adjusting the signature for attributes,
 # hence I need fully qualified imports for typing and django.db
 
 __all__ = ["CreateDjangoModel", "create_django_model"]
 
 
@@ -50,30 +49,33 @@
         dj_model = type(self.dataclass.__name__, (models.Model,), fields)
         BACKEND_LINKER.link(self.dataclass, dj_model)
 
     def translate_fields(
         self, pk_key: str | None, extra_kwgs: dict[str, dict[str, tp.Any]] | None
     ) -> "dict[str, models.Field[tp.Any, tp.Any]]":
         fields = {}
+        fields_to_skip = {Path: ["resave"]}
         for field in dc.fields(self.dataclass):
             try:
                 django_field = self.alt_field_type.pop(field.name)
                 opts: dict[str, tp.Any] = {}
             except KeyError:
                 django_field, opts = self.django_field_precursor(field.type)
             if field.name == pk_key:
                 opts["primary_key"] = True
                 if django_field is models.ForeignKey:
                     django_field = models.OneToOneField
             default = self.get_default(field)
             if default:
                 opts["default"] = default
-            extra = {}
+            extra = dict(**field.metadata)
             if extra_kwgs:
-                extra = extra_kwgs.pop(field.name, {})
+                extra.update(extra_kwgs.pop(field.name, {}))
+            for key in fields_to_skip.get(field.type, []):
+                extra.pop(key)
             fields[field.name] = django_field(**opts, **extra)
         if extra_kwgs:
             raise RuntimeError(
                 f"unconsumed extra kwgs ({extra_kwgs}) found for {self.dataclass}, please adjust!"
             )
         if self.alt_field_type:
             raise RuntimeError(
@@ -157,15 +159,15 @@
             for val in type_.__members__.values():
                 choices.append((val.value, val.value))
                 assert len(val.value) < max_length
 
             return models.CharField, dict(max_length=max_length, choices=choices)
 
         if issubclass(type_, Path):
-            return DjangoPathField, dict(max_length=1024)
+            return models.FileField, dict(max_length=1024)
 
         try:  # try Foreign Key relation (many-to-one)
             fk_class = BACKEND_LINKER.backend_class(type_)
             assert issubclass(fk_class, models.Model)
             return models.ForeignKey, dict(
                 to=fk_class, on_delete=models.CASCADE, related_name="+"
             )
```

### Comparing `admem-2.0.0/source/admem/_decorator.py` & `admem-2.1.0/source/admem/_decorator.py`

 * *Files identical despite different names*

### Comparing `admem-2.0.0/source/admem/_django_store.py` & `admem-2.1.0/source/admem/_django_store.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # Copyright (c) 2022-2023 Mario S. Könz; License: MIT
 import dataclasses as dc
 import enum
 import types
 import typing as tp
 from pathlib import Path
 
+from django.core.files import File
+from django.core.files.storage import get_storage_class
+from django.core.files.uploadedfile import UploadedFile
 from django.db import models
 
 from ._create_django_model import InspectDataclass
 from ._decorator import BACKEND_LINKER
 from ._decorator import django_model
+from ._path_proxy import DjangoPath
 from ._protocols import T
-from .fields import DjangoPath
 
 
 @dc.dataclass
 class DjangoStore:
     identifier: str
 
     def dump(self, dc_obj: tp.Any) -> "tuple[models.Model, bool]":
@@ -52,34 +55,72 @@
         manager = self.backend_manager(dataclass)
         yield from manager.filter(**filter_kwgs).all()
 
     def dataclass_to_django(self, dc_obj: tp.Any) -> tp.Any:
         model = django_model(dc_obj)
         kwgs = {}
         m2m = {}
-        update_origin = {}
+        update_origin: dict[str, tp.Any] = {}
         for field in dc.fields(dc_obj):
             key = field.name
             val = getattr(dc_obj, key)
             if type(val) in BACKEND_LINKER.dc_to_backend:
                 val, _ = self.dump(val)
             if isinstance(val, enum.Enum):
                 val = val.value
             if isinstance(val, Path) and val is not None:
-                update_origin[key] = DjangoPath
+                val = self._process_path(val, field, model, update_origin)
 
             # pylint: disable=protected-access
             dj_model = model._meta.get_field(key)
             if isinstance(dj_model, models.ManyToManyField):
                 m2m[key] = val
             else:
                 kwgs[key] = val
 
         return kwgs, m2m, update_origin
 
+    def _process_path(
+        self,
+        val: tp.Any,
+        field: dc.Field[Path],
+        model: type[models.Model],
+        update_origin: dict[str, tp.Any],
+    ) -> tp.Any:
+        key = field.name
+        storage = get_storage_class()()
+        resave = field.metadata.get("resave", "always")
+        if isinstance(val, DjangoPath):
+            name = val.as_posix()
+            if resave == "always":
+                update_origin[key] = lambda x: DjangoPath(
+                    x.name
+                )  # name contains the prefix
+                return UploadedFile(storage.open(name, "rb"), name)
+            if resave == "first":
+                if not storage.exists(name):
+                    raise FileNotFoundError(storage.path(name))
+                return val
+            raise NotImplementedError(resave)
+        if val.exists():
+            # pylint: disable=protected-access
+            dj_field = model._meta.get_field(key)
+            name = dj_field.generate_filename(None, val.name)  # type: ignore
+            update_origin[key] = lambda x: DjangoPath(x.name)
+            exists = storage.exists(name)
+            if resave == "first" and exists:
+                return name
+            if resave == "always" or (resave == "first" and not exists):
+                return File(
+                    open(val, "rb"),  # pylint: disable=consider-using-with
+                    val.name,
+                )
+            raise NotImplementedError(resave)
+        raise NotImplementedError(val)
+
     def django_to_dataclass(self, dj_obj: models.Model) -> tp.Any:
         dataclass = BACKEND_LINKER.backend_to_dc[type(dj_obj)]
         obj_kwgs = {}
         for field in dc.fields(dataclass):
             key = field.name
             val = getattr(dj_obj, key)
             if type(val) in BACKEND_LINKER.backend_to_dc:
@@ -107,15 +148,15 @@
                     val = {self.django_to_dataclass(x) for x in val.all()}
                 else:
                     raise RuntimeError(f"field type {origin} not supported yet!")
 
             if issubclass(field_type, enum.Enum):
                 val = field_type(val)
             if issubclass(field_type, Path):
-                pass
+                val = DjangoPath(val.name)  # contains prefix
             obj_kwgs[field.name] = val
         return dataclass(**obj_kwgs)
 
     parse = django_to_dataclass
 
     def backend_manager(self, dataclass: type[T]) -> tp.Any:
         return django_model(dataclass).objects.using(self.identifier)
```

### Comparing `admem-2.0.0/source/admem/_inspect_dataclass.py` & `admem-2.1.0/source/admem/_inspect_dataclass.py`

 * *Files identical despite different names*

### Comparing `admem-2.0.0/source/admem/_protocols.py` & `admem-2.1.0/source/admem/_protocols.py`

 * *Files identical despite different names*

### Comparing `admem-2.0.0/source/admem/_store_setup.py` & `admem-2.1.0/source/admem/_store_setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import typing as tp
 from pathlib import Path
 
 import django
 from django.apps import apps
 from django.conf import settings
 from django.core.management import call_command
+from django.core.signals import setting_changed
 from django.db import connections
 
 from ._decorator import BACKEND_LINKER
 from ._django_store import DjangoStore
 from ._protocols import BackendStoreProtocol
 
 __all__ = ["set_store", "set_store_for_django", "ACTIVE_STORES", "set_file_backend"]
@@ -40,14 +41,15 @@
     else:
         raise NotImplementedError(flavor)
 
 
 def set_file_backend(media_root: Path) -> None:
     django_config()
     settings.MEDIA_ROOT = media_root
+    setting_changed.send(None, setting="MEDIA_ROOT")
 
 
 @contextlib.contextmanager
 def django_setup(identifier: str) -> tp.Iterator[dict[str, tp.Any]]:
     django_config()
 
     assert identifier != "default"
@@ -59,14 +61,15 @@
         for app_label in BACKEND_LINKER.app_labels:
             if app_label in new_apps:
                 settings.INSTALLED_APPS.append(app_label)
 
         apps.apps_ready = apps.models_ready = apps.loading = apps.ready = False
         apps.clear_cache()
         apps.populate(settings.INSTALLED_APPS)
+        setting_changed.send(None, setting="INSTALLED_APPS")
 
         try:
             with contextlib.redirect_stdout(io.StringIO()):
                 call_command("makemigrations", "--noinput")
         except SystemExit:
             call_command("makemigrations")
```

### Comparing `admem-2.0.0/source/admem/_sync_store.py` & `admem-2.1.0/source/admem/_sync_store.py`

 * *Files identical despite different names*

### Comparing `admem-2.0.0/source/admem.egg-info/SOURCES.txt` & `admem-2.1.0/source/admem.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 setup.py
 source/admem/__init__.py
 source/admem/_backend_manager_proxy.py
 source/admem/_create_django_model.py
 source/admem/_decorator.py
 source/admem/_django_store.py
 source/admem/_inspect_dataclass.py
+source/admem/_path_proxy.py
 source/admem/_protocols.py
 source/admem/_store_setup.py
 source/admem/_sync_store.py
 source/admem/_util.py
-source/admem/fields.py
 source/admem/py.typed
 source/admem.egg-info/PKG-INFO
 source/admem.egg-info/SOURCES.txt
 source/admem.egg-info/dependency_links.txt
 source/admem.egg-info/not-zip-safe
 source/admem.egg-info/requires.txt
 source/admem.egg-info/top_level.txt
```

