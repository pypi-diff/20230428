# Comparing `tmp/arkindex-base-worker-0.3.3rc2.tar.gz` & `tmp/arkindex-base-worker-0.3.3rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkindex-base-worker-0.3.3rc2.tar", last modified: Tue Apr 25 08:57:11 2023, max compression
+gzip compressed data, was "arkindex-base-worker-0.3.3rc3.tar", last modified: Fri Apr 28 11:09:42 2023, max compression
```

## Comparing `arkindex-base-worker-0.3.3rc2.tar` & `arkindex-base-worker-0.3.3rc3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:57:11.720569 arkindex-base-worker-0.3.3rc2/
--rw-r--r--   0 root         (0) root         (0)      248 2023-04-25 08:57:11.720569 arkindex-base-worker-0.3.3rc2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:57:11.716569 arkindex-base-worker-0.3.3rc2/arkindex_base_worker.egg-info/
--rw-r--r--   0 root         (0) root         (0)      248 2023-04-25 08:57:11.000000 arkindex-base-worker-0.3.3rc2/arkindex_base_worker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1349 2023-04-25 08:57:11.000000 arkindex-base-worker-0.3.3rc2/arkindex_base_worker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 08:57:11.000000 arkindex-base-worker-0.3.3rc2/arkindex_base_worker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      318 2023-04-25 08:57:11.000000 arkindex-base-worker-0.3.3rc2/arkindex_base_worker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-25 08:57:11.000000 arkindex-base-worker-0.3.3rc2/arkindex_base_worker.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:57:11.716569 arkindex-base-worker-0.3.3rc2/arkindex_worker/
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10871 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/cache.py
--rw-rw-rw-   0 root         (0) root         (0)    15338 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/git.py
--rw-rw-rw-   0 root         (0) root         (0)    13466 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/image.py
--rw-rw-rw-   0 root         (0) root         (0)     9619 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/models.py
--rw-rw-rw-   0 root         (0) root         (0)     8012 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/reporting.py
--rw-rw-rw-   0 root         (0) root         (0)     5507 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:57:11.716569 arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/
--rw-rw-rw-   0 root         (0) root         (0)    11662 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15968 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/base.py
--rw-rw-rw-   0 root         (0) root         (0)    10935 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/classification.py
--rw-rw-rw-   0 root         (0) root         (0)    19034 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/element.py
--rw-rw-rw-   0 root         (0) root         (0)    14657 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/entity.py
--rw-rw-rw-   0 root         (0) root         (0)     6657 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    10374 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/training.py
--rw-rw-rw-   0 root         (0) root         (0)    19105 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/transcription.py
--rw-rw-rw-   0 root         (0) root         (0)     1460 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/version.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-04-25 08:57:11.720569 arkindex-base-worker-0.3.3rc2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      768 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:57:11.720569 arkindex-base-worker-0.3.3rc2/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17541 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    21333 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_base_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     8705 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    12961 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_element.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:57:11.720569 arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    32744 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_classifications.py
--rw-rw-rw-   0 root         (0) root         (0)     2751 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    52786 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_elements.py
--rw-rw-rw-   0 root         (0) root         (0)    36695 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_entities.py
--rw-rw-rw-   0 root         (0) root         (0)    18023 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     8292 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_training.py
--rw-rw-rw-   0 root         (0) root         (0)    69404 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_transcriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    10239 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_worker.py
--rw-rw-rw-   0 root         (0) root         (0)    14944 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_git.py
--rw-rw-rw-   0 root         (0) root         (0)    14353 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_image.py
--rw-rw-rw-   0 root         (0) root         (0)     8406 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_merge.py
--rw-rw-rw-   0 root         (0) root         (0)     8802 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_reporting.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:09:42.643734 arkindex-base-worker-0.3.3rc3/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-04-28 11:09:42.643734 arkindex-base-worker-0.3.3rc3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:09:42.639734 arkindex-base-worker-0.3.3rc3/arkindex_base_worker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-04-28 11:09:42.000000 arkindex-base-worker-0.3.3rc3/arkindex_base_worker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1349 2023-04-28 11:09:42.000000 arkindex-base-worker-0.3.3rc3/arkindex_base_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 11:09:42.000000 arkindex-base-worker-0.3.3rc3/arkindex_base_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      318 2023-04-28 11:09:42.000000 arkindex-base-worker-0.3.3rc3/arkindex_base_worker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 11:09:42.000000 arkindex-base-worker-0.3.3rc3/arkindex_base_worker.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:09:42.639734 arkindex-base-worker-0.3.3rc3/arkindex_worker/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9882 2023-04-28 10:27:51.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    15338 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/git.py
+-rw-rw-rw-   0 root         (0) root         (0)    13466 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     9619 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     8012 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/reporting.py
+-rw-rw-rw-   0 root         (0) root         (0)     6926 2023-04-28 11:06:20.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:09:42.639734 arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/
+-rw-rw-rw-   0 root         (0) root         (0)    11662 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16983 2023-04-28 10:27:51.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    10935 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)    19034 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/element.py
+-rw-rw-rw-   0 root         (0) root         (0)    14657 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/entity.py
+-rw-rw-rw-   0 root         (0) root         (0)     6657 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    10211 2023-04-28 11:06:20.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/training.py
+-rw-rw-rw-   0 root         (0) root         (0)    19105 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/transcription.py
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-04-28 11:09:42.643734 arkindex-base-worker-0.3.3rc3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      768 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:09:42.639734 arkindex-base-worker-0.3.3rc3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17541 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    22358 2023-04-28 10:27:51.000000 arkindex-base-worker-0.3.3rc3/tests/test_base_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     8705 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    12961 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_element.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:09:42.643734 arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    32744 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_classifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    52786 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_elements.py
+-rw-rw-rw-   0 root         (0) root         (0)    36695 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)    18023 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     8292 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_training.py
+-rw-rw-rw-   0 root         (0) root         (0)    69404 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_transcriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10239 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)    14944 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_git.py
+-rw-rw-rw-   0 root         (0) root         (0)    14353 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     8402 2023-04-28 10:27:51.000000 arkindex-base-worker-0.3.3rc3/tests/test_merge.py
+-rw-rw-rw-   0 root         (0) root         (0)     8802 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_reporting.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_utils.py
```

### Comparing `arkindex-base-worker-0.3.3rc2/arkindex_base_worker.egg-info/SOURCES.txt` & `arkindex-base-worker-0.3.3rc3/arkindex_base_worker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/arkindex_worker/cache.py` & `arkindex-base-worker-0.3.3rc3/arkindex_worker/cache.py`

 * *Files 9% similar despite different names*

```diff
@@ -298,48 +298,14 @@
                 version = None
 
             assert (
                 version == SQL_VERSION
             ), f"The SQLite database {cache_path} does not have the correct cache version, it should be {SQL_VERSION}"
 
 
