# Comparing `tmp/admem-2.2.0.tar.gz` & `tmp/admem-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "admem-2.2.0.tar", last modified: Thu Apr 27 22:20:15 2023, max compression
+gzip compressed data, was "admem-2.3.0.tar", last modified: Fri Apr 28 09:19:35 2023, max compression
```

## Comparing `admem-2.2.0.tar` & `admem-2.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 22:20:15.402606 admem-2.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1059 2023-04-20 07:45:29.000000 admem-2.2.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      351 2023-04-27 22:20:15.402606 admem-2.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-27 22:20:15.406606 admem-2.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 admem-2.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 22:20:15.386606 admem-2.2.0/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 22:20:15.398606 admem-2.2.0/source/admem/
--rw-rw-rw-   0 root         (0) root         (0)      584 2023-04-27 21:17:11.000000 admem-2.2.0/source/admem/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1212 2023-04-20 07:45:29.000000 admem-2.2.0/source/admem/_backend_manager_proxy.py
--rw-rw-rw-   0 root         (0) root         (0)     6653 2023-04-27 21:17:11.000000 admem-2.2.0/source/admem/_create_django_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1575 2023-04-20 07:45:29.000000 admem-2.2.0/source/admem/_decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     7178 2023-04-27 21:17:11.000000 admem-2.2.0/source/admem/_django_store.py
--rw-rw-rw-   0 root         (0) root         (0)     2350 2023-04-20 07:45:29.000000 admem-2.2.0/source/admem/_inspect_dataclass.py
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-04-26 22:14:31.000000 admem-2.2.0/source/admem/_path_proxy.py
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-04-27 21:17:11.000000 admem-2.2.0/source/admem/_protocols.py
--rw-rw-rw-   0 root         (0) root         (0)     2960 2023-04-26 22:14:31.000000 admem-2.2.0/source/admem/_store_setup.py
--rw-rw-rw-   0 root         (0) root         (0)     2242 2023-04-27 21:17:11.000000 admem-2.2.0/source/admem/_sync_store.py
--rw-rw-rw-   0 root         (0) root         (0)      498 2023-04-20 07:45:29.000000 admem-2.2.0/source/admem/_util.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 07:45:29.000000 admem-2.2.0/source/admem/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 22:20:15.402606 admem-2.2.0/source/admem.egg-info/
--rw-r--r--   0 root         (0) root         (0)      351 2023-04-27 22:20:15.000000 admem-2.2.0/source/admem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      593 2023-04-27 22:20:15.000000 admem-2.2.0/source/admem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 22:20:15.000000 admem-2.2.0/source/admem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 22:19:56.000000 admem-2.2.0/source/admem.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      232 2023-04-27 22:20:15.000000 admem-2.2.0/source/admem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-27 22:20:15.000000 admem-2.2.0/source/admem.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:19:35.503958 admem-2.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2023-04-20 07:45:29.000000 admem-2.3.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      351 2023-04-28 09:19:35.503958 admem-2.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-28 09:19:35.507958 admem-2.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 admem-2.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:19:35.487958 admem-2.3.0/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:19:35.499958 admem-2.3.0/source/admem/
+-rw-rw-rw-   0 root         (0) root         (0)      584 2023-04-28 09:14:04.000000 admem-2.3.0/source/admem/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2023-04-20 07:45:29.000000 admem-2.3.0/source/admem/_backend_manager_proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     6684 2023-04-28 09:16:24.000000 admem-2.3.0/source/admem/_create_django_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1575 2023-04-20 07:45:29.000000 admem-2.3.0/source/admem/_decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     8304 2023-04-28 09:04:15.000000 admem-2.3.0/source/admem/_django_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     2350 2023-04-20 07:45:29.000000 admem-2.3.0/source/admem/_inspect_dataclass.py
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2023-04-28 09:04:15.000000 admem-2.3.0/source/admem/_path_proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-04-27 21:17:11.000000 admem-2.3.0/source/admem/_protocols.py
+-rw-rw-rw-   0 root         (0) root         (0)     2960 2023-04-26 22:14:31.000000 admem-2.3.0/source/admem/_store_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     2242 2023-04-27 21:17:11.000000 admem-2.3.0/source/admem/_sync_store.py
+-rw-rw-rw-   0 root         (0) root         (0)      498 2023-04-20 07:45:29.000000 admem-2.3.0/source/admem/_util.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 07:45:29.000000 admem-2.3.0/source/admem/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:19:35.503958 admem-2.3.0/source/admem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-04-28 09:19:35.000000 admem-2.3.0/source/admem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      593 2023-04-28 09:19:35.000000 admem-2.3.0/source/admem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 09:19:35.000000 admem-2.3.0/source/admem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 09:19:17.000000 admem-2.3.0/source/admem.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      232 2023-04-28 09:19:35.000000 admem-2.3.0/source/admem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-28 09:19:35.000000 admem-2.3.0/source/admem.egg-info/top_level.txt
```

### Comparing `admem-2.2.0/LICENSE.txt` & `admem-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `admem-2.2.0/setup.cfg` & `admem-2.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `admem-2.2.0/source/admem/__init__.py` & `admem-2.3.0/source/admem/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
     + _sync_store.__all__
     + _store_setup.__all__
     + _create_django_model.__all__
     + _inspect_dataclass.__all__
 )
 
 
