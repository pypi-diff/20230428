# Comparing `tmp/encord-0.1.73.tar.gz` & `tmp/encord-0.1.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encord-0.1.73.tar", max compression
+gzip compressed data, was "encord-0.1.74.tar", max compression
```

## Comparing `encord-0.1.73.tar` & `encord-0.1.74.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0    11330 2023-04-26 13:30:18.704367 encord-0.1.73/LICENSE
--rw-r--r--   0        0        0     2595 2023-04-26 13:30:18.704367 encord-0.1.73/README.md
--rw-r--r--   0        0        0       84 2023-04-26 13:30:18.704367 encord-0.1.73/cord/__init__.py
--rw-r--r--   0        0        0      158 2023-04-26 13:30:18.720368 encord-0.1.73/encord/__init__.py
--rw-r--r--   0        0        0      214 2023-04-26 13:30:18.720368 encord-0.1.73/encord/_version.py
--rw-r--r--   0        0        0    47245 2023-04-26 13:30:18.720368 encord-0.1.73/encord/client.py
--rw-r--r--   0        0        0    10825 2023-04-26 13:30:18.720368 encord-0.1.73/encord/configs.py
--rw-r--r--   0        0        0        0 2023-04-26 13:30:18.720368 encord-0.1.73/encord/constants/__init__.py
--rw-r--r--   0        0        0      810 2023-04-26 13:30:18.720368 encord-0.1.73/encord/constants/enums.py
--rw-r--r--   0        0        0     3211 2023-04-26 13:30:18.720368 encord-0.1.73/encord/constants/model.py
--rw-r--r--   0        0        0     6068 2023-04-26 13:30:18.720368 encord-0.1.73/encord/constants/model_weights.py
--rw-r--r--   0        0        0     1119 2023-04-26 13:30:18.720368 encord-0.1.73/encord/constants/string_constants.py
--rw-r--r--   0        0        0        0 2023-04-26 13:30:18.720368 encord-0.1.73/encord/constants/test/__init__.py
--rw-r--r--   0        0        0      634 2023-04-26 13:30:18.720368 encord-0.1.73/encord/constants/test/test_enums.py
--rw-r--r--   0        0        0    16035 2023-04-26 13:30:18.720368 encord-0.1.73/encord/dataset.py
--rw-r--r--   0        0        0     5621 2023-04-26 13:30:18.720368 encord-0.1.73/encord/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-26 13:30:18.720368 encord-0.1.73/encord/http/__init__.py
--rw-r--r--   0        0        0      535 2023-04-26 13:30:18.720368 encord-0.1.73/encord/http/constants.py
--rw-r--r--   0        0        0     6275 2023-04-26 13:30:18.720368 encord-0.1.73/encord/http/error_utils.py
--rw-r--r--   0        0        0     5999 2023-04-26 13:30:18.720368 encord-0.1.73/encord/http/querier.py
--rw-r--r--   0        0        0      697 2023-04-26 13:30:18.720368 encord-0.1.73/encord/http/query_methods.py
--rw-r--r--   0        0        0     1691 2023-04-26 13:30:18.720368 encord-0.1.73/encord/http/request.py
--rw-r--r--   0        0        0     5880 2023-04-26 13:30:18.720368 encord-0.1.73/encord/http/utils.py
--rw-r--r--   0        0        0      340 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/__init__.py
--rw-r--r--   0        0        0      145 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/classification.py
--rw-r--r--   0        0        0    29709 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/common.py
--rw-r--r--   0        0        0      172 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/constants.py
--rw-r--r--   0        0        0     5631 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/coordinates.py
--rw-r--r--   0        0        0     3419 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/frames.py
--rw-r--r--   0        0        0    21407 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/internal_helpers.py
--rw-r--r--   0        0        0   132196 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/ontology_labels_impl.py
--rw-r--r--   0        0        0      137 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/ontology_object.py
--rw-r--r--   0        0        0      148 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/ontology_structure.py
--rw-r--r--   0        0        0      549 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/project.py
--rw-r--r--   0        0        0     1240 2023-04-26 13:30:18.720368 encord-0.1.73/encord/objects/utils.py
--rw-r--r--   0        0        0     3430 2023-04-26 13:30:18.720368 encord-0.1.73/encord/ontology.py
--rw-r--r--   0        0        0        0 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/__init__.py
--rw-r--r--   0        0        0      982 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/api_key.py
--rw-r--r--   0        0        0     5377 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/base_orm.py
--rw-r--r--   0        0        0      111 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/cloud_integration.py
--rw-r--r--   0        0        0    32206 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/dataset.py
--rw-r--r--   0        0        0      828 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/dataset_with_user_role.py
--rw-r--r--   0        0        0      201 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/formatter.py
--rw-r--r--   0        0        0     1155 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/label_log.py
--rw-r--r--   0        0        0    11122 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/label_row.py
--rw-r--r--   0        0        0     1577 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/labeling_algorithm.py
--rw-r--r--   0        0        0     6687 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/model.py
--rw-r--r--   0        0        0      745 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/ontology.py
--rw-r--r--   0        0        0     8844 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/project.py
--rw-r--r--   0        0        0      625 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/project_api_key.py
--rw-r--r--   0        0        0      828 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/project_with_user_role.py
--rw-r--r--   0        0        0        0 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/test/__init__.py
--rw-r--r--   0        0        0      570 2023-04-26 13:30:18.720368 encord-0.1.73/encord/orm/test/test_dataset.py
--rw-r--r--   0        0        0    38298 2023-04-26 13:30:18.720368 encord-0.1.73/encord/project.py
--rw-r--r--   0        0        0        0 2023-04-26 13:30:18.720368 encord-0.1.73/encord/project_ontology/__init__.py
--rw-r--r--   0        0        0     1316 2023-04-26 13:30:18.720368 encord-0.1.73/encord/project_ontology/classification_attribute.py
--rw-r--r--   0        0        0      525 2023-04-26 13:30:18.720368 encord-0.1.73/encord/project_ontology/classification_option.py
--rw-r--r--   0        0        0      357 2023-04-26 13:30:18.720368 encord-0.1.73/encord/project_ontology/classification_type.py
--rw-r--r--   0        0        0      237 2023-04-26 13:30:18.724368 encord-0.1.73/encord/project_ontology/object_type.py
--rw-r--r--   0        0        0     9526 2023-04-26 13:30:18.724368 encord-0.1.73/encord/project_ontology/ontology.py
--rw-r--r--   0        0        0      630 2023-04-26 13:30:18.724368 encord-0.1.73/encord/project_ontology/ontology_classification.py
--rw-r--r--   0        0        0      683 2023-04-26 13:30:18.724368 encord-0.1.73/encord/project_ontology/ontology_object.py
--rw-r--r--   0        0        0    27801 2023-04-26 13:30:18.724368 encord-0.1.73/encord/user_client.py
--rw-r--r--   0        0        0        0 2023-04-26 13:30:18.724368 encord-0.1.73/encord/utilities/__init__.py
--rw-r--r--   0        0        0     4231 2023-04-26 13:30:18.724368 encord-0.1.73/encord/utilities/client_utilities.py
--rw-r--r--   0        0        0      253 2023-04-26 13:30:18.724368 encord-0.1.73/encord/utilities/common.py
--rw-r--r--   0        0        0     3270 2023-04-26 13:30:18.724368 encord-0.1.73/encord/utilities/label_utilities.py
--rw-r--r--   0        0        0      343 2023-04-26 13:30:18.724368 encord-0.1.73/encord/utilities/ontology_user.py
--rw-r--r--   0        0        0      578 2023-04-26 13:30:18.724368 encord-0.1.73/encord/utilities/project_user.py
--rw-r--r--   0        0        0      467 2023-04-26 13:30:18.724368 encord-0.1.73/encord/utilities/project_utilities.py
--rw-r--r--   0        0        0     1681 2023-04-26 13:30:18.724368 encord-0.1.73/pyproject.toml
--rw-r--r--   0        0        0     3724 2023-04-26 13:31:35.974219 encord-0.1.73/setup.py
--rw-r--r--   0        0        0     3726 2023-04-26 13:31:35.974603 encord-0.1.73/PKG-INFO
+-rw-r--r--   0        0        0    11330 2023-04-28 14:21:09.197584 encord-0.1.74/LICENSE
+-rw-r--r--   0        0        0     2595 2023-04-28 14:21:09.197584 encord-0.1.74/README.md
+-rw-r--r--   0        0        0       84 2023-04-28 14:21:09.197584 encord-0.1.74/cord/__init__.py
+-rw-r--r--   0        0        0      158 2023-04-28 14:21:09.213585 encord-0.1.74/encord/__init__.py
+-rw-r--r--   0        0        0      214 2023-04-28 14:21:09.213585 encord-0.1.74/encord/_version.py
+-rw-r--r--   0        0        0    47245 2023-04-28 14:21:09.213585 encord-0.1.74/encord/client.py
+-rw-r--r--   0        0        0    10825 2023-04-28 14:21:09.213585 encord-0.1.74/encord/configs.py
+-rw-r--r--   0        0        0        0 2023-04-28 14:21:09.213585 encord-0.1.74/encord/constants/__init__.py
+-rw-r--r--   0        0        0      810 2023-04-28 14:21:09.213585 encord-0.1.74/encord/constants/enums.py
+-rw-r--r--   0        0        0     3211 2023-04-28 14:21:09.213585 encord-0.1.74/encord/constants/model.py
+-rw-r--r--   0        0        0     6068 2023-04-28 14:21:09.213585 encord-0.1.74/encord/constants/model_weights.py
+-rw-r--r--   0        0        0     1119 2023-04-28 14:21:09.213585 encord-0.1.74/encord/constants/string_constants.py
+-rw-r--r--   0        0        0        0 2023-04-28 14:21:09.213585 encord-0.1.74/encord/constants/test/__init__.py
+-rw-r--r--   0        0        0      634 2023-04-28 14:21:09.213585 encord-0.1.74/encord/constants/test/test_enums.py
+-rw-r--r--   0        0        0    16035 2023-04-28 14:21:09.213585 encord-0.1.74/encord/dataset.py
+-rw-r--r--   0        0        0     5621 2023-04-28 14:21:09.213585 encord-0.1.74/encord/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-28 14:21:09.213585 encord-0.1.74/encord/http/__init__.py
+-rw-r--r--   0        0        0      535 2023-04-28 14:21:09.213585 encord-0.1.74/encord/http/constants.py
+-rw-r--r--   0        0        0     6275 2023-04-28 14:21:09.213585 encord-0.1.74/encord/http/error_utils.py
+-rw-r--r--   0        0        0     5999 2023-04-28 14:21:09.213585 encord-0.1.74/encord/http/querier.py
+-rw-r--r--   0        0        0      697 2023-04-28 14:21:09.213585 encord-0.1.74/encord/http/query_methods.py
+-rw-r--r--   0        0        0     1691 2023-04-28 14:21:09.213585 encord-0.1.74/encord/http/request.py
+-rw-r--r--   0        0        0     5880 2023-04-28 14:21:09.213585 encord-0.1.74/encord/http/utils.py
+-rw-r--r--   0        0        0      340 2023-04-28 14:21:09.213585 encord-0.1.74/encord/objects/__init__.py
+-rw-r--r--   0        0        0      145 2023-04-28 14:21:09.213585 encord-0.1.74/encord/objects/classification.py
+-rw-r--r--   0        0        0    29709 2023-04-28 14:21:09.213585 encord-0.1.74/encord/objects/common.py
+-rw-r--r--   0        0        0      172 2023-04-28 14:21:09.213585 encord-0.1.74/encord/objects/constants.py
+-rw-r--r--   0        0        0     5631 2023-04-28 14:21:09.213585 encord-0.1.74/encord/objects/coordinates.py
+-rw-r--r--   0        0        0     3419 2023-04-28 14:21:09.213585 encord-0.1.74/encord/objects/frames.py
+-rw-r--r--   0        0        0    21407 2023-04-28 14:21:09.217585 encord-0.1.74/encord/objects/internal_helpers.py
+-rw-r--r--   0        0        0   132977 2023-04-28 14:21:09.217585 encord-0.1.74/encord/objects/ontology_labels_impl.py
+-rw-r--r--   0        0        0      137 2023-04-28 14:21:09.217585 encord-0.1.74/encord/objects/ontology_object.py
+-rw-r--r--   0        0        0      148 2023-04-28 14:21:09.217585 encord-0.1.74/encord/objects/ontology_structure.py
+-rw-r--r--   0        0        0      549 2023-04-28 14:21:09.217585 encord-0.1.74/encord/objects/project.py
+-rw-r--r--   0        0        0     1240 2023-04-28 14:21:09.217585 encord-0.1.74/encord/objects/utils.py
+-rw-r--r--   0        0        0     3430 2023-04-28 14:21:09.217585 encord-0.1.74/encord/ontology.py
+-rw-r--r--   0        0        0        0 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/__init__.py
+-rw-r--r--   0        0        0      982 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/api_key.py
+-rw-r--r--   0        0        0     5377 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/base_orm.py
+-rw-r--r--   0        0        0      111 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/cloud_integration.py
+-rw-r--r--   0        0        0    32206 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/dataset.py
+-rw-r--r--   0        0        0      828 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/dataset_with_user_role.py
+-rw-r--r--   0        0        0      201 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/formatter.py
+-rw-r--r--   0        0        0     1155 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/label_log.py
+-rw-r--r--   0        0        0    11122 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/label_row.py
+-rw-r--r--   0        0        0     1577 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/labeling_algorithm.py
+-rw-r--r--   0        0        0     6687 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/model.py
+-rw-r--r--   0        0        0      745 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/ontology.py
+-rw-r--r--   0        0        0     8844 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/project.py
+-rw-r--r--   0        0        0      625 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/project_api_key.py
+-rw-r--r--   0        0        0      828 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/project_with_user_role.py
+-rw-r--r--   0        0        0        0 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/test/__init__.py
+-rw-r--r--   0        0        0      570 2023-04-28 14:21:09.217585 encord-0.1.74/encord/orm/test/test_dataset.py
+-rw-r--r--   0        0        0    38298 2023-04-28 14:21:09.217585 encord-0.1.74/encord/project.py
+-rw-r--r--   0        0        0        0 2023-04-28 14:21:09.217585 encord-0.1.74/encord/project_ontology/__init__.py
+-rw-r--r--   0        0        0     1316 2023-04-28 14:21:09.217585 encord-0.1.74/encord/project_ontology/classification_attribute.py
+-rw-r--r--   0        0        0      525 2023-04-28 14:21:09.217585 encord-0.1.74/encord/project_ontology/classification_option.py
+-rw-r--r--   0        0        0      357 2023-04-28 14:21:09.217585 encord-0.1.74/encord/project_ontology/classification_type.py
+-rw-r--r--   0        0        0      237 2023-04-28 14:21:09.217585 encord-0.1.74/encord/project_ontology/object_type.py
+-rw-r--r--   0        0        0     9526 2023-04-28 14:21:09.217585 encord-0.1.74/encord/project_ontology/ontology.py
+-rw-r--r--   0        0        0      630 2023-04-28 14:21:09.217585 encord-0.1.74/encord/project_ontology/ontology_classification.py
+-rw-r--r--   0        0        0      683 2023-04-28 14:21:09.217585 encord-0.1.74/encord/project_ontology/ontology_object.py
+-rw-r--r--   0        0        0    27801 2023-04-28 14:21:09.217585 encord-0.1.74/encord/user_client.py
+-rw-r--r--   0        0        0        0 2023-04-28 14:21:09.217585 encord-0.1.74/encord/utilities/__init__.py
+-rw-r--r--   0        0        0     4231 2023-04-28 14:21:09.217585 encord-0.1.74/encord/utilities/client_utilities.py
+-rw-r--r--   0        0        0      253 2023-04-28 14:21:09.217585 encord-0.1.74/encord/utilities/common.py
+-rw-r--r--   0        0        0     3270 2023-04-28 14:21:09.217585 encord-0.1.74/encord/utilities/label_utilities.py
+-rw-r--r--   0        0        0      343 2023-04-28 14:21:09.217585 encord-0.1.74/encord/utilities/ontology_user.py
+-rw-r--r--   0        0        0      578 2023-04-28 14:21:09.217585 encord-0.1.74/encord/utilities/project_user.py
+-rw-r--r--   0        0        0      467 2023-04-28 14:21:09.217585 encord-0.1.74/encord/utilities/project_utilities.py
+-rw-r--r--   0        0        0     1659 2023-04-28 14:21:09.217585 encord-0.1.74/pyproject.toml
+-rw-r--r--   0        0        0     3728 1970-01-01 00:00:00.000000 encord-0.1.74/setup.py
+-rw-r--r--   0        0        0     3774 1970-01-01 00:00:00.000000 encord-0.1.74/PKG-INFO
```

### Comparing `encord-0.1.73/LICENSE` & `encord-0.1.74/LICENSE`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/README.md` & `encord-0.1.74/README.md`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/client.py` & `encord-0.1.74/encord/client.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/configs.py` & `encord-0.1.74/encord/configs.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/constants/enums.py` & `encord-0.1.74/encord/constants/enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/constants/model.py` & `encord-0.1.74/encord/constants/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/constants/model_weights.py` & `encord-0.1.74/encord/constants/model_weights.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/constants/string_constants.py` & `encord-0.1.74/encord/constants/string_constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/constants/test/test_enums.py` & `encord-0.1.74/encord/constants/test/test_enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/dataset.py` & `encord-0.1.74/encord/dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/exceptions.py` & `encord-0.1.74/encord/exceptions.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/http/constants.py` & `encord-0.1.74/encord/http/constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/http/error_utils.py` & `encord-0.1.74/encord/http/error_utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/http/querier.py` & `encord-0.1.74/encord/http/querier.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/http/query_methods.py` & `encord-0.1.74/encord/http/query_methods.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/http/request.py` & `encord-0.1.74/encord/http/request.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/http/utils.py` & `encord-0.1.74/encord/http/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/objects/common.py` & `encord-0.1.74/encord/objects/common.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/objects/coordinates.py` & `encord-0.1.74/encord/objects/coordinates.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/objects/frames.py` & `encord-0.1.74/encord/objects/frames.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/objects/internal_helpers.py` & `encord-0.1.74/encord/objects/internal_helpers.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/objects/ontology_labels_impl.py` & `encord-0.1.74/encord/objects/ontology_labels_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,19 +399,19 @@
         return self._parent is not None
 
     def set_for_frames(
         self,
         frames: Frames = 0,
         *,
         overwrite: bool = False,
-        created_at: datetime = datetime.now(),
+        created_at: Optional[datetime] = None,
         created_by: str = None,
         confidence: int = DEFAULT_CONFIDENCE,
         manual_annotation: bool = DEFAULT_MANUAL_ANNOTATION,
-        last_edited_at: datetime = datetime.now(),
+        last_edited_at: Optional[datetime] = None,
         last_edited_by: Optional[str] = None,
         reviews: Optional[List[dict]] = None,
     ) -> None:
         """
         Places the classification onto the specified frame. If the classification already exists on the frame and
         overwrite is set to `True`, the currently specified values will be overwritten.
 
@@ -434,14 +434,20 @@
             confidence:
                 Optionally specify the confidence of the classification instance on this frame. Defaults to `1.0`.
             manual_annotation:
                 Optionally specify whether the classification instance on this frame was manually annotated. Defaults to `True`.
             reviews:
                 Should only be set by internal functions.
         """
