# Comparing `tmp/ogc_na-0.1.1.tar.gz` & `tmp/ogc_na-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogc_na-0.1.1.tar", last modified: Wed Apr 26 07:04:37 2023, max compression
+gzip compressed data, was "ogc_na-0.1.2.tar", last modified: Fri Apr 28 08:49:57 2023, max compression
```

## Comparing `ogc_na-0.1.1.tar` & `ogc_na-0.1.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:37.460713 ogc_na-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:37.456713 ogc_na-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:37.456713 ogc_na-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-26 07:04:25.000000 ogc_na-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-04-26 07:04:25.000000 ogc_na-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-26 07:04:25.000000 ogc_na-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-26 07:04:37.460713 ogc_na-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-26 07:04:25.000000 ogc_na-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:37.456713 ogc_na-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-04-26 07:04:25.000000 ogc_na-0.1.1/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-26 07:04:25.000000 ogc_na-0.1.1/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-26 07:04:25.000000 ogc_na-0.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-04-26 07:04:25.000000 ogc_na-0.1.1/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-26 07:04:25.000000 ogc_na-0.1.1/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:37.456713 ogc_na-0.1.1/ogc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:37.456713 ogc_na-0.1.1/ogc/na/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-26 07:04:25.000000 ogc_na-0.1.1/ogc/na/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18120 2023-04-26 07:04:25.000000 ogc_na-0.1.1/ogc/na/annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-04-26 07:04:25.000000 ogc_na-0.1.1/ogc/na/domain_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-26 07:04:25.000000 ogc_na-0.1.1/ogc/na/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    30863 2023-04-26 07:04:25.000000 ogc_na-0.1.1/ogc/na/ingest_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-04-26 07:04:25.000000 ogc_na-0.1.1/ogc/na/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-26 07:04:25.000000 ogc_na-0.1.1/ogc/na/provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    17174 2023-04-26 07:04:25.000000 ogc_na-0.1.1/ogc/na/update_vocabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-04-26 07:04:25.000000 ogc_na-0.1.1/ogc/na/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-26 07:04:25.000000 ogc_na-0.1.1/ogc/na/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:37.456713 ogc_na-0.1.1/ogc_na.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-26 07:04:37.000000 ogc_na-0.1.1/ogc_na.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-26 07:04:37.000000 ogc_na-0.1.1/ogc_na.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:04:37.000000 ogc_na-0.1.1/ogc_na.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-26 07:04:37.000000 ogc_na-0.1.1/ogc_na.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-26 07:04:37.000000 ogc_na-0.1.1/ogc_na.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-26 07:04:25.000000 ogc_na-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:37.456713 ogc_na-0.1.1/rdf/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-26 07:04:25.000000 ogc_na-0.1.1/rdf/catalog-v001.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-26 07:04:25.000000 ogc_na-0.1.1/rdf/domaincfg.vocab.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-26 07:04:25.000000 ogc_na-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 07:04:37.460713 ogc_na-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-26 07:04:25.000000 ogc_na-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:37.460713 ogc_na-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:25.000000 ogc_na-0.1.1/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:37.460713 ogc_na-0.1.1/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:25.000000 ogc_na-0.1.1/test/data/empty.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-26 07:04:25.000000 ogc_na-0.1.1/test/data/profile_tree.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-26 07:04:25.000000 ogc_na-0.1.1/test/data/profile_tree_cyclic.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-26 07:04:25.000000 ogc_na-0.1.1/test/data/uplift_context_valid.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-26 07:04:25.000000 ogc_na-0.1.1/test/test_annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-26 07:04:25.000000 ogc_na-0.1.1/test/test_ingest_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-26 07:04:25.000000 ogc_na-0.1.1/test/test_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:57.156715 ogc_na-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:57.144714 ogc_na-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:57.148715 ogc_na-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-28 08:49:43.000000 ogc_na-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-04-28 08:49:43.000000 ogc_na-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-28 08:49:43.000000 ogc_na-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-28 08:49:57.156715 ogc_na-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-28 08:49:43.000000 ogc_na-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:57.148715 ogc_na-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-04-28 08:49:43.000000 ogc_na-0.1.2/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-28 08:49:43.000000 ogc_na-0.1.2/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-28 08:49:43.000000 ogc_na-0.1.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-04-28 08:49:43.000000 ogc_na-0.1.2/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-28 08:49:43.000000 ogc_na-0.1.2/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:57.148715 ogc_na-0.1.2/ogc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:57.152715 ogc_na-0.1.2/ogc/na/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-28 08:49:43.000000 ogc_na-0.1.2/ogc/na/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-04-28 08:49:43.000000 ogc_na-0.1.2/ogc/na/annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-04-28 08:49:43.000000 ogc_na-0.1.2/ogc/na/domain_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-04-28 08:49:43.000000 ogc_na-0.1.2/ogc/na/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30863 2023-04-28 08:49:43.000000 ogc_na-0.1.2/ogc/na/ingest_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-04-28 08:49:43.000000 ogc_na-0.1.2/ogc/na/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-28 08:49:43.000000 ogc_na-0.1.2/ogc/na/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17174 2023-04-28 08:49:43.000000 ogc_na-0.1.2/ogc/na/update_vocabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-04-28 08:49:43.000000 ogc_na-0.1.2/ogc/na/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-28 08:49:43.000000 ogc_na-0.1.2/ogc/na/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:57.152715 ogc_na-0.1.2/ogc_na.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-28 08:49:57.000000 ogc_na-0.1.2/ogc_na.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-28 08:49:57.000000 ogc_na-0.1.2/ogc_na.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 08:49:57.000000 ogc_na-0.1.2/ogc_na.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-28 08:49:57.000000 ogc_na-0.1.2/ogc_na.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-28 08:49:57.000000 ogc_na-0.1.2/ogc_na.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-28 08:49:43.000000 ogc_na-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:57.152715 ogc_na-0.1.2/rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-28 08:49:43.000000 ogc_na-0.1.2/rdf/catalog-v001.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-28 08:49:43.000000 ogc_na-0.1.2/rdf/domaincfg.vocab.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-28 08:49:43.000000 ogc_na-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 08:49:57.156715 ogc_na-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-28 08:49:43.000000 ogc_na-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:57.152715 ogc_na-0.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:43.000000 ogc_na-0.1.2/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:57.156715 ogc_na-0.1.2/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 08:49:43.000000 ogc_na-0.1.2/test/data/empty.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-28 08:49:43.000000 ogc_na-0.1.2/test/data/profile_tree.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-28 08:49:43.000000 ogc_na-0.1.2/test/data/profile_tree_cyclic.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-28 08:49:43.000000 ogc_na-0.1.2/test/data/uplift_context_valid.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-28 08:49:43.000000 ogc_na-0.1.2/test/test_annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-28 08:49:43.000000 ogc_na-0.1.2/test/test_ingest_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-28 08:49:43.000000 ogc_na-0.1.2/test/test_profile.py
```

### Comparing `ogc_na-0.1.1/.github/workflows/python-publish.yml` & `ogc_na-0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.1/.gitignore` & `ogc_na-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.1/PKG-INFO` & `ogc_na-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc_na
-Version: 0.1.1
+Version: 0.1.2
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.com/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.1.1/README.md` & `ogc_na-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.1/docs/examples.md` & `ogc_na-0.1.2/docs/examples.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.1/docs/gen_ref_pages.py` & `ogc_na-0.1.2/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.1/docs/index.md` & `ogc_na-0.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.1/docs/tutorials.md` & `ogc_na-0.1.2/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.1/mkdocs.yml` & `ogc_na-0.1.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.1/ogc/na/annotate_schema.py` & `ogc_na-0.1.2/ogc/na/annotate_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,15 +340,15 @@
                     else:
                         logger.info(' >> Found $ref to new schema: %s', prop_value['$ref'])
                         if ref_url:
                             self._process_schema(url=ref)
                         else:
                             self._process_schema(fn=ref)
 