-def retrieve_parents_cache_path(
-    parent_ids: list, data_dir: Path = Path("/data"), chunk: int = None
-) -> list:
-    """
-    Retrieve the path of the given parent's in the
-    :param parent_ids: List of element IDs to search
-    :param data_dir: Base folder where to look for
-    :param chunk: Index of the chunk of the db that might contain the paths
-    :return: The corresponding list of paths
-    """
-    assert isinstance(parent_ids, list)
-    assert data_dir.is_dir()
-
-    # Handle possible chunk in parent task name
-    # This is needed to support the init_elements databases
-    filenames = [
-        "db.sqlite",
-    ]
-    if chunk is not None:
-        filenames.append(f"db_{chunk}.sqlite")
-
-    # Find all the paths for these databases
-    return list(
-        filter(
-            lambda p: p.is_file(),
-            [
-                Path(data_dir, parent, name)
-                for parent in parent_ids
-                for name in filenames
-            ],
-        )
-    )
-
-
 def merge_parents_cache(paths: list, current_database: Path):
     """
     Merge all the potential parent task's databases into the existing local one
     :param paths: Path to cache databases
     :param current_database: Path to the current database
     """
     assert current_database.exists()
```

### Comparing `arkindex-base-worker-0.3.3rc2/arkindex_worker/git.py` & `arkindex-base-worker-0.3.3rc3/arkindex_worker/git.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/arkindex_worker/image.py` & `arkindex-base-worker-0.3.3rc3/arkindex_worker/image.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/arkindex_worker/models.py` & `arkindex-base-worker-0.3.3rc3/arkindex_worker/models.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/arkindex_worker/reporting.py` & `arkindex-base-worker-0.3.3rc3/arkindex_worker/reporting.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/arkindex_worker/utils.py` & `arkindex-base-worker-0.3.3rc3/arkindex_worker/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 import hashlib
 import logging
 import os
 import tarfile
 import tempfile
 from pathlib import Path