+        if created_at is None:
+            created_at = datetime.now()
+
+        if last_edited_at is None:
+            last_edited_at = datetime.now()
+
         frames_list = frames_class_to_frames_list(frames)
 
         self._check_classification_already_present(frames_list)
 
         for frame in frames_list:
             self._check_within_range(frame)
             self._set_frame_and_frame_data(
@@ -452,14 +458,18 @@
                 confidence=confidence,
                 manual_annotation=manual_annotation,
                 last_edited_at=last_edited_at,
                 last_edited_by=last_edited_by,
                 reviews=reviews,
             )
 
+        if self.is_assigned_to_label_row():
+            self._parent._add_frames_to_classification(self.ontology_item, frames_list)
+            self._parent._add_to_frame_to_hashes_map(self)
+
     def get_annotation(self, frame: Union[int, str] = 0) -> Annotation:
         """
         Args:
             frame: Either the frame number or the image hash if the data type is an image or image group.
                 Defaults to the first frame.
         """
         if isinstance(frame, str):
@@ -719,19 +729,19 @@
                 )
 
         def _get_object_frame_instance_data(self) -> ClassificationInstance.FrameData:
             return self._classification_instance._frames_to_data[self._frame]
 
     @dataclass
     class FrameData:
-        created_at: datetime = datetime.now()
+        created_at: datetime = field(default_factory=datetime.now)
         created_by: Optional[str] = None
         confidence: int = DEFAULT_CONFIDENCE
         manual_annotation: bool = DEFAULT_MANUAL_ANNOTATION
