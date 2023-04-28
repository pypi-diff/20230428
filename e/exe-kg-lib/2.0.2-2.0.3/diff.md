# Comparing `tmp/exe_kg_lib-2.0.2.tar.gz` & `tmp/exe_kg_lib-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exe_kg_lib-2.0.2.tar", max compression
+gzip compressed data, was "exe_kg_lib-2.0.3.tar", max compression
```

## Comparing `exe_kg_lib-2.0.2.tar` & `exe_kg_lib-2.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       28 2023-03-08 10:20:37.754368 exe_kg_lib-2.0.2/exe_kg_lib/__init__.py
--rw-r--r--   0        0        0      106 2023-03-01 22:09:32.028451 exe_kg_lib-2.0.2/exe_kg_lib/classes/__init__.py
--rw-r--r--   0        0        0     1283 2023-03-01 22:09:32.030452 exe_kg_lib-2.0.2/exe_kg_lib/classes/data_entity.py
--rw-r--r--   0        0        0      816 2023-04-28 15:47:33.489509 exe_kg_lib-2.0.2/exe_kg_lib/classes/entity.py
--rw-r--r--   0        0        0    32418 2023-04-28 15:47:33.498941 exe_kg_lib-2.0.2/exe_kg_lib/classes/exe_kg.py
--rw-r--r--   0        0        0      797 2023-03-01 22:09:32.037458 exe_kg_lib-2.0.2/exe_kg_lib/classes/kg_schema.py
--rw-r--r--   0        0        0     3621 2023-03-01 22:09:32.038459 exe_kg_lib-2.0.2/exe_kg_lib/classes/task.py
--rw-r--r--   0        0        0        0 2023-03-01 22:09:32.044470 exe_kg_lib-2.0.2/exe_kg_lib/classes/tasks/__init__.py
--rw-r--r--   0        0        0     5758 2023-03-08 10:20:37.803377 exe_kg_lib-2.0.2/exe_kg_lib/classes/tasks/ml_tasks.py
--rw-r--r--   0        0        0     1957 2023-03-01 22:09:32.042465 exe_kg_lib-2.0.2/exe_kg_lib/classes/tasks/README.md
--rw-r--r--   0        0        0     2013 2023-03-08 10:20:37.812380 exe_kg_lib-2.0.2/exe_kg_lib/classes/tasks/statistic_tasks.py
--rw-r--r--   0        0        0     3204 2023-03-08 10:20:37.819384 exe_kg_lib-2.0.2/exe_kg_lib/classes/tasks/visual_tasks.py
--rw-r--r--   0        0        0        0 2023-03-03 15:57:35.720305 exe_kg_lib-2.0.2/exe_kg_lib/cli/__init__.py
--rw-r--r--   0        0        0      979 2023-04-28 15:47:33.504161 exe_kg_lib-2.0.2/exe_kg_lib/cli/main.py
--rw-r--r--   0        0        0      112 2023-03-01 22:09:32.063494 exe_kg_lib-2.0.2/exe_kg_lib/utils/__init__.py
--rw-r--r--   0        0        0     3220 2023-03-08 10:20:37.835382 exe_kg_lib-2.0.2/exe_kg_lib/utils/cli_utils.py
--rw-r--r--   0        0        0     7510 2023-04-28 15:47:33.509156 exe_kg_lib-2.0.2/exe_kg_lib/utils/kg_creation_utils.py
--rw-r--r--   0        0        0     6443 2023-03-08 10:20:37.853392 exe_kg_lib-2.0.2/exe_kg_lib/utils/query_utils.py
--rw-r--r--   0        0        0      708 2023-03-01 22:09:32.070503 exe_kg_lib-2.0.2/exe_kg_lib/utils/string_utils.py
--rw-r--r--   0        0        0        0 2023-03-01 22:09:32.073014 exe_kg_lib-2.0.2/exe_kg_lib/utils/task_utils/__init__.py
--rw-r--r--   0        0        0     2757 2023-03-01 22:09:32.076009 exe_kg_lib-2.0.2/exe_kg_lib/utils/task_utils/ml_utils.py
--rw-r--r--   0        0        0     2689 2023-03-01 22:09:32.078020 exe_kg_lib-2.0.2/exe_kg_lib/utils/task_utils/statistic_utils.py
--rw-r--r--   0        0        0     2480 2023-03-01 22:09:32.080018 exe_kg_lib-2.0.2/exe_kg_lib/utils/task_utils/visual_utils.py
--rw-r--r--   0        0        0    34943 2023-03-01 22:09:31.953791 exe_kg_lib-2.0.2/LICENSE.md
--rw-r--r--   0        0        0     3773 2023-04-28 15:55:11.800195 exe_kg_lib-2.0.2/pyproject.toml
--rw-r--r--   0        0        0    15858 2023-04-28 15:47:33.428964 exe_kg_lib-2.0.2/README.md
--rw-r--r--   0        0        0    17179 1970-01-01 00:00:00.000000 exe_kg_lib-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0    34283 2023-04-28 16:15:11.562069 exe_kg_lib-2.0.3/LICENSE.md
+-rw-r--r--   0        0        0    15731 2023-04-28 16:15:11.562069 exe_kg_lib-2.0.3/README.md
+-rw-r--r--   0        0        0       27 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/__init__.py
+-rw-r--r--   0        0        0      102 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/classes/__init__.py
+-rw-r--r--   0        0        0     1253 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/classes/data_entity.py
+-rw-r--r--   0        0        0      788 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/classes/entity.py
+-rw-r--r--   0        0        0    31697 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/classes/exe_kg.py
+-rw-r--r--   0        0        0      773 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/classes/kg_schema.py
+-rw-r--r--   0        0        0     3528 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/classes/task.py
+-rw-r--r--   0        0        0     1914 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/classes/tasks/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/classes/tasks/__init__.py
+-rw-r--r--   0        0        0     5619 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/classes/tasks/ml_tasks.py
+-rw-r--r--   0        0        0     1967 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/classes/tasks/statistic_tasks.py
+-rw-r--r--   0        0        0     3108 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/classes/tasks/visual_tasks.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/cli/__init__.py
+-rw-r--r--   0        0        0      938 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/cli/main.py
+-rw-r--r--   0        0        0      108 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/utils/__init__.py
+-rw-r--r--   0        0        0     3130 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/utils/cli_utils.py
+-rw-r--r--   0        0        0     7290 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/utils/kg_creation_utils.py
+-rw-r--r--   0        0        0     6250 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/utils/query_utils.py
+-rw-r--r--   0        0        0      679 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/utils/string_utils.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/utils/task_utils/__init__.py
+-rw-r--r--   0        0        0     2660 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/utils/task_utils/ml_utils.py
+-rw-r--r--   0        0        0     2606 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/utils/task_utils/statistic_utils.py
+-rw-r--r--   0        0        0     2388 2023-04-28 16:15:11.566069 exe_kg_lib-2.0.3/exe_kg_lib/utils/task_utils/visual_utils.py
+-rw-r--r--   0        0        0     3645 2023-04-28 16:15:36.235572 exe_kg_lib-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0    17179 1970-01-01 00:00:00.000000 exe_kg_lib-2.0.3/PKG-INFO
```

### Comparing `exe_kg_lib-2.0.2/exe_kg_lib/classes/data_entity.py` & `exe_kg_lib-2.0.3/exe_kg_lib/classes/data_entity.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Copyright (c) 2022 Robert Bosch GmbH
-# SPDX-License-Identifier: AGPL-3.0
-
-from .entity import Entity
-
-
-class DataEntity(Entity):
-    """
-    Abstraction of owl:class DataEntity.
-
-    ❗ Important for contributors ❗
-    The fields that contain "_" are by convention the snake-case conversions of the equivalent camel-case property names in the KG.
-    e.g. has_source field corresponds to hasSource property in the KG.
-    This is necessary for automatically mapping KG properties to Python object fields while parsing the KG.
-    """
-
-    def __init__(
-        self,
-        iri: str,
-        parent_entity: Entity,
-        has_source_value: str = None,
-        has_data_semantics_iri: str = None,
-        has_data_structure_iri: str = None,
-        has_reference: str = None,
-    ):
-        super().__init__(iri, parent_entity)
-        self.has_source = has_source_value  # used as column name to retrieve data from the pipeline's input file
-        self.has_data_semantics = has_data_semantics_iri  # IRI of KG entity of type DataSemantics
-        self.has_data_structure = has_data_structure_iri  # IRI of KG entity of type DataStructure
-        self.has_reference = has_reference  # reference to another data entity in the KG, expecting an IRI
+# Copyright (c) 2022 Robert Bosch GmbH
+# SPDX-License-Identifier: AGPL-3.0
+
+from .entity import Entity
+
+
+class DataEntity(Entity):
+    """
+    Abstraction of owl:class DataEntity.
+
+    ❗ Important for contributors ❗
+    The fields that contain "_" are by convention the snake-case conversions of the equivalent camel-case property names in the KG.
+    e.g. has_source field corresponds to hasSource property in the KG.
+    This is necessary for automatically mapping KG properties to Python object fields while parsing the KG.
+    """
+
+    def __init__(
+        self,
+        iri: str,
+        parent_entity: Entity,
+        has_source_value: str = None,
+        has_data_semantics_iri: str = None,
+        has_data_structure_iri: str = None,
+        has_reference: str = None,
+    ):
+        super().__init__(iri, parent_entity)
+        self.has_source = has_source_value  # used as column name to retrieve data from the pipeline's input file
+        self.has_data_semantics = has_data_semantics_iri  # IRI of KG entity of type DataSemantics
+        self.has_data_structure = has_data_structure_iri  # IRI of KG entity of type DataStructure
+        self.has_reference = has_reference  # reference to another data entity in the KG, expecting an IRI
```

### Comparing `exe_kg_lib-2.0.2/exe_kg_lib/classes/exe_kg.py` & `exe_kg_lib-2.0.3/exe_kg_lib/classes/exe_kg.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,721 +1,721 @@
-# Copyright (c) 2022 Robert Bosch GmbH
-# SPDX-License-Identifier: AGPL-3.0
-
-import os
-from typing import Dict, Union
-
-import pandas as pd
-from rdflib import Literal
-
-from ..utils.cli_utils import (get_input_for_existing_data_entities,
-                               get_input_for_new_data_entities)
-from ..utils.kg_creation_utils import (add_and_attach_data_entity,
-                                       add_data_entity_instance,
-                                       add_instance_from_parent_with_relation,
-                                       add_literal, create_pipeline_task,
-                                       name_instance)
-from ..utils.query_utils import *
-from ..utils.query_utils import (
-    get_data_properties_plus_inherited_by_class_iri, get_method_by_task_iri,
-    get_pipeline_and_first_task_iri)
-from ..utils.string_utils import property_name_to_field_name
-from .data_entity import DataEntity
-from .entity import Entity
-from .kg_schema import KGSchema
-from .task import Task
-from .tasks import ml_tasks, statistic_tasks, visual_tasks
-
-KG_SCHEMAS = {
-    "Data Science": {
-        "path": "https://raw.githubusercontent.com/nsai-uio/ExeKGOntology/main/ds_exeKGOntology.ttl",
-        "namespace": "https://raw.githubusercontent.com/nsai-uio/ExeKGOntology/main/ds_exeKGOntology.ttl#",
-        "namespace_prefix": "ds",
-    },
-    "Visualization": {
-        "path": "https://raw.githubusercontent.com/nsai-uio/ExeKGOntology/main/visu_exeKGOntology.ttl",
-        "namespace": "https://raw.githubusercontent.com/nsai-uio/ExeKGOntology/main/visu_exeKGOntology.ttl#",
-        "namespace_prefix": "visu",
-    },
-    "Statistics": {
-        "path": "https://raw.githubusercontent.com/nsai-uio/ExeKGOntology/main/stats_exeKGOntology.ttl",
-        "namespace": "https://raw.githubusercontent.com/nsai-uio/ExeKGOntology/main/stats_exeKGOntology.ttl#",
-        "namespace_prefix": "stats",
-    },
-    "Machine Learning": {
-        "path": "https://raw.githubusercontent.com/nsai-uio/ExeKGOntology/main/ml_exeKGOntology.ttl",
-        "namespace": "https://raw.githubusercontent.com/nsai-uio/ExeKGOntology/main/ml_exeKGOntology.ttl#",
-        "namespace_prefix": "ml",
-    },
-}
-
-
-class ExeKG:
-    def __init__(self, input_exe_kg_path: str = None):
-        """
-
-        Args:
-            input_exe_kg_path: path of KG to be executed
-                               acts as switch for KG execution mode (if filled, mode is on)
-        """
-        self.top_level_schema = KGSchema.from_schema_info(KG_SCHEMAS["Data Science"])  # top-level KG schema
-        self.bottom_level_schemata = {}
-
-        # top-level KG schema entities
-        self.atomic_task = Entity(self.top_level_schema.namespace.AtomicTask)
-        self.atomic_method = Entity(self.top_level_schema.namespace.AtomicMethod)
-        self.data_entity = Entity(self.top_level_schema.namespace.DataEntity)
-        self.pipeline = Entity(self.top_level_schema.namespace.Pipeline)
-        self.data = Entity(self.top_level_schema.namespace.Data)
-        self.data_semantics = Entity(self.top_level_schema.namespace.DataSemantics)
-        self.data_structure = Entity(self.top_level_schema.namespace.DataStructure)
-
-        # self.input_kg: KG eventually filled with 3 KG schemas and the input executable KG in case of KG execution
-        self.input_kg = Graph(bind_namespaces="rdflib")
-        if input_exe_kg_path:  # KG execution mode
-            self.input_kg.parse(input_exe_kg_path, format="n3")  # parse input executable KG
-            all_ns = [n for n in self.input_kg.namespace_manager.namespaces()]
-            bottom_level_schema_info_set = False  # flag indicating that a bottom-level schema was found
-            for schema_name, schema_info in KG_SCHEMAS.items():  # search for used bottom-level schema
-                if (
-                    schema_name == "Data Science"  # or schema_name == "Visualization"
-                ):  # skip top-level KG schema and Visualization schema that is always used
-                    continue
-
-                if (schema_info["namespace_prefix"], URIRef(schema_info["namespace"])) in all_ns:
-                    # bottom-level schema found
-                    self.bottom_level_schemata[schema_info["namespace_prefix"]] = KGSchema.from_schema_info(schema_info)
-                    bottom_level_schema_info_set = True
-
-            if not bottom_level_schema_info_set:  # no bottom-level schema found, input executable KG is invalid
-                print("Input executable KG did not have any bottom level KG schemas")
-                exit(1)
-        else:  # KG construction mode
-            for schema_name, schema_info in KG_SCHEMAS.items():  # search for used bottom-level schema
-                if (
-                    schema_name == "Data Science"  # or schema_name == "Visualization"
-                ):  # skip top-level KG schema and Visualization schema that is always used
-                    continue
-
-                self.bottom_level_schemata[schema_info["namespace_prefix"]] = KGSchema.from_schema_info(schema_info)
-
-        bottom_level_schemata_kgs = [kg_schema.kg for kg_schema in self.bottom_level_schemata.values()]
-
-        self.input_kg += self.top_level_schema.kg  # + self.visu_schema.kg  # combine all KG schemas in input KG
-
-        for bottom_level_schema_kg in bottom_level_schemata_kgs:
-            self.input_kg += bottom_level_schema_kg
-
-        self.output_kg = Graph(bind_namespaces="rdflib")  # KG to be filled while constructing executable KG
-
-        self._bind_used_namespaces([self.input_kg, self.output_kg])
-
-        # below variables are filled in self._parse_kgs()
-        self.task_type_dict = {}  # dict for uniquely naming each new pipeline task
-        self.method_type_dict = {}  # dict for uniquely naming each new pipeline method
-        self.atomic_task_list = []  # list for storing the available sub-classes of ds:AtomicTask
-        self.atomic_method_list = []  # list for storing the available sub-classes of ds:AtomicMethod
-        self.data_type_list = []  # list for storing the available sub-classes of ds:DataEntity
-        self.data_semantics_list = []  # list for storing the available sub-classes of ds:DataSemantics
-        self.data_structure_list = []  # list for storing the available sub-classes of ds:DataStructure
-
-        self.existing_data_entity_list = (
-            []
-        )  # contains existing data entities that are output entities of previous tasks during KG construction
-        self.last_created_task = (
-            None  # last created pipeline task, for connecting consecutive pipeline tasks during KG construction
-        )
-        self.canvas_task_created = False  # indicates if canvas task was created during KG construction, and used for hiding the other Visualization tasks in CLI
-
-        self._parse_kgs()
-
-    def _bind_used_namespaces(self, kgs: List[Graph]):
-        """
-        Binds top-level, bottom-level and Visualization KG schemas' namespaces with their prefixes
-        Adds these bindings to the Graphs of kgs list
-        Args:
-            kgs: list of Graph objects to which the namespace bindings are added
-        """
-        for kg in kgs:
-            kg.bind(self.top_level_schema.namespace_prefix, self.top_level_schema.namespace)
-            for bottom_level_kg_schema in self.bottom_level_schemata.values():
-                kg.bind(
-                    bottom_level_kg_schema.namespace_prefix,
-                    bottom_level_kg_schema.namespace,
-                )
-
-    def _parse_kgs(self) -> None:
-        """
-        Fills lists with subclasses of top-level KG schema classes and initializes dicts used for unique naming
-        """
-        atomic_task_subclasses = get_subclasses_of(self.atomic_task.iri, self.input_kg)
-        for t in list(atomic_task_subclasses):
-            task = Entity(t[0], self.atomic_task)
-            self.atomic_task_list.append(task)
-            self.task_type_dict[task.name] = 1
-
-        atomic_method_subclasses = get_subclasses_of(self.atomic_method.iri, self.input_kg)
-        for m in list(atomic_method_subclasses):
-            method = Entity(m[0], self.atomic_method)
-            self.atomic_method_list.append(method)
-            self.method_type_dict[method.name] = 1
-
-        data_type_subclasses = get_subclasses_of(self.data_entity.iri, self.input_kg)
-        for d in list(data_type_subclasses):
-            data_type = Entity(d[0], self.data_entity)
-            self.data_type_list.append(data_type)
-
-        data_semantics_subclasses = get_subclasses_of(self.data_semantics.iri, self.top_level_schema.kg)
-        for d in list(data_semantics_subclasses):
-            if d[0] == self.data_entity.iri:
-                continue
-            data_semantics = Entity(d[0], self.data_semantics)
-            self.data_semantics_list.append(data_semantics)
-
-        data_structure_subclasses = get_subclasses_of(self.data_structure.iri, self.top_level_schema.kg)
-        for d in list(data_structure_subclasses):
-            if d[0] == self.data_entity.iri:
-                continue
-            data_structure = Entity(d[0], self.data_structure)
-            self.data_structure_list.append(data_structure)
-
-    def create_pipeline_task(self, pipeline_name: str, input_data_path: str) -> Task:
-        """
-        Instantiates and adds a new pipeline task entity to self.output_kg
-        Args:
-            pipeline_name: name for the pipeline
-            input_data_path: path for the input data to be used by the pipeline's tasks
-
-        Returns:
-            Task: created pipeline
-        """
-        pipeline = create_pipeline_task(
-            self.top_level_schema.namespace,
-            self.pipeline,
-            self.output_kg,
-            pipeline_name,
-            input_data_path,
-        )
-        self.last_created_task = pipeline
-        return pipeline
-
-    def create_data_entity(
-        self,
-        name: str,
-        source_value: str,
-        data_semantics_name: str,
-        data_structure_name: str,
-    ) -> DataEntity:
-        """
-        Creates a DataEntity object
-        Args:
-            name: name of the data entity
-            source_value: name of the data source corresponding to a column of the data
-            data_semantics_name: name of the data semantics entity
-            data_structure_name: name of the data structure entity
-
-        Returns:
-            DataEntity: object initialized with the given parameter values
-        """
-        return DataEntity(
-            self.top_level_schema.namespace + name,
-            self.data_entity,
-            source_value,
-            self.top_level_schema.namespace + data_semantics_name,
-            self.top_level_schema.namespace + data_structure_name,
-        )
-
-    def add_task(
-        self,
-        kg_schema_short: str,
-        task: str,
-        input_data_entity_dict: Dict[str, List[DataEntity]],
-        method: str,
-        properties_dict: Dict[str, Union[str, int, float]],
-    ) -> Task:
-        """
-        Instantiates and adds a new task entity to self.output_kg
-        Components attached to the task during creation: input and output data entities, and a method with properties
-        Args:
-            kg_schema_short: abbreviated name of the KG schema in which the task and method belong
-            task: task name
-            input_data_entity_dict: keys -> input names of the specified task
-                                    values -> lists of DataEntity objects to be added as input to the task
-            method: method name
-            properties_dict: keys -> property names of the specified method
-                             values -> values to be added as parameters to the method
-
-        Returns:
-            Task: object of the created task
-        """
-        kg_schema_to_use = self.bottom_level_schemata[kg_schema_short]
-
-        relation_iri = (
-            self.top_level_schema.namespace.hasNextTask
-            if self.last_created_task.type != "Pipeline"
-            else self.top_level_schema.namespace.hasStartTask
-        )  # use relation depending on the previous task
-
-        # instantiate task and link it with the previous one
-        parent_task = Task(kg_schema_to_use.namespace + task, self.atomic_task)
-        added_entity = add_instance_from_parent_with_relation(
-            kg_schema_to_use.namespace,
-            self.output_kg,
-            parent_task,
-            relation_iri,
-            self.last_created_task,
-            name_instance(self.task_type_dict, self.method_type_dict, parent_task),
-        )
-        next_task = Task.from_entity(added_entity)  # create Task object from Entity object
-
-        # instantiate and add given input data entities to the task
-        self._add_inputs_to_task(kg_schema_to_use.namespace, next_task, input_data_entity_dict)
-        # instantiate and add output data entities to the task, as specified in the KG schema
-        self._add_outputs_to_task(next_task)
-
-        method_parent = Entity(kg_schema_to_use.namespace + method, self.atomic_method)
-
-        # fetch compatible methods and their properties from KG schema
-        results = list(
-            get_method_properties_and_methods(
-                self.input_kg,
-                self.top_level_schema.namespace_prefix,
-                next_task.parent_entity.iri,
-            )
-        )
-
-        chosen_property_method = next(
-            filter(lambda pair: pair[1].split("#")[1] == method, results), None
-        )  # match given method_type with query result
-        if chosen_property_method is None:
-            print(f"Property connecting task of type {task} with method of type {method} not found")
-            exit(1)
-
-        # instantiate method and link it with the task using the appropriate chosen_property_method[0] relation
-        add_instance_from_parent_with_relation(
-            kg_schema_to_use.namespace,
-            self.output_kg,
-            method_parent,
-            chosen_property_method[0],
-            next_task,
-            name_instance(self.task_type_dict, self.method_type_dict, method_parent),
-        )
-
-        # fetch compatible data properties from KG schema
-        property_list = get_data_properties_plus_inherited_by_class_iri(self.input_kg, method_parent.iri)
-
-        # add data properties to the task with given values
-        for pair in property_list:
-            property_iri = pair[0]
-            property_name = property_iri.split("#")[1]
-            range_iri = pair[1]
-            input_property = Literal(
-                lexical_or_value=properties_dict[property_name],
-                datatype=range_iri,
-            )
-            add_literal(self.output_kg, next_task, property_iri, input_property)
-
-        self.last_created_task = next_task  # store created task
-
-        return next_task
-
-    def _add_inputs_to_task(
-        self,
-        namespace: Namespace,
-        task_entity: Task,
-        input_data_entity_dict: Dict[str, List[DataEntity]] = None,
-    ) -> None:
-        """
-        Instantiates and adds given input data entities to the given task of self.output_kg
-        if input_data_entity_dict is None, user is asked to specify input data entities
-        Args:
-            task_entity: the task to add the input to
-            input_data_entity_dict: keys -> input entity names corresponding to the given task as defined in the chosen bottom-level KG schema
-                                    values -> list of corresponding data entities to be added as input to the task
-        """
-        # fetch compatible inputs from KG schema
-        results = list(
-            get_input_properties_and_inputs(
-                self.input_kg,
-                self.top_level_schema.namespace_prefix,
-                task_entity.parent_entity.iri,
-            )
-        )
-
-        # task_type_index was incremented when creating the task entity
-        # reset the index to match the currently created task's index
-        task_type_index = self.task_type_dict[task_entity.type] - 1
-        for _, input_entity_iri in results:
-            input_entity_name = input_entity_iri.split("#")[1]
-            if input_data_entity_dict:
-                input_data_entity_list = input_data_entity_dict[input_entity_name]
-            else:
-                # use CLI
-                print(f"Specify input corresponding to {input_entity_name}")
-                input_data_entity_list = get_input_for_existing_data_entities(self.existing_data_entity_list)
-                input_data_entity_list += get_input_for_new_data_entities(
-                    self.data_semantics_list,
-                    self.data_structure_list,
-                    namespace,
-                    self.data_entity,
-                )
-
-            same_input_index = 1
-            for input_data_entity in input_data_entity_list:
-                # instantiate data entity corresponding to the found input_entity_name
-                data_entity_iri = input_entity_iri + str(task_type_index) + "_" + str(same_input_index)
-                # instantiate given data entity
-                add_data_entity_instance(
-                    self.output_kg,
-                    self.data,
-                    self.top_level_schema.kg,
-                    self.top_level_schema.namespace,
-                    input_data_entity,
-                )
-                # instantiate and attach data entity with reference to the given data entity
-                data_entity = DataEntity(
-                    data_entity_iri,
-                    DataEntity(input_entity_iri, self.data_entity),
-                    has_reference=input_data_entity.iri,
-                )
-                add_and_attach_data_entity(
-                    self.output_kg,
-                    self.data,
-                    self.top_level_schema.kg,
-                    self.top_level_schema.namespace,
-                    data_entity,
-                    self.top_level_schema.namespace.hasInput,
-                    task_entity,
-                )
-                task_entity.input_dict[input_entity_name] = data_entity
-                same_input_index += 1
-
-    def _add_outputs_to_task(self, task_entity: Task) -> None:
-        """
-        Instantiates and adds output data entities to the given task of self.output_kg, based on the task's definition in the KG schema
-        Args:
-            task_entity: the task to add the output to
-        """
-        # fetch compatible outputs from KG schema
-        results = list(
-            get_output_properties_and_outputs(
-                self.input_kg,
-                self.top_level_schema.namespace_prefix,
-                task_entity.parent_entity.iri,
-            )
-        )
-
-        # task_type_index was incremented when creating the task entity
-        # reset the index to match the currently created task's index
-        task_type_index = self.task_type_dict[task_entity.type] - 1
-        for output_property, output_entity_iri in results:
-            # instantiate and add data entity
-            data_entity_iri = output_entity_iri + str(task_type_index)
-            data_entity = DataEntity(data_entity_iri, self.data_entity)
-            add_and_attach_data_entity(
-                self.output_kg,
-                self.data,
-                self.top_level_schema.kg,
-                self.top_level_schema.namespace,
-                data_entity,
-                self.top_level_schema.namespace.hasOutput,
-                task_entity,
-            )
-            task_entity.output_dict[output_entity_iri.split("#")[1]] = data_entity
-            self.existing_data_entity_list.append(data_entity)
-
-    def _create_next_task_cli(self) -> Union[None, Task]:
-        """
-        Instantiates and adds task (without method) based on user input to self.output_kg
-        Adds task's output data entities to self.existing_data_entity_list
-        Returns:
-            None: in case user wants to end the pipeline creation
-            Task: object of the created task
-        """
-        print("Please choose the next task")
-        for i, t in enumerate(self.atomic_task_list):
-            if not self.canvas_task_created and t.name == "PlotTask":
-                continue
-            if self.canvas_task_created and t.name == "CanvasTask":
-                continue
-            print(f"\t{str(i)}. {t.name}")
-        print(f"\t{str(-1)}. End pipeline")
-        next_task_id = int(input())
-        if next_task_id == -1:
-            return None
-
-        next_task_parent = self.atomic_task_list[next_task_id]
-        relation_iri = (
-            self.top_level_schema.namespace.hasNextTask
-            if self.last_created_task.type != "Pipeline"
-            else self.top_level_schema.namespace.hasStartTask
-        )  # use relation depending on the previous task
-
-        # instantiate task and link it with the previous one
-        task_entity = add_instance_from_parent_with_relation(
-            next_task_parent.namespace,
-            self.output_kg,
-            next_task_parent,
-            relation_iri,
-            self.last_created_task,
-            name_instance(self.task_type_dict, self.method_type_dict, next_task_parent),
-        )
-
-        task_entity = Task(task_entity.iri, task_entity.parent_entity)  # create Task object from Entity object's info
-
-        # instantiate and add input data entities to the task based on user input
-        self._add_inputs_to_task(next_task_parent.namespace, task_entity)
-        # instantiate and add output data entities to the task, as specified in the KG schema
-        self._add_outputs_to_task(task_entity)
-
-        self.last_created_task = task_entity
-        if task_entity.type == "CanvasTask":
-            self.canvas_task_created = True
-
-        return task_entity
-
-    def _create_method(self, task_to_attach_to: Entity) -> None:
-        """
-        Instantiate and attach method to task of self.output_kg
-        Args:
-            task_to_attach_to: the task to attach the created method to
-        """
-        print(f"Please choose a method for {task_to_attach_to.type}:")
-
-        # fetch compatible methods and their properties from KG schema
-        results = list(
-            get_method_properties_and_methods(
-                self.input_kg,
-                self.top_level_schema.namespace_prefix,
-                task_to_attach_to.parent_entity.iri,
-            )
-        )
-        for i, pair in enumerate(results):
-            tmp_method = pair[1].split("#")[1]
-            print(f"\t{str(i)}. {tmp_method}")
-
-        method_id = int(input())
-        selected_property_and_method = results[method_id]
-        method_parent = next(
-            filter(
-                lambda m: m.iri == selected_property_and_method[1],
-                self.atomic_method_list,
-            ),
-            None,
-        )
-        # instantiate method and link it with the task using the appropriate selected_property_and_method[0] relation
-        add_instance_from_parent_with_relation(
-            task_to_attach_to.namespace,
-            self.output_kg,
-            method_parent,
-            selected_property_and_method[0],
-            task_to_attach_to,
-            name_instance(self.task_type_dict, self.method_type_dict, method_parent),
-        )
-
-        # fetch compatible data properties from KG schema
-        property_list = get_data_properties_plus_inherited_by_class_iri(self.input_kg, method_parent.iri)
-
-        if property_list:
-            print(f"Please enter requested properties for {method_parent.name}:")
-            # add data properties to the task with given values
-            for pair in property_list:
-                property_instance = URIRef(pair[0])
-                range = pair[1].split("#")[1]
-                range_iri = pair[1]
-                input_property = Literal(
-                    lexical_or_value=input("\t{} in range({}): ".format(pair[0].split("#")[1], range)),
-                    datatype=range_iri,
-                )
-                add_literal(self.output_kg, task_to_attach_to, property_instance, input_property)
-
-    def start_pipeline_creation(self, pipeline_name: str, input_data_path: str) -> None:
-        """
-        Handles the pipeline creation through CLI
-        Args:
-            pipeline_name: name for the pipeline
-            input_data_path: path for the input data to be used by the pipeline's tasks
-        """
-        pipeline = create_pipeline_task(
-            self.top_level_schema.namespace,
-            self.pipeline,
-            self.output_kg,
-            pipeline_name,
-            input_data_path,
-        )
-
-        self.last_created_task = pipeline
-
-        while True:
-            next_task = self._create_next_task_cli()
-            if next_task is None:
-                break
-
-            self._create_method(next_task)
-
-    def save_created_kg(self, file_path: str) -> None:
-        """
-        Saves self.output_kg to a file
-        Args:
-            file_path: path of the output file
-        """
-        dir_path = os.path.dirname(file_path)
-        os.makedirs(dir_path, exist_ok=True)
-
-        self.output_kg.serialize(destination=file_path)
-        print(f"Executable KG saved in {file_path}")
-
-    def _property_value_to_field_value(self, property_value: str) -> Union[str, DataEntity]:
-        """
-        Converts property value to Python class field value
-        If property_value is not a data entity's IRI, it is returned as is
-        Else, its property values are converted recursively and stored in a DataEntity object
-        Args:
-            property_value: value of the property as found in KG
-
-        Returns:
-            str: property_value parameter as is
-            DataEntity: object containing parsed data entity properties
-        """
-        if "#" in property_value:
-            data_entity = self._parse_data_entity_by_iri(property_value)
-            if data_entity is None:
-                return property_value
-            return data_entity
-
-        return property_value
-
-    def _parse_data_entity_by_iri(self, in_out_data_entity_iri: str) -> Optional[DataEntity]:
-        """
-        Parses an input or output data entity of self.input_kg and stores the parsed info in a Python object
-        Args:
-            in_out_data_entity_iri: IRI of the KG entity to parse
-
-        Returns:
-            None: if given IRI does not belong to an instance of a sub-class of self.top_level_schema.namespace.DataEntity
-            DataEntity: object with data entity's parsed properties
-        """
-        # fetch type of entity with given IRI
-        query_result = get_first_query_result_if_exists(
-            query_entity_parent_iri,
-            self.input_kg,
-            in_out_data_entity_iri,
-            self.top_level_schema.namespace.DataEntity,
-        )
-        if query_result is None:
-            return None
-
-        data_entity_parent_iri = str(query_result[0])
-
-        # fetch IRI of data entity that is referenced by the given entity
-        query_result = get_first_query_result_if_exists(
-            query_data_entity_reference_iri,
-            self.input_kg,
-            self.top_level_schema.namespace_prefix,
-            in_out_data_entity_iri,
-        )
-
-        if query_result is None:  # no referenced data entity found
-            data_entity_ref_iri = in_out_data_entity_iri
-        else:
-            data_entity_ref_iri = str(query_result[0])
-
-        # create DataEntity object to store all the parsed properties
-        data_entity = DataEntity(in_out_data_entity_iri, Entity(data_entity_parent_iri))
-        data_entity.has_reference = data_entity_ref_iri.split("#")[1]
-
-        for s, p, o in self.input_kg.triples((URIRef(data_entity_ref_iri), None, None)):
-            # parse property name and value
-            field_name = property_name_to_field_name(str(p))
-            if not hasattr(data_entity, field_name) or field_name == "type":
-                continue
-            field_value = self._property_value_to_field_value(str(o))
-            setattr(data_entity, field_name, field_value)  # set field value dynamically
-
-        return data_entity
-
-    def _parse_task_by_iri(self, task_iri: str, canvas_method: visual_tasks.CanvasTaskCanvasMethod = None) -> Task:
-        """
-        Parses a task of self.input_kg and stores the info in an object of a sub-class of Task
-        The sub-class name and the object's fields are mapped dynamically based on the found KG components
-        Args:
-            task_iri: IRI of the task to be parsed
-            canvas_method: optional object to pass as argument for task object initialization
-
-        Returns:
-            Task: object of a sub-class of Task, containing all the parsed info
-        """
-        # fetch type of entity with given IRI
-        query_result = get_first_query_result_if_exists(
-            query_entity_parent_iri,
-            self.input_kg,
-            task_iri,
-            self.top_level_schema.namespace.AtomicTask,
-        )
-
-        if (
-            query_result is None
-        ):  # given IRI does not belong to an instance of a sub-class of self.top_level_schema.namespace.AtomicTask
-            print(f"Cannot retrieve parent of task with iri {task_iri}. Exiting...")
-            exit(1)
-
-        task_parent_iri = str(query_result[0])
-
-        task = Task(task_iri, Task(task_parent_iri))
-        method = get_method_by_task_iri(
-            self.input_kg,
-            self.top_level_schema.namespace_prefix,
-            self.top_level_schema.namespace,
-            task_iri,
-        )
-        if method is None:
-            print(f"Cannot retrieve method for task with iri: {task_iri}")
-
-        # perform automatic mapping of KG task class to Python sub-class
-        class_name = task.type + method.type
-        Class = getattr(visual_tasks, class_name, None)
-        if Class is None:
-            Class = getattr(statistic_tasks, class_name, None)
-        if Class is None:
-            Class = getattr(ml_tasks, class_name, None)
-
-        # create Task sub-class object
-        if canvas_method:
-            task = Class(task_iri, Task(task_parent_iri), canvas_method)
-        else:
-            task = Class(task_iri, Task(task_parent_iri))
-
-        for s, p, o in self.input_kg.triples((URIRef(task_iri), None, None)):
-            # parse property name and value
-            field_name = property_name_to_field_name(str(p))
-            if not hasattr(task, field_name) or field_name == "type":
-                continue
-            field_value = self._property_value_to_field_value(str(o))
-
-            # set field value dynamically
-            if field_name == "has_input" or field_name == "has_output":
-                getattr(task, field_name).append(field_value)
-            else:
-                setattr(task, field_name, field_value)
-
-        return task
-
-    def execute_pipeline(self):
-        """
-        Retrieves and executes pipeline by parsing self.input_kg
-        """
-        pipeline_iri, input_data_path, next_task_iri = get_pipeline_and_first_task_iri(
-            self.input_kg, self.top_level_schema.namespace_prefix
-        )
-        input_data = pd.read_csv(input_data_path, delimiter=",", encoding="ISO-8859-1")
-        canvas_method = None  # stores Task object that corresponds to a task of type CanvasTask
-        task_output_dict = {}  # gradually filled with outputs of executed tasks
-        while next_task_iri is not None:
-            next_task = self._parse_task_by_iri(next_task_iri, canvas_method)
-            output = next_task.run_method(task_output_dict, input_data)
-            if output:
-                task_output_dict.update(output)
-
-            if next_task.type == "CanvasTask":
-                canvas_method = next_task
-
-            next_task_iri = next_task.has_next_task
+# Copyright (c) 2022 Robert Bosch GmbH
+# SPDX-License-Identifier: AGPL-3.0
+
+import os
+from typing import Dict, Union
+
+import pandas as pd
+from rdflib import Literal
+
+from ..utils.cli_utils import (get_input_for_existing_data_entities,
+                               get_input_for_new_data_entities)
+from ..utils.kg_creation_utils import (add_and_attach_data_entity,
+                                       add_data_entity_instance,
+                                       add_instance_from_parent_with_relation,
+                                       add_literal, create_pipeline_task,
+                                       name_instance)
+from ..utils.query_utils import *
+from ..utils.query_utils import (
+    get_data_properties_plus_inherited_by_class_iri, get_method_by_task_iri,
+    get_pipeline_and_first_task_iri)
+from ..utils.string_utils import property_name_to_field_name
+from .data_entity import DataEntity
+from .entity import Entity
+from .kg_schema import KGSchema
+from .task import Task
+from .tasks import ml_tasks, statistic_tasks, visual_tasks
+
+KG_SCHEMAS = {
+    "Data Science": {
+        "path": "https://raw.githubusercontent.com/nsai-uio/ExeKGOntology/main/ds_exeKGOntology.ttl",
+        "namespace": "https://raw.githubusercontent.com/nsai-uio/ExeKGOntology/main/ds_exeKGOntology.ttl#",
+        "namespace_prefix": "ds",
+    },
+    "Visualization": {
+        "path": "https://raw.githubusercontent.com/nsai-uio/ExeKGOntology/main/visu_exeKGOntology.ttl",
+        "namespace": "https://raw.githubusercontent.com/nsai-uio/ExeKGOntology/main/visu_exeKGOntology.ttl#",
+        "namespace_prefix": "visu",
+    },
+    "Statistics": {
+        "path": "https://raw.githubusercontent.com/nsai-uio/ExeKGOntology/main/stats_exeKGOntology.ttl",
+        "namespace": "https://raw.githubusercontent.com/nsai-uio/ExeKGOntology/main/stats_exeKGOntology.ttl#",
+        "namespace_prefix": "stats",
+    },
+    "Machine Learning": {
+        "path": "https://raw.githubusercontent.com/nsai-uio/ExeKGOntology/main/ml_exeKGOntology.ttl",
+        "namespace": "https://raw.githubusercontent.com/nsai-uio/ExeKGOntology/main/ml_exeKGOntology.ttl#",
+        "namespace_prefix": "ml",
+    },
+}
+
+
+class ExeKG:
+    def __init__(self, input_exe_kg_path: str = None):
+        """
+
+        Args:
+            input_exe_kg_path: path of KG to be executed
+                               acts as switch for KG execution mode (if filled, mode is on)
+        """
+        self.top_level_schema = KGSchema.from_schema_info(KG_SCHEMAS["Data Science"])  # top-level KG schema
+        self.bottom_level_schemata = {}
+
+        # top-level KG schema entities
+        self.atomic_task = Entity(self.top_level_schema.namespace.AtomicTask)
+        self.atomic_method = Entity(self.top_level_schema.namespace.AtomicMethod)
+        self.data_entity = Entity(self.top_level_schema.namespace.DataEntity)
+        self.pipeline = Entity(self.top_level_schema.namespace.Pipeline)
+        self.data = Entity(self.top_level_schema.namespace.Data)
+        self.data_semantics = Entity(self.top_level_schema.namespace.DataSemantics)
+        self.data_structure = Entity(self.top_level_schema.namespace.DataStructure)
+
+        # self.input_kg: KG eventually filled with 3 KG schemas and the input executable KG in case of KG execution
+        self.input_kg = Graph(bind_namespaces="rdflib")
+        if input_exe_kg_path:  # KG execution mode
+            self.input_kg.parse(input_exe_kg_path, format="n3")  # parse input executable KG
+            all_ns = [n for n in self.input_kg.namespace_manager.namespaces()]
+            bottom_level_schema_info_set = False  # flag indicating that a bottom-level schema was found
+            for schema_name, schema_info in KG_SCHEMAS.items():  # search for used bottom-level schema
+                if (
+                    schema_name == "Data Science"  # or schema_name == "Visualization"
+                ):  # skip top-level KG schema and Visualization schema that is always used
+                    continue
+
+                if (schema_info["namespace_prefix"], URIRef(schema_info["namespace"])) in all_ns:
+                    # bottom-level schema found
+                    self.bottom_level_schemata[schema_info["namespace_prefix"]] = KGSchema.from_schema_info(schema_info)
+                    bottom_level_schema_info_set = True
+
+            if not bottom_level_schema_info_set:  # no bottom-level schema found, input executable KG is invalid
+                print("Input executable KG did not have any bottom level KG schemas")
+                exit(1)
+        else:  # KG construction mode
+            for schema_name, schema_info in KG_SCHEMAS.items():  # search for used bottom-level schema
+                if (
+                    schema_name == "Data Science"  # or schema_name == "Visualization"
+                ):  # skip top-level KG schema and Visualization schema that is always used
+                    continue
+
+                self.bottom_level_schemata[schema_info["namespace_prefix"]] = KGSchema.from_schema_info(schema_info)
+
+        bottom_level_schemata_kgs = [kg_schema.kg for kg_schema in self.bottom_level_schemata.values()]
+
+        self.input_kg += self.top_level_schema.kg  # + self.visu_schema.kg  # combine all KG schemas in input KG
+
+        for bottom_level_schema_kg in bottom_level_schemata_kgs:
+            self.input_kg += bottom_level_schema_kg
+
+        self.output_kg = Graph(bind_namespaces="rdflib")  # KG to be filled while constructing executable KG
+
+        self._bind_used_namespaces([self.input_kg, self.output_kg])
+
+        # below variables are filled in self._parse_kgs()
+        self.task_type_dict = {}  # dict for uniquely naming each new pipeline task
+        self.method_type_dict = {}  # dict for uniquely naming each new pipeline method
+        self.atomic_task_list = []  # list for storing the available sub-classes of ds:AtomicTask
+        self.atomic_method_list = []  # list for storing the available sub-classes of ds:AtomicMethod
+        self.data_type_list = []  # list for storing the available sub-classes of ds:DataEntity
+        self.data_semantics_list = []  # list for storing the available sub-classes of ds:DataSemantics
+        self.data_structure_list = []  # list for storing the available sub-classes of ds:DataStructure
+
+        self.existing_data_entity_list = (
+            []
+        )  # contains existing data entities that are output entities of previous tasks during KG construction
+        self.last_created_task = (
+            None  # last created pipeline task, for connecting consecutive pipeline tasks during KG construction
+        )
+        self.canvas_task_created = False  # indicates if canvas task was created during KG construction, and used for hiding the other Visualization tasks in CLI
+
+        self._parse_kgs()
+
+    def _bind_used_namespaces(self, kgs: List[Graph]):
+        """
+        Binds top-level, bottom-level and Visualization KG schemas' namespaces with their prefixes
+        Adds these bindings to the Graphs of kgs list
+        Args:
+            kgs: list of Graph objects to which the namespace bindings are added
+        """
+        for kg in kgs:
+            kg.bind(self.top_level_schema.namespace_prefix, self.top_level_schema.namespace)
+            for bottom_level_kg_schema in self.bottom_level_schemata.values():
+                kg.bind(
+                    bottom_level_kg_schema.namespace_prefix,
+                    bottom_level_kg_schema.namespace,
+                )
+
+    def _parse_kgs(self) -> None:
+        """
+        Fills lists with subclasses of top-level KG schema classes and initializes dicts used for unique naming
+        """
+        atomic_task_subclasses = get_subclasses_of(self.atomic_task.iri, self.input_kg)
+        for t in list(atomic_task_subclasses):
+            task = Entity(t[0], self.atomic_task)
+            self.atomic_task_list.append(task)
+            self.task_type_dict[task.name] = 1
+
+        atomic_method_subclasses = get_subclasses_of(self.atomic_method.iri, self.input_kg)
+        for m in list(atomic_method_subclasses):
+            method = Entity(m[0], self.atomic_method)
+            self.atomic_method_list.append(method)
+            self.method_type_dict[method.name] = 1
+
+        data_type_subclasses = get_subclasses_of(self.data_entity.iri, self.input_kg)
+        for d in list(data_type_subclasses):
+            data_type = Entity(d[0], self.data_entity)
+            self.data_type_list.append(data_type)
+
+        data_semantics_subclasses = get_subclasses_of(self.data_semantics.iri, self.top_level_schema.kg)
+        for d in list(data_semantics_subclasses):
+            if d[0] == self.data_entity.iri:
+                continue
+            data_semantics = Entity(d[0], self.data_semantics)
+            self.data_semantics_list.append(data_semantics)
+
+        data_structure_subclasses = get_subclasses_of(self.data_structure.iri, self.top_level_schema.kg)
+        for d in list(data_structure_subclasses):
+            if d[0] == self.data_entity.iri:
+                continue
+            data_structure = Entity(d[0], self.data_structure)
+            self.data_structure_list.append(data_structure)
+
+    def create_pipeline_task(self, pipeline_name: str, input_data_path: str) -> Task:
+        """
+        Instantiates and adds a new pipeline task entity to self.output_kg
+        Args:
+            pipeline_name: name for the pipeline
+            input_data_path: path for the input data to be used by the pipeline's tasks
+
+        Returns:
+            Task: created pipeline
+        """
+        pipeline = create_pipeline_task(
+            self.top_level_schema.namespace,
+            self.pipeline,
+            self.output_kg,
+            pipeline_name,
+            input_data_path,
+        )
+        self.last_created_task = pipeline
+        return pipeline
+
+    def create_data_entity(
+        self,
+        name: str,
+        source_value: str,
+        data_semantics_name: str,
+        data_structure_name: str,
+    ) -> DataEntity:
+        """
+        Creates a DataEntity object
+        Args:
+            name: name of the data entity
+            source_value: name of the data source corresponding to a column of the data
+            data_semantics_name: name of the data semantics entity
+            data_structure_name: name of the data structure entity
+
+        Returns:
+            DataEntity: object initialized with the given parameter values
+        """
+        return DataEntity(
+            self.top_level_schema.namespace + name,
+            self.data_entity,
+            source_value,
+            self.top_level_schema.namespace + data_semantics_name,
+            self.top_level_schema.namespace + data_structure_name,
+        )
+
+    def add_task(
+        self,
+        kg_schema_short: str,
+        task: str,
+        input_data_entity_dict: Dict[str, List[DataEntity]],
+        method: str,
+        properties_dict: Dict[str, Union[str, int, float]],
+    ) -> Task:
+        """
+        Instantiates and adds a new task entity to self.output_kg
+        Components attached to the task during creation: input and output data entities, and a method with properties
+        Args:
+            kg_schema_short: abbreviated name of the KG schema in which the task and method belong
+            task: task name
+            input_data_entity_dict: keys -> input names of the specified task
+                                    values -> lists of DataEntity objects to be added as input to the task
+            method: method name
+            properties_dict: keys -> property names of the specified method
+                             values -> values to be added as parameters to the method
+
+        Returns:
+            Task: object of the created task
+        """
+        kg_schema_to_use = self.bottom_level_schemata[kg_schema_short]
+
+        relation_iri = (
+            self.top_level_schema.namespace.hasNextTask
+            if self.last_created_task.type != "Pipeline"
+            else self.top_level_schema.namespace.hasStartTask
+        )  # use relation depending on the previous task
+
+        # instantiate task and link it with the previous one
+        parent_task = Task(kg_schema_to_use.namespace + task, self.atomic_task)
+        added_entity = add_instance_from_parent_with_relation(
+            kg_schema_to_use.namespace,
+            self.output_kg,
+            parent_task,
+            relation_iri,
+            self.last_created_task,
+            name_instance(self.task_type_dict, self.method_type_dict, parent_task),
+        )
+        next_task = Task.from_entity(added_entity)  # create Task object from Entity object
+
+        # instantiate and add given input data entities to the task
+        self._add_inputs_to_task(kg_schema_to_use.namespace, next_task, input_data_entity_dict)
+        # instantiate and add output data entities to the task, as specified in the KG schema
+        self._add_outputs_to_task(next_task)
+
+        method_parent = Entity(kg_schema_to_use.namespace + method, self.atomic_method)
+
+        # fetch compatible methods and their properties from KG schema
+        results = list(
+            get_method_properties_and_methods(
+                self.input_kg,
+                self.top_level_schema.namespace_prefix,
+                next_task.parent_entity.iri,
+            )
+        )
+
+        chosen_property_method = next(
+            filter(lambda pair: pair[1].split("#")[1] == method, results), None
+        )  # match given method_type with query result
+        if chosen_property_method is None:
+            print(f"Property connecting task of type {task} with method of type {method} not found")
+            exit(1)
+
+        # instantiate method and link it with the task using the appropriate chosen_property_method[0] relation
+        add_instance_from_parent_with_relation(
+            kg_schema_to_use.namespace,
+            self.output_kg,
+            method_parent,
+            chosen_property_method[0],
+            next_task,
+            name_instance(self.task_type_dict, self.method_type_dict, method_parent),
+        )
+
+        # fetch compatible data properties from KG schema
+        property_list = get_data_properties_plus_inherited_by_class_iri(self.input_kg, method_parent.iri)
+
+        # add data properties to the task with given values
+        for pair in property_list:
+            property_iri = pair[0]
+            property_name = property_iri.split("#")[1]
+            range_iri = pair[1]
+            input_property = Literal(
+                lexical_or_value=properties_dict[property_name],
+                datatype=range_iri,
+            )
+            add_literal(self.output_kg, next_task, property_iri, input_property)
+
+        self.last_created_task = next_task  # store created task
+
+        return next_task
+
+    def _add_inputs_to_task(
+        self,
+        namespace: Namespace,
+        task_entity: Task,
+        input_data_entity_dict: Dict[str, List[DataEntity]] = None,
+    ) -> None:
+        """
+        Instantiates and adds given input data entities to the given task of self.output_kg
+        if input_data_entity_dict is None, user is asked to specify input data entities
+        Args:
+            task_entity: the task to add the input to
+            input_data_entity_dict: keys -> input entity names corresponding to the given task as defined in the chosen bottom-level KG schema
+                                    values -> list of corresponding data entities to be added as input to the task
+        """
+        # fetch compatible inputs from KG schema
+        results = list(
+            get_input_properties_and_inputs(
+                self.input_kg,
+                self.top_level_schema.namespace_prefix,
+                task_entity.parent_entity.iri,
+            )
+        )
+
+        # task_type_index was incremented when creating the task entity
+        # reset the index to match the currently created task's index
+        task_type_index = self.task_type_dict[task_entity.type] - 1
+        for _, input_entity_iri in results:
+            input_entity_name = input_entity_iri.split("#")[1]
+            if input_data_entity_dict:
+                input_data_entity_list = input_data_entity_dict[input_entity_name]
+            else:
+                # use CLI
+                print(f"Specify input corresponding to {input_entity_name}")
+                input_data_entity_list = get_input_for_existing_data_entities(self.existing_data_entity_list)
+                input_data_entity_list += get_input_for_new_data_entities(
+                    self.data_semantics_list,
+                    self.data_structure_list,
+                    namespace,
+                    self.data_entity,
+                )
+
+            same_input_index = 1
+            for input_data_entity in input_data_entity_list:
+                # instantiate data entity corresponding to the found input_entity_name
+                data_entity_iri = input_entity_iri + str(task_type_index) + "_" + str(same_input_index)
+                # instantiate given data entity
+                add_data_entity_instance(
+                    self.output_kg,
+                    self.data,
+                    self.top_level_schema.kg,
+                    self.top_level_schema.namespace,
+                    input_data_entity,
+                )
+                # instantiate and attach data entity with reference to the given data entity
+                data_entity = DataEntity(
+                    data_entity_iri,
+                    DataEntity(input_entity_iri, self.data_entity),
+                    has_reference=input_data_entity.iri,
+                )
+                add_and_attach_data_entity(
+                    self.output_kg,
+                    self.data,
+                    self.top_level_schema.kg,
+                    self.top_level_schema.namespace,
+                    data_entity,
+                    self.top_level_schema.namespace.hasInput,
+                    task_entity,
+                )
+                task_entity.input_dict[input_entity_name] = data_entity
+                same_input_index += 1
+
+    def _add_outputs_to_task(self, task_entity: Task) -> None:
+        """
+        Instantiates and adds output data entities to the given task of self.output_kg, based on the task's definition in the KG schema
+        Args:
+            task_entity: the task to add the output to
+        """
+        # fetch compatible outputs from KG schema
+        results = list(
+            get_output_properties_and_outputs(
+                self.input_kg,
+                self.top_level_schema.namespace_prefix,
+                task_entity.parent_entity.iri,
+            )
+        )
+
+        # task_type_index was incremented when creating the task entity
+        # reset the index to match the currently created task's index
+        task_type_index = self.task_type_dict[task_entity.type] - 1
+        for output_property, output_entity_iri in results:
+            # instantiate and add data entity
+            data_entity_iri = output_entity_iri + str(task_type_index)
+            data_entity = DataEntity(data_entity_iri, self.data_entity)
+            add_and_attach_data_entity(
+                self.output_kg,
+                self.data,
+                self.top_level_schema.kg,
+                self.top_level_schema.namespace,
+                data_entity,
+                self.top_level_schema.namespace.hasOutput,
+                task_entity,
+            )
+            task_entity.output_dict[output_entity_iri.split("#")[1]] = data_entity
+            self.existing_data_entity_list.append(data_entity)
+
+    def _create_next_task_cli(self) -> Union[None, Task]:
+        """
+        Instantiates and adds task (without method) based on user input to self.output_kg
+        Adds task's output data entities to self.existing_data_entity_list
+        Returns:
+            None: in case user wants to end the pipeline creation
+            Task: object of the created task
+        """
+        print("Please choose the next task")
+        for i, t in enumerate(self.atomic_task_list):
+            if not self.canvas_task_created and t.name == "PlotTask":
+                continue
+            if self.canvas_task_created and t.name == "CanvasTask":
+                continue
+            print(f"\t{str(i)}. {t.name}")
+        print(f"\t{str(-1)}. End pipeline")
+        next_task_id = int(input())
+        if next_task_id == -1:
+            return None
+
+        next_task_parent = self.atomic_task_list[next_task_id]
+        relation_iri = (
+            self.top_level_schema.namespace.hasNextTask
+            if self.last_created_task.type != "Pipeline"
+            else self.top_level_schema.namespace.hasStartTask
+        )  # use relation depending on the previous task
+
+        # instantiate task and link it with the previous one
+        task_entity = add_instance_from_parent_with_relation(
+            next_task_parent.namespace,
+            self.output_kg,
+            next_task_parent,
+            relation_iri,
+            self.last_created_task,
+            name_instance(self.task_type_dict, self.method_type_dict, next_task_parent),
+        )
+
+        task_entity = Task(task_entity.iri, task_entity.parent_entity)  # create Task object from Entity object's info
+
+        # instantiate and add input data entities to the task based on user input
+        self._add_inputs_to_task(next_task_parent.namespace, task_entity)
+        # instantiate and add output data entities to the task, as specified in the KG schema
+        self._add_outputs_to_task(task_entity)
+
+        self.last_created_task = task_entity
+        if task_entity.type == "CanvasTask":
+            self.canvas_task_created = True
+
+        return task_entity
+
+    def _create_method(self, task_to_attach_to: Entity) -> None:
+        """
+        Instantiate and attach method to task of self.output_kg
+        Args:
+            task_to_attach_to: the task to attach the created method to
+        """
+        print(f"Please choose a method for {task_to_attach_to.type}:")
+
+        # fetch compatible methods and their properties from KG schema
+        results = list(
+            get_method_properties_and_methods(
+                self.input_kg,
+                self.top_level_schema.namespace_prefix,
+                task_to_attach_to.parent_entity.iri,
+            )
+        )
+        for i, pair in enumerate(results):
+            tmp_method = pair[1].split("#")[1]
+            print(f"\t{str(i)}. {tmp_method}")
+
+        method_id = int(input())
+        selected_property_and_method = results[method_id]
+        method_parent = next(
+            filter(
+                lambda m: m.iri == selected_property_and_method[1],
+                self.atomic_method_list,
+            ),
+            None,
+        )
+        # instantiate method and link it with the task using the appropriate selected_property_and_method[0] relation
+        add_instance_from_parent_with_relation(
+            task_to_attach_to.namespace,
+            self.output_kg,
+            method_parent,
+            selected_property_and_method[0],
+            task_to_attach_to,
+            name_instance(self.task_type_dict, self.method_type_dict, method_parent),
+        )
+
+        # fetch compatible data properties from KG schema
+        property_list = get_data_properties_plus_inherited_by_class_iri(self.input_kg, method_parent.iri)
+
+        if property_list:
+            print(f"Please enter requested properties for {method_parent.name}:")
+            # add data properties to the task with given values
+            for pair in property_list:
+                property_instance = URIRef(pair[0])
+                range = pair[1].split("#")[1]
+                range_iri = pair[1]
+                input_property = Literal(
+                    lexical_or_value=input("\t{} in range({}): ".format(pair[0].split("#")[1], range)),
+                    datatype=range_iri,
+                )
+                add_literal(self.output_kg, task_to_attach_to, property_instance, input_property)
+
+    def start_pipeline_creation(self, pipeline_name: str, input_data_path: str) -> None:
+        """
+        Handles the pipeline creation through CLI
+        Args:
+            pipeline_name: name for the pipeline
+            input_data_path: path for the input data to be used by the pipeline's tasks
+        """
+        pipeline = create_pipeline_task(
+            self.top_level_schema.namespace,
+            self.pipeline,
+            self.output_kg,
+            pipeline_name,
+            input_data_path,
+        )
+
+        self.last_created_task = pipeline
+
+        while True:
+            next_task = self._create_next_task_cli()
+            if next_task is None:
+                break
+
+            self._create_method(next_task)
+
+    def save_created_kg(self, file_path: str) -> None:
+        """
+        Saves self.output_kg to a file
+        Args:
+            file_path: path of the output file
+        """
+        dir_path = os.path.dirname(file_path)
+        os.makedirs(dir_path, exist_ok=True)
+
+        self.output_kg.serialize(destination=file_path)
+        print(f"Executable KG saved in {file_path}")
+
+    def _property_value_to_field_value(self, property_value: str) -> Union[str, DataEntity]:
+        """
+        Converts property value to Python class field value
+        If property_value is not a data entity's IRI, it is returned as is
+        Else, its property values are converted recursively and stored in a DataEntity object
+        Args:
+            property_value: value of the property as found in KG
+
+        Returns:
+            str: property_value parameter as is
+            DataEntity: object containing parsed data entity properties
+        """
+        if "#" in property_value:
+            data_entity = self._parse_data_entity_by_iri(property_value)
+            if data_entity is None:
+                return property_value
+            return data_entity
+
+        return property_value
+
+    def _parse_data_entity_by_iri(self, in_out_data_entity_iri: str) -> Optional[DataEntity]:
+        """
+        Parses an input or output data entity of self.input_kg and stores the parsed info in a Python object
+        Args:
+            in_out_data_entity_iri: IRI of the KG entity to parse
+
+        Returns:
+            None: if given IRI does not belong to an instance of a sub-class of self.top_level_schema.namespace.DataEntity
+            DataEntity: object with data entity's parsed properties
+        """
+        # fetch type of entity with given IRI
+        query_result = get_first_query_result_if_exists(
+            query_entity_parent_iri,
+            self.input_kg,
+            in_out_data_entity_iri,
+            self.top_level_schema.namespace.DataEntity,
+        )
+        if query_result is None:
+            return None
+
+        data_entity_parent_iri = str(query_result[0])
+
+        # fetch IRI of data entity that is referenced by the given entity
+        query_result = get_first_query_result_if_exists(
+            query_data_entity_reference_iri,
+            self.input_kg,
+            self.top_level_schema.namespace_prefix,
+            in_out_data_entity_iri,
+        )
+
+        if query_result is None:  # no referenced data entity found
+            data_entity_ref_iri = in_out_data_entity_iri
+        else:
+            data_entity_ref_iri = str(query_result[0])
+
+        # create DataEntity object to store all the parsed properties
+        data_entity = DataEntity(in_out_data_entity_iri, Entity(data_entity_parent_iri))
+        data_entity.has_reference = data_entity_ref_iri.split("#")[1]
+
+        for s, p, o in self.input_kg.triples((URIRef(data_entity_ref_iri), None, None)):
+            # parse property name and value
+            field_name = property_name_to_field_name(str(p))
+            if not hasattr(data_entity, field_name) or field_name == "type":
+                continue
+            field_value = self._property_value_to_field_value(str(o))
+            setattr(data_entity, field_name, field_value)  # set field value dynamically
+
+        return data_entity
+
+    def _parse_task_by_iri(self, task_iri: str, canvas_method: visual_tasks.CanvasTaskCanvasMethod = None) -> Task:
+        """
+        Parses a task of self.input_kg and stores the info in an object of a sub-class of Task
+        The sub-class name and the object's fields are mapped dynamically based on the found KG components
+        Args:
+            task_iri: IRI of the task to be parsed
+            canvas_method: optional object to pass as argument for task object initialization
+
+        Returns:
+            Task: object of a sub-class of Task, containing all the parsed info
+        """
+        # fetch type of entity with given IRI
+        query_result = get_first_query_result_if_exists(
+            query_entity_parent_iri,
+            self.input_kg,
+            task_iri,
+            self.top_level_schema.namespace.AtomicTask,
+        )
+
+        if (
+            query_result is None
+        ):  # given IRI does not belong to an instance of a sub-class of self.top_level_schema.namespace.AtomicTask
+            print(f"Cannot retrieve parent of task with iri {task_iri}. Exiting...")
+            exit(1)
+
+        task_parent_iri = str(query_result[0])
+
+        task = Task(task_iri, Task(task_parent_iri))
+        method = get_method_by_task_iri(
+            self.input_kg,
+            self.top_level_schema.namespace_prefix,
+            self.top_level_schema.namespace,
+            task_iri,
+        )
+        if method is None:
+            print(f"Cannot retrieve method for task with iri: {task_iri}")
+
+        # perform automatic mapping of KG task class to Python sub-class
+        class_name = task.type + method.type
+        Class = getattr(visual_tasks, class_name, None)
+        if Class is None:
+            Class = getattr(statistic_tasks, class_name, None)
+        if Class is None:
+            Class = getattr(ml_tasks, class_name, None)
+
+        # create Task sub-class object
+        if canvas_method:
+            task = Class(task_iri, Task(task_parent_iri), canvas_method)
+        else:
+            task = Class(task_iri, Task(task_parent_iri))
+
+        for s, p, o in self.input_kg.triples((URIRef(task_iri), None, None)):
+            # parse property name and value
+            field_name = property_name_to_field_name(str(p))
+            if not hasattr(task, field_name) or field_name == "type":
+                continue
+            field_value = self._property_value_to_field_value(str(o))
+
+            # set field value dynamically
+            if field_name == "has_input" or field_name == "has_output":
+                getattr(task, field_name).append(field_value)
+            else:
+                setattr(task, field_name, field_value)
+
+        return task
+
+    def execute_pipeline(self):
+        """
+        Retrieves and executes pipeline by parsing self.input_kg
+        """
+        pipeline_iri, input_data_path, next_task_iri = get_pipeline_and_first_task_iri(
+            self.input_kg, self.top_level_schema.namespace_prefix
+        )
+        input_data = pd.read_csv(input_data_path, delimiter=",", encoding="ISO-8859-1")
+        canvas_method = None  # stores Task object that corresponds to a task of type CanvasTask
+        task_output_dict = {}  # gradually filled with outputs of executed tasks
+        while next_task_iri is not None:
+            next_task = self._parse_task_by_iri(next_task_iri, canvas_method)
+            output = next_task.run_method(task_output_dict, input_data)
+            if output:
+                task_output_dict.update(output)
+
+            if next_task.type == "CanvasTask":
+                canvas_method = next_task
+
+            next_task_iri = next_task.has_next_task
```

### Comparing `exe_kg_lib-2.0.2/exe_kg_lib/classes/kg_schema.py` & `exe_kg_lib-2.0.3/exe_kg_lib/classes/kg_schema.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# Copyright (c) 2022 Robert Bosch GmbH
-# SPDX-License-Identifier: AGPL-3.0
-
-from typing import Dict
-
-from rdflib import Graph, Namespace
-
-
-class KGSchema:
-    """
-    Stores a Graph object and some metadata corresponding to a KG schema
-    """
-
-    def __init__(self, path: str, namespace: str, namespace_prefix: str):
-        self.path = path  # path of the KG schema definition, can be local or remote
-        self.namespace = Namespace(namespace)
-        self.namespace_prefix = namespace_prefix
-
-        self.kg = Graph(bind_namespaces="rdflib")
-        self.kg.parse(self.path, format="n3")
-
-    @classmethod
-    def from_schema_info(cls, schema_info: Dict[str, str]):
-        return cls(schema_info["path"], schema_info["namespace"], schema_info["namespace_prefix"])
+# Copyright (c) 2022 Robert Bosch GmbH
+# SPDX-License-Identifier: AGPL-3.0
+
+from typing import Dict
+
+from rdflib import Graph, Namespace
+
+
+class KGSchema:
+    """
+    Stores a Graph object and some metadata corresponding to a KG schema
+    """
+
+    def __init__(self, path: str, namespace: str, namespace_prefix: str):
+        self.path = path  # path of the KG schema definition, can be local or remote
+        self.namespace = Namespace(namespace)
+        self.namespace_prefix = namespace_prefix
+
+        self.kg = Graph(bind_namespaces="rdflib")
+        self.kg.parse(self.path, format="n3")
+
+    @classmethod
+    def from_schema_info(cls, schema_info: Dict[str, str]):
+        return cls(schema_info["path"], schema_info["namespace"], schema_info["namespace_prefix"])
```

### Comparing `exe_kg_lib-2.0.2/exe_kg_lib/classes/task.py` & `exe_kg_lib-2.0.3/exe_kg_lib/classes/task.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-# Copyright (c) 2022 Robert Bosch GmbH
-# SPDX-License-Identifier: AGPL-3.0
-
-from abc import abstractmethod
-from typing import Dict
-
-import numpy as np
-import pandas as pd
-
-from .entity import Entity
-
-
-class Task(Entity):
-    """
-    Abstraction of owl:class Task.
-
-    ❗ Important for contributors ❗
-    The fields that contain "_" are by convention the snake-case conversions of the equivalent camel-case property names in the KG.
-    e.g. has_next_task field corresponds to hasNextTask property in the KG.
-    This is necessary for automatically mapping KG properties to Python object fields while parsing the KG.
-    """
-
-    def __init__(
-        self,
-        iri: str,
-        parent_entity: Entity = None,
-    ):
-        super().__init__(iri, parent_entity)
-        self.has_next_task = None
-        self.has_method = None
-        self.has_input = []
-        self.has_output = []
-        self.input_dict = {}  # used for storing input DataEntity objects during KG creation
-        self.output_dict = {}  # used for storing output DataEntity objects during KG creation
-
-    @classmethod
-    def from_entity(cls, entity: Entity):
-        return cls(entity.iri, entity.parent_entity)
-
-    def create_output_dict(self, keyword_value_dict: dict) -> dict:
-        """
-        For each key in keyword_value_dict, checks if the key exists in an output name of the Task.
-        If yes, adds the output name with its value to out_dict.
-        Args:
-            keyword_value_dict: key-value pairs where key is a keyword to find in an output name of the Task
-                                  and value is the value corresponding to that output name
-
-        Returns:
-            dict: pairs of Task's output names and corresponding output values
-        """
-        if len(self.has_output) == 0:
-            # assume one output and use task name as key
-            return {self.name: list(keyword_value_dict.values())[0]}
-
-        output_names = [has_output_elem.name for has_output_elem in self.has_output]
-        out_dict = {}
-        for output_name in output_names:
-            for key, value in keyword_value_dict.items():
-                if key in output_name:
-                    out_dict[output_name] = value
-
-        return out_dict
-
-    def get_inputs(self, dict_to_search: dict, fallback_df: pd.DataFrame) -> Dict[str, np.ndarray]:
-        """
-        Tries to match the Task's input names with the keys of dict_to_search
-        and fills input_dict list with their corresponding values.
-        If the matches fail, it retrieves columns of the provided fallback_df
-        Args:
-            dict_to_search: contains key-value pairs where key is a possible input name and value is its corresponding value
-            fallback_df: contains data to return as an alternative
-
-        Returns:
-            Dict[str, np.ndarray]: pairs of input entity types and corresponding input values
-        """
-        input_dict = {}
-        for input in self.has_input:
-            try:
-                input_dict[input.type] = dict_to_search[input.has_reference]
-            except KeyError:
-                input_dict[input.type] = fallback_df[input.has_source]
-
-        return input_dict
-
-    @abstractmethod
-    def run_method(self, *args):
-        """
-        Abstract method to be implemented by Task sub-classes that are in the bottom of the hierarchy.
-        Executes the logic that is needed to fulfill the Task.
-        Args:
-            *args: defined by sub-classes
-        """
-        raise NotImplementedError
+# Copyright (c) 2022 Robert Bosch GmbH
+# SPDX-License-Identifier: AGPL-3.0
+
+from abc import abstractmethod
+from typing import Dict
+
+import numpy as np
+import pandas as pd
+
+from .entity import Entity
+
+
+class Task(Entity):
+    """
+    Abstraction of owl:class Task.
+
+    ❗ Important for contributors ❗
+    The fields that contain "_" are by convention the snake-case conversions of the equivalent camel-case property names in the KG.
+    e.g. has_next_task field corresponds to hasNextTask property in the KG.
+    This is necessary for automatically mapping KG properties to Python object fields while parsing the KG.
+    """
+
+    def __init__(
+        self,
+        iri: str,
+        parent_entity: Entity = None,
+    ):
+        super().__init__(iri, parent_entity)
+        self.has_next_task = None
+        self.has_method = None
+        self.has_input = []
+        self.has_output = []
+        self.input_dict = {}  # used for storing input DataEntity objects during KG creation
+        self.output_dict = {}  # used for storing output DataEntity objects during KG creation
+
+    @classmethod
+    def from_entity(cls, entity: Entity):
+        return cls(entity.iri, entity.parent_entity)
+
+    def create_output_dict(self, keyword_value_dict: dict) -> dict:
+        """
+        For each key in keyword_value_dict, checks if the key exists in an output name of the Task.
+        If yes, adds the output name with its value to out_dict.
+        Args:
+            keyword_value_dict: key-value pairs where key is a keyword to find in an output name of the Task
+                                  and value is the value corresponding to that output name
+
+        Returns:
+            dict: pairs of Task's output names and corresponding output values
+        """
+        if len(self.has_output) == 0:
+            # assume one output and use task name as key
+            return {self.name: list(keyword_value_dict.values())[0]}
+
+        output_names = [has_output_elem.name for has_output_elem in self.has_output]
+        out_dict = {}
+        for output_name in output_names:
+            for key, value in keyword_value_dict.items():
+                if key in output_name:
+                    out_dict[output_name] = value
+
+        return out_dict
+
+    def get_inputs(self, dict_to_search: dict, fallback_df: pd.DataFrame) -> Dict[str, np.ndarray]:
+        """
+        Tries to match the Task's input names with the keys of dict_to_search
+        and fills input_dict list with their corresponding values.
+        If the matches fail, it retrieves columns of the provided fallback_df
+        Args:
+            dict_to_search: contains key-value pairs where key is a possible input name and value is its corresponding value
+            fallback_df: contains data to return as an alternative
+
+        Returns:
+            Dict[str, np.ndarray]: pairs of input entity types and corresponding input values
+        """
+        input_dict = {}
+        for input in self.has_input:
+            try:
+                input_dict[input.type] = dict_to_search[input.has_reference]
+            except KeyError:
+                input_dict[input.type] = fallback_df[input.has_source]
+
+        return input_dict
+
+    @abstractmethod
+    def run_method(self, *args):
+        """
+        Abstract method to be implemented by Task sub-classes that are in the bottom of the hierarchy.
+        Executes the logic that is needed to fulfill the Task.
+        Args:
+            *args: defined by sub-classes
+        """
+        raise NotImplementedError
```

### Comparing `exe_kg_lib-2.0.2/exe_kg_lib/classes/tasks/ml_tasks.py` & `exe_kg_lib-2.0.3/exe_kg_lib/classes/tasks/ml_tasks.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-# Copyright (c) 2022 Robert Bosch GmbH
-# SPDX-License-Identifier: AGPL-3.0
-
-from ...utils.task_utils.ml_utils import *
-from ..entity import Entity
-from ..task import Task
-
-"""
-❗ Important for contributors: See the package's README.md before extending the code's functionality.
-"""
-
-
-class ConcatenationConcatenationMethod(Task):
-    def __init__(self, iri: str, parent_entity: Entity):
-        super().__init__(iri, parent_entity)
-
-    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
-        input_dict = self.get_inputs(other_task_output_dict, input_data)
-        concatenation_result = concatenation(list(input_dict.values()))
-        return self.create_output_dict({"DataOutConcatenatedData": concatenation_result})
-
-
-class DataSplittingDataSplittingMethod(Task):
-    def __init__(self, iri: str, parent_entity: Entity):
-        super().__init__(iri, parent_entity)
-        self.has_split_ratio = None
-
-    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
-        input_dict = self.get_inputs(other_task_output_dict, input_data)
-        input_x = input_dict["DataInDataSplittingX"]
-        input_y = input_dict["DataInDataSplittingY"]
-        train_x, test_x, train_y, test_y = data_splitting(input_x, input_y, self.has_split_ratio)
-
-        return self.create_output_dict(
-            {
-                "DataOutSplittedTrainDataX": train_x,
-                "DataOutSplittedTestDataX": test_x,
-                "DataOutSplittedTrainDataY": train_y,
-                "DataOutSplittedTestDataY": test_y,
-            }
-        )
-
-
-class TrainKNNTrain(Task):
-    def __init__(self, iri: str, parent_entity: Entity):
-        super().__init__(iri, parent_entity)
-
-    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
-        input_dict = self.get_inputs(other_task_output_dict, input_data)
-        input_x = input_dict["DataInTrainX"]
-        input_y = input_dict["DataInTrainY"]
-        model, predicted_y = k_nn_train(input_x, input_y)
-
-        return self.create_output_dict({"DataOutTrainModel": model, "DataOutPredictedValueTrain": predicted_y})
-
-
-class TestKNNTest(Task):
-    def __init__(self, iri: str, parent_entity: Entity):
-        super().__init__(iri, parent_entity)
-
-    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
-        input_dict = self.get_inputs(other_task_output_dict, input_data)
-        model = input_dict["DataInTestModel"]
-        input_x = input_dict["DataInTestX"]
-
-        predicted_y = k_nn_test(model, input_x)
-        return self.create_output_dict({"DataOutPredictedValueTest": predicted_y})
-
-
-class TrainLRTrain(Task):
-    def __init__(self, iri: str, parent_entity: Entity):
-        super().__init__(iri, parent_entity)
-
-    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
-        input_dict = self.get_inputs(other_task_output_dict, input_data)
-        input_x = input_dict["DataInTrainX"]
-        input_y = input_dict["DataInTrainY"]
-
-        model, predicted_y = lr_training(input_x, input_y)
-
-        return self.create_output_dict({"DataOutModel": model, "DataOutPredictedValueTrain": predicted_y})
-
-
-class TestLRTest(Task):
-    def __init__(self, iri: str, parent_entity: Entity):
-        super().__init__(iri, parent_entity)
-
-    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
-        input_dict = self.get_inputs(other_task_output_dict, input_data)
-        model = input_dict["DataInModel"]
-        input_x = input_dict["DataInTestX"]
-
-        predicted_y = lr_testing(model, input_x)
-        return self.create_output_dict({"DataOutPredictedValueTest": predicted_y})
-
-
-class TrainMLPTrain(Task):
-    def __init__(self, iri: str, parent_entity: Entity):
-        super().__init__(iri, parent_entity)
-
-    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
-        input_dict = self.get_inputs(other_task_output_dict, input_data)
-        input_x = input_dict["DataInTrainX"]
-        input_y = input_dict["DataInTrainY"]
-
-        model, predicted_y = mlp_train(input_x, input_y)
-
-        return self.create_output_dict({"DataOutModel": model, "DataOutPredictedValueTrain": predicted_y})
-
-
-class TestMLPTest(Task):
-    def __init__(self, iri: str, parent_entity: Entity):
-        super().__init__(iri, parent_entity)
-
-    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
-        input_dict = self.get_inputs(other_task_output_dict, input_data)
-        model = input_dict["DataInModel"]
-        input_x = input_dict["DataInTestX"]
-
-        predicted_y = mlp_test(model, input_x)
-        return self.create_output_dict({"DataOutPredictedValueTest": predicted_y})
-
-
-class PerformanceCalculationPerformanceCalculationMethod(Task):
-    def __init__(self, iri: str, parent_entity: Entity):
-        super().__init__(iri, parent_entity)
-
-    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
-        input_dict = self.get_inputs(other_task_output_dict, input_data)
-        real_train_y = input_dict["DataInTrainRealY"]
-        real_test_y = input_dict["DataInTestRealY"]
-        predicted_train_y = input_dict["DataInTrainPredictedY"]
-        predicted_test_y = input_dict["DataInTestPredictedY"]
-
-        train_error, test_error = ml_performance_calculation(
-            real_train_y, real_test_y, predicted_train_y, predicted_test_y
-        )
-
-        return self.create_output_dict({"DataOutMLTrainErr": train_error, "DataOutMLTestErr": test_error})
+# Copyright (c) 2022 Robert Bosch GmbH
+# SPDX-License-Identifier: AGPL-3.0
+
+from ...utils.task_utils.ml_utils import *
+from ..entity import Entity
+from ..task import Task
+
+"""
+❗ Important for contributors: See the package's README.md before extending the code's functionality.
+"""
+
+
+class ConcatenationConcatenationMethod(Task):
+    def __init__(self, iri: str, parent_entity: Entity):
+        super().__init__(iri, parent_entity)
+
+    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
+        input_dict = self.get_inputs(other_task_output_dict, input_data)
+        concatenation_result = concatenation(list(input_dict.values()))
+        return self.create_output_dict({"DataOutConcatenatedData": concatenation_result})
+
+
+class DataSplittingDataSplittingMethod(Task):
+    def __init__(self, iri: str, parent_entity: Entity):
+        super().__init__(iri, parent_entity)
+        self.has_split_ratio = None
+
+    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
+        input_dict = self.get_inputs(other_task_output_dict, input_data)
+        input_x = input_dict["DataInDataSplittingX"]
+        input_y = input_dict["DataInDataSplittingY"]
+        train_x, test_x, train_y, test_y = data_splitting(input_x, input_y, self.has_split_ratio)
+
+        return self.create_output_dict(
+            {
+                "DataOutSplittedTrainDataX": train_x,
+                "DataOutSplittedTestDataX": test_x,
+                "DataOutSplittedTrainDataY": train_y,
+                "DataOutSplittedTestDataY": test_y,
+            }
+        )
+
+
+class TrainKNNTrain(Task):
+    def __init__(self, iri: str, parent_entity: Entity):
+        super().__init__(iri, parent_entity)
+
+    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
+        input_dict = self.get_inputs(other_task_output_dict, input_data)
+        input_x = input_dict["DataInTrainX"]
+        input_y = input_dict["DataInTrainY"]
+        model, predicted_y = k_nn_train(input_x, input_y)
+
+        return self.create_output_dict({"DataOutTrainModel": model, "DataOutPredictedValueTrain": predicted_y})
+
+
+class TestKNNTest(Task):
+    def __init__(self, iri: str, parent_entity: Entity):
+        super().__init__(iri, parent_entity)
+
+    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
+        input_dict = self.get_inputs(other_task_output_dict, input_data)
+        model = input_dict["DataInTestModel"]
+        input_x = input_dict["DataInTestX"]
+
+        predicted_y = k_nn_test(model, input_x)
+        return self.create_output_dict({"DataOutPredictedValueTest": predicted_y})
+
+
+class TrainLRTrain(Task):
+    def __init__(self, iri: str, parent_entity: Entity):
+        super().__init__(iri, parent_entity)
+
+    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
+        input_dict = self.get_inputs(other_task_output_dict, input_data)
+        input_x = input_dict["DataInTrainX"]
+        input_y = input_dict["DataInTrainY"]
+
+        model, predicted_y = lr_training(input_x, input_y)
+
+        return self.create_output_dict({"DataOutModel": model, "DataOutPredictedValueTrain": predicted_y})
+
+
+class TestLRTest(Task):
+    def __init__(self, iri: str, parent_entity: Entity):
+        super().__init__(iri, parent_entity)
+
+    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
+        input_dict = self.get_inputs(other_task_output_dict, input_data)
+        model = input_dict["DataInModel"]
+        input_x = input_dict["DataInTestX"]
+
+        predicted_y = lr_testing(model, input_x)
+        return self.create_output_dict({"DataOutPredictedValueTest": predicted_y})
+
+
+class TrainMLPTrain(Task):
+    def __init__(self, iri: str, parent_entity: Entity):
+        super().__init__(iri, parent_entity)
+
+    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
+        input_dict = self.get_inputs(other_task_output_dict, input_data)
+        input_x = input_dict["DataInTrainX"]
+        input_y = input_dict["DataInTrainY"]
+
+        model, predicted_y = mlp_train(input_x, input_y)
+
+        return self.create_output_dict({"DataOutModel": model, "DataOutPredictedValueTrain": predicted_y})
+
+
+class TestMLPTest(Task):
+    def __init__(self, iri: str, parent_entity: Entity):
+        super().__init__(iri, parent_entity)
+
+    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
+        input_dict = self.get_inputs(other_task_output_dict, input_data)
+        model = input_dict["DataInModel"]
+        input_x = input_dict["DataInTestX"]
+
+        predicted_y = mlp_test(model, input_x)
+        return self.create_output_dict({"DataOutPredictedValueTest": predicted_y})
+
+
+class PerformanceCalculationPerformanceCalculationMethod(Task):
+    def __init__(self, iri: str, parent_entity: Entity):
+        super().__init__(iri, parent_entity)
+
+    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
+        input_dict = self.get_inputs(other_task_output_dict, input_data)
+        real_train_y = input_dict["DataInTrainRealY"]
+        real_test_y = input_dict["DataInTestRealY"]
+        predicted_train_y = input_dict["DataInTrainPredictedY"]
+        predicted_test_y = input_dict["DataInTestPredictedY"]
+
+        train_error, test_error = ml_performance_calculation(
+            real_train_y, real_test_y, predicted_train_y, predicted_test_y
+        )
+
+        return self.create_output_dict({"DataOutMLTrainErr": train_error, "DataOutMLTestErr": test_error})
```

### Comparing `exe_kg_lib-2.0.2/exe_kg_lib/classes/tasks/README.md` & `exe_kg_lib-2.0.3/exe_kg_lib/classes/tasks/README.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-## Documentation of `exe_kg_lib.classes.tasks` package
-
-[//]: # (--8<-- [start:content])
-### Overview
-
-This package contains classes that correspond to entities of type `owl:class` that are `rdfs:subClassOf AtomicTask` in
-the KG.
-
-They implement the abstract `run_method()` like so:
-
-1. The input is taken either from outputs of previously executed Tasks (parameter: `other_task_output_dict`) or a
-   dataframe (parameter: `input_data`).
-2. An algorithm is executed using the input.
-
-   There are two conventions:
-    - The algorithm is related to ML, Statistics or Visualization, depending on
-      the Python file's prefix.
-    - The algorithm's implementation is placed in `utils.task_utils` package in the Python file with the corresponding prefix.
-3. The output is returned as a dictionary with pairs of output name and value.
-
-### Naming conventions
-
-- Each class name is a concatenation of 2 strings:
-    1. The name of an `owl:class` that is `rdfs:subClassOf AtomicTask`.
-    2. The name of an `owl:class` that is `rdfs:subClassOf AtomicMethod` and is associated with the above `owl:class` via a property that is `rdfs:subPropertyOf hasMethod`.
-
-    For example, the below KG property associates `CanvasMethod` with `CanvasTask`. So, the corresponding class name will be `CanvasTaskCanvasMethod`.
-    ```turtle
-    visu:hasCanvasMethod
-        a                  owl:ObjectProperty ;
-        rdfs:domain        visu:CanvasTask ;
-        rdfs:range         visu:CanvasMethod ;
-        rdfs:subPropertyOf ds:hasMethod .
-    ```
-
-- The class fields that contain `_` are the snake-case conversions of the equivalent camel-case property names in the
-  KG.
-
-  e.g. `has_split_ratio` field corresponds to `hasSplitRatio` property in the KG.
-
-The above conventions are necessary for automatically mapping KG tasks with methods and properties to Python objects while parsing the KG.
-
-[//]: # (--8<-- [end:content])
+## Documentation of `exe_kg_lib.classes.tasks` package
+
+[//]: # (--8<-- [start:content])
+### Overview
+
+This package contains classes that correspond to entities of type `owl:class` that are `rdfs:subClassOf AtomicTask` in
+the KG.
+
+They implement the abstract `run_method()` like so:
+
+1. The input is taken either from outputs of previously executed Tasks (parameter: `other_task_output_dict`) or a
+   dataframe (parameter: `input_data`).
+2. An algorithm is executed using the input.
+
+   There are two conventions:
+    - The algorithm is related to ML, Statistics or Visualization, depending on
+      the Python file's prefix.
+    - The algorithm's implementation is placed in `utils.task_utils` package in the Python file with the corresponding prefix.
+3. The output is returned as a dictionary with pairs of output name and value.
+
+### Naming conventions
+
+- Each class name is a concatenation of 2 strings:
+    1. The name of an `owl:class` that is `rdfs:subClassOf AtomicTask`.
+    2. The name of an `owl:class` that is `rdfs:subClassOf AtomicMethod` and is associated with the above `owl:class` via a property that is `rdfs:subPropertyOf hasMethod`.
+
+    For example, the below KG property associates `CanvasMethod` with `CanvasTask`. So, the corresponding class name will be `CanvasTaskCanvasMethod`.
+    ```turtle
+    visu:hasCanvasMethod
+        a                  owl:ObjectProperty ;
+        rdfs:domain        visu:CanvasTask ;
+        rdfs:range         visu:CanvasMethod ;
+        rdfs:subPropertyOf ds:hasMethod .
+    ```
+
+- The class fields that contain `_` are the snake-case conversions of the equivalent camel-case property names in the
+  KG.
+
+  e.g. `has_split_ratio` field corresponds to `hasSplitRatio` property in the KG.
+
+The above conventions are necessary for automatically mapping KG tasks with methods and properties to Python objects while parsing the KG.
+
+[//]: # (--8<-- [end:content])
```

### Comparing `exe_kg_lib-2.0.2/exe_kg_lib/classes/tasks/statistic_tasks.py` & `exe_kg_lib-2.0.3/exe_kg_lib/classes/tasks/statistic_tasks.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-# Copyright (c) 2022 Robert Bosch GmbH
-# SPDX-License-Identifier: AGPL-3.0
-
-from ...utils.task_utils.statistic_utils import *
-from ..entity import Entity
-from ..task import Task
-
-"""
-❗ Important for contributors: See the package's README.md before extending the code's functionality.
-"""
-
-
-class TrendCalculationTaskTrendCalculationMethod(Task):
-    def __init__(self, iri: str, parent_entity: Entity):
-        super().__init__(iri, parent_entity)
-
-    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
-        input_dict = self.get_inputs(other_task_output_dict, input_data)
-        input_data = list(input_dict.values())[0]  # one input expected
-        trend_calculation_result = trend_calculation(input_data)
-
-        return self.create_output_dict({"DataOutTrendCalculation": trend_calculation_result})
-
-
-class ScatteringCalculationTaskScatteringCalculationMethod(Task):
-    def __init__(self, iri: str, parent_entity: Entity):
-        super().__init__(iri, parent_entity)
-
-    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
-        input_dict = self.get_inputs(other_task_output_dict, input_data)
-        input_data = list(input_dict.values())[0]  # one input expected
-        scattering_calculation_result = scattering_calculation(input_data)
-
-        return self.create_output_dict({"DataOutScatteringCalculation": scattering_calculation_result})
-
-
-class NormalizationTaskNormalizationMethod(Task):
-    def __init__(self, iri: str, parent_entity: Entity):
-        super().__init__(iri, parent_entity)
-
-    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
-        input_dict = self.get_inputs(other_task_output_dict, input_data)
-        input_data = list(input_dict.values())[0]  # one input expected
-        normalization_result = normalization(input_data)
-
-        return self.create_output_dict({"DataOutNormalization": normalization_result})
+# Copyright (c) 2022 Robert Bosch GmbH
+# SPDX-License-Identifier: AGPL-3.0
+
+from ...utils.task_utils.statistic_utils import *
+from ..entity import Entity
+from ..task import Task
+
+"""
+❗ Important for contributors: See the package's README.md before extending the code's functionality.
+"""
+
+
+class TrendCalculationTaskTrendCalculationMethod(Task):
+    def __init__(self, iri: str, parent_entity: Entity):
+        super().__init__(iri, parent_entity)
+
+    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
+        input_dict = self.get_inputs(other_task_output_dict, input_data)
+        input_data = list(input_dict.values())[0]  # one input expected
+        trend_calculation_result = trend_calculation(input_data)
+
+        return self.create_output_dict({"DataOutTrendCalculation": trend_calculation_result})
+
+
+class ScatteringCalculationTaskScatteringCalculationMethod(Task):
+    def __init__(self, iri: str, parent_entity: Entity):
+        super().__init__(iri, parent_entity)
+
+    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
+        input_dict = self.get_inputs(other_task_output_dict, input_data)
+        input_data = list(input_dict.values())[0]  # one input expected
+        scattering_calculation_result = scattering_calculation(input_data)
+
+        return self.create_output_dict({"DataOutScatteringCalculation": scattering_calculation_result})
+
+
+class NormalizationTaskNormalizationMethod(Task):
+    def __init__(self, iri: str, parent_entity: Entity):
+        super().__init__(iri, parent_entity)
+
+    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame) -> dict:
+        input_dict = self.get_inputs(other_task_output_dict, input_data)
+        input_data = list(input_dict.values())[0]  # one input expected
+        normalization_result = normalization(input_data)
+
+        return self.create_output_dict({"DataOutNormalization": normalization_result})
```

### Comparing `exe_kg_lib-2.0.2/exe_kg_lib/classes/tasks/visual_tasks.py` & `exe_kg_lib-2.0.3/exe_kg_lib/classes/tasks/visual_tasks.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-# Copyright (c) 2022 Robert Bosch GmbH
-# SPDX-License-Identifier: AGPL-3.0
-
-from abc import abstractmethod
-
-from ...utils.task_utils.visual_utils import *
-from ..entity import Entity
-from ..task import Task
-
-"""
-❗ Important for contributors: See the package's README.md before extending the code's functionality.
-"""
-
-
-class CanvasTaskCanvasMethod(Task):
-    def __init__(self, iri: str, parent_entity: Entity):
-        super().__init__(iri, parent_entity)
-        self.grid = None
-        self.fig = None
-        self.has_layout = None
-        self.has_canvas_name = None
-
-    def run_method(self, *args):
-        self.fig, self.grid = canvas_creation(self.has_layout)
-
-        return None
-
-
-class PlotTask(Task):
-    def __init__(self, iri: str, parent_entity: Entity, canvas_method: CanvasTaskCanvasMethod):
-        super().__init__(iri, parent_entity)
-        self.fig = canvas_method.fig
-        self.grid = canvas_method.grid
-
-        self.has_legend_name = None
-        self.has_layout = None
-        self.has_y_label = None
-        self.has_x_label = None
-        self.has_y_lim = None
-        self.has_x_lim = None
-        self.has_line_style = None
-        self.has_line_width = 1
-
-    @abstractmethod
-    def run_method(self, *args):
-        raise NotImplementedError
-
-
-class PlotTaskScatterplotMethod(PlotTask):
-    def __init__(self, iri: str, parent_entity: Entity, canvas_method: CanvasTaskCanvasMethod):
-        super().__init__(iri, parent_entity, canvas_method)
-        self.has_scatter_size = None
-        self.has_scatter_style = None
-
-    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame):
-        input_dict = self.get_inputs(other_task_output_dict, input_data)
-        input_data = list(input_dict.values())[0]  # one input expected
-        scatter_plot(
-            data=input_data,
-            fig=self.fig,
-            grid=self.grid,
-            layout=self.has_layout,
-            line_width=self.has_line_width,
-            line_style=self.has_line_style,
-            legend_name=self.has_legend_name,
-            x_lim=self.has_x_lim,
-            y_lim=self.has_y_lim,
-            x_label=self.has_x_label,
-            y_label=self.has_y_label,
-        )
-
-        return None
-
-
-class PlotTaskLineplotMethod(PlotTask):
-    def __init__(self, iri: str, parent_entity: Entity, canvas_method: CanvasTaskCanvasMethod):
-        super().__init__(iri, parent_entity, canvas_method)
-
-    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame):
-        input_dict = self.get_inputs(other_task_output_dict, input_data)
-        input_data = list(input_dict.values())[0]  # one input expected
-        line_plot(
-            data=input_data,
-            fig=self.fig,
-            grid=self.grid,
-            layout=self.has_layout,
-            line_width=self.has_line_width,
-            line_style=self.has_line_style,
-            legend_name=self.has_legend_name,
-            x_lim=self.has_x_lim,
-            y_lim=self.has_y_lim,
-            x_label=self.has_x_label,
-            y_label=self.has_y_label,
-        )
-
-        return None
+# Copyright (c) 2022 Robert Bosch GmbH
+# SPDX-License-Identifier: AGPL-3.0
+
+from abc import abstractmethod
+
+from ...utils.task_utils.visual_utils import *
+from ..entity import Entity
+from ..task import Task
+
+"""
+❗ Important for contributors: See the package's README.md before extending the code's functionality.
+"""
+
+
+class CanvasTaskCanvasMethod(Task):
+    def __init__(self, iri: str, parent_entity: Entity):
+        super().__init__(iri, parent_entity)
+        self.grid = None
+        self.fig = None
+        self.has_layout = None
+        self.has_canvas_name = None
+
+    def run_method(self, *args):
+        self.fig, self.grid = canvas_creation(self.has_layout)
+
+        return None
+
+
+class PlotTask(Task):
+    def __init__(self, iri: str, parent_entity: Entity, canvas_method: CanvasTaskCanvasMethod):
+        super().__init__(iri, parent_entity)
+        self.fig = canvas_method.fig
+        self.grid = canvas_method.grid
+
+        self.has_legend_name = None
+        self.has_layout = None
+        self.has_y_label = None
+        self.has_x_label = None
+        self.has_y_lim = None
+        self.has_x_lim = None
+        self.has_line_style = None
+        self.has_line_width = 1
+
+    @abstractmethod
+    def run_method(self, *args):
+        raise NotImplementedError
+
+
+class PlotTaskScatterplotMethod(PlotTask):
+    def __init__(self, iri: str, parent_entity: Entity, canvas_method: CanvasTaskCanvasMethod):
+        super().__init__(iri, parent_entity, canvas_method)
+        self.has_scatter_size = None
+        self.has_scatter_style = None
+
+    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame):
+        input_dict = self.get_inputs(other_task_output_dict, input_data)
+        input_data = list(input_dict.values())[0]  # one input expected
+        scatter_plot(
+            data=input_data,
+            fig=self.fig,
+            grid=self.grid,
+            layout=self.has_layout,
+            line_width=self.has_line_width,
+            line_style=self.has_line_style,
+            legend_name=self.has_legend_name,
+            x_lim=self.has_x_lim,
+            y_lim=self.has_y_lim,
+            x_label=self.has_x_label,
+            y_label=self.has_y_label,
+        )
+
+        return None
+
+
+class PlotTaskLineplotMethod(PlotTask):
+    def __init__(self, iri: str, parent_entity: Entity, canvas_method: CanvasTaskCanvasMethod):
+        super().__init__(iri, parent_entity, canvas_method)
+
+    def run_method(self, other_task_output_dict: dict, input_data: pd.DataFrame):
+        input_dict = self.get_inputs(other_task_output_dict, input_data)
+        input_data = list(input_dict.values())[0]  # one input expected
+        line_plot(
+            data=input_data,
+            fig=self.fig,
+            grid=self.grid,
+            layout=self.has_layout,
+            line_width=self.has_line_width,
+            line_style=self.has_line_style,
+            legend_name=self.has_legend_name,
+            x_lim=self.has_x_lim,
+            y_lim=self.has_y_lim,
+            x_label=self.has_x_label,
+            y_label=self.has_y_label,
+        )
+
+        return None
```

### Comparing `exe_kg_lib-2.0.2/exe_kg_lib/utils/cli_utils.py` & `exe_kg_lib-2.0.3/exe_kg_lib/utils/cli_utils.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-# Copyright (c) 2022 Robert Bosch GmbH
-# SPDX-License-Identifier: AGPL-3.0
-
-from typing import List, Tuple
-
-from rdflib import Namespace
-
-from ..classes.data_entity import DataEntity
-from ..classes.entity import Entity
-
-
-def get_input_for_existing_data_entities(
-    existing_data_entity_list: List[DataEntity],
-) -> List[DataEntity]:
-    """
-    Asks user to choose data entities from an existing list
-    Args:
-        existing_data_entity_list: contains DataEntity objects for the user to choose from
-
-    Returns:
-        List[DataEntity]: contains the chosen DataEntity objects
-    """
-    if not existing_data_entity_list:
-        return []
-
-    chosen_data_entity_list = []
-    print("Choose input for the task from existing data entities:")
-    while True:
-        for i, data_entity in enumerate(existing_data_entity_list):
-            print(f"\t{str(i)}. {data_entity.name}")
-        print(f"\t{str(-1)}. Continue")
-        chosen_data_entity_i = int(input())
-        if chosen_data_entity_i == -1:
-            break
-
-        chosen_data_entity_list.append(existing_data_entity_list[chosen_data_entity_i])
-
-    return chosen_data_entity_list
-
-
-def get_input_for_new_data_entities(
-    data_semantics_list: List[Entity], data_structure_list: List[Entity], namespace: Namespace, data_entity: Entity
-) -> List[DataEntity]:
-    """
-    Asks user to specify info of new data entities and creates relevant objects
-    Args:
-        data_semantics_list: contains data semantics for the user to choose from
-        data_structure_list: contains data structures for the user to choose from
-        namespace: KG schema namespace to use when initializing the new entities
-        data_entity: Entity object to assign as parent entity of the new entities
-
-    Returns:
-        List[DataEntity]: contains the created DataEntity objects
-    """
-    data_entities = []
-
-    prompt = "Enter input columns, then 'quit' when done: "
-    source = input(prompt)
-    while source != "quit":
-        new_data_entity = DataEntity(namespace + source, data_entity, source)
-
-        print(f"Choose data semantics for {source}:")
-        for i, t in enumerate(data_semantics_list):
-            print(f"\t{str(i)}. {t.name}")
-        chosen_data_semantics_id = int(input())
-        new_data_entity.has_data_semantics = data_semantics_list[chosen_data_semantics_id].iri
-
-        print(f"Choose data structure for {source}:")
-        for i, t in enumerate(data_structure_list):
-            print(f"\t{str(i)}. {t.name}")
-        chosen_data_structure_id = int(input())
-        new_data_entity.has_data_structure = data_structure_list[chosen_data_structure_id].iri
-
-        data_entities.append(new_data_entity)
-
-        source = input(prompt)
-
-    return data_entities
-
-
-def input_pipeline_info() -> Tuple[str, str]:
-    """
-    Asks user to provide a name for the pipeline and a path for the input data
-    Returns:
-        Tuple[str, str]: contains the provided strings
-    """
-    pipeline_name = input("Enter a name for the pipeline: ")
-    input_data_path = input("Enter a path for the input data: ")
-
-    return pipeline_name, input_data_path
+# Copyright (c) 2022 Robert Bosch GmbH
+# SPDX-License-Identifier: AGPL-3.0
+
+from typing import List, Tuple
+
+from rdflib import Namespace
+
+from ..classes.data_entity import DataEntity
+from ..classes.entity import Entity
+
+
+def get_input_for_existing_data_entities(
+    existing_data_entity_list: List[DataEntity],
+) -> List[DataEntity]:
+    """
+    Asks user to choose data entities from an existing list
+    Args:
+        existing_data_entity_list: contains DataEntity objects for the user to choose from
+
+    Returns:
+        List[DataEntity]: contains the chosen DataEntity objects
+    """
+    if not existing_data_entity_list:
+        return []
+
+    chosen_data_entity_list = []
+    print("Choose input for the task from existing data entities:")
+    while True:
+        for i, data_entity in enumerate(existing_data_entity_list):
+            print(f"\t{str(i)}. {data_entity.name}")
+        print(f"\t{str(-1)}. Continue")
+        chosen_data_entity_i = int(input())
+        if chosen_data_entity_i == -1:
+            break
+
+        chosen_data_entity_list.append(existing_data_entity_list[chosen_data_entity_i])
+
+    return chosen_data_entity_list
+
+
+def get_input_for_new_data_entities(
+    data_semantics_list: List[Entity], data_structure_list: List[Entity], namespace: Namespace, data_entity: Entity
+) -> List[DataEntity]:
+    """
+    Asks user to specify info of new data entities and creates relevant objects
+    Args:
+        data_semantics_list: contains data semantics for the user to choose from
+        data_structure_list: contains data structures for the user to choose from
+        namespace: KG schema namespace to use when initializing the new entities
+        data_entity: Entity object to assign as parent entity of the new entities
+
+    Returns:
+        List[DataEntity]: contains the created DataEntity objects
+    """
+    data_entities = []
+
+    prompt = "Enter input columns, then 'quit' when done: "
+    source = input(prompt)
+    while source != "quit":
+        new_data_entity = DataEntity(namespace + source, data_entity, source)
+
+        print(f"Choose data semantics for {source}:")
+        for i, t in enumerate(data_semantics_list):
+            print(f"\t{str(i)}. {t.name}")
+        chosen_data_semantics_id = int(input())
+        new_data_entity.has_data_semantics = data_semantics_list[chosen_data_semantics_id].iri
+
+        print(f"Choose data structure for {source}:")
+        for i, t in enumerate(data_structure_list):
+            print(f"\t{str(i)}. {t.name}")
+        chosen_data_structure_id = int(input())
+        new_data_entity.has_data_structure = data_structure_list[chosen_data_structure_id].iri
+
+        data_entities.append(new_data_entity)
+
+        source = input(prompt)
+
+    return data_entities
+
+
+def input_pipeline_info() -> Tuple[str, str]:
+    """
+    Asks user to provide a name for the pipeline and a path for the input data
+    Returns:
+        Tuple[str, str]: contains the provided strings
+    """
+    pipeline_name = input("Enter a name for the pipeline: ")
+    input_data_path = input("Enter a path for the input data: ")
+
+    return pipeline_name, input_data_path
```

### Comparing `exe_kg_lib-2.0.2/exe_kg_lib/utils/kg_creation_utils.py` & `exe_kg_lib-2.0.3/exe_kg_lib/utils/kg_creation_utils.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,220 +1,220 @@
-# Copyright (c) 2022 Robert Bosch GmbH
-# SPDX-License-Identifier: AGPL-3.0
-
-from typing import Dict, Union
-
-from rdflib import RDF, XSD, Graph, Literal, Namespace, URIRef
-
-from ..classes.data_entity import DataEntity
-from ..classes.entity import Entity
-from ..classes.task import Task
-from .query_utils import (get_data_properties_by_entity_iri,
-                          get_first_query_result_if_exists)
-
-
-def add_instance(kg: Graph, entity_instance: Entity) -> None:
-    """
-    Adds entity instance to KG only if its parent entity exists and there is no instance with the same IRI
-    Args:
-        kg: Graph object to add to
-        entity_instance: the entity instance to create
-    """
-    if entity_instance.parent_entity and (entity_instance.iri, None, None) not in kg:
-        kg.add((entity_instance.iri, RDF.type, entity_instance.parent_entity.iri))
-
-
-def add_relation(kg: Graph, from_entity: Entity, relation_iri: str, to_entity: Entity) -> None:
-    """
-    Adds relation between 2 given entities to KG
-    Args:
-        kg: Graph object to add to
-        from_entity: relation source
-        relation_iri: IRI that connects the 2 given entities
-        to_entity: relation destination
-    """
-    kg.add(
-        (
-            from_entity.iri,
-            URIRef(relation_iri),
-            to_entity.iri,
-        )
-    )
-
-
-def add_literal(kg: Graph, from_entity: Entity, relation_iri: str, literal: Literal) -> None:
-    """
-    Adds relation between a given entity and a given literal to KG
-    Args:
-        kg: Graph object to add to
-        from_entity: relation source
-        relation_iri: IRI that connects the given entity with the given literal
-        literal: literal to add to Graph object
-    """
-    kg.add((from_entity.iri, URIRef(relation_iri), literal))
-
-
-def add_instance_from_parent_with_relation(
-    namespace: Namespace,
-    kg: Graph,
-    parent_entity: Entity,
-    relation_iri: str,
-    related_entity: Entity,
-    instance_name: str,
-) -> Entity:
-    """
-    Creates an entity object based on the arguments and calls add_instance() and add_relation() to create a new entity instance and relation
-    Args:
-        namespace: namespace for the new instance
-        kg: Graph object to add to
-        parent_entity: parent entity for the new instance
-        relation_iri: IRI that connects the given related_entity with the new instance
-        related_entity: relation source
-        instance_name: name for the new instance
-
-    Returns:
-        Entity: object containing the new entity instance's basic info
-    """
-    entity_iri = namespace + instance_name
-    instance = Entity(entity_iri, parent_entity)
-
-    add_instance(kg, instance)
-    add_relation(kg, related_entity, relation_iri, instance)
-
-    return instance
-
-
-def name_instance(
-    task_type_dict: Dict[str, int],
-    method_type_dict: Dict[str, int],
-    parent_entity: Entity,
-) -> Union[None, str]:
-    """
-    Creates a unique name for a new instance by concatenating the parent entity's name (which is the instance type) with a number
-    Also increments the relevant number of the corresponding dict
-    Args:
-        task_type_dict: contains pairs of task types and numbers
-        method_type_dict: contains pairs of method types and numbers
-        parent_entity: instance's parent entity
-
-    Returns:
-        str: name to be given to the new instance
-        None: if the type of the given parent entity is not equal with "AtomicTask" or "AtomicMethod"
-    """
-    if parent_entity.type == "AtomicTask":
-        entity_type_dict = task_type_dict
-    elif parent_entity.type == "AtomicMethod":
-        entity_type_dict = method_type_dict
-    else:
-        print("Error: Invalid parent entity type")
-        return None
-
-    instance_name = parent_entity.name + str(entity_type_dict[parent_entity.name])
-    entity_type_dict[parent_entity.name] += 1
-    return instance_name
-
-
-def add_data_entity_instance(
-    kg: Graph,
-    data: Entity,
-    top_level_kg: Graph,
-    top_level_schema_namespace: Namespace,
-    data_entity: DataEntity,
-) -> None:
-    """
-    Adds data entity instance to kg with the necessary relations
-    Args:
-        kg: Graph object to add to
-        data: object representing top-level DataEntity class in KG
-        top_level_kg: KG corresponding to the top-level KG schema
-        top_level_schema_namespace: namespace of the top-level KG schema
-        data_entity: data entity to add
-    """
-    add_instance(kg, data_entity)
-
-    if data_entity.has_source:
-        has_source_iri, range_iri = get_first_query_result_if_exists(
-            get_data_properties_by_entity_iri, data.iri, top_level_kg
-        )
-
-        source_literal = Literal(
-            lexical_or_value=data_entity.has_source,
-            datatype=range_iri,
-        )
-
-        add_literal(kg, data_entity, has_source_iri, source_literal)
-
-    if data_entity.has_data_structure:
-        add_relation(
-            kg,
-            data_entity,
-            top_level_schema_namespace.hasDataStructure,
-            Entity(data_entity.has_data_structure),
-        )
-
-    if data_entity.has_data_semantics:
-        add_relation(
-            kg,
-            data_entity,
-            top_level_schema_namespace.hasDataSemantics,
-            Entity(data_entity.has_data_semantics),
-        )
-
-    if data_entity.has_reference:
-        add_relation(
-            kg,
-            data_entity,
-            top_level_schema_namespace.hasReference,
-            Entity(data_entity.has_reference),
-        )
-
-
-def add_and_attach_data_entity(
-    kg: Graph,
-    data: Entity,
-    top_level_kg: Graph,
-    top_level_schema_namespace: Namespace,
-    data_entity: DataEntity,
-    relation: URIRef,
-    task_entity: Task,
-) -> None:
-    """
-    Adds data entity instance to kg with the necessary relations, and attaches it to the given task
-    Args:
-        kg: Graph object to add to
-        data: object representing top-level DataEntity class in KG
-        top_level_kg: KG corresponding to the top-level KG schema
-        top_level_schema_namespace: namespace of the top-level KG schema
-        data_entity: data entity to add
-        relation: IRI of relation to add
-        task_entity: task to attach the data entity to
-    """
-    add_data_entity_instance(kg, data, top_level_kg, top_level_schema_namespace, data_entity)
-    add_relation(kg, task_entity, relation, data_entity)
-
-
-def create_pipeline_task(
-    top_level_schema_namespace: Namespace,
-    parent_entity: Entity,
-    kg: Graph,
-    pipeline_name: str,
-    input_data_path: str,
-) -> Task:
-    """
-    Adds instance of pipeline task to kg
-    Args:
-        top_level_schema_namespace: namespace of the top-level KG schema
-        parent_entity: parent entity of pipeline instance
-        kg: Graph object to add to
-        pipeline_name: name for the pipeline
-        input_data_path: path for the input data to be used by the pipeline's tasks
-
-    Returns:
-        Task: created pipeline task
-    """
-    pipeline = Task(top_level_schema_namespace + pipeline_name, parent_entity)
-    add_instance(kg, pipeline)
-
-    input_data_path_literal = Literal(lexical_or_value=input_data_path, datatype=XSD.string)
-    add_literal(kg, pipeline, top_level_schema_namespace.hasInputDataPath, input_data_path_literal)
-
-    return pipeline
+# Copyright (c) 2022 Robert Bosch GmbH
+# SPDX-License-Identifier: AGPL-3.0
+
+from typing import Dict, Union
+
+from rdflib import RDF, XSD, Graph, Literal, Namespace, URIRef
+
+from ..classes.data_entity import DataEntity
+from ..classes.entity import Entity
+from ..classes.task import Task
+from .query_utils import (get_data_properties_by_entity_iri,
+                          get_first_query_result_if_exists)
+
+
+def add_instance(kg: Graph, entity_instance: Entity) -> None:
+    """
+    Adds entity instance to KG only if its parent entity exists and there is no instance with the same IRI
+    Args:
+        kg: Graph object to add to
+        entity_instance: the entity instance to create
+    """
+    if entity_instance.parent_entity and (entity_instance.iri, None, None) not in kg:
+        kg.add((entity_instance.iri, RDF.type, entity_instance.parent_entity.iri))
+
+
+def add_relation(kg: Graph, from_entity: Entity, relation_iri: str, to_entity: Entity) -> None:
+    """
+    Adds relation between 2 given entities to KG
+    Args:
+        kg: Graph object to add to
+        from_entity: relation source
+        relation_iri: IRI that connects the 2 given entities
+        to_entity: relation destination
+    """
+    kg.add(
+        (
+            from_entity.iri,
+            URIRef(relation_iri),
+            to_entity.iri,
+        )
+    )
+
+
+def add_literal(kg: Graph, from_entity: Entity, relation_iri: str, literal: Literal) -> None:
+    """
+    Adds relation between a given entity and a given literal to KG
+    Args:
+        kg: Graph object to add to
+        from_entity: relation source
+        relation_iri: IRI that connects the given entity with the given literal
+        literal: literal to add to Graph object
+    """
+    kg.add((from_entity.iri, URIRef(relation_iri), literal))
+
+
+def add_instance_from_parent_with_relation(
+    namespace: Namespace,
+    kg: Graph,
+    parent_entity: Entity,
+    relation_iri: str,
+    related_entity: Entity,
+    instance_name: str,
+) -> Entity:
+    """
+    Creates an entity object based on the arguments and calls add_instance() and add_relation() to create a new entity instance and relation
+    Args:
+        namespace: namespace for the new instance
+        kg: Graph object to add to
+        parent_entity: parent entity for the new instance
+        relation_iri: IRI that connects the given related_entity with the new instance
+        related_entity: relation source
+        instance_name: name for the new instance
+
+    Returns:
+        Entity: object containing the new entity instance's basic info
+    """
+    entity_iri = namespace + instance_name
+    instance = Entity(entity_iri, parent_entity)
+
+    add_instance(kg, instance)
+    add_relation(kg, related_entity, relation_iri, instance)
+
+    return instance
+
+
+def name_instance(
+    task_type_dict: Dict[str, int],
+    method_type_dict: Dict[str, int],
+    parent_entity: Entity,
+) -> Union[None, str]:
+    """
+    Creates a unique name for a new instance by concatenating the parent entity's name (which is the instance type) with a number
+    Also increments the relevant number of the corresponding dict
+    Args:
+        task_type_dict: contains pairs of task types and numbers
+        method_type_dict: contains pairs of method types and numbers
+        parent_entity: instance's parent entity
+
+    Returns:
+        str: name to be given to the new instance
+        None: if the type of the given parent entity is not equal with "AtomicTask" or "AtomicMethod"
+    """
+    if parent_entity.type == "AtomicTask":
+        entity_type_dict = task_type_dict
+    elif parent_entity.type == "AtomicMethod":
+        entity_type_dict = method_type_dict
+    else:
+        print("Error: Invalid parent entity type")
+        return None
+
+    instance_name = parent_entity.name + str(entity_type_dict[parent_entity.name])
+    entity_type_dict[parent_entity.name] += 1
+    return instance_name
+
+
+def add_data_entity_instance(
+    kg: Graph,
+    data: Entity,
+    top_level_kg: Graph,
+    top_level_schema_namespace: Namespace,
+    data_entity: DataEntity,
+) -> None:
+    """
+    Adds data entity instance to kg with the necessary relations
+    Args:
+        kg: Graph object to add to
+        data: object representing top-level DataEntity class in KG
+        top_level_kg: KG corresponding to the top-level KG schema
+        top_level_schema_namespace: namespace of the top-level KG schema
+        data_entity: data entity to add
+    """
+    add_instance(kg, data_entity)
+
+    if data_entity.has_source:
+        has_source_iri, range_iri = get_first_query_result_if_exists(
+            get_data_properties_by_entity_iri, data.iri, top_level_kg
+        )
+
+        source_literal = Literal(
+            lexical_or_value=data_entity.has_source,
+            datatype=range_iri,
+        )
+
+        add_literal(kg, data_entity, has_source_iri, source_literal)
+
+    if data_entity.has_data_structure:
+        add_relation(
+            kg,
+            data_entity,
+            top_level_schema_namespace.hasDataStructure,
+            Entity(data_entity.has_data_structure),
+        )
+
+    if data_entity.has_data_semantics:
+        add_relation(
+            kg,
+            data_entity,
+            top_level_schema_namespace.hasDataSemantics,
+            Entity(data_entity.has_data_semantics),
+        )
+
+    if data_entity.has_reference:
+        add_relation(
+            kg,
+            data_entity,
+            top_level_schema_namespace.hasReference,
+            Entity(data_entity.has_reference),
+        )
+
+
+def add_and_attach_data_entity(
+    kg: Graph,
+    data: Entity,
+    top_level_kg: Graph,
+    top_level_schema_namespace: Namespace,
+    data_entity: DataEntity,
+    relation: URIRef,
+    task_entity: Task,
+) -> None:
+    """
+    Adds data entity instance to kg with the necessary relations, and attaches it to the given task
+    Args:
+        kg: Graph object to add to
+        data: object representing top-level DataEntity class in KG
+        top_level_kg: KG corresponding to the top-level KG schema
+        top_level_schema_namespace: namespace of the top-level KG schema
+        data_entity: data entity to add
+        relation: IRI of relation to add
+        task_entity: task to attach the data entity to
+    """
+    add_data_entity_instance(kg, data, top_level_kg, top_level_schema_namespace, data_entity)
+    add_relation(kg, task_entity, relation, data_entity)
+
+
+def create_pipeline_task(
+    top_level_schema_namespace: Namespace,
+    parent_entity: Entity,
+    kg: Graph,
+    pipeline_name: str,
+    input_data_path: str,
+) -> Task:
+    """
+    Adds instance of pipeline task to kg
+    Args:
+        top_level_schema_namespace: namespace of the top-level KG schema
+        parent_entity: parent entity of pipeline instance
+        kg: Graph object to add to
+        pipeline_name: name for the pipeline
+        input_data_path: path for the input data to be used by the pipeline's tasks
+
+    Returns:
+        Task: created pipeline task
+    """
+    pipeline = Task(top_level_schema_namespace + pipeline_name, parent_entity)
+    add_instance(kg, pipeline)
+
+    input_data_path_literal = Literal(lexical_or_value=input_data_path, datatype=XSD.string)
+    add_literal(kg, pipeline, top_level_schema_namespace.hasInputDataPath, input_data_path_literal)
+
+    return pipeline
```

### Comparing `exe_kg_lib-2.0.2/exe_kg_lib/utils/query_utils.py` & `exe_kg_lib-2.0.3/exe_kg_lib/utils/query_utils.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,193 +1,193 @@
-# Copyright (c) 2022 Robert Bosch GmbH
-# SPDX-License-Identifier: AGPL-3.0
-
-from typing import Callable, List, Optional, Tuple
-
-from rdflib import Graph, Namespace, URIRef, query
-
-from ..classes.entity import Entity
-
-
-def query_method_parent_classes(kg, method_iri):
-    return kg.query(
-        f"SELECT ?c WHERE {{ ?method rdfs:subClassOf ?c . }}",
-        initBindings={"method": URIRef(method_iri)},
-    )
-
-
-def query_entity_parent_iri(kg, entity_iri: str, upper_class_uri_ref: URIRef):
-    return kg.query(
-        f"SELECT ?t WHERE {{ ?entity rdf:type ?t ." f"                   ?t rdfs:subClassOf* ?upper_class .}}",
-        initBindings={
-            "entity": URIRef(entity_iri),
-            "upper_class": upper_class_uri_ref,
-        },
-    )
-
-
-def query_data_entity_reference_iri(kg, namespace_prefix, entity_iri: str):
-    return kg.query(
-        f"SELECT ?r WHERE {{ ?entity {namespace_prefix}:hasReference ?r . }}",
-        initBindings={
-            "entity": URIRef(entity_iri),
-        },
-    )
-
-
-def query_method_iri_by_task_iri(kg, namespace_prefix, task_iri: str):
-    return kg.query(
-        f"SELECT ?m WHERE {{ ?task ?m_property ?m ."
-        f"                   ?m_property rdfs:subPropertyOf* {namespace_prefix}:hasMethod .}}",
-        initBindings={"task": URIRef(task_iri)},
-    )
-
-
-def get_first_query_result_if_exists(query_method: Callable, *args) -> Optional[str]:
-    query_result = next(
-        iter(list(query_method(*args))),
-        None,
-    )
-
-    if query_result is None:
-        return None
-
-    return query_result
-
-
-def get_data_properties_by_entity_iri(entity_iri: str, kg: Graph) -> query.Result:
-    return kg.query(
-        "\nSELECT ?p ?r WHERE {?p rdfs:domain ?entity_iri . "
-        "?p rdfs:range ?r . "
-        "?p rdf:type owl:DatatypeProperty . }",
-        initBindings={"entity_iri": URIRef(entity_iri)},
-    )
-
-
-def get_method_properties_and_methods(input_kg, namespace_prefix, entity_parent_iri: str) -> query.Result:
-    return input_kg.query(
-        "\nSELECT ?p ?m WHERE {?p rdfs:domain ?entity_iri . "
-        "?p rdfs:range ?m . "
-        "?m rdfs:subClassOf " + namespace_prefix + ":AtomicMethod . }",
-        initBindings={"entity_iri": URIRef(entity_parent_iri)},
-    )
-
-
-def get_input_properties_and_inputs(input_kg, namespace_prefix, entity_parent_iri: str) -> query.Result:
-    return input_kg.query(
-        "\nSELECT ?p ?m WHERE {?p rdfs:domain ?entity_iri . "
-        "?p rdfs:range ?m ."
-        "?p rdfs:subPropertyOf " + namespace_prefix + ":hasInput ."
-        "?m rdfs:subClassOf " + namespace_prefix + ":DataEntity . }",
-        initBindings={"entity_iri": URIRef(entity_parent_iri)},
-    )
-
-
-def get_output_properties_and_outputs(input_kg, namespace_prefix, entity_parent_iri: str) -> query.Result:
-    return input_kg.query(
-        "\nSELECT ?p ?m WHERE {?p rdfs:domain ?entity_iri . "
-        "?p rdfs:range ?m ."
-        "?p rdfs:subPropertyOf " + namespace_prefix + ":hasOutput ."
-        "?m rdfs:subClassOf " + namespace_prefix + ":DataEntity . }",
-        initBindings={"entity_iri": URIRef(entity_parent_iri)},
-    )
-
-
-def query_pipeline_info(kg, namespace_prefix):
-    return kg.query(
-        f"\nSELECT ?p ?i ?t WHERE {{?p rdf:type {namespace_prefix}:Pipeline ;"
-        f"                          {namespace_prefix}:hasInputDataPath ?i ;"
-        f"                          {namespace_prefix}:hasStartTask ?t . }}"
-    )
-
-
-def get_subclasses_of(class_iri: str, kg: Graph) -> query.Result:
-    return kg.query(
-        "\nSELECT ?t WHERE {?t rdfs:subClassOf ?class_iri . }",
-        initBindings={"class_iri": class_iri},
-    )
-
-
-def get_data_properties_plus_inherited_by_class_iri(kg: Graph, entity_iri: str) -> List:
-    """
-    Retrieves data properties plus the inherited ones, given an entity IRI
-    Args:
-        kg: Graph object to use when querying
-        entity_iri: IRI of entity to query
-
-    Returns:
-        List: contains rows of data property IRIs and their range
-    """
-    property_list = list(get_data_properties_by_entity_iri(entity_iri, kg))
-    method_parent_classes = list(query_method_parent_classes(kg, entity_iri))
-    for method_class_result_row in method_parent_classes:
-        property_list += list(get_data_properties_by_entity_iri(method_class_result_row[0], kg))
-
-    return property_list
-
-
-def get_pipeline_and_first_task_iri(kg: Graph, namespace_prefix: str) -> Tuple[str, str, str]:
-    """
-    Retrieves the necessary information needed to start parsing a pipeline
-    Args:
-        kg: Graph object to use when querying
-        namespace_prefix: namespace prefix to use when querying
-
-    Returns:
-        Tuple[str, str, str]: contains the pipeline IRI, the input data path and the first task's IRI
-    """
-    # assume one pipeline per file
-    query_result = get_first_query_result_if_exists(
-        query_pipeline_info,
-        kg,
-        namespace_prefix,
-    )
-    if query_result is None:
-        print("Error: Pipeline info not found")
-        exit(1)
-
-    pipeline_iri, input_data_path, task_iri = query_result
-
-    return str(pipeline_iri), str(input_data_path), str(task_iri)
-
-
-def get_method_by_task_iri(
-    kg: Graph,
-    namespace_prefix: str,
-    namespace: Namespace,
-    task_iri: str,
-) -> Optional[Entity]:
-    """
-    Retrieves a task's method, given a task IRI
-    Args:
-        kg: Graph object to use when querying
-        namespace_prefix: namespace prefix to use when querying
-        namespace: namespace to use when querying
-        task_iri: IRI of task to query
-
-    Returns:
-        Optional[Entity]: object containing found method's basic info
-                          is equal to None if method IRI wasn't found in KG
-    """
-    query_result = get_first_query_result_if_exists(
-        query_method_iri_by_task_iri,
-        kg,
-        namespace_prefix,
-        task_iri,
-    )
-    if query_result is None:
-        return None
-
-    method_iri = str(query_result[0])
-
-    query_result = get_first_query_result_if_exists(
-        query_entity_parent_iri,
-        kg,
-        method_iri,
-        namespace.AtomicMethod,
-    )
-    if query_result is None:
-        return None
-
-    method_parent_iri = str(query_result[0])
-
-    return Entity(method_iri, Entity(method_parent_iri))
+# Copyright (c) 2022 Robert Bosch GmbH
+# SPDX-License-Identifier: AGPL-3.0
+
+from typing import Callable, List, Optional, Tuple
+
+from rdflib import Graph, Namespace, URIRef, query
+
+from ..classes.entity import Entity
+
+
+def query_method_parent_classes(kg, method_iri):
+    return kg.query(
+        f"SELECT ?c WHERE {{ ?method rdfs:subClassOf ?c . }}",
+        initBindings={"method": URIRef(method_iri)},
+    )
+
+
+def query_entity_parent_iri(kg, entity_iri: str, upper_class_uri_ref: URIRef):
+    return kg.query(
+        f"SELECT ?t WHERE {{ ?entity rdf:type ?t ." f"                   ?t rdfs:subClassOf* ?upper_class .}}",
+        initBindings={
+            "entity": URIRef(entity_iri),
+            "upper_class": upper_class_uri_ref,
+        },
+    )
+
+
+def query_data_entity_reference_iri(kg, namespace_prefix, entity_iri: str):
+    return kg.query(
+        f"SELECT ?r WHERE {{ ?entity {namespace_prefix}:hasReference ?r . }}",
+        initBindings={
+            "entity": URIRef(entity_iri),
+        },
+    )
+
+
+def query_method_iri_by_task_iri(kg, namespace_prefix, task_iri: str):
+    return kg.query(
+        f"SELECT ?m WHERE {{ ?task ?m_property ?m ."
+        f"                   ?m_property rdfs:subPropertyOf* {namespace_prefix}:hasMethod .}}",
+        initBindings={"task": URIRef(task_iri)},
+    )
+
+
+def get_first_query_result_if_exists(query_method: Callable, *args) -> Optional[str]:
+    query_result = next(
+        iter(list(query_method(*args))),
+        None,
+    )
+
+    if query_result is None:
+        return None
+
+    return query_result
+
+
+def get_data_properties_by_entity_iri(entity_iri: str, kg: Graph) -> query.Result:
+    return kg.query(
+        "\nSELECT ?p ?r WHERE {?p rdfs:domain ?entity_iri . "
+        "?p rdfs:range ?r . "
+        "?p rdf:type owl:DatatypeProperty . }",
+        initBindings={"entity_iri": URIRef(entity_iri)},
+    )
+
+
+def get_method_properties_and_methods(input_kg, namespace_prefix, entity_parent_iri: str) -> query.Result:
+    return input_kg.query(
+        "\nSELECT ?p ?m WHERE {?p rdfs:domain ?entity_iri . "
+        "?p rdfs:range ?m . "
+        "?m rdfs:subClassOf " + namespace_prefix + ":AtomicMethod . }",
+        initBindings={"entity_iri": URIRef(entity_parent_iri)},
+    )
+
+
+def get_input_properties_and_inputs(input_kg, namespace_prefix, entity_parent_iri: str) -> query.Result:
+    return input_kg.query(
+        "\nSELECT ?p ?m WHERE {?p rdfs:domain ?entity_iri . "
+        "?p rdfs:range ?m ."
+        "?p rdfs:subPropertyOf " + namespace_prefix + ":hasInput ."
+        "?m rdfs:subClassOf " + namespace_prefix + ":DataEntity . }",
+        initBindings={"entity_iri": URIRef(entity_parent_iri)},
+    )
+
+
+def get_output_properties_and_outputs(input_kg, namespace_prefix, entity_parent_iri: str) -> query.Result:
+    return input_kg.query(
+        "\nSELECT ?p ?m WHERE {?p rdfs:domain ?entity_iri . "
+        "?p rdfs:range ?m ."
+        "?p rdfs:subPropertyOf " + namespace_prefix + ":hasOutput ."
+        "?m rdfs:subClassOf " + namespace_prefix + ":DataEntity . }",
+        initBindings={"entity_iri": URIRef(entity_parent_iri)},
+    )
+
+
+def query_pipeline_info(kg, namespace_prefix):
+    return kg.query(
+        f"\nSELECT ?p ?i ?t WHERE {{?p rdf:type {namespace_prefix}:Pipeline ;"
+        f"                          {namespace_prefix}:hasInputDataPath ?i ;"
+        f"                          {namespace_prefix}:hasStartTask ?t . }}"
+    )
+
+
+def get_subclasses_of(class_iri: str, kg: Graph) -> query.Result:
+    return kg.query(
+        "\nSELECT ?t WHERE {?t rdfs:subClassOf ?class_iri . }",
+        initBindings={"class_iri": class_iri},
+    )
+
+
+def get_data_properties_plus_inherited_by_class_iri(kg: Graph, entity_iri: str) -> List:
+    """
+    Retrieves data properties plus the inherited ones, given an entity IRI
+    Args:
+        kg: Graph object to use when querying
+        entity_iri: IRI of entity to query
+
+    Returns:
+        List: contains rows of data property IRIs and their range
+    """
+    property_list = list(get_data_properties_by_entity_iri(entity_iri, kg))
+    method_parent_classes = list(query_method_parent_classes(kg, entity_iri))
+    for method_class_result_row in method_parent_classes:
+        property_list += list(get_data_properties_by_entity_iri(method_class_result_row[0], kg))
+
+    return property_list
+
+
+def get_pipeline_and_first_task_iri(kg: Graph, namespace_prefix: str) -> Tuple[str, str, str]:
+    """
+    Retrieves the necessary information needed to start parsing a pipeline
+    Args:
+        kg: Graph object to use when querying
+        namespace_prefix: namespace prefix to use when querying
+
+    Returns:
+        Tuple[str, str, str]: contains the pipeline IRI, the input data path and the first task's IRI
+    """
+    # assume one pipeline per file
+    query_result = get_first_query_result_if_exists(
+        query_pipeline_info,
+        kg,
+        namespace_prefix,
+    )
+    if query_result is None:
+        print("Error: Pipeline info not found")
+        exit(1)
+
+    pipeline_iri, input_data_path, task_iri = query_result
+
+    return str(pipeline_iri), str(input_data_path), str(task_iri)
+
+
+def get_method_by_task_iri(
+    kg: Graph,
+    namespace_prefix: str,
+    namespace: Namespace,
+    task_iri: str,
+) -> Optional[Entity]:
+    """
+    Retrieves a task's method, given a task IRI
+    Args:
+        kg: Graph object to use when querying
+        namespace_prefix: namespace prefix to use when querying
+        namespace: namespace to use when querying
+        task_iri: IRI of task to query
+
+    Returns:
+        Optional[Entity]: object containing found method's basic info
+                          is equal to None if method IRI wasn't found in KG
+    """
+    query_result = get_first_query_result_if_exists(
+        query_method_iri_by_task_iri,
+        kg,
+        namespace_prefix,
+        task_iri,
+    )
+    if query_result is None:
+        return None
+
+    method_iri = str(query_result[0])
+
+    query_result = get_first_query_result_if_exists(
+        query_entity_parent_iri,
+        kg,
+        method_iri,
+        namespace.AtomicMethod,
+    )
+    if query_result is None:
+        return None
+
+    method_parent_iri = str(query_result[0])
+
+    return Entity(method_iri, Entity(method_parent_iri))
```

### Comparing `exe_kg_lib-2.0.2/exe_kg_lib/utils/string_utils.py` & `exe_kg_lib-2.0.3/exe_kg_lib/utils/string_utils.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# Copyright (c) 2022 Robert Bosch GmbH
-# SPDX-License-Identifier: AGPL-3.0
-
-import re
-
-
-def camel_to_snake(text: str) -> str:
-    """
-    Converts camel-case string to snake-case
-    Args:
-        text: string to convert
-
-    Returns:
-        str: converted string
-    """
-    text = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", text)
-    return re.sub("([a-z0-9])([A-Z])", r"\1_\2", text).lower()
-
-
-def property_name_to_field_name(property_name: str) -> str:
-    """
-    Extracts property name from IRI and converts it to snake-case
-    Args:
-        property_name: IRI to parse
-
-    Returns:
-        str: converted string
-    """
-    return camel_to_snake(property_name.split("#")[1])
+# Copyright (c) 2022 Robert Bosch GmbH
+# SPDX-License-Identifier: AGPL-3.0
+
+import re
+
+
+def camel_to_snake(text: str) -> str:
+    """
+    Converts camel-case string to snake-case
+    Args:
+        text: string to convert
+
+    Returns:
+        str: converted string
+    """
+    text = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", text)
+    return re.sub("([a-z0-9])([A-Z])", r"\1_\2", text).lower()
+
+
+def property_name_to_field_name(property_name: str) -> str:
+    """
+    Extracts property name from IRI and converts it to snake-case
+    Args:
+        property_name: IRI to parse
+
+    Returns:
+        str: converted string
+    """
+    return camel_to_snake(property_name.split("#")[1])
```

### Comparing `exe_kg_lib-2.0.2/exe_kg_lib/utils/task_utils/ml_utils.py` & `exe_kg_lib-2.0.3/exe_kg_lib/utils/task_utils/ml_utils.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-# Copyright (c) 2022 Robert Bosch GmbH
-# SPDX-License-Identifier: AGPL-3.0
-
-from typing import List, Tuple
-
-import numpy as np
-import pandas as pd
-from sklearn.linear_model import LinearRegression
-from sklearn.neighbors import KNeighborsRegressor
-from sklearn.neural_network import MLPRegressor
-
-
-def concatenation(inputs: List[np.ndarray]) -> pd.DataFrame:
-    return pd.concat(inputs, axis=1)
-
-
-def data_splitting(
-    input_x: pd.DataFrame, input_y: np.ndarray, split_ratio: str
-) -> Tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame, pd.DataFrame]:
-    """split data into training and testing set"""
-
-    splitting_point = int(float(split_ratio) * float(input_x.shape[0]))
-
-    train_x = input_x.iloc[:splitting_point]
-    test_x = input_x.iloc[splitting_point:]
-    train_y = input_y.iloc[:splitting_point]
-    test_y = input_y.iloc[splitting_point:]
-
-    return train_x, test_x, train_y, test_y
-
-
-def k_nn_train(
-    input_x: np.ndarray, input_y: np.ndarray, n_neighbors: int = 3
-) -> Tuple[KNeighborsRegressor, np.ndarray]:
-    print("n_neighbors = ", n_neighbors)
-    model = KNeighborsRegressor(n_neighbors=n_neighbors)
-    model.fit(input_x, input_y)
-
-    predicted_y = model.predict(input_x)
-
-    print("KNN training finished")
-
-    return model, predicted_y
-
-
-def k_nn_test(model: KNeighborsRegressor, input_x: np.ndarray) -> np.ndarray:
-    predicted_y = model.predict(input_x)
-
-    print("KNN testing finished")
-
-    return predicted_y
-
-
-def lr_training(input_x: np.ndarray, input_y: np.ndarray) -> Tuple[LinearRegression, np.ndarray]:
-    model = LinearRegression()
-    model.fit(input_x, input_y)
-    predicted_y = model.predict(input_x)
-
-    print("LR training finished")
-    return model, predicted_y
-
-
-def lr_testing(model: LinearRegression, input_x: np.ndarray):
-    predict_y = model.predict(input_x)
-
-    return predict_y
-
-
-def mlp_train(input_x: np.ndarray, input_y: np.ndarray, solver="adam") -> Tuple[MLPRegressor, np.ndarray]:
-    model = MLPRegressor(solver=solver)
-    model.fit(input_x, input_y)
-
-    predicted_y = model.predict(input_x)
-
-    print("MLP training finished")
-
-    return model, predicted_y
-
-
-def mlp_test(model: MLPRegressor, input_x: np.ndarray) -> np.ndarray:
-    predicted_y = model.predict(input_x)
-
-    print("MLP testing finished")
-
-    return predicted_y
-
-
-def ml_performance_calculation(
-    real_train: np.ndarray = 0,
-    real_test: np.ndarray = 0,
-    predicted_train: np.ndarray = 0,
-    predicted_test: np.ndarray = 0,
-) -> Tuple[pd.DataFrame, pd.DataFrame]:
-    train_err = pd.DataFrame(real_train - predicted_train)
-    test_err = pd.DataFrame(real_test - predicted_test)
-
-    return train_err, test_err
+# Copyright (c) 2022 Robert Bosch GmbH
+# SPDX-License-Identifier: AGPL-3.0
+
+from typing import List, Tuple
+
+import numpy as np
+import pandas as pd
+from sklearn.linear_model import LinearRegression
+from sklearn.neighbors import KNeighborsRegressor
+from sklearn.neural_network import MLPRegressor
+
+
+def concatenation(inputs: List[np.ndarray]) -> pd.DataFrame:
+    return pd.concat(inputs, axis=1)
+
+
+def data_splitting(
+    input_x: pd.DataFrame, input_y: np.ndarray, split_ratio: str
+) -> Tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame, pd.DataFrame]:
+    """split data into training and testing set"""
+
+    splitting_point = int(float(split_ratio) * float(input_x.shape[0]))
+
+    train_x = input_x.iloc[:splitting_point]
+    test_x = input_x.iloc[splitting_point:]
+    train_y = input_y.iloc[:splitting_point]
+    test_y = input_y.iloc[splitting_point:]
+
+    return train_x, test_x, train_y, test_y
+
+
+def k_nn_train(
+    input_x: np.ndarray, input_y: np.ndarray, n_neighbors: int = 3
+) -> Tuple[KNeighborsRegressor, np.ndarray]:
+    print("n_neighbors = ", n_neighbors)
+    model = KNeighborsRegressor(n_neighbors=n_neighbors)
+    model.fit(input_x, input_y)
+
+    predicted_y = model.predict(input_x)
+
+    print("KNN training finished")
+
+    return model, predicted_y
+
+
+def k_nn_test(model: KNeighborsRegressor, input_x: np.ndarray) -> np.ndarray:
+    predicted_y = model.predict(input_x)
+
+    print("KNN testing finished")
+
+    return predicted_y
+
+
+def lr_training(input_x: np.ndarray, input_y: np.ndarray) -> Tuple[LinearRegression, np.ndarray]:
+    model = LinearRegression()
+    model.fit(input_x, input_y)
+    predicted_y = model.predict(input_x)
+
+    print("LR training finished")
+    return model, predicted_y
+
+
+def lr_testing(model: LinearRegression, input_x: np.ndarray):
+    predict_y = model.predict(input_x)
+
+    return predict_y
+
+
+def mlp_train(input_x: np.ndarray, input_y: np.ndarray, solver="adam") -> Tuple[MLPRegressor, np.ndarray]:
+    model = MLPRegressor(solver=solver)
+    model.fit(input_x, input_y)
+
+    predicted_y = model.predict(input_x)
+
+    print("MLP training finished")
+
+    return model, predicted_y
+
+
+def mlp_test(model: MLPRegressor, input_x: np.ndarray) -> np.ndarray:
+    predicted_y = model.predict(input_x)
+
+    print("MLP testing finished")
+
+    return predicted_y
+
+
+def ml_performance_calculation(
+    real_train: np.ndarray = 0,
+    real_test: np.ndarray = 0,
+    predicted_train: np.ndarray = 0,
+    predicted_test: np.ndarray = 0,
+) -> Tuple[pd.DataFrame, pd.DataFrame]:
+    train_err = pd.DataFrame(real_train - predicted_train)
+    test_err = pd.DataFrame(real_test - predicted_test)
+
+    return train_err, test_err
```

### Comparing `exe_kg_lib-2.0.2/exe_kg_lib/utils/task_utils/statistic_utils.py` & `exe_kg_lib-2.0.3/exe_kg_lib/utils/task_utils/statistic_utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-# Copyright (c) 2022 Robert Bosch GmbH
-# SPDX-License-Identifier: AGPL-3.0
-
-import numpy as np
-import pandas as pd
-
-
-def trend_calculation(
-    input_data: np.ndarray,
-    half_window_size: int = 2,
-    padding: str = "same",
-) -> np.ndarray:
-    """calculate the trend of the data, which is the sliding-window average"""
-
-    def padding_input(input: np.ndarray, half_window_size: int, padding: str = "same") -> np.ndarray:
-        """padding the beginning and end of the input data by the beginning or end value"""
-        if padding == "same":
-            begin_padding = pd.Series([input.iloc[0]] * half_window_size)
-            end_padding = pd.Series([input.iloc[len(input) - 1]] * half_window_size)
-            output = pd.concat([begin_padding, input, end_padding]).reset_index().drop("index", axis=1)
-            return output
-
-        else:
-            return 0
-
-    input = padding_input(input_data, half_window_size)
-
-    output = 0
-    input_len = len(input) - 2 * half_window_size
-    for i in range(2 * half_window_size + 1):
-        output += np.array(input.iloc[i : i + input_len])
-
-    output = output / (2 * half_window_size + 1)
-
-    return output
-
-
-def mean_calculation(input_data: np.ndarray) -> np.ndarray:
-    return np.mean(input_data)
-
-
-def std_deviation(input_data: np.ndarray) -> np.ndarray:
-    return np.std(input_data)
-
-
-def minimum_calculation(input_data: np.ndarray) -> np.ndarray:
-    return np.min(input_data)
-
-
-def maximum_calculation(input_data: np.ndarray) -> np.ndarray:
-    return np.max(input_data)
-
-
-def iqr_calculation(input_data: np.ndarray, percent: int = 50) -> np.ndarray:
-    """return quarter of the input_data"""
-    return np.percentile(input_data, percent)
-
-
-def outlier_calculation(input: np.ndarray, iq1: float = None, iq3: float = None) -> np.ndarray:
-    """return the outliers in the data"""
-    iq1 = iqr_calculation(input, 25) if (not iq1) else iq1
-    iq3 = iqr_calculation(input, 75) if (not iq3) else iq3
-    median = np.median(input)
-    iqr = iq3 - iq1
-    high_outliers = input < median - 1.5 * iqr
-    low_outliers = input > median + 1.5 * iqr
-    outlier_rows = [low_outliers.iloc[i] or high_outliers.iloc[i] for i in range(len(input))]
-    return outlier_rows
-
-
-def scattering_calculation(input_data: np.ndarray) -> np.ndarray:
-    trend_calc_output = trend_calculation(input_data)
-    output = input_data - trend_calc_output
-
-    return output
-
-
-def normalization(input_data: np.ndarray) -> np.ndarray:
-    mean = mean_calculation(input_data)
-    std = std_deviation(input_data)
-    output = (input_data - mean) / std
-
-    return output
+# Copyright (c) 2022 Robert Bosch GmbH
+# SPDX-License-Identifier: AGPL-3.0
+
+import numpy as np
+import pandas as pd
+
+
+def trend_calculation(
+    input_data: np.ndarray,
+    half_window_size: int = 2,
+    padding: str = "same",
+) -> np.ndarray:
+    """calculate the trend of the data, which is the sliding-window average"""
+
+    def padding_input(input: np.ndarray, half_window_size: int, padding: str = "same") -> np.ndarray:
+        """padding the beginning and end of the input data by the beginning or end value"""
+        if padding == "same":
+            begin_padding = pd.Series([input.iloc[0]] * half_window_size)
+            end_padding = pd.Series([input.iloc[len(input) - 1]] * half_window_size)
+            output = pd.concat([begin_padding, input, end_padding]).reset_index().drop("index", axis=1)
+            return output
+
+        else:
+            return 0
+
+    input = padding_input(input_data, half_window_size)
+
+    output = 0
+    input_len = len(input) - 2 * half_window_size
+    for i in range(2 * half_window_size + 1):
+        output += np.array(input.iloc[i : i + input_len])
+
+    output = output / (2 * half_window_size + 1)
+
+    return output
+
+
+def mean_calculation(input_data: np.ndarray) -> np.ndarray:
+    return np.mean(input_data)
+
+
+def std_deviation(input_data: np.ndarray) -> np.ndarray:
+    return np.std(input_data)
+
+
+def minimum_calculation(input_data: np.ndarray) -> np.ndarray:
+    return np.min(input_data)
+
+
+def maximum_calculation(input_data: np.ndarray) -> np.ndarray:
+    return np.max(input_data)
+
+
+def iqr_calculation(input_data: np.ndarray, percent: int = 50) -> np.ndarray:
+    """return quarter of the input_data"""
+    return np.percentile(input_data, percent)
+
+
+def outlier_calculation(input: np.ndarray, iq1: float = None, iq3: float = None) -> np.ndarray:
+    """return the outliers in the data"""
+    iq1 = iqr_calculation(input, 25) if (not iq1) else iq1
+    iq3 = iqr_calculation(input, 75) if (not iq3) else iq3
+    median = np.median(input)
+    iqr = iq3 - iq1
+    high_outliers = input < median - 1.5 * iqr
+    low_outliers = input > median + 1.5 * iqr
+    outlier_rows = [low_outliers.iloc[i] or high_outliers.iloc[i] for i in range(len(input))]
+    return outlier_rows
+
+
+def scattering_calculation(input_data: np.ndarray) -> np.ndarray:
+    trend_calc_output = trend_calculation(input_data)
+    output = input_data - trend_calc_output
+
+    return output
+
+
+def normalization(input_data: np.ndarray) -> np.ndarray:
+    mean = mean_calculation(input_data)
+    std = std_deviation(input_data)
+    output = (input_data - mean) / std
+
+    return output
```

### Comparing `exe_kg_lib-2.0.2/exe_kg_lib/utils/task_utils/visual_utils.py` & `exe_kg_lib-2.0.3/exe_kg_lib/utils/task_utils/visual_utils.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-# Copyright (c) 2022 Robert Bosch GmbH
-# SPDX-License-Identifier: AGPL-3.0
-
-from typing import Optional, Tuple
-
-import pandas as pd
-from matplotlib import pyplot as plt
-from matplotlib.figure import Figure
-from matplotlib.font_manager import FontProperties
-
-
-def canvas_creation(layout: str) -> Tuple[Figure, Optional[plt.GridSpec]]:
-    """the canvas task taking as input the starting task POs and output the fig and grid"""
-
-    font = FontProperties()
-    font.set_size(10)
-    font.set_name("Verdana")
-
-    try:
-        n_rows, n_cols = (int(i) for i in layout[0].split(" "))
-    except:
-        n_rows, n_cols = (1, 1)
-
-    fig = plt.figure(figsize=(7, 5))
-
-    grid = None if (n_rows == n_cols and n_rows == 1) else plt.GridSpec(n_rows, n_cols, hspace=0.3, wspace=0.3)
-
-    return fig, grid
-
-
-# def scatter_plot(data: pd.Series, fig: Figure, grid: plt.GridSpec, layout: str, line_width: str, line_style: str,
-#                  legend_name: str, x_lim: str, y_lim: str, x_label: str, y_label: str):
-def scatter_plot(**kwargs):
-    plot_creation("scatter", **kwargs)
-
-
-def line_plot(**kwargs):
-    plot_creation("line", **kwargs)
-
-
-def plot_creation(
-    plot_type: str,
-    data: pd.Series,
-    fig: Figure,
-    grid: plt.GridSpec,
-    layout: str,
-    line_width: str,
-    line_style: str,
-    legend_name: str,
-    x_lim: str,
-    y_lim: str,
-    x_label: str,
-    y_label: str,
-):
-    plot = plt
-    if grid is not None:
-        row_start, row_end, col_start, col_end = (int(i) for i in layout.split())
-        plot = fig.add_subplot(grid[row_start:row_end, col_start:col_end])
-
-    if plot_type == "line":
-        plot.plot(
-            data.index,
-            data,
-            linestyle=line_style,
-            linewidth=int(line_width),
-            label=legend_name,
-        )
-    elif plot_type == "scatter":
-        plot.scatter(
-            data.index,
-            data,
-            s=int(int(line_width) * 10),
-            marker=line_style,
-            linewidth=int(line_width),
-            label=legend_name,
-        )
-    else:
-        print("Invalid plot type given")
-
-    if grid is None:
-        plot.xlim(x_lim)
-        plot.ylim(y_lim)
-        plot.xlabel(x_label)
-        plot.ylabel(y_label)
-    else:
-        plot.set_xlim(x_lim)
-        plot.set_ylim(y_lim)
-        plot.set_xlabel(x_label)
-        plot.set_ylabel(y_label)
-
-    plt.legend()
-    plt.show()
+# Copyright (c) 2022 Robert Bosch GmbH
+# SPDX-License-Identifier: AGPL-3.0
+
+from typing import Optional, Tuple
+
+import pandas as pd
+from matplotlib import pyplot as plt
+from matplotlib.figure import Figure
+from matplotlib.font_manager import FontProperties
+
+
+def canvas_creation(layout: str) -> Tuple[Figure, Optional[plt.GridSpec]]:
+    """the canvas task taking as input the starting task POs and output the fig and grid"""
+
+    font = FontProperties()
+    font.set_size(10)
+    font.set_name("Verdana")
+
+    try:
+        n_rows, n_cols = (int(i) for i in layout[0].split(" "))
+    except:
+        n_rows, n_cols = (1, 1)
+
+    fig = plt.figure(figsize=(7, 5))
+
+    grid = None if (n_rows == n_cols and n_rows == 1) else plt.GridSpec(n_rows, n_cols, hspace=0.3, wspace=0.3)
+
+    return fig, grid
+
+
+# def scatter_plot(data: pd.Series, fig: Figure, grid: plt.GridSpec, layout: str, line_width: str, line_style: str,
+#                  legend_name: str, x_lim: str, y_lim: str, x_label: str, y_label: str):
+def scatter_plot(**kwargs):
+    plot_creation("scatter", **kwargs)
+
+
+def line_plot(**kwargs):
+    plot_creation("line", **kwargs)
+
+
+def plot_creation(
+    plot_type: str,
+    data: pd.Series,
+    fig: Figure,
+    grid: plt.GridSpec,
+    layout: str,
+    line_width: str,
+    line_style: str,
+    legend_name: str,
+    x_lim: str,
+    y_lim: str,
+    x_label: str,
+    y_label: str,
+):
+    plot = plt
+    if grid is not None:
+        row_start, row_end, col_start, col_end = (int(i) for i in layout.split())
+        plot = fig.add_subplot(grid[row_start:row_end, col_start:col_end])
+
+    if plot_type == "line":
+        plot.plot(
+            data.index,
+            data,
+            linestyle=line_style,
+            linewidth=int(line_width),
+            label=legend_name,
+        )
+    elif plot_type == "scatter":
+        plot.scatter(
+            data.index,
+            data,
+            s=int(int(line_width) * 10),
+            marker=line_style,
+            linewidth=int(line_width),
+            label=legend_name,
+        )
+    else:
+        print("Invalid plot type given")
+
+    if grid is None:
+        plot.xlim(x_lim)
+        plot.ylim(y_lim)
+        plot.xlabel(x_label)
+        plot.ylabel(y_label)
+    else:
+        plot.set_xlim(x_lim)
+        plot.set_ylim(y_lim)
+        plot.set_xlabel(x_label)
+        plot.set_ylabel(y_label)
+
+    plt.legend()
+    plt.show()
```

### Comparing `exe_kg_lib-2.0.2/LICENSE.md` & `exe_kg_lib-2.0.3/LICENSE.md`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,660 +1,660 @@
-### GNU AFFERO GENERAL PUBLIC LICENSE
-
-Version 3, 19 November 2007
-
-Copyright (C) 2007 Free Software Foundation, Inc.
-<https://fsf.org/>
-
-Everyone is permitted to copy and distribute verbatim copies of this
-license document, but changing it is not allowed.
-
-### Preamble
-
-The GNU Affero General Public License is a free, copyleft license for
-software and other kinds of works, specifically designed to ensure
-cooperation with the community in the case of network server software.
-
-The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works. By contrast,
-our General Public Licenses are intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains
-free software for all its users.
-
-When we speak of free software, we are referring to freedom, not
-price. Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-Developers that use our General Public Licenses protect your rights
-with two steps: (1) assert copyright on the software, and (2) offer
-you this License which gives you legal permission to copy, distribute
-and/or modify the software.
-
-A secondary benefit of defending all users' freedom is that
-improvements made in alternate versions of the program, if they
-receive widespread use, become available for other developers to
-incorporate. Many developers of free software are heartened and
-encouraged by the resulting cooperation. However, in the case of
-software used on network servers, this result may fail to come about.
-The GNU General Public License permits making a modified version and
-letting the public access it on a server without ever releasing its
-source code to the public.
-
-The GNU Affero General Public License is designed specifically to
-ensure that, in such cases, the modified source code becomes available
-to the community. It requires the operator of a network server to
-provide the source code of the modified version running there to the
-users of that server. Therefore, public use of a modified version, on
-a publicly accessible server, gives the public access to the source
-code of the modified version.
-
-An older license, called the Affero General Public License and
-published by Affero, was designed to accomplish similar goals. This is
-a different license, not a version of the Affero GPL, but Affero has
-released a new version of the Affero GPL which permits relicensing
-under this license.
-
-The precise terms and conditions for copying, distribution and
-modification follow.
-
-### TERMS AND CONDITIONS
-
-#### 0. Definitions.
-
-"This License" refers to version 3 of the GNU Affero General Public
-License.
-
-"Copyright" also means copyright-like laws that apply to other kinds
-of works, such as semiconductor masks.
-
-"The Program" refers to any copyrightable work licensed under this
-License. Each licensee is addressed as "you". "Licensees" and
-"recipients" may be individuals or organizations.
-
-To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of
-an exact copy. The resulting work is called a "modified version" of
-the earlier work or a work "based on" the earlier work.
-
-A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy. Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies. Mere interaction with a user
-through a computer network, with no transfer of a copy, is not
-conveying.
-
-An interactive user interface displays "Appropriate Legal Notices" to
-the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License. If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-#### 1. Source Code.
-
-The "source code" for a work means the preferred form of the work for
-making modifications to it. "Object code" means any non-source form of
-a work.
-
-A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form. A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities. However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work. For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-The Corresponding Source need not include anything that users can
-regenerate automatically from other parts of the Corresponding Source.
-
-The Corresponding Source for a work in source code form is that same
-work.
-
-#### 2. Basic Permissions.
-
-All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met. This License explicitly affirms your unlimited
-permission to run the unmodified Program. The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work. This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-You may make, run and propagate covered works that you do not convey,
-without conditions so long as your license otherwise remains in force.
-You may convey covered works to others for the sole purpose of having
-them make modifications exclusively for you, or provide you with
-facilities for running those works, provided that you comply with the
-terms of this License in conveying all material for which you do not
-control copyright. Those thus making or running the covered works for
-you must do so exclusively on your behalf, under your direction and
-control, on terms that prohibit them from making any copies of your
-copyrighted material outside their relationship with you.
-
-Conveying under any other circumstances is permitted solely under the
-conditions stated below. Sublicensing is not allowed; section 10 makes
-it unnecessary.
-
-#### 3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such
-circumvention is effected by exercising rights under this License with
-respect to the covered work, and you disclaim any intention to limit
-operation or modification of the work as a means of enforcing, against
-the work's users, your or third parties' legal rights to forbid
-circumvention of technological measures.
-
-#### 4. Conveying Verbatim Copies.
-
-You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-#### 5. Conveying Modified Source Versions.
-
-You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these
-conditions:
-
--   a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
--   b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under
-    section 7. This requirement modifies the requirement in section 4
-    to "keep intact all notices".
--   c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy. This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged. This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
--   d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit. Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-#### 6. Conveying Non-Source Forms.
-
-You may convey a covered work in object code form under the terms of
-sections 4 and 5, provided that you also convey the machine-readable
-Corresponding Source under the terms of this License, in one of these
-ways:
-
--   a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
--   b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the Corresponding
-    Source from a network server at no charge.
--   c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source. This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
--   d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge. You need not require recipients to copy the
-    Corresponding Source along with the object code. If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source. Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
--   e) Convey the object code using peer-to-peer transmission,
-    provided you inform other peers where the object code and
-    Corresponding Source of the work are being offered to the general
-    public at no charge under subsection 6d.
-
-A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal,
-family, or household purposes, or (2) anything designed or sold for
-incorporation into a dwelling. In determining whether a product is a
-consumer product, doubtful cases shall be resolved in favor of
-coverage. For a particular product received by a particular user,
-"normally used" refers to a typical or common use of that class of
-product, regardless of the status of the particular user or of the way
-in which the particular user actually uses, or expects or is expected
-to use, the product. A product is a consumer product regardless of
-whether the product has substantial commercial, industrial or
-non-consumer uses, unless such uses represent the only significant
-mode of use of the product.
-
-"Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to
-install and execute modified versions of a covered work in that User
-Product from a modified version of its Corresponding Source. The
-information must suffice to ensure that the continued functioning of
-the modified object code is in no case prevented or interfered with
-solely because modification has been made.
-
-If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information. But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or
-updates for a work that has been modified or installed by the
-recipient, or for the User Product in which it has been modified or
-installed. Access to a network may be denied when the modification
-itself materially and adversely affects the operation of the network
-or violates the rules and protocols for communication across the
-network.
-
-Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-#### 7. Additional Terms.
-
-"Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law. If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it. (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.) You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders
-of that material) supplement the terms of this License with terms:
-
--   a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
--   b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
--   c) Prohibiting misrepresentation of the origin of that material,
-    or requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
--   d) Limiting the use for publicity purposes of names of licensors
-    or authors of the material; or
--   e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
--   f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions
-    of it) with contractual assumptions of liability to the recipient,
-    for any liability that these contractual assumptions directly
-    impose on those licensors and authors.
-
-All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10. If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term. If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions; the
-above requirements apply either way.
-
-#### 8. Termination.
-
-You may not propagate or modify a covered work except as expressly
-provided under this License. Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-However, if you cease all violation of this License, then your license
-from a particular copyright holder is reinstated (a) provisionally,
-unless and until the copyright holder explicitly and finally
-terminates your license, and (b) permanently, if the copyright holder
-fails to notify you of the violation by some reasonable means prior to
-60 days after the cessation.
-
-Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License. If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-#### 9. Acceptance Not Required for Having Copies.
-
-You are not required to accept this License in order to receive or run
-a copy of the Program. Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance. However,
-nothing other than this License grants you permission to propagate or
-modify any covered work. These actions infringe copyright if you do
-not accept this License. Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-#### 10. Automatic Licensing of Downstream Recipients.
-
-Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License. You are not responsible
-for enforcing compliance by third parties with this License.
-
-An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations. If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License. For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-#### 11. Patents.
-
-A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based. The
-work thus licensed is called the contributor's "contributor version".
-
-A contributor's "essential patent claims" are all patent claims owned
-or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version. For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement). To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients. "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-A patent license is "discriminatory" if it does not include within the
-scope of its coverage, prohibits the exercise of, or is conditioned on
-the non-exercise of one or more of the rights that are specifically
-granted under this License. You may not convey a covered work if you
-are a party to an arrangement with a third party that is in the
-business of distributing software, under which you make payment to the
-third party based on the extent of your activity of conveying the
-work, and under which the third party grants, to any of the parties
-who would receive the covered work from you, a discriminatory patent
-license (a) in connection with copies of the covered work conveyed by
-you (or copies made from those copies), or (b) primarily for and in
-connection with specific products or compilations that contain the
-covered work, unless you entered into that arrangement, or that patent
-license was granted, prior to 28 March 2007.
-
-Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-#### 12. No Surrender of Others' Freedom.
-
-If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License. If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under
-this License and any other pertinent obligations, then as a
-consequence you may not convey it at all. For example, if you agree to
-terms that obligate you to collect a royalty for further conveying
-from those to whom you convey the Program, the only way you could
-satisfy both those terms and this License would be to refrain entirely
-from conveying the Program.
-
-#### 13. Remote Network Interaction; Use with the GNU General Public License.
-
-Notwithstanding any other provision of this License, if you modify the
-Program, your modified version must prominently offer all users
-interacting with it remotely through a computer network (if your
-version supports such interaction) an opportunity to receive the
-Corresponding Source of your version by providing access to the
-Corresponding Source from a network server at no charge, through some
-standard or customary means of facilitating copying of software. This
-Corresponding Source shall include the Corresponding Source for any
-work covered by version 3 of the GNU General Public License that is
-incorporated pursuant to the following paragraph.
-
-Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU General Public License into a single
-combined work, and to convey the resulting work. The terms of this
-License will continue to apply to the part which is the covered work,
-but the work with which it is combined will remain governed by version
-3 of the GNU General Public License.
-
-#### 14. Revised Versions of this License.
-
-The Free Software Foundation may publish revised and/or new versions
-of the GNU Affero General Public License from time to time. Such new
-versions will be similar in spirit to the present version, but may
-differ in detail to address new problems or concerns.
-
-Each version is given a distinguishing version number. If the Program
-specifies that a certain numbered version of the GNU Affero General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation. If the Program does not specify a version number of the
-GNU Affero General Public License, you may choose any version ever
-published by the Free Software Foundation.
-
-If the Program specifies that a proxy can decide which future versions
-of the GNU Affero General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-Later license versions may give you additional or different
-permissions. However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-#### 15. Disclaimer of Warranty.
-
-THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT
-WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT
-LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
-A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND
-PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE
-DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR
-CORRECTION.
-
-#### 16. Limitation of Liability.
-
-IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR
-CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES,
-INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES
-ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT
-NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR
-LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM
-TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER
-PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
-
-#### 17. Interpretation of Sections 15 and 16.
-
-If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-END OF TERMS AND CONDITIONS
-
-### How to Apply These Terms to Your New Programs
-
-If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these
-terms.
-
-To do so, attach the following notices to the program. It is safest to
-attach them to the start of each source file to most effectively state
-the exclusion of warranty; and each file should have at least the
-"copyright" line and a pointer to where the full notice is found.
-
-        <one line to give the program's name and a brief idea of what it does.>
-        Copyright (C) <year>  <name of author>
-
-        This program is free software: you can redistribute it and/or modify
-        it under the terms of the GNU Affero General Public License as
-        published by the Free Software Foundation, either version 3 of the
-        License, or (at your option) any later version.
-
-        This program is distributed in the hope that it will be useful,
-        but WITHOUT ANY WARRANTY; without even the implied warranty of
-        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-        GNU Affero General Public License for more details.
-
-        You should have received a copy of the GNU Affero General Public License
-        along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper
-mail.
-
-If your software can interact with users remotely through a computer
-network, you should also make sure that it provides a way for users to
-get its source. For example, if your program is a web application, its
-interface could display a "Source" link that leads users to an archive
-of the code. There are many ways you could offer source, and different
-solutions will be better for different programs; see section 13 for
-the specific requirements.
-
-You should also get your employer (if you work as a programmer) or
-school, if any, to sign a "copyright disclaimer" for the program, if
-necessary. For more information on this, and how to apply and follow
-the GNU AGPL, see <https://www.gnu.org/licenses/>.
+### GNU AFFERO GENERAL PUBLIC LICENSE
+
+Version 3, 19 November 2007
+
+Copyright (C) 2007 Free Software Foundation, Inc.
+<https://fsf.org/>
+
+Everyone is permitted to copy and distribute verbatim copies of this
+license document, but changing it is not allowed.
+
+### Preamble
+
+The GNU Affero General Public License is a free, copyleft license for
+software and other kinds of works, specifically designed to ensure
+cooperation with the community in the case of network server software.
+
+The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works. By contrast,
+our General Public Licenses are intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains
+free software for all its users.
+
+When we speak of free software, we are referring to freedom, not
+price. Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+Developers that use our General Public Licenses protect your rights
+with two steps: (1) assert copyright on the software, and (2) offer
+you this License which gives you legal permission to copy, distribute
+and/or modify the software.
+
+A secondary benefit of defending all users' freedom is that
+improvements made in alternate versions of the program, if they
+receive widespread use, become available for other developers to
+incorporate. Many developers of free software are heartened and
+encouraged by the resulting cooperation. However, in the case of
+software used on network servers, this result may fail to come about.
+The GNU General Public License permits making a modified version and
+letting the public access it on a server without ever releasing its
+source code to the public.
+
+The GNU Affero General Public License is designed specifically to
+ensure that, in such cases, the modified source code becomes available
+to the community. It requires the operator of a network server to
+provide the source code of the modified version running there to the
+users of that server. Therefore, public use of a modified version, on
+a publicly accessible server, gives the public access to the source
+code of the modified version.
+
+An older license, called the Affero General Public License and
+published by Affero, was designed to accomplish similar goals. This is
+a different license, not a version of the Affero GPL, but Affero has
+released a new version of the Affero GPL which permits relicensing
+under this license.
+
+The precise terms and conditions for copying, distribution and
+modification follow.
+
+### TERMS AND CONDITIONS
+
+#### 0. Definitions.
+
+"This License" refers to version 3 of the GNU Affero General Public
+License.
+
+"Copyright" also means copyright-like laws that apply to other kinds
+of works, such as semiconductor masks.
+
+"The Program" refers to any copyrightable work licensed under this
+License. Each licensee is addressed as "you". "Licensees" and
+"recipients" may be individuals or organizations.
+
+To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of
+an exact copy. The resulting work is called a "modified version" of
+the earlier work or a work "based on" the earlier work.
+
+A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy. Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies. Mere interaction with a user
+through a computer network, with no transfer of a copy, is not
+conveying.
+
+An interactive user interface displays "Appropriate Legal Notices" to
+the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License. If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+#### 1. Source Code.
+
+The "source code" for a work means the preferred form of the work for
+making modifications to it. "Object code" means any non-source form of
+a work.
+
+A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form. A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities. However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work. For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+The Corresponding Source need not include anything that users can
+regenerate automatically from other parts of the Corresponding Source.
+
+The Corresponding Source for a work in source code form is that same
+work.
+
+#### 2. Basic Permissions.
+
+All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met. This License explicitly affirms your unlimited
+permission to run the unmodified Program. The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work. This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+You may make, run and propagate covered works that you do not convey,
+without conditions so long as your license otherwise remains in force.
+You may convey covered works to others for the sole purpose of having
+them make modifications exclusively for you, or provide you with
+facilities for running those works, provided that you comply with the
+terms of this License in conveying all material for which you do not
+control copyright. Those thus making or running the covered works for
+you must do so exclusively on your behalf, under your direction and
+control, on terms that prohibit them from making any copies of your
+copyrighted material outside their relationship with you.
+
+Conveying under any other circumstances is permitted solely under the
+conditions stated below. Sublicensing is not allowed; section 10 makes
+it unnecessary.
+
+#### 3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such
+circumvention is effected by exercising rights under this License with
+respect to the covered work, and you disclaim any intention to limit
+operation or modification of the work as a means of enforcing, against
+the work's users, your or third parties' legal rights to forbid
+circumvention of technological measures.
+
+#### 4. Conveying Verbatim Copies.
+
+You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+#### 5. Conveying Modified Source Versions.
+
+You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these
+conditions:
+
+-   a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+-   b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under
+    section 7. This requirement modifies the requirement in section 4
+    to "keep intact all notices".
+-   c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy. This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged. This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+-   d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit. Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+#### 6. Conveying Non-Source Forms.
+
+You may convey a covered work in object code form under the terms of
+sections 4 and 5, provided that you also convey the machine-readable
+Corresponding Source under the terms of this License, in one of these
+ways:
+
+-   a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+-   b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the Corresponding
+    Source from a network server at no charge.
+-   c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source. This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+-   d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge. You need not require recipients to copy the
+    Corresponding Source along with the object code. If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source. Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+-   e) Convey the object code using peer-to-peer transmission,
+    provided you inform other peers where the object code and
+    Corresponding Source of the work are being offered to the general
+    public at no charge under subsection 6d.
+
+A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal,
+family, or household purposes, or (2) anything designed or sold for
+incorporation into a dwelling. In determining whether a product is a
+consumer product, doubtful cases shall be resolved in favor of
+coverage. For a particular product received by a particular user,
+"normally used" refers to a typical or common use of that class of
+product, regardless of the status of the particular user or of the way
+in which the particular user actually uses, or expects or is expected
+to use, the product. A product is a consumer product regardless of
+whether the product has substantial commercial, industrial or
+non-consumer uses, unless such uses represent the only significant
+mode of use of the product.
+
+"Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to
+install and execute modified versions of a covered work in that User
+Product from a modified version of its Corresponding Source. The
+information must suffice to ensure that the continued functioning of
+the modified object code is in no case prevented or interfered with
+solely because modification has been made.
+
+If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information. But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or
+updates for a work that has been modified or installed by the
+recipient, or for the User Product in which it has been modified or
+installed. Access to a network may be denied when the modification
+itself materially and adversely affects the operation of the network
+or violates the rules and protocols for communication across the
+network.
+
+Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+#### 7. Additional Terms.
+
+"Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law. If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it. (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.) You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders
+of that material) supplement the terms of this License with terms:
+
+-   a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+-   b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+-   c) Prohibiting misrepresentation of the origin of that material,
+    or requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+-   d) Limiting the use for publicity purposes of names of licensors
+    or authors of the material; or
+-   e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+-   f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions
+    of it) with contractual assumptions of liability to the recipient,
+    for any liability that these contractual assumptions directly
+    impose on those licensors and authors.
+
+All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10. If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term. If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions; the
+above requirements apply either way.
+
+#### 8. Termination.
+
+You may not propagate or modify a covered work except as expressly
+provided under this License. Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+However, if you cease all violation of this License, then your license
+from a particular copyright holder is reinstated (a) provisionally,
+unless and until the copyright holder explicitly and finally
+terminates your license, and (b) permanently, if the copyright holder
+fails to notify you of the violation by some reasonable means prior to
+60 days after the cessation.
+
+Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License. If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+#### 9. Acceptance Not Required for Having Copies.
+
+You are not required to accept this License in order to receive or run
+a copy of the Program. Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance. However,
+nothing other than this License grants you permission to propagate or
+modify any covered work. These actions infringe copyright if you do
+not accept this License. Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+#### 10. Automatic Licensing of Downstream Recipients.
+
+Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License. You are not responsible
+for enforcing compliance by third parties with this License.
+
+An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations. If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License. For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+#### 11. Patents.
+
+A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based. The
+work thus licensed is called the contributor's "contributor version".
+
+A contributor's "essential patent claims" are all patent claims owned
+or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version. For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement). To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients. "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+A patent license is "discriminatory" if it does not include within the
+scope of its coverage, prohibits the exercise of, or is conditioned on
+the non-exercise of one or more of the rights that are specifically
+granted under this License. You may not convey a covered work if you
+are a party to an arrangement with a third party that is in the
+business of distributing software, under which you make payment to the
+third party based on the extent of your activity of conveying the
+work, and under which the third party grants, to any of the parties
+who would receive the covered work from you, a discriminatory patent
+license (a) in connection with copies of the covered work conveyed by
+you (or copies made from those copies), or (b) primarily for and in
+connection with specific products or compilations that contain the
+covered work, unless you entered into that arrangement, or that patent
+license was granted, prior to 28 March 2007.
+
+Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+#### 12. No Surrender of Others' Freedom.
+
+If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License. If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under
+this License and any other pertinent obligations, then as a
+consequence you may not convey it at all. For example, if you agree to
+terms that obligate you to collect a royalty for further conveying
+from those to whom you convey the Program, the only way you could
+satisfy both those terms and this License would be to refrain entirely
+from conveying the Program.
+
+#### 13. Remote Network Interaction; Use with the GNU General Public License.
+
+Notwithstanding any other provision of this License, if you modify the
+Program, your modified version must prominently offer all users
+interacting with it remotely through a computer network (if your
+version supports such interaction) an opportunity to receive the
+Corresponding Source of your version by providing access to the
+Corresponding Source from a network server at no charge, through some
+standard or customary means of facilitating copying of software. This
+Corresponding Source shall include the Corresponding Source for any
+work covered by version 3 of the GNU General Public License that is
+incorporated pursuant to the following paragraph.
+
+Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU General Public License into a single
+combined work, and to convey the resulting work. The terms of this
+License will continue to apply to the part which is the covered work,
+but the work with which it is combined will remain governed by version
+3 of the GNU General Public License.
+
+#### 14. Revised Versions of this License.
+
+The Free Software Foundation may publish revised and/or new versions
+of the GNU Affero General Public License from time to time. Such new
+versions will be similar in spirit to the present version, but may
+differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number. If the Program
+specifies that a certain numbered version of the GNU Affero General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation. If the Program does not specify a version number of the
+GNU Affero General Public License, you may choose any version ever
+published by the Free Software Foundation.
+
+If the Program specifies that a proxy can decide which future versions
+of the GNU Affero General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+Later license versions may give you additional or different
+permissions. However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+#### 15. Disclaimer of Warranty.
+
+THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT
+WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT
+LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
+A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND
+PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE
+DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR
+CORRECTION.
+
+#### 16. Limitation of Liability.
+
+IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR
+CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES,
+INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES
+ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT
+NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR
+LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM
+TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER
+PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
+
+#### 17. Interpretation of Sections 15 and 16.
+
+If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+END OF TERMS AND CONDITIONS
+
+### How to Apply These Terms to Your New Programs
+
+If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these
+terms.
+
+To do so, attach the following notices to the program. It is safest to
+attach them to the start of each source file to most effectively state
+the exclusion of warranty; and each file should have at least the
+"copyright" line and a pointer to where the full notice is found.
+
+        <one line to give the program's name and a brief idea of what it does.>
+        Copyright (C) <year>  <name of author>
+
+        This program is free software: you can redistribute it and/or modify
+        it under the terms of the GNU Affero General Public License as
+        published by the Free Software Foundation, either version 3 of the
+        License, or (at your option) any later version.
+
+        This program is distributed in the hope that it will be useful,
+        but WITHOUT ANY WARRANTY; without even the implied warranty of
+        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+        GNU Affero General Public License for more details.
+
+        You should have received a copy of the GNU Affero General Public License
+        along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper
+mail.
+
+If your software can interact with users remotely through a computer
+network, you should also make sure that it provides a way for users to
+get its source. For example, if your program is a web application, its
+interface could display a "Source" link that leads users to an archive
+of the code. There are many ways you could offer source, and different
+solutions will be better for different programs; see section 13 for
+the specific requirements.
+
+You should also get your employer (if you work as a programmer) or
+school, if any, to sign a "copyright disclaimer" for the program, if
+necessary. For more information on this, and how to apply and follow
+the GNU AGPL, see <https://www.gnu.org/licenses/>.
```