-            properties.update({p: {ANNOTATION_ID: terms[p]} for p in empty_properties})
+            properties.update({p: {ANNOTATION_ID: terms[p]} for p in empty_properties if p in terms})
 
         schema_type = schema.get('type')
 
         if schema_type == 'object':
             process_properties(schema)
         elif schema_type == 'array':
             for k in ('prefixItems', 'items', 'contains'):
@@ -391,15 +391,15 @@
 
         own_context = {}
 
         def read_properties(where: dict):
             if not isinstance(where, dict):
                 return
             for prop, prop_val in where.get('properties', {}).items():
-                if ANNOTATION_ID in prop_val:
+                if isinstance(prop_val, dict) and ANNOTATION_ID in prop_val:
                     prop_context = {
                         '@id': prop_val[ANNOTATION_ID]
                     }
                     if ANNOTATION_TYPE in prop_val:
                         prop_context['@type'] = prop_val[ANNOTATION_TYPE]
 
                     if '$ref' in prop_val:
```

### Comparing `ogc_na-0.1.1/ogc/na/domain_config.py` & `ogc_na-0.1.2/ogc/na/domain_config.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.1/ogc/na/download.py` & `ogc_na-0.1.2/ogc/na/download.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #!/usr/bin/env python3
 from __future__ import annotations