-        last_edited_at: datetime = datetime.now()
+        last_edited_at: datetime = field(default_factory=datetime.now)
         last_edited_by: Optional[str] = None
         reviews: Optional[List[dict]] = None
 
         @staticmethod
         def from_dict(d: dict) -> ClassificationInstance.FrameData:
             if "lastEditedAt" in d:
                 last_edited_at = parse(d["lastEditedAt"])
@@ -1428,21 +1438,27 @@
                 self._label_row.add_object_instance(object_instance)
 
         def add_classification_instance(
             self,
             classification_instance: ClassificationInstance,
             *,
             overwrite: bool = False,
-            created_at: datetime = datetime.now(),
+            created_at: Optional[datetime] = None,
             created_by: str = None,
             confidence: int = DEFAULT_CONFIDENCE,
             manual_annotation: bool = DEFAULT_MANUAL_ANNOTATION,
-            last_edited_at: datetime = datetime.now(),
+            last_edited_at: Optional[datetime] = None,
             last_edited_by: Optional[str] = None,
         ) -> None:
+            if created_at is None:
+                created_at = datetime.now()
+
+            if last_edited_at is None:
+                last_edited_at = datetime.now()
+
             label_row = classification_instance.is_assigned_to_label_row()
             if label_row and self._label_row != label_row:
                 raise LabelRowError(
                     "This object instance is already assigned to a different label row. It can not be "
                     "added to multiple label rows at once."
                 )
 