-__version__ = "2.2.0"
+__version__ = "2.3.0"
```

### Comparing `admem-2.2.0/source/admem/_backend_manager_proxy.py` & `admem-2.3.0/source/admem/_backend_manager_proxy.py`

 * *Files identical despite different names*

### Comparing `admem-2.2.0/source/admem/_create_django_model.py` & `admem-2.3.0/source/admem/_create_django_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         dj_model = type(self.dataclass.__name__, (models.Model,), fields)
         BACKEND_LINKER.link(self.dataclass, dj_model)
 
     def translate_fields(
         self, pk_key: str | None, extra_kwgs: dict[str, dict[str, tp.Any]] | None
     ) -> "dict[str, models.Field[tp.Any, tp.Any]]":
         fields = {}
-        fields_to_skip = {Path: ["resave"]}
+        fields_to_skip = {Path: ["resave"], Path | None: ["resave"]}
         for field in dc.fields(self.dataclass):
             try:
                 django_field = self.alt_field_type.pop(field.name)
                 opts: dict[str, tp.Any] = {}
             except KeyError:
                 django_field, opts = self.django_field_precursor(field.type)
             if field.name == pk_key:
@@ -67,15 +67,15 @@
             default = self.get_default(field)
             if default:
                 opts["default"] = default
             extra = dict(**field.metadata)
             if extra_kwgs:
                 extra.update(extra_kwgs.pop(field.name, {}))
             for key in fields_to_skip.get(field.type, []):
-                extra.pop(key)
+                extra.pop(key, None)
             fields[field.name] = django_field(**{**opts, **extra})
         if extra_kwgs:
             raise RuntimeError(
                 f"unconsumed extra kwgs ({extra_kwgs}) found for {self.dataclass}, please adjust!"
             )
         if self.alt_field_type:
             raise RuntimeError(
```

### Comparing `admem-2.2.0/source/admem/_decorator.py` & `admem-2.3.0/source/admem/_decorator.py`

 * *Files identical despite different names*

### Comparing `admem-2.2.0/source/admem/_django_store.py` & `admem-2.3.0/source/admem/_django_store.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import typing as tp
 from pathlib import Path
 
 from django.core.files import File
 from django.core.files.storage import get_storage_class
 from django.core.files.uploadedfile import UploadedFile
 from django.db import models
+from django.db.models.fields.files import FieldFile
 
 from ._create_django_model import InspectDataclass
 from ._decorator import BACKEND_LINKER
 from ._decorator import django_model
 from ._path_proxy import DjangoPath
 from ._protocols import T
 
@@ -85,42 +86,66 @@
         field: dc.Field[Path],
         model: type[models.Model],
         update_origin: dict[str, tp.Any],
     ) -> tp.Any:
         key = field.name
         storage = get_storage_class()()
         resave = field.metadata.get("resave", "always")
+        # pylint: disable=protected-access
+        dj_field = model._meta.get_field(key)
+        create_dj_path = self.create_dj_path(model, field)
         if isinstance(val, DjangoPath):