### Comparing `exe_kg_lib-2.0.2/pyproject.toml` & `exe_kg_lib-2.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-[tool.poetry]
-name = "exe-kg-lib"
-version = "2.0.2" # not used when bumping version via poe bump-version-tag or cd.yaml
-description = "Library for executable ML pipelines represented by KGs."
-license = "AGPL-3.0"
-authors = ["Antonis Klironomos <antonis.klironomos@de.bosch.com>", "Mohamed Gad-Elrab <mohamed.gad-elrab@de.bosch.com>"]
-
-classifiers = [
-  "Development Status :: 1 - Planning",
-  "Intended Audience :: Developers",
-  "Intended Audience :: Science/Research",
-  "Natural Language :: English",
-  "Programming Language :: Python :: 3",
-  "Topic :: Scientific/Engineering",
-  "Topic :: Software Development",
-]
-
-homepage = "https://boschresearch.github.io/ExeKGLib"
-include = ["README.md", "pyproject.toml"]
-maintainers = ["Antonis Klironomos <antonis.klironomos@de.bosch.com>", "Mohamed Gad-Elrab <mohamed.gad-elrab@de.bosch.com>"]
-readme = "README.md"
-repository = "https://github.com/boschresearch/ExeKGLib"
-
-[build-system]
-requires = ["poetry-core>=1.3.2"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.poetry.dependencies]
-python = "^3.8"
-typer = "^0.7.0"
-pandas = "^1.5.2"
-scikit-learn = "^1.1.3"
-black = {extras = ["d"], version = ">=22.10,<24.0"}
-matplotlib = "^3.6.2"
-rdflib = "^6.2.0"
-mkdocs = "^1.4.2"
-typer-cli = "^0.0.13"
-
-[tool.poetry.group.dev.dependencies]
-black = ">=22.10,<24.0"
-genbadge = {extras = ["coverage", "tests"], version = "^1.1.0"}
-isort = {extras = ["colors"], version = "^5.10.1"}
-mkdocs-gen-files = "^0.4.0"
-mkdocs-git-revision-date-localized-plugin = "^1.1.0"
-mkdocs-literate-nav = ">=0.5,<0.7"
-mkdocs-material = ">=8.5.10,<10.0.0"
-mkdocs-minify-plugin = "^0.6.2"
-mkdocstrings-python = "^0.8.2"
-poethepoet = ">=0.16.5,<0.19.0"
-pre-commit = ">=2.20,<4.0"
-pytest = ">=7.2.0"
-pytest-cov = "^4.0.0"
-pytest-html = "^3.2.0"
-pytest-xdist = "^3.0.2"
-pyupgrade = "^3.2.3"
-
-# Tools config
-[tool.black]
-line-length = 120
-
-[tool.coverage.report]
-fail_under = 60
-show_missing = true
-skip_empty = true
-
-[tool.coverage.run]
-branch = true
-source = ["exe_kg_lib"]
-
-[tool.pytest.ini_options]
-addopts = [
-  "--cov",
-  "--cov-config=pyproject.toml",
-  "--full-trace",
-  "--html=docs/exported/tests/report.html",
-  "--junit-xml=pytest.xml",
-  "--numprocesses=auto",
-  "--self-contained-html",
-  "--showlocals",
-  "-ra",
-]
-
-# Task runner config
-[tool.poe]
-shell_interpreter = "bash"
-verbosity = 1
-
-[tool.poe.tasks.format]
-sequence = [
-  { shell = "shopt -s globstar; black ${check:+ --check --diff} ${files}" },
-  { shell = "shopt -s globstar; isort --color ${check:+ --check --diff} ${files}" },
-  { shell = "shopt -s globstar; pyupgrade --py38-plus ${files}" },
-]
-help = "Format Python files with black & isort."
-args = [
-  { name = "check", type = "boolean", help = "Only check" },
-  { name = "files", positional = true, multiple = true, default = "**/*.py", help = "List of files (optional)" },
-]
-
-[tool.poe.tasks.bump-version-tag]
-shell = """
-GIT_LATEST_TAG=$(git describe --tags --abbrev=0)
-poetry version $GIT_LATEST_TAG
-poetry version ${rule}
-VERSION=$(poetry version | cut -d' ' -f2 | tr -d '\n')
-git tag -a "${VERSION}" -m "Version ${VERSION}"
-git push --follow-tags
-"""
-help = "Bump Poetry version and create Git tag."
-args = [
-  { name = "rule", positional = true, help = "Version bump rule." },
-]
-
-[tool.poe.tasks.bump-version-tag-with-semantic-rule]
-shell = """
-HEAD_COMMIT_CONTENT=$(git log -1)
-
-RULE="patch"
-if [[ $HEAD_COMMIT_CONTENT == *"MAJOR_CHANGE"* ]]; then
-  RULE="major"
-elif [[ $HEAD_COMMIT_CONTENT == *"MINOR_CHANGE"* ]]; then
-  RULE="minor"
-fi
-
-poetry run poe bump-version-tag ${RULE}
-"""
-help = "Bump Poetry version after semantically checking HEAD commit message and create Git tag."
-args = []
+[tool.poetry]
+name = "exe-kg-lib"
+version = "2.0.3" # not used when bumping version via poe bump-version-tag or cd.yaml
+description = "Library for executable ML pipelines represented by KGs."
+license = "AGPL-3.0"
+authors = ["Antonis Klironomos <antonis.klironomos@de.bosch.com>", "Mohamed Gad-Elrab <mohamed.gad-elrab@de.bosch.com>"]
+
+classifiers = [
+  "Development Status :: 1 - Planning",
+  "Intended Audience :: Developers",
+  "Intended Audience :: Science/Research",
+  "Natural Language :: English",
+  "Programming Language :: Python :: 3",
+  "Topic :: Scientific/Engineering",
+  "Topic :: Software Development",
+]
+
+homepage = "https://boschresearch.github.io/ExeKGLib"
+include = ["README.md", "pyproject.toml"]
+maintainers = ["Antonis Klironomos <antonis.klironomos@de.bosch.com>", "Mohamed Gad-Elrab <mohamed.gad-elrab@de.bosch.com>"]
+readme = "README.md"
+repository = "https://github.com/boschresearch/ExeKGLib"
+
+[build-system]
+requires = ["poetry-core>=1.3.2"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.dependencies]
+python = "^3.8"
+typer = "^0.7.0"
+pandas = "^1.5.2"
+scikit-learn = "^1.1.3"
+black = {extras = ["d"], version = ">=22.10,<24.0"}
+matplotlib = "^3.6.2"
+rdflib = "^6.2.0"
+mkdocs = "^1.4.2"
+typer-cli = "^0.0.13"
+
+[tool.poetry.group.dev.dependencies]
+black = ">=22.10,<24.0"
+genbadge = {extras = ["coverage", "tests"], version = "^1.1.0"}
+isort = {extras = ["colors"], version = "^5.10.1"}
+mkdocs-gen-files = "^0.4.0"
+mkdocs-git-revision-date-localized-plugin = "^1.1.0"
+mkdocs-literate-nav = ">=0.5,<0.7"
+mkdocs-material = ">=8.5.10,<10.0.0"
+mkdocs-minify-plugin = "^0.6.2"
+mkdocstrings-python = "^0.8.2"
+poethepoet = ">=0.16.5,<0.19.0"
+pre-commit = ">=2.20,<4.0"
+pytest = ">=7.2.0"
+pytest-cov = "^4.0.0"
+pytest-html = "^3.2.0"
+pytest-xdist = "^3.0.2"
+pyupgrade = "^3.2.3"
+
+# Tools config
+[tool.black]
+line-length = 120
+
+[tool.coverage.report]
+fail_under = 60
+show_missing = true
+skip_empty = true
+
+[tool.coverage.run]
+branch = true
+source = ["exe_kg_lib"]
+
+[tool.pytest.ini_options]
+addopts = [
+  "--cov",
+  "--cov-config=pyproject.toml",
+  "--full-trace",
+  "--html=docs/exported/tests/report.html",
+  "--junit-xml=pytest.xml",
+  "--numprocesses=auto",
+  "--self-contained-html",
+  "--showlocals",
+  "-ra",
+]
+
+# Task runner config
+[tool.poe]
+shell_interpreter = "bash"
+verbosity = 1
+
+[tool.poe.tasks.format]
+sequence = [
+  { shell = "shopt -s globstar; black ${check:+ --check --diff} ${files}" },
+  { shell = "shopt -s globstar; isort --color ${check:+ --check --diff} ${files}" },
+  { shell = "shopt -s globstar; pyupgrade --py38-plus ${files}" },
+]
+help = "Format Python files with black & isort."
+args = [
+  { name = "check", type = "boolean", help = "Only check" },
+  { name = "files", positional = true, multiple = true, default = "**/*.py", help = "List of files (optional)" },
+]
+
+[tool.poe.tasks.bump-version-tag]
+shell = """
+GIT_LATEST_TAG=$(git describe --tags --abbrev=0)
+poetry version $GIT_LATEST_TAG
+poetry version ${rule}
+VERSION=$(poetry version | cut -d' ' -f2 | tr -d '\n')
+git tag -a "${VERSION}" -m "Version ${VERSION}"
+git push --follow-tags
+"""
+help = "Bump Poetry version and create Git tag."
+args = [
+  { name = "rule", positional = true, help = "Version bump rule." },
+]
+
+[tool.poe.tasks.bump-version-tag-with-semantic-rule]
+shell = """
+HEAD_COMMIT_CONTENT=$(git log -1)
+
+RULE="patch"
+if [[ $HEAD_COMMIT_CONTENT == *"MAJOR_CHANGE"* ]]; then
+  RULE="major"
+elif [[ $HEAD_COMMIT_CONTENT == *"MINOR_CHANGE"* ]]; then
+  RULE="minor"
+fi
+
+poetry run poe bump-version-tag ${RULE}
+"""
+help = "Bump Poetry version after semantically checking HEAD commit message and create Git tag."
+args = []
```

### Comparing `exe_kg_lib-2.0.2/README.md` & `exe_kg_lib-2.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-# ExeKGLib
-
-![PyPI](https://img.shields.io/pypi/v/exe-kg-lib)
-![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)
-![Poetry](https://img.shields.io/badge/poetry-v1.2.2-blue)
-[![Code style: black][black-badge]][black]
-[![License](https://img.shields.io/badge/license-AGPL%203.0-blue)](https://www.gnu.org/licenses/agpl-3.0.en.html)
-
-[//]: # (--8<-- [start:overview])
-Python library for conveniently constructing and executing Machine Learning (ML) pipelines represented by Knowledge Graphs (KGs). It features a coding interface and a CLI, and allows the user to:
-
-1. **Construct** an ML pipeline that gets a CSV as input and processes the data using any of the [available tasks and methods](https://github.com/boschresearch/ExeKGLib/tree/main/README.md#Ready-to-use-ML-related-tasks-and-methods).
-2. **Save** the constructed pipeline as a KG in Turtle format.
-3. **Execute** the generated KG.
-
-The coding interface is demonstrated with [three sample Python files](https://github.com/boschresearch/ExeKGLib/tree/main/examples). The pipelines represented by the generated sample KGs are briefly explained below:
-
-1. **ML pipeline**: Loads features and labels from an input CSV dataset, splits the data, trains and tests a k-NN model, and visualizes the prediction errors.
-2. **Statistics pipeline**: Loads a feature from an input CSV dataset, normalizes it, and plots its values (before and after normalization) using a scatter plot.
-3. **Visualization pipeline**: Loads a feature from an input CSV dataset and plots its values using a line plot.
-
-Under the hood, **ExeKGLib** uses well-known Python libraries for data processing and visualization and performing predictions such as [pandas](https://pandas.pydata.org/), [matplotlib](https://matplotlib.org/), and [scikit-learn](https://scikit-learn.org/).
-
-**ExeKGLib** is part of the following paper submitted to ESWC 2023:<br>
-_Klironomos A., Zhou B., Tan Z., Zheng Z., Gad-Elrab M., Paulheim H., Kharlamov E.: **ExeKGLib: A Python Library for Machine Learning Analytics based on Knowledge Graphs**_
-
-[//]: # (--8<-- [end:overview])
-
-Detailed information (installation, documentation etc.) about **ExeKGLib** can be found in [its website](https://boschresearch.github.io/ExeKGLib/) and basic information is shown below.
-
-## Installation
-
-[//]: # (--8<-- [start:installation])
-To install, run `pip install exe-kg-lib`.
-
-[//]: # (--8<-- [end:installation])
-
-For detailed installation instructions, refer to the [installation page](https://boschresearch.github.io/ExeKGLib/installation/) of **ExeKGLib**'s website.
-
-## Ready-to-use ML-related tasks and methods
-
-<details>
-  <summary>Click to expand</summary>
-
-<!-- --8<-- [start:supportedmethods] -->
-| KG schema (abbreviation) | Task                      | Method                       | Properties                                                                                    | Input (data structure)                                                                                                                                           | Output (data structure)                                                                                                                                                                    | Implemented by Python class                          |
-| ------------------------ | ------------------------- | ---------------------------- | --------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------- |
-| Machine Learning (ML)    | Train                     | KNNTrain                     | \-                                                                                            | DataInTrainX (Matrix or Vector)<br>DataInTrainY (Matrix or Vector)                                                                                               | DataOutPredictedValueTrain (Matrix or Vector)<br>DataOutTrainModel (SingleValue)                                                                                                           | TrainKNNTrain                                        |
-| Machine Learning (ML)    | Train                     | MLPTrain                     | \-                                                                                            | DataInTrainX (Matrix or Vector)<br>DataInTrainY (Matrix or Vector)                                                                                               | DataOutPredictedValueTrain (Matrix or Vector)<br>DataOutTrainModel (SingleValue)                                                                                                           | TrainMLPTrain                                        |
-| Machine Learning (ML)    | Train                     | LRTrain                      | \-                                                                                            | DataInTrainX (Matrix or Vector)<br>DataInTrainY (Matrix or Vector)                                                                                               | DataOutPredictedValueTrain (Matrix or Vector)<br>DataOutTrainModel (SingleValue)                                                                                                           | TrainLRTrain                                         |
-| Machine Learning (ML)    | Test                      | KNNTest                      | \-                                                                                            | DataInTestModel (SingleValue)<br>DataInTestX (Matrix or Vector)                                                                                                  | DataOutPredictedValueTest (Matrix or Vector)                                                                                                                                               | TestKNNTest                                          |
-| Machine Learning (ML)    | Test                      | MLPTest                      | \-                                                                                            | DataInTestModel (SingleValue)<br>DataInTestX (Matrix or Vector)                                                                                                  | DataOutPredictedValueTest (Matrix or Vector)                                                                                                                                               | TestMLPTest                                          |
-| Machine Learning (ML)    | Test                      | LRTest                       | \-                                                                                            | DataInTestModel (SingleValue)<br>DataInTestX (Matrix or Vector)                                                                                                  | DataOutPredictedValueTest (Matrix or Vector)                                                                                                                                               | TestLRTest                                           |
-| Machine Learning (ML)    | PerformanceCalculation    | PerformanceCalculationMethod | \-                                                                                            | DataInTrainRealY (Matrix or Vector)<br>DataInTrainPredictedY (Matrix or Vector)<br>DataInTestPredictedY (Matrix or Vector)<br>DataInTestRealY (Matrix or Vector) | DataOutMLTestErr (Vector)<br>DataOutMLTrainErr (Vector)                                                                                                                                    | PerformanceCalculationPerformanceCalculationMethod   |
-| Machine Learning (ML)    | Concatenation             | ConcatenationMethod          | \-                                                                                            | DataInConcatenation (list of Vector)                                                                                                                             | DataOutConcatenatedData (Matrix)                                                                                                                                                           | ConcatenationConcatenationMethod                     |
-| Machine Learning (ML)    | DataSplitting             | DataSplittingMethod          | \-                                                                                            | DataInDataSplittingX (Matrix or Vector)<br>DataInDataSplittingY (Matrix or Vector)                                                                               | DataOutSplittedTestDataX (Matrix or Vector)<br>DataOutSplittedTrainDataY (Matrix or Vector)<br>DataOutSplittedTrainDataX (Matrix or Vector)<br>DataOutSplittedTestDataY (Matrix or Vector) | DataSplittingDataSplittingMethod                     |
-| Visualization (Visu)     | CanvasTask                | CanvasMethod                 | hasCanvasName (string)<br>hasLayout (string)                                                  | \-                                                                                                                                                               | \-                                                                                                                                                                                         | CanvasTaskCanvasMethod                               |
-| Visualization (Visu)     | PlotTask                  | LineplotMethod               | hasLineStyle (string)<br>hasLineWidth (int)<br>hasLegendName (string)                         | DataInVector (Vector)                                                                                                                                            | \-                                                                                                                                                                                         | PlotTaskLineplotMethod                               |
-| Visualization (Visu)     | PlotTask                  | ScatterplotMethod            | hasLineStyle (string)<br>hasLineWidth (int)<br>hasScatterSize (int)<br>hasLegendName (string) | DataInVector (Vector)                                                                                                                                            | \-                                                                                                                                                                                         | PlotTaskScatterplotMethod                            |
-| Statistics (Stats)       | TrendCalculationTask      | TrendCalculationMethod       | \-                                                                                            | DataInTrendCalculation (Vector)                                                                                                                                  | DataOutTrendCalculation (Vector)                                                                                                                                                           | TrendCalculationTaskTrendCalculationMethod           |
-| Statistics (Stats)       | NormalizationTask         | NormalizationMethod          | \-                                                                                            | DataInNormalization (Vector)                                                                                                                                     | DataOutNormalization (Vector)                                                                                                                                                              | NormalizationTaskNormalizationMethod                 |
-| Statistics (Stats)       | ScatteringCalculationTask | ScatteringCalculationMethod  | \-                                                                                            | DataInScatteringCalculation (Vector)                                                                                                                             | DataOutScatteringCalculation (Vector)                                                                                                                                                      | ScatteringCalculationTaskScatteringCalculationMethod |
-
-[//]: # (--8<-- [end:supportedmethods])
-
-</details>
-
-## Usage
-
-[//]: # (--8<-- [start:usage])
-### Creating an ML pipeline
-
-- **Via code**: See the [provided examples](https://github.com/boschresearch/ExeKGLib/tree/main/examples). To fetch them to your working directory for easy access, run `typer exe_kg_lib.cli.main run get-examples`.
-- **Step-by-step via CLI**: Run `typer exe_kg_lib.cli.main run create-pipeline`.
-
-### Executing an ML pipeline
-Run `typer exe_kg_lib.cli.main run run-pipeline <pipeline_path>`.
-
-[//]: # (--8<-- [end:usage])
-
-## Adding a new ML-related task and method
-
-[//]: # (--8<-- [start:extending])
-To perform this type of **ExeKGLib** extension, there are 3 required steps:
-
-1. Selection of a relevant bottom-level KG schema (Statistics, ML, or Visualization) according to the type of the new task and method.
-2. Addition of new semantic components (entities, properties, etc) to the selected KG schema.
-3. Addition of a Python class to the corresponding module of `exe_kg_lib.classes.tasks` package.
-
-For steps 2 and 3, refer to the [relevant page](https://boschresearch.github.io/ExeKGLib/adding-new-task-and-method/) of **ExeKGLib**'s website.
-
-[//]: # (--8<-- [end:extending])
-
-## Documentation
-See the _Code Reference_ and _Development_ sections of the [**ExeKGLib**'s website](https://boschresearch.github.io/ExeKGLib/).
-
-## External resources
-
-[//]: # (--8<-- [start:externalresources])
-### KG schemata
-
-- **Top-level**: [Data Science](https://w3id.org/def/exekg-ds)
-- **Bottom-level**: [Visualization](https://w3id.org/def/exekg-visu) | [Statistics](https://w3id.org/def/exekg-stats) | [Machine Learning](https://w3id.org/def/exekg-ml)
-
-The above KG schemata are included in the [ExeKGOntology repository](https://github.com/nsai-uio/ExeKGOntology).
-
-### Dataset used in code examples
-[The dataset](https://github.com/boschresearch/ExeKGLib/tree/main/examples/data/dummy_data.csv) was generated using the `sklearn.datasets.make_classification()` function of the [scikit-learn Python library](https://scikit-learn.org/).
-
-[//]: # (--8<-- [end:externalresources])
-
-## License
-
-ExeKGLib is open-sourced under the AGPL-3.0 license. See the
-[LICENSE](LICENSE.md) file for details.
-
-<!-- URLs -->
-[black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
-[black]: https://github.com/psf/black
-[ci-badge]: https://github.com/boschresearch/ExeKGLib/actions/workflows/ci.yaml/badge.svg
-[ci]: https://github.com/boschresearch/ExeKGLib/actions/workflows/ci.yaml
-[docs-badge]: https://img.shields.io/badge/docs-gh--pages-inactive
-[docs]: https://github.com/boschresearch/ExeKGLib/tree/gh-pages
-[license-badge]: https://img.shields.io/badge/License-All%20rights%20reserved-informational
-[license-url]: https://pages.github.boschdevcloud.com/bcai-internal//latest/license
-[pre-commit-badge]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
-[pre-commit]: https://github.com/pre-commit/pre-commit
+# ExeKGLib
+
+![PyPI](https://img.shields.io/pypi/v/exe-kg-lib)
+![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)
+![Poetry](https://img.shields.io/badge/poetry-v1.2.2-blue)
+[![Code style: black][black-badge]][black]
+[![License](https://img.shields.io/badge/license-AGPL%203.0-blue)](https://www.gnu.org/licenses/agpl-3.0.en.html)
+
+[//]: # (--8<-- [start:overview])
+Python library for conveniently constructing and executing Machine Learning (ML) pipelines represented by Knowledge Graphs (KGs). It features a coding interface and a CLI, and allows the user to:
+
+1. **Construct** an ML pipeline that gets a CSV as input and processes the data using any of the [available tasks and methods](https://github.com/boschresearch/ExeKGLib/tree/main/README.md#Ready-to-use-ML-related-tasks-and-methods).
+2. **Save** the constructed pipeline as a KG in Turtle format.
+3. **Execute** the generated KG.
+
+The coding interface is demonstrated with [three sample Python files](https://github.com/boschresearch/ExeKGLib/tree/main/examples). The pipelines represented by the generated sample KGs are briefly explained below:
+
+1. **ML pipeline**: Loads features and labels from an input CSV dataset, splits the data, trains and tests a k-NN model, and visualizes the prediction errors.
+2. **Statistics pipeline**: Loads a feature from an input CSV dataset, normalizes it, and plots its values (before and after normalization) using a scatter plot.
+3. **Visualization pipeline**: Loads a feature from an input CSV dataset and plots its values using a line plot.
+
+Under the hood, **ExeKGLib** uses well-known Python libraries for data processing and visualization and performing predictions such as [pandas](https://pandas.pydata.org/), [matplotlib](https://matplotlib.org/), and [scikit-learn](https://scikit-learn.org/).
+
+**ExeKGLib** is part of the following paper submitted to ESWC 2023:<br>
+_Klironomos A., Zhou B., Tan Z., Zheng Z., Gad-Elrab M., Paulheim H., Kharlamov E.: **ExeKGLib: A Python Library for Machine Learning Analytics based on Knowledge Graphs**_
+
+[//]: # (--8<-- [end:overview])
+
+Detailed information (installation, documentation etc.) about **ExeKGLib** can be found in [its website](https://boschresearch.github.io/ExeKGLib/) and basic information is shown below.
+
+## Installation
+
+[//]: # (--8<-- [start:installation])
+To install, run `pip install exe-kg-lib`.
+
+[//]: # (--8<-- [end:installation])
+
+For detailed installation instructions, refer to the [installation page](https://boschresearch.github.io/ExeKGLib/installation/) of **ExeKGLib**'s website.
+
+## Ready-to-use ML-related tasks and methods
+
+<details>
+  <summary>Click to expand</summary>
+
+<!-- --8<-- [start:supportedmethods] -->
+| KG schema (abbreviation) | Task                      | Method                       | Properties                                                                                    | Input (data structure)                                                                                                                                           | Output (data structure)                                                                                                                                                                    | Implemented by Python class                          |
+| ------------------------ | ------------------------- | ---------------------------- | --------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------- |
+| Machine Learning (ml)    | Train                     | KNNTrain                     | \-                                                                                            | DataInTrainX (Matrix or Vector)<br>DataInTrainY (Matrix or Vector)                                                                                               | DataOutPredictedValueTrain (Matrix or Vector)<br>DataOutTrainModel (SingleValue)                                                                                                           | TrainKNNTrain                                        |
+| Machine Learning (ml)    | Train                     | MLPTrain                     | \-                                                                                            | DataInTrainX (Matrix or Vector)<br>DataInTrainY (Matrix or Vector)                                                                                               | DataOutPredictedValueTrain (Matrix or Vector)<br>DataOutTrainModel (SingleValue)                                                                                                           | TrainMLPTrain                                        |
+| Machine Learning (ml)    | Train                     | LRTrain                      | \-                                                                                            | DataInTrainX (Matrix or Vector)<br>DataInTrainY (Matrix or Vector)                                                                                               | DataOutPredictedValueTrain (Matrix or Vector)<br>DataOutTrainModel (SingleValue)                                                                                                           | TrainLRTrain                                         |
+| Machine Learning (ml)    | Test                      | KNNTest                      | \-                                                                                            | DataInTestModel (SingleValue)<br>DataInTestX (Matrix or Vector)                                                                                                  | DataOutPredictedValueTest (Matrix or Vector)                                                                                                                                               | TestKNNTest                                          |
+| Machine Learning (ml)    | Test                      | MLPTest                      | \-                                                                                            | DataInTestModel (SingleValue)<br>DataInTestX (Matrix or Vector)                                                                                                  | DataOutPredictedValueTest (Matrix or Vector)                                                                                                                                               | TestMLPTest                                          |
+| Machine Learning (ml)    | Test                      | LRTest                       | \-                                                                                            | DataInTestModel (SingleValue)<br>DataInTestX (Matrix or Vector)                                                                                                  | DataOutPredictedValueTest (Matrix or Vector)                                                                                                                                               | TestLRTest                                           |
+| Machine Learning (ml)    | PerformanceCalculation    | PerformanceCalculationMethod | \-                                                                                            | DataInTrainRealY (Matrix or Vector)<br>DataInTrainPredictedY (Matrix or Vector)<br>DataInTestPredictedY (Matrix or Vector)<br>DataInTestRealY (Matrix or Vector) | DataOutMLTestErr (Vector)<br>DataOutMLTrainErr (Vector)                                                                                                                                    | PerformanceCalculationPerformanceCalculationMethod   |
+| Machine Learning (ml)    | Concatenation             | ConcatenationMethod          | \-                                                                                            | DataInConcatenation (list of Vector)                                                                                                                             | DataOutConcatenatedData (Matrix)                                                                                                                                                           | ConcatenationConcatenationMethod                     |
+| Machine Learning (ml)    | DataSplitting             | DataSplittingMethod          | \-                                                                                            | DataInDataSplittingX (Matrix or Vector)<br>DataInDataSplittingY (Matrix or Vector)                                                                               | DataOutSplittedTestDataX (Matrix or Vector)<br>DataOutSplittedTrainDataY (Matrix or Vector)<br>DataOutSplittedTrainDataX (Matrix or Vector)<br>DataOutSplittedTestDataY (Matrix or Vector) | DataSplittingDataSplittingMethod                     |
+| Visualization (visu)     | CanvasTask                | CanvasMethod                 | hasCanvasName (string)<br>hasLayout (string)                                                  | \-                                                                                                                                                               | \-                                                                                                                                                                                         | CanvasTaskCanvasMethod                               |
+| Visualization (visu)     | PlotTask                  | LineplotMethod               | hasLineStyle (string)<br>hasLineWidth (int)<br>hasLegendName (string)                         | DataInVector (Vector)                                                                                                                                            | \-                                                                                                                                                                                         | PlotTaskLineplotMethod                               |
+| Visualization (visu)     | PlotTask                  | ScatterplotMethod            | hasLineStyle (string)<br>hasLineWidth (int)<br>hasScatterSize (int)<br>hasLegendName (string) | DataInVector (Vector)                                                                                                                                            | \-                                                                                                                                                                                         | PlotTaskScatterplotMethod                            |
+| Statistics (stats)       | TrendCalculationTask      | TrendCalculationMethod       | \-                                                                                            | DataInTrendCalculation (Vector)                                                                                                                                  | DataOutTrendCalculation (Vector)                                                                                                                                                           | TrendCalculationTaskTrendCalculationMethod           |
+| Statistics (stats)       | NormalizationTask         | NormalizationMethod          | \-                                                                                            | DataInNormalization (Vector)                                                                                                                                     | DataOutNormalization (Vector)                                                                                                                                                              | NormalizationTaskNormalizationMethod                 |
+| Statistics (stats)       | ScatteringCalculationTask | ScatteringCalculationMethod  | \-                                                                                            | DataInScatteringCalculation (Vector)                                                                                                                             | DataOutScatteringCalculation (Vector)                                                                                                                                                      | ScatteringCalculationTaskScatteringCalculationMethod |
+
+[//]: # (--8<-- [end:supportedmethods])
+
+</details>
+
+## Usage
+
+[//]: # (--8<-- [start:usage])
+### Creating an ML pipeline
+
+- **Via code**: See the [provided examples](https://github.com/boschresearch/ExeKGLib/tree/main/examples). To fetch them to your working directory for easy access, run `typer exe_kg_lib.cli.main run get-examples`.
+- **Step-by-step via CLI**: Run `typer exe_kg_lib.cli.main run create-pipeline`.
+
+### Executing an ML pipeline
+Run `typer exe_kg_lib.cli.main run run-pipeline <pipeline_path>`.
+
+[//]: # (--8<-- [end:usage])
+
+## Adding a new ML-related task and method
+
+[//]: # (--8<-- [start:extending])
+To perform this type of **ExeKGLib** extension, there are 3 required steps:
+
+1. Selection of a relevant bottom-level KG schema (Statistics, ML, or Visualization) according to the type of the new task and method.
+2. Addition of new semantic components (entities, properties, etc) to the selected KG schema.
+3. Addition of a Python class to the corresponding module of `exe_kg_lib.classes.tasks` package.
+
+For steps 2 and 3, refer to the [relevant page](https://boschresearch.github.io/ExeKGLib/adding-new-task-and-method/) of **ExeKGLib**'s website.
+
+[//]: # (--8<-- [end:extending])
+
+## Documentation
+See the _Code Reference_ and _Development_ sections of the [**ExeKGLib**'s website](https://boschresearch.github.io/ExeKGLib/).
+
+## External resources
+
+[//]: # (--8<-- [start:externalresources])
+### KG schemata
+
+- **Top-level**: [Data Science](https://w3id.org/def/exekg-ds)
+- **Bottom-level**: [Visualization](https://w3id.org/def/exekg-visu) | [Statistics](https://w3id.org/def/exekg-stats) | [Machine Learning](https://w3id.org/def/exekg-ml)
+
+The above KG schemata are included in the [ExeKGOntology repository](https://github.com/nsai-uio/ExeKGOntology).
+
+### Dataset used in code examples
+[The dataset](https://github.com/boschresearch/ExeKGLib/tree/main/examples/data/dummy_data.csv) was generated using the `sklearn.datasets.make_classification()` function of the [scikit-learn Python library](https://scikit-learn.org/).
+
+[//]: # (--8<-- [end:externalresources])
+
+## License
+
+ExeKGLib is open-sourced under the AGPL-3.0 license. See the
+[LICENSE](LICENSE.md) file for details.
+
+<!-- URLs -->
+[black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
+[black]: https://github.com/psf/black
+[ci-badge]: https://github.com/boschresearch/ExeKGLib/actions/workflows/ci.yaml/badge.svg
+[ci]: https://github.com/boschresearch/ExeKGLib/actions/workflows/ci.yaml
+[docs-badge]: https://img.shields.io/badge/docs-gh--pages-inactive
+[docs]: https://github.com/boschresearch/ExeKGLib/tree/gh-pages
+[license-badge]: https://img.shields.io/badge/License-All%20rights%20reserved-informational
+[license-url]: https://pages.github.boschdevcloud.com/bcai-internal//latest/license
+[pre-commit-badge]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
+[pre-commit]: https://github.com/pre-commit/pre-commit
```

### Comparing `exe_kg_lib-2.0.2/PKG-INFO` & `exe_kg_lib-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exe-kg-lib
-Version: 2.0.2
+Version: 2.0.3
 Summary: Library for executable ML pipelines represented by KGs.
 Home-page: https://boschresearch.github.io/ExeKGLib
 License: AGPL-3.0
 Author: Antonis Klironomos
 Author-email: antonis.klironomos@de.bosch.com
 Maintainer: Antonis Klironomos
 Maintainer-email: antonis.klironomos@de.bosch.com
@@ -76,29 +76,29 @@
 
 <details>
   <summary>Click to expand</summary>
 
 <!-- --8<-- [start:supportedmethods] -->
 | KG schema (abbreviation) | Task                      | Method                       | Properties                                                                                    | Input (data structure)                                                                                                                                           | Output (data structure)                                                                                                                                                                    | Implemented by Python class                          |
 | ------------------------ | ------------------------- | ---------------------------- | --------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------- |
-| Machine Learning (ML)    | Train                     | KNNTrain                     | \-                                                                                            | DataInTrainX (Matrix or Vector)<br>DataInTrainY (Matrix or Vector)                                                                                               | DataOutPredictedValueTrain (Matrix or Vector)<br>DataOutTrainModel (SingleValue)                                                                                                           | TrainKNNTrain                                        |
-| Machine Learning (ML)    | Train                     | MLPTrain                     | \-                                                                                            | DataInTrainX (Matrix or Vector)<br>DataInTrainY (Matrix or Vector)                                                                                               | DataOutPredictedValueTrain (Matrix or Vector)<br>DataOutTrainModel (SingleValue)                                                                                                           | TrainMLPTrain                                        |
-| Machine Learning (ML)    | Train                     | LRTrain                      | \-                                                                                            | DataInTrainX (Matrix or Vector)<br>DataInTrainY (Matrix or Vector)                                                                                               | DataOutPredictedValueTrain (Matrix or Vector)<br>DataOutTrainModel (SingleValue)                                                                                                           | TrainLRTrain                                         |
-| Machine Learning (ML)    | Test                      | KNNTest                      | \-                                                                                            | DataInTestModel (SingleValue)<br>DataInTestX (Matrix or Vector)                                                                                                  | DataOutPredictedValueTest (Matrix or Vector)                                                                                                                                               | TestKNNTest                                          |
-| Machine Learning (ML)    | Test                      | MLPTest                      | \-                                                                                            | DataInTestModel (SingleValue)<br>DataInTestX (Matrix or Vector)                                                                                                  | DataOutPredictedValueTest (Matrix or Vector)                                                                                                                                               | TestMLPTest                                          |
-| Machine Learning (ML)    | Test                      | LRTest                       | \-                                                                                            | DataInTestModel (SingleValue)<br>DataInTestX (Matrix or Vector)                                                                                                  | DataOutPredictedValueTest (Matrix or Vector)                                                                                                                                               | TestLRTest                                           |
-| Machine Learning (ML)    | PerformanceCalculation    | PerformanceCalculationMethod | \-                                                                                            | DataInTrainRealY (Matrix or Vector)<br>DataInTrainPredictedY (Matrix or Vector)<br>DataInTestPredictedY (Matrix or Vector)<br>DataInTestRealY (Matrix or Vector) | DataOutMLTestErr (Vector)<br>DataOutMLTrainErr (Vector)                                                                                                                                    | PerformanceCalculationPerformanceCalculationMethod   |
-| Machine Learning (ML)    | Concatenation             | ConcatenationMethod          | \-                                                                                            | DataInConcatenation (list of Vector)                                                                                                                             | DataOutConcatenatedData (Matrix)                                                                                                                                                           | ConcatenationConcatenationMethod                     |
-| Machine Learning (ML)    | DataSplitting             | DataSplittingMethod          | \-                                                                                            | DataInDataSplittingX (Matrix or Vector)<br>DataInDataSplittingY (Matrix or Vector)                                                                               | DataOutSplittedTestDataX (Matrix or Vector)<br>DataOutSplittedTrainDataY (Matrix or Vector)<br>DataOutSplittedTrainDataX (Matrix or Vector)<br>DataOutSplittedTestDataY (Matrix or Vector) | DataSplittingDataSplittingMethod                     |
-| Visualization (Visu)     | CanvasTask                | CanvasMethod                 | hasCanvasName (string)<br>hasLayout (string)                                                  | \-                                                                                                                                                               | \-                                                                                                                                                                                         | CanvasTaskCanvasMethod                               |
-| Visualization (Visu)     | PlotTask                  | LineplotMethod               | hasLineStyle (string)<br>hasLineWidth (int)<br>hasLegendName (string)                         | DataInVector (Vector)                                                                                                                                            | \-                                                                                                                                                                                         | PlotTaskLineplotMethod                               |
-| Visualization (Visu)     | PlotTask                  | ScatterplotMethod            | hasLineStyle (string)<br>hasLineWidth (int)<br>hasScatterSize (int)<br>hasLegendName (string) | DataInVector (Vector)                                                                                                                                            | \-                                                                                                                                                                                         | PlotTaskScatterplotMethod                            |
-| Statistics (Stats)       | TrendCalculationTask      | TrendCalculationMethod       | \-                                                                                            | DataInTrendCalculation (Vector)                                                                                                                                  | DataOutTrendCalculation (Vector)                                                                                                                                                           | TrendCalculationTaskTrendCalculationMethod           |
-| Statistics (Stats)       | NormalizationTask         | NormalizationMethod          | \-                                                                                            | DataInNormalization (Vector)                                                                                                                                     | DataOutNormalization (Vector)                                                                                                                                                              | NormalizationTaskNormalizationMethod                 |
-| Statistics (Stats)       | ScatteringCalculationTask | ScatteringCalculationMethod  | \-                                                                                            | DataInScatteringCalculation (Vector)                                                                                                                             | DataOutScatteringCalculation (Vector)                                                                                                                                                      | ScatteringCalculationTaskScatteringCalculationMethod |
+| Machine Learning (ml)    | Train                     | KNNTrain                     | \-                                                                                            | DataInTrainX (Matrix or Vector)<br>DataInTrainY (Matrix or Vector)                                                                                               | DataOutPredictedValueTrain (Matrix or Vector)<br>DataOutTrainModel (SingleValue)                                                                                                           | TrainKNNTrain                                        |
+| Machine Learning (ml)    | Train                     | MLPTrain                     | \-                                                                                            | DataInTrainX (Matrix or Vector)<br>DataInTrainY (Matrix or Vector)                                                                                               | DataOutPredictedValueTrain (Matrix or Vector)<br>DataOutTrainModel (SingleValue)                                                                                                           | TrainMLPTrain                                        |
+| Machine Learning (ml)    | Train                     | LRTrain                      | \-                                                                                            | DataInTrainX (Matrix or Vector)<br>DataInTrainY (Matrix or Vector)                                                                                               | DataOutPredictedValueTrain (Matrix or Vector)<br>DataOutTrainModel (SingleValue)                                                                                                           | TrainLRTrain                                         |
+| Machine Learning (ml)    | Test                      | KNNTest                      | \-                                                                                            | DataInTestModel (SingleValue)<br>DataInTestX (Matrix or Vector)                                                                                                  | DataOutPredictedValueTest (Matrix or Vector)                                                                                                                                               | TestKNNTest                                          |
+| Machine Learning (ml)    | Test                      | MLPTest                      | \-                                                                                            | DataInTestModel (SingleValue)<br>DataInTestX (Matrix or Vector)                                                                                                  | DataOutPredictedValueTest (Matrix or Vector)                                                                                                                                               | TestMLPTest                                          |
+| Machine Learning (ml)    | Test                      | LRTest                       | \-                                                                                            | DataInTestModel (SingleValue)<br>DataInTestX (Matrix or Vector)                                                                                                  | DataOutPredictedValueTest (Matrix or Vector)                                                                                                                                               | TestLRTest                                           |
+| Machine Learning (ml)    | PerformanceCalculation    | PerformanceCalculationMethod | \-                                                                                            | DataInTrainRealY (Matrix or Vector)<br>DataInTrainPredictedY (Matrix or Vector)<br>DataInTestPredictedY (Matrix or Vector)<br>DataInTestRealY (Matrix or Vector) | DataOutMLTestErr (Vector)<br>DataOutMLTrainErr (Vector)                                                                                                                                    | PerformanceCalculationPerformanceCalculationMethod   |
+| Machine Learning (ml)    | Concatenation             | ConcatenationMethod          | \-                                                                                            | DataInConcatenation (list of Vector)                                                                                                                             | DataOutConcatenatedData (Matrix)                                                                                                                                                           | ConcatenationConcatenationMethod                     |
+| Machine Learning (ml)    | DataSplitting             | DataSplittingMethod          | \-                                                                                            | DataInDataSplittingX (Matrix or Vector)<br>DataInDataSplittingY (Matrix or Vector)                                                                               | DataOutSplittedTestDataX (Matrix or Vector)<br>DataOutSplittedTrainDataY (Matrix or Vector)<br>DataOutSplittedTrainDataX (Matrix or Vector)<br>DataOutSplittedTestDataY (Matrix or Vector) | DataSplittingDataSplittingMethod                     |
+| Visualization (visu)     | CanvasTask                | CanvasMethod                 | hasCanvasName (string)<br>hasLayout (string)                                                  | \-                                                                                                                                                               | \-                                                                                                                                                                                         | CanvasTaskCanvasMethod                               |
+| Visualization (visu)     | PlotTask                  | LineplotMethod               | hasLineStyle (string)<br>hasLineWidth (int)<br>hasLegendName (string)                         | DataInVector (Vector)                                                                                                                                            | \-                                                                                                                                                                                         | PlotTaskLineplotMethod                               |
+| Visualization (visu)     | PlotTask                  | ScatterplotMethod            | hasLineStyle (string)<br>hasLineWidth (int)<br>hasScatterSize (int)<br>hasLegendName (string) | DataInVector (Vector)                                                                                                                                            | \-                                                                                                                                                                                         | PlotTaskScatterplotMethod                            |
+| Statistics (stats)       | TrendCalculationTask      | TrendCalculationMethod       | \-                                                                                            | DataInTrendCalculation (Vector)                                                                                                                                  | DataOutTrendCalculation (Vector)                                                                                                                                                           | TrendCalculationTaskTrendCalculationMethod           |
+| Statistics (stats)       | NormalizationTask         | NormalizationMethod          | \-                                                                                            | DataInNormalization (Vector)                                                                                                                                     | DataOutNormalization (Vector)                                                                                                                                                              | NormalizationTaskNormalizationMethod                 |
+| Statistics (stats)       | ScatteringCalculationTask | ScatteringCalculationMethod  | \-                                                                                            | DataInScatteringCalculation (Vector)                                                                                                                             | DataOutScatteringCalculation (Vector)                                                                                                                                                      | ScatteringCalculationTaskScatteringCalculationMethod |
 
 [//]: # (--8<-- [end:supportedmethods])
 
 </details>
 
 ## Usage
```