@@ -1749,14 +1765,17 @@
     ) -> Optional[int]:
         present_frames = self._classifications_to_frames.get(classification, set())
         for frame in frames:
             if frame in present_frames:
                 return frame
         return None
 
+    def _add_frames_to_classification(self, classification: Classification, frames: Iterable[int]) -> None:
+        self._classifications_to_frames[classification].update(set(frames))
+
     def _remove_frames_from_classification(self, classification: Classification, frames: Iterable[int]) -> None:
         present_frames = self._classifications_to_frames.get(classification, set())
         for frame in frames:
             present_frames.remove(frame)
 
     def _add_to_frame_to_hashes_map(self, label_item: Union[ObjectInstance, ClassificationInstance]) -> None:
         """This can be called by the ObjectInstance."""
@@ -2469,18 +2488,18 @@
             if self._frame not in self._object_instance._frames_to_instance_data:
                 raise LabelRowError(
                     "Tryinannotation to use an ObjectInstance.Annotation for an ObjectInstance that is not on the frameAnnotation"
                 )
 
     @dataclass
     class FrameInfo:
-        created_at: datetime = datetime.now()
+        created_at: datetime = field(default_factory=datetime.now)
         created_by: Optional[str] = None
         """None defaults to the user of the SDK once uploaded to the server."""