-from typing import Tuple
+from typing import Optional, Tuple, Union
 
 import zstandard
 import zstandard as zstd
 
 logger = logging.getLogger(__name__)
 
 CHUNK_SIZE = 1024
@@ -84,56 +84,71 @@
     try:
         os.close(file_descriptor)
         file_path.unlink()
     except OSError as e:
         logger.warning(f"Unable to delete file {file_path}: {e}")
 
 
-def zstd_compress(source: Path) -> Tuple[int, Path, str]:
+def zstd_compress(
+    source: Path, destination: Optional[Path] = None
+) -> Tuple[Union[int, None], Path, str]:
     """Compress a file using the Zstandard compression algorithm.
 
     :param source: Path to the file to compress.
-    :return: The file descriptor and path to the compressed file, hash of its content.
+    :param destination: Optional path for the created ZSTD archive. A tempfile will be created if this is omitted.
+    :return: The file descriptor (if one was created) and path to the compressed file, hash of its content.
     """
     compressor = zstd.ZstdCompressor(level=3)
     archive_hasher = hashlib.md5()
-    file_d, path_to_zst_archive = tempfile.mkstemp(prefix="teklia-", suffix=".tar.zst")
-    logger.debug(f"Compressing file to {path_to_zst_archive}")
-    path_to_zst_archive = Path(path_to_zst_archive)
+
+    # Parse destination and create a tmpfile if none was specified
+    file_d, destination = (
+        tempfile.mkstemp(prefix="teklia-", suffix=".tar.zst")
+        if destination is None
+        else (None, destination)
+    )
+    destination = Path(destination)
+    logger.debug(f"Compressing file to {destination}")
+
     try:
-        with path_to_zst_archive.open("wb") as archive_file, source.open(
-            "rb"
-        ) as model_data:
+        with destination.open("wb") as archive_file, source.open("rb") as model_data:
             for model_chunk in iter(lambda: model_data.read(CHUNK_SIZE), b""):
                 compressed_chunk = compressor.compress(model_chunk)
                 archive_hasher.update(compressed_chunk)
                 archive_file.write(compressed_chunk)
         logger.debug(f"Successfully compressed {source}")
     except zstandard.ZstdError as e:
         raise Exception(f"Couldn't compress archive: {e}")
-    return file_d, path_to_zst_archive, archive_hasher.hexdigest()
+    return file_d, destination, archive_hasher.hexdigest()
 
 
-def create_tar_archive(path: Path) -> Tuple[Path, str]:
+def create_tar_archive(
+    path: Path, destination: Optional[Path] = None
+) -> Tuple[Union[int, None], Path, str]:
     """Create a tar archive using the content at specified location.
 
     :param path: Path to the file to archive
-    :return: The file descriptor and path to the TAR archive, hash of its content.
+    :param destination: Optional path for the created TAR archive. A tempfile will be created if this is omitted.
+    :return: The file descriptor (if one was created) and path to the TAR archive, hash of its content.
     """
