# Comparing `tmp/pyprocessors-generative_augmenter-0.5.15.tar.gz` & `tmp/pyprocessors-generative_augmenter-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprocessors-generative_augmenter-0.5.15.tar", last modified: Fri Apr 28 06:37:18 2023, max compression
+gzip compressed data, was "pyprocessors-generative_augmenter-0.5.9.tar", last modified: Thu Apr 27 11:12:50 2023, max compression
```

## Comparing `pyprocessors-generative_augmenter-0.5.15.tar` & `pyprocessors-generative_augmenter-0.5.9.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0       97 2023-04-27 10:51:51.452409 pyprocessors-generative_augmenter-0.5.15/.dockerignore
--rw-r--r--   0        0        0      167 2023-04-27 11:04:50.634861 pyprocessors-generative_augmenter-0.5.15/.gitignore
--rw-r--r--   0        0        0      448 2023-04-27 10:51:51.452409 pyprocessors-generative_augmenter-0.5.15/Dockerfile
--rw-r--r--   0        0        0    10240 2023-04-27 10:51:51.452409 pyprocessors-generative_augmenter-0.5.15/Jenkinsfile
--rw-r--r--   0        0        0      380 2023-04-27 10:51:51.453409 pyprocessors-generative_augmenter-0.5.15/README.md
--rw-r--r--   0        0        0     1559 2023-04-27 10:51:51.453409 pyprocessors-generative_augmenter-0.5.15/bumpversion.py
--rw-r--r--   0        0        0       55 2023-04-28 06:37:16.775480 pyprocessors-generative_augmenter-0.5.15/pyprocessors_generative_augmenter/__init__.py
--rw-r--r--   0        0        0     5857 2023-04-27 10:51:51.453409 pyprocessors-generative_augmenter-0.5.15/pyprocessors_generative_augmenter/generative_augmenter.py
--rw-r--r--   0        0        0     2593 2023-04-27 10:51:51.453409 pyprocessors-generative_augmenter-0.5.15/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-27 10:51:51.453409 pyprocessors-generative_augmenter-0.5.15/tests/__init__.py
--rw-r--r--   0        0        0     9161 2023-04-27 10:51:51.454409 pyprocessors-generative_augmenter-0.5.15/tests/data/jinjadocs.json
--rw-r--r--   0        0        0     3031 2023-04-27 15:48:11.728253 pyprocessors-generative_augmenter-0.5.15/tests/data/jinjadocs_en.json
--rw-r--r--   0        0        0    13529 2023-04-28 06:34:53.916726 pyprocessors-generative_augmenter-0.5.15/tests/data/jinjadocs_preserve_entities.json
--rw-r--r--   0        0        0    17884 2023-04-28 06:37:14.065409 pyprocessors-generative_augmenter-0.5.15/tests/data/jinjadocs_preserve_entities_augmented.json
--rw-r--r--   0        0        0    14427 2023-04-28 06:34:53.920726 pyprocessors-generative_augmenter-0.5.15/tests/data/jinjadocs_substitute_entities.json
--rw-r--r--   0        0        0    19309 2023-04-28 06:37:14.071409 pyprocessors-generative_augmenter-0.5.15/tests/data/jinjadocs_substitute_entities_augmented.json
--rw-r--r--   0        0        0     1380 2023-04-28 06:34:53.923726 pyprocessors-generative_augmenter-0.5.15/tests/test_generative_augmenter.py
--rw-r--r--   0        0        0      951 2023-04-27 10:51:51.455409 pyprocessors-generative_augmenter-0.5.15/tox.ini
--rw-r--r--   0        0        0     1341 1970-01-01 00:00:00.000000 pyprocessors-generative_augmenter-0.5.15/setup.py
--rw-r--r--   0        0        0     2491 1970-01-01 00:00:00.000000 pyprocessors-generative_augmenter-0.5.15/PKG-INFO
+-rw-r--r--   0        0        0       97 2023-04-27 10:51:51.452409 pyprocessors-generative_augmenter-0.5.9/.dockerignore
+-rw-r--r--   0        0        0      167 2023-04-27 11:04:50.634861 pyprocessors-generative_augmenter-0.5.9/.gitignore
+-rw-r--r--   0        0        0      448 2023-04-27 10:51:51.452409 pyprocessors-generative_augmenter-0.5.9/Dockerfile
+-rw-r--r--   0        0        0    10240 2023-04-27 10:51:51.452409 pyprocessors-generative_augmenter-0.5.9/Jenkinsfile
+-rw-r--r--   0        0        0      380 2023-04-27 10:51:51.453409 pyprocessors-generative_augmenter-0.5.9/README.md
+-rw-r--r--   0        0        0     1559 2023-04-27 10:51:51.453409 pyprocessors-generative_augmenter-0.5.9/bumpversion.py
+-rw-r--r--   0        0        0       54 2023-04-27 11:12:49.262433 pyprocessors-generative_augmenter-0.5.9/pyprocessors_generative_augmenter/__init__.py
+-rw-r--r--   0        0        0     5857 2023-04-27 10:51:51.453409 pyprocessors-generative_augmenter-0.5.9/pyprocessors_generative_augmenter/generative_augmenter.py
+-rw-r--r--   0        0        0     2593 2023-04-27 10:51:51.453409 pyprocessors-generative_augmenter-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-27 10:51:51.453409 pyprocessors-generative_augmenter-0.5.9/tests/__init__.py
+-rw-r--r--   0        0        0     9161 2023-04-27 10:51:51.454409 pyprocessors-generative_augmenter-0.5.9/tests/data/jinjadocs.json
+-rw-r--r--   0        0        0     6757 2023-04-27 10:51:51.454409 pyprocessors-generative_augmenter-0.5.9/tests/data/jinjadocs_preserve_entities.json
+-rw-r--r--   0        0        0     7931 2023-04-27 11:12:46.257354 pyprocessors-generative_augmenter-0.5.9/tests/data/jinjadocs_preserve_entities_augmented.json
+-rw-r--r--   0        0        0     6713 2023-04-27 10:51:51.454409 pyprocessors-generative_augmenter-0.5.9/tests/data/jinjadocs_substitute_entities.json
+-rw-r--r--   0        0        0     8111 2023-04-27 11:12:46.260354 pyprocessors-generative_augmenter-0.5.9/tests/data/jinjadocs_substitute_entities_augmented.json
+-rw-r--r--   0        0        0     1379 2023-04-27 10:51:51.455409 pyprocessors-generative_augmenter-0.5.9/tests/test_generative_augmenter.py
+-rw-r--r--   0        0        0      951 2023-04-27 10:51:51.455409 pyprocessors-generative_augmenter-0.5.9/tox.ini
+-rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 pyprocessors-generative_augmenter-0.5.9/setup.py
+-rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 pyprocessors-generative_augmenter-0.5.9/PKG-INFO
```

### Comparing `pyprocessors-generative_augmenter-0.5.15/Jenkinsfile` & `pyprocessors-generative_augmenter-0.5.9/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `pyprocessors-generative_augmenter-0.5.15/bumpversion.py` & `pyprocessors-generative_augmenter-0.5.9/bumpversion.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-generative_augmenter-0.5.15/pyprocessors_generative_augmenter/generative_augmenter.py` & `pyprocessors-generative_augmenter-0.5.9/pyprocessors_generative_augmenter/generative_augmenter.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-generative_augmenter-0.5.15/pyproject.toml` & `pyprocessors-generative_augmenter-0.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyprocessors-generative_augmenter-0.5.15/tests/data/jinjadocs.json` & `pyprocessors-generative_augmenter-0.5.9/tests/data/jinjadocs.json`

 * *Files identical despite different names*

