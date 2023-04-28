# Comparing `tmp/pyprocessors-gallery-0.1.3.tar.gz` & `tmp/pyprocessors-gallery-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprocessors-gallery-0.1.3.tar", last modified: Thu Mar 16 07:55:24 2023, max compression
+gzip compressed data, was "pyprocessors-gallery-0.1.4.tar", last modified: Fri Apr 28 06:43:54 2023, max compression
```

## Comparing `pyprocessors-gallery-0.1.3.tar` & `pyprocessors-gallery-0.1.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      496 2022-09-08 12:54:54.660317 pyprocessors-gallery-0.1.3/.bumpversion.cfg
--rw-r--r--   0        0        0     1386 2022-09-08 12:54:54.692317 pyprocessors-gallery-0.1.3/.github/workflows/main.yml
--rw-r--r--   0        0        0     1739 2022-09-12 08:18:13.705761 pyprocessors-gallery-0.1.3/.gitignore
--rw-r--r--   0        0        0      176 2022-09-08 13:09:43.669293 pyprocessors-gallery-0.1.3/.idea/.gitignore
--rw-r--r--   0        0        0      867 2022-09-08 13:09:43.429293 pyprocessors-gallery-0.1.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2022-09-08 13:09:43.565293 pyprocessors-gallery-0.1.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      203 2022-09-08 13:12:35.536526 pyprocessors-gallery-0.1.3/.idea/misc.xml
--rw-r--r--   0        0        0      292 2022-09-08 13:09:43.549293 pyprocessors-gallery-0.1.3/.idea/modules.xml
--rw-r--r--   0        0        0      492 2022-09-08 13:12:35.528526 pyprocessors-gallery-0.1.3/.idea/pyprocessors_gallery.iml
--rw-r--r--   0        0        0      419 2022-09-08 12:54:54.648317 pyprocessors-gallery-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      202 2022-09-08 12:54:54.632317 pyprocessors-gallery-0.1.3/.readthedocs.yml
--rw-r--r--   0        0        0      116 2022-09-08 12:54:54.648317 pyprocessors-gallery-0.1.3/AUTHORS.md
--rw-r--r--   0        0        0      268 2022-09-08 12:54:54.648317 pyprocessors-gallery-0.1.3/CHANGELOG.md
--rw-r--r--   0        0        0      448 2022-09-08 12:54:54.640317 pyprocessors-gallery-0.1.3/Dockerfile
--rw-r--r--   0        0        0     7064 2022-09-08 12:54:54.660317 pyprocessors-gallery-0.1.3/Jenkinsfile
--rw-r--r--   0        0        0     1082 2022-09-08 12:54:54.652317 pyprocessors-gallery-0.1.3/LICENSE
--rw-r--r--   0        0        0     1545 2022-09-08 12:54:54.644317 pyprocessors-gallery-0.1.3/README.md
--rw-r--r--   0        0        0      939 2022-09-08 12:54:54.644317 pyprocessors-gallery-0.1.3/RELEASE.md
--rw-r--r--   0        0        0     1563 2022-09-08 12:54:54.660317 pyprocessors-gallery-0.1.3/bumpversion.py
--rw-r--r--   0        0        0       62 2022-09-08 12:54:54.672317 pyprocessors-gallery-0.1.3/docs/.gitignore
--rw-r--r--   0        0        0      268 2022-09-08 12:54:54.672317 pyprocessors-gallery-0.1.3/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2022-09-08 12:54:54.672317 pyprocessors-gallery-0.1.3/docs/LICENSE
--rw-r--r--   0        0        0        0 2022-09-08 12:54:54.680317 pyprocessors-gallery-0.1.3/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2022-09-08 12:54:54.680317 pyprocessors-gallery-0.1.3/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     2874 2022-09-08 12:54:54.676317 pyprocessors-gallery-0.1.3/docs/conf.py
--rw-r--r--   0        0        0      141 2022-09-08 12:54:54.676317 pyprocessors-gallery-0.1.3/docs/index.rst
--rw-r--r--   0        0        0       98 2022-09-08 12:54:54.648317 pyprocessors-gallery-0.1.3/mypy.ini
--rw-r--r--   0        0        0     2141 2022-09-08 12:54:54.636317 pyprocessors-gallery-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       74 2023-03-16 07:54:33.341507 pyprocessors-gallery-0.1.3/src/pyprocessors_gallery/__init__.py
--rw-r--r--   0        0        0     3175 2022-10-06 10:22:49.620720 pyprocessors-gallery-0.1.3/src/pyprocessors_gallery/gallery.py
--rw-r--r--   0        0        0       26 2022-09-08 12:54:54.668317 pyprocessors-gallery-0.1.3/tests/data/test.txt
--rw-r--r--   0        0        0      536 2022-09-08 12:54:54.668317 pyprocessors-gallery-0.1.3/tests/test_gallery.py
--rw-r--r--   0        0        0     1041 2022-09-08 12:54:54.656317 pyprocessors-gallery-0.1.3/tox.ini
--rw-r--r--   0        0        0     1255 1970-01-01 00:00:00.000000 pyprocessors-gallery-0.1.3/setup.py
--rw-r--r--   0        0        0     3183 1970-01-01 00:00:00.000000 pyprocessors-gallery-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      496 2022-09-08 12:54:54.660317 pyprocessors-gallery-0.1.4/.bumpversion.cfg
+-rw-r--r--   0        0        0     1386 2022-09-08 12:54:54.692317 pyprocessors-gallery-0.1.4/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1739 2022-09-12 08:18:13.705761 pyprocessors-gallery-0.1.4/.gitignore
+-rw-r--r--   0        0        0      176 2022-09-08 13:09:43.669293 pyprocessors-gallery-0.1.4/.idea/.gitignore
+-rw-r--r--   0        0        0      867 2022-09-08 13:09:43.429293 pyprocessors-gallery-0.1.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2022-09-08 13:09:43.565293 pyprocessors-gallery-0.1.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      203 2022-09-08 13:12:35.536526 pyprocessors-gallery-0.1.4/.idea/misc.xml
+-rw-r--r--   0        0        0      292 2022-09-08 13:09:43.549293 pyprocessors-gallery-0.1.4/.idea/modules.xml
+-rw-r--r--   0        0        0      492 2022-09-08 13:12:35.528526 pyprocessors-gallery-0.1.4/.idea/pyprocessors_gallery.iml
+-rw-r--r--   0        0        0      419 2022-09-08 12:54:54.648317 pyprocessors-gallery-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      202 2022-09-08 12:54:54.632317 pyprocessors-gallery-0.1.4/.readthedocs.yml
+-rw-r--r--   0        0        0      116 2022-09-08 12:54:54.648317 pyprocessors-gallery-0.1.4/AUTHORS.md
+-rw-r--r--   0        0        0      268 2022-09-08 12:54:54.648317 pyprocessors-gallery-0.1.4/CHANGELOG.md
+-rw-r--r--   0        0        0      448 2022-09-08 12:54:54.640317 pyprocessors-gallery-0.1.4/Dockerfile
+-rw-r--r--   0        0        0     7064 2022-09-08 12:54:54.660317 pyprocessors-gallery-0.1.4/Jenkinsfile
+-rw-r--r--   0        0        0     1082 2022-09-08 12:54:54.652317 pyprocessors-gallery-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1545 2022-09-08 12:54:54.644317 pyprocessors-gallery-0.1.4/README.md
+-rw-r--r--   0        0        0      939 2022-09-08 12:54:54.644317 pyprocessors-gallery-0.1.4/RELEASE.md
+-rw-r--r--   0        0        0     1563 2022-09-08 12:54:54.660317 pyprocessors-gallery-0.1.4/bumpversion.py
+-rw-r--r--   0        0        0       62 2022-09-08 12:54:54.672317 pyprocessors-gallery-0.1.4/docs/.gitignore
+-rw-r--r--   0        0        0      268 2022-09-08 12:54:54.672317 pyprocessors-gallery-0.1.4/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2022-09-08 12:54:54.672317 pyprocessors-gallery-0.1.4/docs/LICENSE
+-rw-r--r--   0        0        0        0 2022-09-08 12:54:54.680317 pyprocessors-gallery-0.1.4/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2022-09-08 12:54:54.680317 pyprocessors-gallery-0.1.4/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     2874 2022-09-08 12:54:54.676317 pyprocessors-gallery-0.1.4/docs/conf.py
+-rw-r--r--   0        0        0      141 2022-09-08 12:54:54.676317 pyprocessors-gallery-0.1.4/docs/index.rst
+-rw-r--r--   0        0        0       98 2022-09-08 12:54:54.648317 pyprocessors-gallery-0.1.4/mypy.ini
+-rw-r--r--   0        0        0     2141 2022-09-08 12:54:54.636317 pyprocessors-gallery-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-04-28 06:43:26.737039 pyprocessors-gallery-0.1.4/src/pyprocessors_gallery/__init__.py
+-rw-r--r--   0        0        0     3342 2023-04-28 06:39:45.526058 pyprocessors-gallery-0.1.4/src/pyprocessors_gallery/gallery.py
+-rw-r--r--   0        0        0       26 2022-09-08 12:54:54.668317 pyprocessors-gallery-0.1.4/tests/data/test.txt
+-rw-r--r--   0        0        0      536 2022-09-08 12:54:54.668317 pyprocessors-gallery-0.1.4/tests/test_gallery.py
+-rw-r--r--   0        0        0     1041 2022-09-08 12:54:54.656317 pyprocessors-gallery-0.1.4/tox.ini
+-rw-r--r--   0        0        0     1255 1970-01-01 00:00:00.000000 pyprocessors-gallery-0.1.4/setup.py
+-rw-r--r--   0        0        0     3183 1970-01-01 00:00:00.000000 pyprocessors-gallery-0.1.4/PKG-INFO
```

### Comparing `pyprocessors-gallery-0.1.3/.github/workflows/main.yml` & `pyprocessors-gallery-0.1.4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pyprocessors-gallery-0.1.3/.gitignore` & `pyprocessors-gallery-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pyprocessors-gallery-0.1.3/.idea/inspectionProfiles/Project_Default.xml` & `pyprocessors-gallery-0.1.4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `pyprocessors-gallery-0.1.3/Jenkinsfile` & `pyprocessors-gallery-0.1.4/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `pyprocessors-gallery-0.1.3/LICENSE` & `pyprocessors-gallery-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprocessors-gallery-0.1.3/README.md` & `pyprocessors-gallery-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyprocessors-gallery-0.1.3/RELEASE.md` & `pyprocessors-gallery-0.1.4/RELEASE.md`

 * *Files identical despite different names*

### Comparing `pyprocessors-gallery-0.1.3/bumpversion.py` & `pyprocessors-gallery-0.1.4/bumpversion.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-gallery-0.1.3/docs/LICENSE` & `pyprocessors-gallery-0.1.4/docs/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprocessors-gallery-0.1.3/docs/conf.py` & `pyprocessors-gallery-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-gallery-0.1.3/pyproject.toml` & `pyprocessors-gallery-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyprocessors-gallery-0.1.3/src/pyprocessors_gallery/gallery.py` & `pyprocessors-gallery-0.1.4/src/pyprocessors_gallery/gallery.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,16 +45,18 @@
     one_lexicon: str = Field(None, description="One lexicon", extra="lexicon")
     one_enum: GalleryEnum = Field(GalleryEnum.A,
                                   description="One enum with default value")
     lexicon2enum_mapping: Dict[str, GalleryEnum] = Field(None,
                                                          description="Lexicon to component enum",
                                                          extra="key:lexicon")
     many_enums: List[GalleryEnum] = Field(None,
-                                  description="List of values from enum")
-    label2many_enums_mapping: Dict[str, List[GalleryEnum]] = Field(None, description="Label to json mapping", extra="key:label")
+                                          description="List of values from enum")
+    label2many_enums_mapping: Dict[str, List[GalleryEnum]] = Field(None, description="Label to json mapping",
+                                                                   extra="key:label")
+    one_multi: str = Field(None, description="""Multiline text areas""", extra="multiline")
 
 
 class GalleryProcessor(ProcessorBase):
     """[Gallery](https://fr.wikipedia.org/wiki/Gallery) processor .
     #languages:en,fr,de
     #needs-segments
     """
```

### Comparing `pyprocessors-gallery-0.1.3/tests/test_gallery.py` & `pyprocessors-gallery-0.1.4/tests/test_gallery.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-gallery-0.1.3/tox.ini` & `pyprocessors-gallery-0.1.4/tox.ini`

 * *Files identical despite different names*

### Comparing `pyprocessors-gallery-0.1.3/setup.py` & `pyprocessors-gallery-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
           'tox']}
 
 entry_points = \
 {'pyprocessors.plugins': ['gallery = '
                           'pyprocessors_gallery.gallery:GalleryProcessor']}
 
 setup(name='pyprocessors-gallery',
-      version='0.1.3',
+      version='0.1.4',
       description='Multirole to be used as a test gallery for the UI',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://github.com/oterrier/pyprocessors_gallery/',
       packages=packages,
       package_data=package_data,
       package_dir=package_dir,
```

### Comparing `pyprocessors-gallery-0.1.3/PKG-INFO` & `pyprocessors-gallery-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprocessors-gallery
-Version: 0.1.3
+Version: 0.1.4
 Summary: Multirole to be used as a test gallery for the UI
 Home-page: https://github.com/oterrier/pyprocessors_gallery/
 Keywords: 
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