-    # Remove extension from the model filename
-    tar_descriptor, path_to_tar_archive = tempfile.mkstemp(
-        prefix="teklia-", suffix=".tar"
+    # Parse destination and create a tmpfile if none was specified
+    file_d, destination = (
+        tempfile.mkstemp(prefix="teklia-", suffix=".tar")
+        if destination is None
+        else (None, destination)
     )
+    destination = Path(destination)
+    logger.debug(f"Compressing file to {destination}")
 
     # Create an uncompressed tar archive with all the needed files
     # Files hierarchy ifs kept in the archive.
     files = []
     try:
-        logger.debug(f"Compressing files to {path_to_tar_archive}")
-        with tarfile.open(path_to_tar_archive, "w") as tar:
+        logger.debug(f"Compressing files to {destination}")
+        with tarfile.open(destination, "w") as tar:
             for p in path.rglob("*"):
                 x = p.relative_to(path)
                 tar.add(p, arcname=x, recursive=False)
                 # Only keep files when computing the hash
                 if p.is_file():
                     files.append(p)
         logger.debug(f"Successfully created Tar archive from files @ {path}")
@@ -145,8 +160,27 @@
 
     content_hasher = hashlib.md5()
     # Compute hash of the files
     for file_path in files:
         with file_path.open("rb") as file_data:
             for chunk in iter(lambda: file_data.read(CHUNK_SIZE), b""):
                 content_hasher.update(chunk)
-    return tar_descriptor, Path(path_to_tar_archive), content_hasher.hexdigest()
+    return file_d, destination, content_hasher.hexdigest()
+
+
+def create_tar_zst_archive(
+    source: Path, destination: Optional[Path] = None
+) -> Tuple[Union[int, None], Path, str, str]:
+    """Helper to create a TAR+ZST archive from a source folder.
+
+    :param source: Path to the folder whose content should be archived.
+    :param destination: Path to the created archive, defaults to None. If unspecified, a temporary file will be created.
+    :return: The file descriptor of the created tempfile (if one was created), path to the archive, its hash and the hash of the tar archive's content.
+    """
+    # Create tar archive
+    tar_fd, tar_archive, tar_hash = create_tar_archive(source)
+
+    zstd_fd, zstd_archive, zstd_hash = zstd_compress(tar_archive, destination)
+
+    close_delete_file(tar_fd, tar_archive)
+
+    return zstd_fd, zstd_archive, zstd_hash, tar_hash
```

### Comparing `arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/__init__.py` & `arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/base.py` & `arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 
 import argparse
 import json
 import logging
 import os
 from pathlib import Path
-from typing import Optional
+from typing import List, Optional
 
 import gnupg
 import yaml
 from apistar.exceptions import ErrorResponse
 from tenacity import (
     before_sleep_log,
     retry,
@@ -25,15 +25,14 @@
 from arkindex_worker import logger
 from arkindex_worker.cache import (
     check_version,
     create_tables,
     create_version_table,
     init_cache_db,
     merge_parents_cache,
-    retrieve_parents_cache_path,
 )
 
 
 def _is_500_error(exc: Exception) -> bool:
     """
     Check if an Arkindex API error has a HTTP 5xx error code.
     Used to retry most API calls in [BaseWorker][arkindex_worker.worker.base.BaseWorker].
@@ -139,20 +138,20 @@
         self.process_information = None
         # corpus_id will be updated in configure() using the worker_run's corpus
         # or in configure_for_developers() from the environment
         self.corpus_id = None
         self.user_configuration = {}
         self.model_configuration = {}
         self.support_cache = support_cache
-        # use_cache will be updated in configure() if the cache is supported and if there
-        # is at least one available sqlite database either given or in the parent tasks
+        # use_cache will be updated in configure_cache() if the cache is supported and if
+        # there is at least one available sqlite database either given or in the parent tasks
         self.use_cache = False
 
-        # task_parents will be updated in configure() if the cache is supported and if there
-        # is at least one available sqlite database either given or in the parent tasks
+        # task_parents will be updated in configure_cache() if the cache is supported and if
+        # there is at least one available sqlite database either given or in the parent tasks
         self.task_parents = []
 
         # Define API Client
         self.setup_api_client()
 
     @property
     def is_read_only(self) -> bool:
@@ -249,15 +248,15 @@
                 "user_configuration"
             ].items():
                 if "default" in value:
                     self.user_configuration[key] = value["default"]
 
         # Load all required secrets
         required_secrets = worker_version["configuration"].get("secrets", [])
-        self.secrets = {name: self.load_secret(name) for name in required_secrets}
+        self.secrets = {name: self.load_secret(Path(name)) for name in required_secrets}
 
         # Load worker run configuration when available
         worker_configuration = worker_run.get("configuration")
         if worker_configuration and worker_configuration.get("configuration"):
             logger.info("Loaded user configuration from WorkerRun")
             self.user_configuration.update(worker_configuration.get("configuration"))
 
@@ -281,19 +280,15 @@
         """
         paths = None
         if self.support_cache and self.args.database is not None:
             self.use_cache = True
         elif self.support_cache and self.task_id:
             task = self.request("RetrieveTaskFromAgent", id=self.task_id)
             self.task_parents = task["parents"]
-            paths = retrieve_parents_cache_path(
-                self.task_parents,
-                data_dir=self.task_data_dir,
-                chunk=self.task_chunk,
-            )
+            paths = self.find_parents_file_paths(Path("db.sqlite"))
             self.use_cache = len(paths) > 0
 
         if self.use_cache:
             if self.args.database is not None:
                 assert (
                     self.args.database.is_file()
                 ), f"Database in {self.args.database} does not exist"
@@ -392,14 +387,45 @@
             model_dir = Path(model_dir)
             if not model_dir.exists():
                 raise ModelNotFoundError(
                     f"The path {model_dir} does not link to any directory"
                 )
             return model_dir
 
+    def find_parents_file_paths(self, filename: Path) -> List[Path]:
+        """
+        Find the paths of a specific file from the parent tasks.
+        Only works if the task_parents attributes is updated, so if the cache is supported and
+        if there is at least one available sqlite database either given or in the parent tasks
+
+        :param filename: Name of the file to find
+        :return: Paths to the parent files
+        """
+        # Handle possible chunk in parent task name
+        # This is needed to support the init_elements databases
+        filenames = [
+            filename,
+        ]
+        if self.task_chunk is not None:
+            filenames.append(
+                f"{filename.name.replace(filename.suffix, '')}_{self.task_chunk}{filename.suffix}"
+            )
+
+        # Find all the paths for these files
+        return list(
+            filter(
+                lambda p: p.is_file(),
+                [
+                    self.task_data_dir / parent_id / name
+                    for parent_id in self.task_parents
+                    for name in filenames
+                ],
+            )
+        )
+
     @retry(
         retry=retry_if_exception(_is_500_error),
         wait=wait_exponential(multiplier=2, min=3),
         reraise=True,
         stop=stop_after_attempt(5),
         before_sleep=before_sleep_log(logger, logging.INFO),
     )
```

### Comparing `arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/classification.py` & `arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/classification.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/element.py` & `arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/element.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/entity.py` & `arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/entity.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/metadata.py` & `arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/metadata.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/training.py` & `arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import NewType, Optional, Tuple, Union
 from uuid import UUID
 
 import requests
 from apistar.exceptions import ErrorResponse
 
 from arkindex_worker import logger
-from arkindex_worker.utils import close_delete_file, create_tar_archive, zstd_compress
+from arkindex_worker.utils import close_delete_file, create_tar_zst_archive
 
 DirPath = NewType("DirPath", Path)
 """Path to a directory"""
 
 Hash = NewType("Hash", str)
 """MD5 Hash"""
 
@@ -33,21 +33,17 @@
     Yield its location, its hash, its size and its content's hash.
 
     :param path: Create a compressed tar archive from the files
     :returns: The location of the created archive, its hash, its size and its content's hash
     """
     assert path.is_dir(), "create_archive needs a directory"
 
-    tar_descriptor, tar_archive, content_hash = create_tar_archive(path)
-
-    # Compress the archive
-    zstd_descriptor, zstd_archive, archive_hash = zstd_compress(tar_archive)
-
-    # Remove the tar archive
-    close_delete_file(tar_descriptor, tar_archive)
+    zstd_descriptor, zstd_archive, archive_hash, content_hash = create_tar_zst_archive(
+        path
+    )
 
     # Get content hash, archive size and hash
     yield zstd_archive, content_hash, zstd_archive.stat().st_size, archive_hash
 
     # Remove the zstd archive
     close_delete_file(zstd_descriptor, zstd_archive)
```

### Comparing `arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/transcription.py` & `arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/transcription.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/version.py` & `arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/version.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/setup.py` & `arkindex-base-worker-0.3.3rc3/setup.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/tests/conftest.py` & `arkindex-base-worker-0.3.3rc3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/tests/test_base_worker.py` & `arkindex-base-worker-0.3.3rc3/tests/test_base_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -646,7 +646,35 @@
 
     worker = BaseWorker()
     worker.args = worker.parser.parse_args()
     worker.config = {"model_dir": model_path}
 
     with pytest.raises(ModelNotFoundError, match=error):
         worker.find_model_directory()
+
+
+def test_find_parents_file_paths(responses, mock_base_worker_with_cache, tmp_path):
+    responses.add(
+        responses.GET,
+        "http://testserver/api/v1/task/my_task/from-agent/",
+        status=200,
+        json={"parents": ["first", "second", "third"]},
+    )
+
+    filename = Path("my_file.txt")
+    for parent_id, content in zip(["first", "third"], ["Some text", "Other text"]):
+        (tmp_path / parent_id).mkdir()
+        file_path = tmp_path / parent_id / filename
+        with file_path.open("w", encoding="utf-8") as f:
+            f.write(content)
+
+    # Configure worker with a specific data directory
+    mock_base_worker_with_cache.task_data_dir = tmp_path
+    mock_base_worker_with_cache.args = mock_base_worker_with_cache.parser.parse_args()
+
+    mock_base_worker_with_cache.configure()
+    mock_base_worker_with_cache.configure_cache()
+
+    assert mock_base_worker_with_cache.find_parents_file_paths(filename) == [
+        tmp_path / "first" / filename,
+        tmp_path / "third" / filename,
+    ]
```

### Comparing `arkindex-base-worker-0.3.3rc2/tests/test_cache.py` & `arkindex-base-worker-0.3.3rc3/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/tests/test_element.py` & `arkindex-base-worker-0.3.3rc3/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_classifications.py` & `arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_classifications.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_cli.py` & `arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_cli.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_elements.py` & `arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_elements.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_entities.py` & `arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_entities.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_metadata.py` & `arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_metadata.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_training.py` & `arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_training.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_transcriptions.py` & `arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_transcriptions.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_worker.py` & `arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_worker.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/tests/test_git.py` & `arkindex-base-worker-0.3.3rc3/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/tests/test_image.py` & `arkindex-base-worker-0.3.3rc3/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/tests/test_merge.py` & `arkindex-base-worker-0.3.3rc3/tests/test_merge.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     CachedElement,
     CachedEntity,
     CachedImage,
     CachedTranscription,
     CachedTranscriptionEntity,
     Version,
     merge_parents_cache,
-    retrieve_parents_cache_path,
 )
 
 
 @pytest.mark.parametrize(
     "parents, expected_elements, expected_transcriptions",
     (
         # Nothing happen when no parents are available
@@ -87,15 +86,18 @@
         assert CachedElement.select().count() == 0
         assert CachedTranscription.select().count() == 0
         assert CachedClassification.select().count() == 0
         assert CachedEntity.select().count() == 0
         assert CachedTranscriptionEntity.select().count() == 0
 
     # Retrieve parents databases paths
-    paths = retrieve_parents_cache_path(parents, data_dir=tmp_path)
+    paths = filter(
+        lambda p: p.is_file(),
+        [tmp_path / parent / "db.sqlite" for parent in parents],
+    )
 
     # Merge all requested parents databases into our target
     merge_parents_cache(paths, mock_databases["target"]["path"])
 
     # The target now should have the expected elements and transcriptions
     with mock_databases["target"]["db"].bind_ctx(MODELS):
         assert CachedImage.select().count() == 0
@@ -124,24 +126,21 @@
         assert CachedTranscription.select().count() == 0
         assert CachedClassification.select().count() == 0
         assert CachedEntity.select().count() == 0
         assert CachedTranscriptionEntity.select().count() == 0
 
     # Check filenames
     assert mock_databases["chunk_42"]["path"].name == "db_42.sqlite"
-    assert mock_databases["second"]["path"].name == "db.sqlite"
+    assert mock_databases["first"]["path"].name == "db.sqlite"
+
+    paths = [
+        tmp_path / "chunk_42" / "db_42.sqlite",
+        tmp_path / "first" / "db.sqlite",
+    ]
 
-    paths = retrieve_parents_cache_path(
-        [
-            "chunk_42",
-            "first",
-        ],
-        data_dir=tmp_path,
-        chunk="42",
-    )
     merge_parents_cache(paths, mock_databases["target"]["path"])
 
     # The target should now have 3 elements and 0 transcription
     with mock_databases["target"]["db"].bind_ctx(MODELS):
         assert CachedImage.select().count() == 0
         assert CachedElement.select().count() == 3
         assert CachedTranscription.select().count() == 0
@@ -217,15 +216,18 @@
         Version.update(version=fake_version).execute()
         assert Version.get() == Version(version=fake_version)
 
     with mock_databases["target"]["db"].bind_ctx([Version]):
         assert Version.get() == Version(version=SQL_VERSION)
 
     # Retrieve parents databases paths
-    paths = retrieve_parents_cache_path(["first", "second"], data_dir=tmp_path)
+    paths = [
+        tmp_path / "first" / "db.sqlite",
+        tmp_path / "second" / "db.sqlite",
+    ]
 
     # Merge all requested parents databases into our target, the "second" parent have a differing version
     with pytest.raises(AssertionError) as e:
         merge_parents_cache(paths, mock_databases["target"]["path"])
 
     assert (
         str(e.value)
```

### Comparing `arkindex-base-worker-0.3.3rc2/tests/test_reporting.py` & `arkindex-base-worker-0.3.3rc3/tests/test_reporting.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc2/tests/test_utils.py` & `arkindex-base-worker-0.3.3rc3/tests/test_utils.py`

 * *Files identical despite different names*