-            name = val.as_posix()
-            if resave == "always":
-                update_origin[key] = lambda x: DjangoPath(
-                    x.name
-                )  # name contains the prefix
-                return UploadedFile(storage.open(name, "rb"), name)
+            # the DjangoPath can be from another Model,
+            # hence we strip the prefix and add it again
+            name = val.name_wo_prefix()
+            prefix_name = dj_field.generate_filename(None, name)  # type: ignore
+            cross_model = prefix_name != val.as_posix()
+            if resave == "always" or (
+                cross_model and resave == "first" and not storage.exists(prefix_name)
+            ):
+                update_origin[key] = create_dj_path
+                return UploadedFile(val.open("rb"), name)
             if resave == "first":
-                if not storage.exists(name):
-                    raise FileNotFoundError(storage.path(name))
+                if not storage.exists(prefix_name):
+                    raise FileNotFoundError(storage.path(prefix_name))
+                if cross_model:
+                    return prefix_name
                 return val
             raise NotImplementedError(resave)
         if val.exists():
-            # pylint: disable=protected-access
-            dj_field = model._meta.get_field(key)
-            name = dj_field.generate_filename(None, val.name)  # type: ignore
-            update_origin[key] = lambda x: DjangoPath(x.name)
-            exists = storage.exists(name)
+            prefix_name = dj_field.generate_filename(None, val.name)  # type: ignore
+            update_origin[key] = create_dj_path
+            exists = storage.exists(prefix_name)
             if resave == "first" and exists:
-                return name
+                return prefix_name
             if resave == "always" or (resave == "first" and not exists):
                 return File(
                     open(val, "rb"),  # pylint: disable=consider-using-with
                     val.name,
                 )
             raise NotImplementedError(resave)
         raise NotImplementedError(val)
 
+    def create_dj_path(
+        self, model: type[models.Model], dc_field: dc.Field[Path]
+    ) -> tp.Callable[[FieldFile], DjangoPath]:
+        # pylint: disable=protected-access
+        dj_field = model._meta.get_field(dc_field.name)
+        prefix = None
+        if hasattr(dj_field, "upload_to"):
+            prefix = getattr(dj_field, "upload_to")
+
+        def inner(fieldfile: FieldFile) -> DjangoPath:
+            assert fieldfile.name
+            res = DjangoPath(fieldfile.name)
+            res._prefix = prefix  # type: ignore
+            return res
+
+        return inner
+
     def django_to_dataclass(self, dj_obj: models.Model) -> tp.Any:
         dataclass = BACKEND_LINKER.backend_to_dc[type(dj_obj)]
         obj_kwgs = {}
         for field in dc.fields(dataclass):
             key = field.name
             val = getattr(dj_obj, key)
             if type(val) in BACKEND_LINKER.backend_to_dc:
@@ -148,15 +173,16 @@
                     val = {self.django_to_dataclass(x) for x in val.all()}
                 else:
                     raise RuntimeError(f"field type {origin} not supported yet!")
 
             if issubclass(field_type, enum.Enum):
                 val = field_type(val)
             if issubclass(field_type, Path):
-                val = DjangoPath(val.name)  # contains prefix
+                create_dj_path = self.create_dj_path(dj_obj.__class__, field)
+                val = create_dj_path(val)  # contains prefix
             obj_kwgs[field.name] = val
         return dataclass(**obj_kwgs)
 
     parse = django_to_dataclass
 
     def backend_manager(self, dataclass: type[T]) -> tp.Any:
         return django_model(dataclass).objects.using(self.identifier)
```

### Comparing `admem-2.2.0/source/admem/_inspect_dataclass.py` & `admem-2.3.0/source/admem/_inspect_dataclass.py`

 * *Files identical despite different names*

### Comparing `admem-2.2.0/source/admem/_protocols.py` & `admem-2.3.0/source/admem/_protocols.py`

 * *Files identical despite different names*

### Comparing `admem-2.2.0/source/admem/_store_setup.py` & `admem-2.3.0/source/admem/_store_setup.py`

 * *Files identical despite different names*

### Comparing `admem-2.2.0/source/admem/_sync_store.py` & `admem-2.3.0/source/admem/_sync_store.py`

 * *Files identical despite different names*

### Comparing `admem-2.2.0/source/admem.egg-info/SOURCES.txt` & `admem-2.3.0/source/admem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