-        last_edited_at: datetime = datetime.now()
+        last_edited_at: datetime = field(default_factory=datetime.now)
         last_edited_by: Optional[str] = None
         """None defaults to the user of the SDK once uploaded to the server."""
         confidence: float = DEFAULT_CONFIDENCE
         manual_annotation: bool = DEFAULT_MANUAL_ANNOTATION
         reviews: Optional[List[dict]] = None
         is_deleted: Optional[bool] = None
```

### Comparing `encord-0.1.73/encord/objects/project.py` & `encord-0.1.74/encord/objects/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/objects/utils.py` & `encord-0.1.74/encord/objects/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/ontology.py` & `encord-0.1.74/encord/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/orm/api_key.py` & `encord-0.1.74/encord/orm/api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/orm/base_orm.py` & `encord-0.1.74/encord/orm/base_orm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/orm/dataset.py` & `encord-0.1.74/encord/orm/dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/orm/dataset_with_user_role.py` & `encord-0.1.74/encord/orm/dataset_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/orm/label_log.py` & `encord-0.1.74/encord/orm/label_log.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/orm/label_row.py` & `encord-0.1.74/encord/orm/label_row.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/orm/labeling_algorithm.py` & `encord-0.1.74/encord/orm/labeling_algorithm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/orm/model.py` & `encord-0.1.74/encord/orm/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/orm/ontology.py` & `encord-0.1.74/encord/orm/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/orm/project.py` & `encord-0.1.74/encord/orm/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/orm/project_api_key.py` & `encord-0.1.74/encord/orm/project_api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/orm/project_with_user_role.py` & `encord-0.1.74/encord/orm/project_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/orm/test/test_dataset.py` & `encord-0.1.74/encord/orm/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/project.py` & `encord-0.1.74/encord/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/project_ontology/classification_attribute.py` & `encord-0.1.74/encord/project_ontology/classification_attribute.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/project_ontology/classification_option.py` & `encord-0.1.74/encord/project_ontology/classification_option.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/project_ontology/ontology.py` & `encord-0.1.74/encord/project_ontology/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/project_ontology/ontology_classification.py` & `encord-0.1.74/encord/project_ontology/ontology_classification.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/project_ontology/ontology_object.py` & `encord-0.1.74/encord/project_ontology/ontology_object.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/user_client.py` & `encord-0.1.74/encord/user_client.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/utilities/client_utilities.py` & `encord-0.1.74/encord/utilities/client_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/utilities/label_utilities.py` & `encord-0.1.74/encord/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/encord/utilities/project_user.py` & `encord-0.1.74/encord/utilities/project_user.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.73/pyproject.toml` & `encord-0.1.74/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encord"
-version = "0.1.73"
+version = "0.1.74"
 description = "Encord Python SDK Client"
 authors = ["Cord Technologies Limited <hello@encord.com>"]
 license = "Apache Software License"
 keywords = ["cord", "encord"]
 packages = [
     { include = "cord"},
     { include = "encord"},
@@ -36,15 +36,14 @@
 sphinx-copybutton = "^0.5.0"
 sphinx-toolbox = "^3.4.0"
 prettyprinter = "0.18.0"
 isort = "^5.10.1"
 pydata-sphinx-theme = "^0.8.1"
 Pillow = "^9.1.0"
 sphinx-gallery = "^0.10.1"
-matplotlib = "^3.5.2"
 deepdiff = "^6.2.1"
 
 
 [build-system]
 requires = ["poetry-core>=1.3.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `encord-0.1.73/setup.py` & `encord-0.1.74/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,21 +23,21 @@
  'tqdm>=4.32.1,<5.0.0']
 
 extras_require = \
 {':python_version < "3.8"': ['importlib_metadata>=6.1.0,<7.0.0']}
 
 setup_kwargs = {
     'name': 'encord',
-    'version': '0.1.73',
+    'version': '0.1.74',
     'description': 'Encord Python SDK Client',
     'long_description': '<h1 align="center">\n  <p align="center">Encord Python API Client</p>\n  <a href="https://encord.com"><img src="./docs/_static/logo.svg" width="100" alt="Cord logo"/></a>\n</h1>\n\n[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n\n***The data engine for computer vision***\n\n## 💻 Features\n\n- Minimal low-level Python client that allows you to interact with Encord\'s API\n- Supports Python: `3.7`, `3.8`, `3.9`, and `3.10`\n\n## ✨ Relevant Links\n* [Encord website](https://encord.com)\n* [Encord web app](https://app.encord.com)\n* [Encord documentation](https://docs.encord.com)\n\n## 💡 Getting Started\n\nFor full documentation, please visit [Encord Python SDK](https://python.docs.encord.com/).\n\nFirst, install Encord Python API Client using the [pip](https://pip.pypa.io/en/stable/installing) package manager:\n\n```bash\npip install encord\n```\n\nThen, create an API key for authentication via the [Encord web app](https://app.encord.com). Pass the resource ID and API key as environment variables or pass them explicitly when you initialise the EncordClient object.\n\n```bash\nexport ENCORD_PROJECT_ID="<project_id>"\nexport ENCORD_API_KEY="<project_api_key>"\n```\n\nPassing the resource ID and API key as environment variables, you can initialise the Encord client directly.\n\n```python\nfrom encord.client import EncordClient\n\nclient = EncordClient.initialise()\n```\n\nIf you want to avoid setting environment variables, you can initialise the Encord client by passing the resource ID and API key as strings.\n\n```python\nfrom encord.client import EncordClient\n\nclient = EncordClient.initialise("<resource_id>", "<resource_api_key>")\n```\n\nIf you wish to instantiate several client objects and avoid passing parameters each time, you can instantiate a EncordConfig object, pass the resource ID and API key as strings, and initialise the client with the config object.\n\n```py\nfrom encord.client import EncordClient\nfrom encord.client import EncordConfig\n\nconfig = EncordConfig("<resource_id>", "<resource_api_key>")\nclient = EncordClient.initialise_with_config(config)\n```\n\nOnce you have instantiated an Encord client, it is easy to fetch information associated with the given resource ID.\n\n```py\nfrom encord.client import EncordClient\n\nclient = EncordClient.initialise()\nproject = client.get_project()\n```\n\n## 🐛 Troubleshooting\n\nPlease report bugs to [GitHub Issues](https://github.com/encord-team/encord-client-python/issues). Just make sure you read the [Encord documentation](https://docs.encord.com) and search for related issues first.\n',
     'author': 'Cord Technologies Limited',
     'author_email': 'hello@encord.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/encord-team/encord-client-python',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'python_requires': '>=3.7,<4.0',
 }
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['cord',
 'encord', 'encord.constants', 'encord.constants.test', 'encord.http',
 'encord.objects', 'encord.orm', 'encord.orm.test', 'encord.project_ontology',
 'encord.utilities'] package_data = \ {'': ['*']} install_requires = \
 ['cryptography>=3.4.8,<4.0.0', 'python-dateutil>=2.8.2,<3.0.0',
 'requests>=2.25.0,<3.0.0', 'tqdm>=4.32.1,<5.0.0'] extras_require = \ {':
 python_version < "3.8"': ['importlib_metadata>=6.1.0,<7.0.0']} setup_kwargs =
-{ 'name': 'encord', 'version': '0.1.73', 'description': 'Encord Python SDK
+{ 'name': 'encord', 'version': '0.1.74', 'description': 'Encord Python SDK
 Client', 'long_description': '
            ****** \nEncord Python API Client\n [Cord_logo]\n ******
 \n\n[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)]
 (https://opensource.org/licenses/Apache-2.0)\n\n***The data engine for computer
 vision***\n\n## ð» Features\n\n- Minimal low-level Python client that allows
 you to interact with Encord\'s API\n- Supports Python: `3.7`, `3.8`, `3.9`, and
 `3.10`\n\n## â¨ Relevant Links\n* [Encord website](https://encord.com)\n*
@@ -37,12 +37,12 @@
 (config)\n```\n\nOnce you have instantiated an Encord client, it is easy to
 fetch information associated with the given resource ID.\n\n```py\nfrom
 encord.client import EncordClient\n\nclient = EncordClient.initialise
 ()\nproject = client.get_project()\n```\n\n## ð Troubleshooting\n\nPlease
 report bugs to [GitHub Issues](https://github.com/encord-team/encord-client-
 python/issues). Just make sure you read the [Encord documentation](https://
 docs.encord.com) and search for related issues first.\n', 'author': 'Cord
-Technologies Limited', 'author_email': 'hello@encord.com', 'maintainer': None,
-'maintainer_email': None, 'url': 'https://github.com/encord-team/encord-client-
-python', 'packages': packages, 'package_data': package_data,
+Technologies Limited', 'author_email': 'hello@encord.com', 'maintainer':
+'None', 'maintainer_email': 'None', 'url': 'https://github.com/encord-team/
+encord-client-python', 'packages': packages, 'package_data': package_data,
 'install_requires': install_requires, 'extras_require': extras_require,
 'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
```

### Comparing `encord-0.1.73/PKG-INFO` & `encord-0.1.74/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: encord
-Version: 0.1.73
+Version: 0.1.74
 Summary: Encord Python SDK Client
 Home-page: https://github.com/encord-team/encord-client-python
 License: Apache Software License
 Keywords: cord,encord
 Author: Cord Technologies Limited
 Author-email: hello@encord.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3
 Requires-Dist: cryptography (>=3.4.8,<4.0.0)
 Requires-Dist: importlib_metadata (>=6.1.0,<7.0.0); python_version < "3.8"
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.25.0,<3.0.0)
 Requires-Dist: tqdm (>=4.32.1,<5.0.0)
 Project-URL: Documentation, https://python.docs.encord.com/
 Project-URL: Repository, https://github.com/encord-team/encord-client-python
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: encord Version: 0.1.73 Summary: Encord Python SDK
+Metadata-Version: 2.1 Name: encord Version: 0.1.74 Summary: Encord Python SDK
 Client Home-page: https://github.com/encord-team/encord-client-python License:
 Apache Software License Keywords: cord,encord Author: Cord Technologies Limited
 Author-email: hello@encord.com Requires-Python: >=3.7,<4.0 Classifier: License
 :: OSI Approved :: Apache Software License Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Requires-Dist: cryptography (>=3.4.8,<4.0.0) Requires-Dist:
-importlib_metadata (>=6.1.0,<7.0.0); python_version < "3.8" Requires-Dist:
-python-dateutil (>=2.8.2,<3.0.0) Requires-Dist: requests (>=2.25.0,<3.0.0)
-Requires-Dist: tqdm (>=4.32.1,<5.0.0) Project-URL: Documentation, https://
-python.docs.encord.com/ Project-URL: Repository, https://github.com/encord-
-team/encord-client-python Description-Content-Type: text/markdown
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3 Requires-Dist:
+cryptography (>=3.4.8,<4.0.0) Requires-Dist: importlib_metadata
+(>=6.1.0,<7.0.0); python_version < "3.8" Requires-Dist: python-dateutil
+(>=2.8.2,<3.0.0) Requires-Dist: requests (>=2.25.0,<3.0.0) Requires-Dist: tqdm
+(>=4.32.1,<5.0.0) Project-URL: Documentation, https://python.docs.encord.com/
+Project-URL: Repository, https://github.com/encord-team/encord-client-python
+Description-Content-Type: text/markdown
                ****** Encord Python API Client[Cord_logo] ******
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https:
 //opensource.org/licenses/Apache-2.0) ***The data engine for computer vision***
 ## ð» Features - Minimal low-level Python client that allows you to interact
 with Encord's API - Supports Python: `3.7`, `3.8`, `3.9`, and `3.10` ## â¨
 Relevant Links * [Encord website](https://encord.com) * [Encord web app](https:
 //app.encord.com) * [Encord documentation](https://docs.encord.com) ## ð¡
```