+
 import argparse
-import json
 import logging
-from pathlib import Path
-from typing import Sequence, Iterable
-from urllib import request
-import sys
 import os
+import sys
+from pathlib import Path
+from typing import Iterable
 from urllib.parse import urlparse
 
 import requests
 
 from ogc.na import util
 
 logger = logging.getLogger(__name__)
@@ -38,27 +37,35 @@
                 raise
     if overwrite:
         dest.parent.mkdir(parents=True, exist_ok=True)
         with open(dest, 'wb') as f:
             f.write(r.content)
 
 
-def download_files(spec: Iterable[dict] | str | Path,
+def download_files(spec: dict | Iterable[dict] | str | Path,
                    object_diff: bool = True,
                    ignore_diff_errors: bool = True):
 
     if isinstance(spec, str) or isinstance(spec, Path):
         spec = util.load_yaml(filename=spec)
 
+    if 'json-downloads' in spec:
+        spec = spec['json-downloads']
+
+    if not spec:
+        return
+
     if not isinstance(spec, Iterable):
         raise ValueError('Unknown spec type: {}'.format(type(spec)))
 
     for entry in spec:
+        entry_object_diff = entry.get('object-diff', object_diff)
         download_file(entry['url'], entry['dest'],
-                      object_diff=object_diff, ignore_diff_errors=ignore_diff_errors)
+                      object_diff=entry_object_diff,
+                      ignore_diff_errors=ignore_diff_errors)
 
 
 def _process_cmdln():
     parser = argparse.ArgumentParser(
         epilog='Either a URL (with an optional destination) or a --spec must be provided.'
     )
 
@@ -97,15 +104,15 @@
         dest = args.destination or os.path.basename(urlparse(args.url).path)
         if not dest:
             raise ValueError('Destination file not provided and cannot be inferred')
         download_file(args.url, dest,
                       object_diff=not args.disable_diff,
                       ignore_diff_errors=not args.fail_on_diff_error)
     elif args.spec:
-        download_files(args.spec)
+        download_files(spec=args.spec)
     else:
         parser.print_usage()
 
 
 if __name__ == '__main__':
 
     logging.basicConfig(
```

### Comparing `ogc_na-0.1.1/ogc/na/ingest_json.py` & `ogc_na-0.1.2/ogc/na/ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.1/ogc/na/profile.py` & `ogc_na-0.1.2/ogc/na/profile.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.1/ogc/na/provenance.py` & `ogc_na-0.1.2/ogc/na/provenance.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.1/ogc/na/update_vocabs.py` & `ogc_na-0.1.2/ogc/na/update_vocabs.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.1/ogc/na/util.py` & `ogc_na-0.1.2/ogc/na/util.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.1/ogc/na/validation.py` & `ogc_na-0.1.2/ogc/na/validation.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.1/ogc_na.egg-info/PKG-INFO` & `ogc_na-0.1.2/ogc_na.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc-na
-Version: 0.1.1
+Version: 0.1.2
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.com/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.1.1/ogc_na.egg-info/SOURCES.txt` & `ogc_na-0.1.2/ogc_na.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.1/pyproject.toml` & `ogc_na-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.1/rdf/domaincfg.vocab.ttl` & `ogc_na-0.1.2/rdf/domaincfg.vocab.ttl`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.1/test/data/uplift_context_valid.yml` & `ogc_na-0.1.2/test/data/uplift_context_valid.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.1/test/test_annotate_schema.py` & `ogc_na-0.1.2/test/test_annotate_schema.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.1/test/test_ingest_json.py` & `ogc_na-0.1.2/test/test_ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.1/test/test_profile.py` & `ogc_na-0.1.2/test/test_profile.py`

 * *Files identical despite different names*