### Comparing `pyprocessors-generative_augmenter-0.5.15/tests/test_generative_augmenter.py` & `pyprocessors-generative_augmenter-0.5.9/tests/test_generative_augmenter.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,27 +16,27 @@
     model_class = model.construct().__class__
     assert model_class == GenerativeAugmenterParameters
 
 
 @pytest.mark.parametrize("variant", ['preserve_entities', 'substitute_entities'])
 def test_augment_doc(variant):
     parameters = GenerativeAugmenterParameters(
-        to_lowercase=False,
+        to_lowercase=True,
         variant_altText=variant,
         variant_separator_regex="^- "
     )
     processor = GenerativeAugmenterProcessor()
     testdir = Path(__file__).parent
     source = Path(
         testdir,
         f"data/jinjadocs_{variant}.json",
     )
     with source.open("r") as fin:
         jdocs = json.load(fin)
         docs = [Document(**jdoc) for jdoc in jdocs]
         docs = processor.process(docs, parameters)
-        assert docs == HasLen(6)
+        assert docs == HasLen(3)
         sum_file = testdir / f"data/jinjadocs_{variant}_augmented.json"
         dl = DocumentList(__root__=docs)
         with sum_file.open("w") as fout:
             print(dl.json(exclude_none=True, exclude_unset=True, indent=2), file=fout)
     # noqa: E501
```

### Comparing `pyprocessors-generative_augmenter-0.5.15/tox.ini` & `pyprocessors-generative_augmenter-0.5.9/tox.ini`

 * *Files identical despite different names*

### Comparing `pyprocessors-generative_augmenter-0.5.15/setup.py` & `pyprocessors-generative_augmenter-0.5.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
           'flask==2.1.3']}
 
 entry_points = \
 {'pyprocessors.plugins': ['generative_augmenter = '
                           'pyprocessors_generative_augmenter.generative_augmenter:GenerativeAugmenterProcessor']}
 
 setup(name='pyprocessors-generative_augmenter',
-      version='0.5.15',
+      version='0.5.9',
       description='GenerativeazA$$ processor',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://kairntech.com/',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `pyprocessors-generative_augmenter-0.5.15/PKG-INFO` & `pyprocessors-generative_augmenter-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprocessors-generative_augmenter
-Version: 0.5.15
+Version: 0.5.9
 Summary: GenerativeazA$$ processor
 Home-page: https://kairntech.com/
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
```

