# Comparing `tmp/exe_kg_lib-1.1.2.tar.gz` & `tmp/exe_kg_lib-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exe_kg_lib-1.1.2.tar", max compression
+gzip compressed data, was "exe_kg_lib-1.1.3.tar", max compression
```

## Comparing `exe_kg_lib-1.1.2.tar` & `exe_kg_lib-1.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    34283 2023-03-20 09:32:20.710882 exe_kg_lib-1.1.2/LICENSE.md
--rw-r--r--   0        0        0     6635 2023-03-20 09:32:20.710882 exe_kg_lib-1.1.2/README.md
--rw-r--r--   0        0        0       27 2023-03-20 09:32:20.710882 exe_kg_lib-1.1.2/exe_kg_lib/__init__.py
--rw-r--r--   0        0        0      102 2023-03-20 09:32:20.714882 exe_kg_lib-1.1.2/exe_kg_lib/classes/__init__.py
--rw-r--r--   0        0        0     1253 2023-03-20 09:32:20.714882 exe_kg_lib-1.1.2/exe_kg_lib/classes/data_entity.py
--rw-r--r--   0        0        0      782 2023-03-20 09:32:20.714882 exe_kg_lib-1.1.2/exe_kg_lib/classes/entity.py
--rw-r--r--   0        0        0    33396 2023-03-20 09:32:20.714882 exe_kg_lib-1.1.2/exe_kg_lib/classes/exe_kg.py
--rw-r--r--   0        0        0      773 2023-03-20 09:32:20.714882 exe_kg_lib-1.1.2/exe_kg_lib/classes/kg_schema.py
--rw-r--r--   0        0        0     3528 2023-03-20 09:32:20.714882 exe_kg_lib-1.1.2/exe_kg_lib/classes/task.py
--rw-r--r--   0        0        0     1914 2023-03-20 09:32:20.714882 exe_kg_lib-1.1.2/exe_kg_lib/classes/tasks/README.md
--rw-r--r--   0        0        0        0 2023-03-20 09:32:20.714882 exe_kg_lib-1.1.2/exe_kg_lib/classes/tasks/__init__.py
--rw-r--r--   0        0        0     5619 2023-03-20 09:32:20.714882 exe_kg_lib-1.1.2/exe_kg_lib/classes/tasks/ml_tasks.py
--rw-r--r--   0        0        0     1967 2023-03-20 09:32:20.714882 exe_kg_lib-1.1.2/exe_kg_lib/classes/tasks/statistic_tasks.py
--rw-r--r--   0        0        0     3108 2023-03-20 09:32:20.714882 exe_kg_lib-1.1.2/exe_kg_lib/classes/tasks/visual_tasks.py
--rw-r--r--   0        0        0        0 2023-03-20 09:32:20.714882 exe_kg_lib-1.1.2/exe_kg_lib/cli/__init__.py
--rw-r--r--   0        0        0     1017 2023-03-20 09:32:20.714882 exe_kg_lib-1.1.2/exe_kg_lib/cli/main.py
--rw-r--r--   0        0        0      108 2023-03-20 09:32:20.714882 exe_kg_lib-1.1.2/exe_kg_lib/utils/__init__.py
--rw-r--r--   0        0        0     3130 2023-03-20 09:32:20.714882 exe_kg_lib-1.1.2/exe_kg_lib/utils/cli_utils.py
--rw-r--r--   0        0        0     7418 2023-03-20 09:32:20.714882 exe_kg_lib-1.1.2/exe_kg_lib/utils/kg_creation_utils.py
--rw-r--r--   0        0        0     6250 2023-03-20 09:32:20.714882 exe_kg_lib-1.1.2/exe_kg_lib/utils/query_utils.py
--rw-r--r--   0        0        0      679 2023-03-20 09:32:20.714882 exe_kg_lib-1.1.2/exe_kg_lib/utils/string_utils.py
--rw-r--r--   0        0        0        0 2023-03-20 09:32:20.714882 exe_kg_lib-1.1.2/exe_kg_lib/utils/task_utils/__init__.py
--rw-r--r--   0        0        0     2660 2023-03-20 09:32:20.714882 exe_kg_lib-1.1.2/exe_kg_lib/utils/task_utils/ml_utils.py
--rw-r--r--   0        0        0     2606 2023-03-20 09:32:20.714882 exe_kg_lib-1.1.2/exe_kg_lib/utils/task_utils/statistic_utils.py
--rw-r--r--   0        0        0     2388 2023-03-20 09:32:20.714882 exe_kg_lib-1.1.2/exe_kg_lib/utils/task_utils/visual_utils.py
--rw-r--r--   0        0        0     3645 2023-03-20 09:32:49.655030 exe_kg_lib-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     8083 1970-01-01 00:00:00.000000 exe_kg_lib-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    34283 2023-04-28 15:41:32.695519 exe_kg_lib-1.1.3/LICENSE.md
+-rw-r--r--   0        0        0    15731 2023-04-28 15:41:32.695519 exe_kg_lib-1.1.3/README.md
+-rw-r--r--   0        0        0       27 2023-04-28 15:41:32.699519 exe_kg_lib-1.1.3/exe_kg_lib/__init__.py
+-rw-r--r--   0        0        0      102 2023-04-28 15:41:32.699519 exe_kg_lib-1.1.3/exe_kg_lib/classes/__init__.py
+-rw-r--r--   0        0        0     1253 2023-04-28 15:41:32.699519 exe_kg_lib-1.1.3/exe_kg_lib/classes/data_entity.py
+-rw-r--r--   0        0        0      788 2023-04-28 15:41:32.699519 exe_kg_lib-1.1.3/exe_kg_lib/classes/entity.py
+-rw-r--r--   0        0        0    31697 2023-04-28 15:41:32.699519 exe_kg_lib-1.1.3/exe_kg_lib/classes/exe_kg.py
+-rw-r--r--   0        0        0      773 2023-04-28 15:41:32.699519 exe_kg_lib-1.1.3/exe_kg_lib/classes/kg_schema.py
+-rw-r--r--   0        0        0     3528 2023-04-28 15:41:32.699519 exe_kg_lib-1.1.3/exe_kg_lib/classes/task.py
+-rw-r--r--   0        0        0     1914 2023-04-28 15:41:32.699519 exe_kg_lib-1.1.3/exe_kg_lib/classes/tasks/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 15:41:32.699519 exe_kg_lib-1.1.3/exe_kg_lib/classes/tasks/__init__.py
+-rw-r--r--   0        0        0     5619 2023-04-28 15:41:32.699519 exe_kg_lib-1.1.3/exe_kg_lib/classes/tasks/ml_tasks.py
+-rw-r--r--   0        0        0     1967 2023-04-28 15:41:32.699519 exe_kg_lib-1.1.3/exe_kg_lib/classes/tasks/statistic_tasks.py
+-rw-r--r--   0        0        0     3108 2023-04-28 15:41:32.699519 exe_kg_lib-1.1.3/exe_kg_lib/classes/tasks/visual_tasks.py
+-rw-r--r--   0        0        0        0 2023-04-28 15:41:32.699519 exe_kg_lib-1.1.3/exe_kg_lib/cli/__init__.py
+-rw-r--r--   0        0        0      938 2023-04-28 15:41:32.699519 exe_kg_lib-1.1.3/exe_kg_lib/cli/main.py
+-rw-r--r--   0        0        0      108 2023-04-28 15:41:32.699519 exe_kg_lib-1.1.3/exe_kg_lib/utils/__init__.py
+-rw-r--r--   0        0        0     3130 2023-04-28 15:41:32.699519 exe_kg_lib-1.1.3/exe_kg_lib/utils/cli_utils.py
+-rw-r--r--   0        0        0     7290 2023-04-28 15:41:32.699519 exe_kg_lib-1.1.3/exe_kg_lib/utils/kg_creation_utils.py
+-rw-r--r--   0        0        0     6250 2023-04-28 15:41:32.699519 exe_kg_lib-1.1.3/exe_kg_lib/utils/query_utils.py
+-rw-r--r--   0        0        0      679 2023-04-28 15:41:32.699519 exe_kg_lib-1.1.3/exe_kg_lib/utils/string_utils.py
+-rw-r--r--   0        0        0        0 2023-04-28 15:41:32.699519 exe_kg_lib-1.1.3/exe_kg_lib/utils/task_utils/__init__.py
+-rw-r--r--   0        0        0     2660 2023-04-28 15:41:32.699519 exe_kg_lib-1.1.3/exe_kg_lib/utils/task_utils/ml_utils.py
+-rw-r--r--   0        0        0     2606 2023-04-28 15:41:32.699519 exe_kg_lib-1.1.3/exe_kg_lib/utils/task_utils/statistic_utils.py
+-rw-r--r--   0        0        0     2388 2023-04-28 15:41:32.699519 exe_kg_lib-1.1.3/exe_kg_lib/utils/task_utils/visual_utils.py
+-rw-r--r--   0        0        0     3645 2023-04-28 15:41:53.979811 exe_kg_lib-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0    17179 1970-01-01 00:00:00.000000 exe_kg_lib-1.1.3/PKG-INFO
```

### Comparing `exe_kg_lib-1.1.2/LICENSE.md` & `exe_kg_lib-1.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-1.1.2/exe_kg_lib/classes/data_entity.py` & `exe_kg_lib-1.1.3/exe_kg_lib/classes/data_entity.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-1.1.2/exe_kg_lib/classes/entity.py` & `exe_kg_lib-1.1.3/exe_kg_lib/classes/entity.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,12 +17,12 @@
         self.namespace = self.get_namespace(iri)
         self.name = self.type = self.get_descriptor(iri)
         if parent_entity:
             self.type = parent_entity.name
 
     @staticmethod
     def get_namespace(iri: str) -> str:
-        return iri.split("#")[0]
+        return iri.split("#")[0] + "#"
 
     @staticmethod
     def get_descriptor(iri: str) -> str:
         return iri.split("#")[1]
```

### Comparing `exe_kg_lib-1.1.2/exe_kg_lib/classes/exe_kg.py` & `exe_kg_lib-1.1.3/exe_kg_lib/classes/exe_kg.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,24 +46,23 @@
         "namespace": "https://raw.githubusercontent.com/nsai-uio/ExeKGOntology/main/ml_exeKGOntology.ttl#",
         "namespace_prefix": "ml",
     },
 }
 
 
 class ExeKG:
-    def __init__(self, kg_schema_name: str = None, input_exe_kg_path: str = None):
+    def __init__(self, input_exe_kg_path: str = None):
         """
 
         Args:
-            kg_schema_name: name of chosen bottom-level KG schema to use in case of KG construction (must be equal to one of KG_SCHEMAS keys)
-                            acts as switch for KG construction mode (if filled, mode is on)
             input_exe_kg_path: path of KG to be executed
                                acts as switch for KG execution mode (if filled, mode is on)
         """
         self.top_level_schema = KGSchema.from_schema_info(KG_SCHEMAS["Data Science"])  # top-level KG schema
+        self.bottom_level_schemata = {}
 
         # top-level KG schema entities
         self.atomic_task = Entity(self.top_level_schema.namespace.AtomicTask)
         self.atomic_method = Entity(self.top_level_schema.namespace.AtomicMethod)
         self.data_entity = Entity(self.top_level_schema.namespace.DataEntity)
         self.pipeline = Entity(self.top_level_schema.namespace.Pipeline)
         self.data = Entity(self.top_level_schema.namespace.Data)
@@ -74,46 +73,41 @@
         self.input_kg = Graph(bind_namespaces="rdflib")
         if input_exe_kg_path:  # KG execution mode
             self.input_kg.parse(input_exe_kg_path, format="n3")  # parse input executable KG
             all_ns = [n for n in self.input_kg.namespace_manager.namespaces()]
             bottom_level_schema_info_set = False  # flag indicating that a bottom-level schema was found
             for schema_name, schema_info in KG_SCHEMAS.items():  # search for used bottom-level schema
                 if (
-                    schema_name == "Data Science" or schema_name == "Visualization"
+                    schema_name == "Data Science"  # or schema_name == "Visualization"
                 ):  # skip top-level KG schema and Visualization schema that is always used
                     continue
 
                 if (schema_info["namespace_prefix"], URIRef(schema_info["namespace"])) in all_ns:
                     # bottom-level schema found
-                    self.bottom_level_schema = KGSchema.from_schema_info(schema_info)
+                    self.bottom_level_schemata[schema_info["namespace_prefix"]] = KGSchema.from_schema_info(schema_info)
                     bottom_level_schema_info_set = True
-                    break
-
-            visu_schema_info = KG_SCHEMAS["Visualization"]
-            if (
-                not bottom_level_schema_info_set
-                and (visu_schema_info["namespace_prefix"], URIRef(visu_schema_info["namespace"])) in all_ns
-            ):  # Visualization schema is considered the bottom-level schema ONLY IF no other bottom-level schema was found
-                self.bottom_level_schema = KGSchema.from_schema_info(visu_schema_info)
-                bottom_level_schema_info_set = True
 
             if not bottom_level_schema_info_set:  # no bottom-level schema found, input executable KG is invalid
                 print("Input executable KG did not have any bottom level KG schemas")
                 exit(1)
         else:  # KG construction mode
-            # bottom-level schema used as compatibility guide for constructing executable KG
-            self.bottom_level_schema = KGSchema.from_schema_info(KG_SCHEMAS[kg_schema_name])
+            for schema_name, schema_info in KG_SCHEMAS.items():  # search for used bottom-level schema
+                if (
+                    schema_name == "Data Science"  # or schema_name == "Visualization"
+                ):  # skip top-level KG schema and Visualization schema that is always used
+                    continue
 
-        self.visu_schema = KGSchema.from_schema_info(
-            KG_SCHEMAS["Visualization"]
-        )  # Visualization KG schema, always used
-
-        self.input_kg += (
-            self.top_level_schema.kg + self.bottom_level_schema.kg + self.visu_schema.kg
-        )  # combine all KG schemas in input KG
+                self.bottom_level_schemata[schema_info["namespace_prefix"]] = KGSchema.from_schema_info(schema_info)
+
+        bottom_level_schemata_kgs = [kg_schema.kg for kg_schema in self.bottom_level_schemata.values()]
+
+        self.input_kg += self.top_level_schema.kg  # + self.visu_schema.kg  # combine all KG schemas in input KG
+
+        for bottom_level_schema_kg in bottom_level_schemata_kgs:
+            self.input_kg += bottom_level_schema_kg
 
         self.output_kg = Graph(bind_namespaces="rdflib")  # KG to be filled while constructing executable KG
 
         self._bind_used_namespaces([self.input_kg, self.output_kg])
 
         # below variables are filled in self._parse_kgs()
         self.task_type_dict = {}  # dict for uniquely naming each new pipeline task
@@ -139,22 +133,19 @@
         Binds top-level, bottom-level and Visualization KG schemas' namespaces with their prefixes
         Adds these bindings to the Graphs of kgs list
         Args:
             kgs: list of Graph objects to which the namespace bindings are added
         """
         for kg in kgs:
             kg.bind(self.top_level_schema.namespace_prefix, self.top_level_schema.namespace)
-            kg.bind(
-                self.bottom_level_schema.namespace_prefix,
-                self.bottom_level_schema.namespace,
-            )
-            kg.bind(
-                self.visu_schema.namespace_prefix,
-                self.visu_schema.namespace,
-            )
+            for bottom_level_kg_schema in self.bottom_level_schemata.values():
+                kg.bind(
+                    bottom_level_kg_schema.namespace_prefix,
+                    bottom_level_kg_schema.namespace,
+                )
 
     def _parse_kgs(self) -> None:
         """
         Fills lists with subclasses of top-level KG schema classes and initializes dicts used for unique naming
         """
         atomic_task_subclasses = get_subclasses_of(self.atomic_task.iri, self.input_kg)
         for t in list(atomic_task_subclasses):
@@ -195,15 +186,14 @@
             input_data_path: path for the input data to be used by the pipeline's tasks
 
         Returns:
             Task: created pipeline
         """
         pipeline = create_pipeline_task(
             self.top_level_schema.namespace,
-            self.bottom_level_schema.namespace,
             self.pipeline,
             self.output_kg,
             pipeline_name,
             input_data_path,
         )
         self.last_created_task = pipeline
         return pipeline
@@ -223,93 +213,90 @@
             data_semantics_name: name of the data semantics entity
             data_structure_name: name of the data structure entity
 
         Returns:
             DataEntity: object initialized with the given parameter values
         """
         return DataEntity(
-            self.bottom_level_schema.namespace + name,
+            self.top_level_schema.namespace + name,
             self.data_entity,
             source_value,
             self.top_level_schema.namespace + data_semantics_name,
             self.top_level_schema.namespace + data_structure_name,
         )
 
     def add_task(
         self,
-        task_type: str,
+        kg_schema_short: str,
+        task: str,
         input_data_entity_dict: Dict[str, List[DataEntity]],
-        method_type: str,
-        data_properties: Dict[str, Union[str, int, float]],
-        visualization: bool = False,
+        method: str,
+        properties_dict: Dict[str, Union[str, int, float]],
     ) -> Task:
         """
         Instantiates and adds a new task entity to self.output_kg
-        Components added to the task during creation: input and output entities, and a method with data properties
+        Components attached to the task during creation: input and output data entities, and a method with properties
         Args:
-            task_type: type of the task
-            input_data_entity_dict: keys -> input entity names corresponding to the given task_type as defined in the chosen bottom-level KG schema
-                                    values -> list of corresponding data entities to be added as input to the task
-            method_type: type of the task's method
-            data_properties: keys -> data property names corresponding to the given method_type as defined in the chosen bottom-level KG schema
-                             values -> list of corresponding values to be added as property values to the task
-            visualization: if True, the namespace prefix of Visualization KG schema is used during creation of the task
-                           else, the namespace prefix of the chosen bottom-level KG schema is used
+            kg_schema_short: abbreviated name of the KG schema in which the task and method belong
+            task: task name
+            input_data_entity_dict: keys -> input names of the specified task
+                                    values -> lists of DataEntity objects to be added as input to the task
+            method: method name
+            properties_dict: keys -> property names of the specified method
+                             values -> values to be added as parameters to the method
 
         Returns:
             Task: object of the created task
         """
-        namespace_to_use = (
-            self.visu_schema.namespace if visualization else self.bottom_level_schema.namespace
-        )  # use appropriate namespace for the task
+        kg_schema_to_use = self.bottom_level_schemata[kg_schema_short]
 
         relation_iri = (
             self.top_level_schema.namespace.hasNextTask
             if self.last_created_task.type != "Pipeline"
             else self.top_level_schema.namespace.hasStartTask
         )  # use relation depending on the previous task
 
         # instantiate task and link it with the previous one
-        parent_task = Task(namespace_to_use + task_type, self.atomic_task)
+        parent_task = Task(kg_schema_to_use.namespace + task, self.atomic_task)
         added_entity = add_instance_from_parent_with_relation(
-            self.bottom_level_schema.namespace,
+            kg_schema_to_use.namespace,
             self.output_kg,
             parent_task,
             relation_iri,
             self.last_created_task,
             name_instance(self.task_type_dict, self.method_type_dict, parent_task),
         )
         next_task = Task.from_entity(added_entity)  # create Task object from Entity object
 
         # instantiate and add given input data entities to the task
-        self._add_inputs_to_task(next_task, input_data_entity_dict)
+        self._add_inputs_to_task(kg_schema_to_use.namespace, next_task, input_data_entity_dict)
         # instantiate and add output data entities to the task, as specified in the KG schema
         self._add_outputs_to_task(next_task)
 
-        method_parent = Entity(namespace_to_use + method_type, self.atomic_method)
+        method_parent = Entity(kg_schema_to_use.namespace + method, self.atomic_method)
 
         # fetch compatible methods and their properties from KG schema
         results = list(
             get_method_properties_and_methods(
                 self.input_kg,
                 self.top_level_schema.namespace_prefix,
                 next_task.parent_entity.iri,
             )
         )
 
         chosen_property_method = next(
-            filter(lambda pair: pair[1].split("#")[1] == method_type, results), None
+            filter(lambda pair: pair[1].split("#")[1] == method, results), None
         )  # match given method_type with query result
         if chosen_property_method is None:
-            print(f"Property connecting task of type {task_type} with method of type {method_type} not found")
+            print(f"Property connecting task of type {task} with method of type {method} not found")
             exit(1)
 
         # instantiate method and link it with the task using the appropriate chosen_property_method[0] relation
         add_instance_from_parent_with_relation(
-            self.bottom_level_schema.namespace,
+            kg_schema_to_use.namespace,
             self.output_kg,
             method_parent,
             chosen_property_method[0],
             next_task,
             name_instance(self.task_type_dict, self.method_type_dict, method_parent),
         )
 
@@ -318,25 +305,28 @@
 
         # add data properties to the task with given values
         for pair in property_list:
             property_iri = pair[0]
             property_name = property_iri.split("#")[1]
             range_iri = pair[1]
             input_property = Literal(
-                lexical_or_value=data_properties[property_name],
+                lexical_or_value=properties_dict[property_name],
                 datatype=range_iri,
             )
             add_literal(self.output_kg, next_task, property_iri, input_property)
 
         self.last_created_task = next_task  # store created task
 
         return next_task
 
     def _add_inputs_to_task(
-        self, task_entity: Task, input_data_entity_dict: Dict[str, List[DataEntity]] = None
+        self,
+        namespace: Namespace,
+        task_entity: Task,
+        input_data_entity_dict: Dict[str, List[DataEntity]] = None,
     ) -> None:
         """
         Instantiates and adds given input data entities to the given task of self.output_kg
         if input_data_entity_dict is None, user is asked to specify input data entities
         Args:
             task_entity: the task to add the input to
             input_data_entity_dict: keys -> input entity names corresponding to the given task as defined in the chosen bottom-level KG schema
@@ -361,15 +351,15 @@
             else:
                 # use CLI
                 print(f"Specify input corresponding to {input_entity_name}")
                 input_data_entity_list = get_input_for_existing_data_entities(self.existing_data_entity_list)
                 input_data_entity_list += get_input_for_new_data_entities(
                     self.data_semantics_list,
                     self.data_structure_list,
-                    self.bottom_level_schema.namespace,
+                    namespace,
                     self.data_entity,
                 )
 
             same_input_index = 1
             for input_data_entity in input_data_entity_list:
                 # instantiate data entity corresponding to the found input_entity_name
                 data_entity_iri = input_entity_iri + str(task_type_index) + "_" + str(same_input_index)
@@ -458,26 +448,26 @@
             self.top_level_schema.namespace.hasNextTask
             if self.last_created_task.type != "Pipeline"
             else self.top_level_schema.namespace.hasStartTask
         )  # use relation depending on the previous task
 
         # instantiate task and link it with the previous one
         task_entity = add_instance_from_parent_with_relation(
-            self.bottom_level_schema.namespace,
+            next_task_parent.namespace,
             self.output_kg,
             next_task_parent,
             relation_iri,
             self.last_created_task,
             name_instance(self.task_type_dict, self.method_type_dict, next_task_parent),
         )
 
         task_entity = Task(task_entity.iri, task_entity.parent_entity)  # create Task object from Entity object's info
 
         # instantiate and add input data entities to the task based on user input
-        self._add_inputs_to_task(task_entity)
+        self._add_inputs_to_task(next_task_parent.namespace, task_entity)
         # instantiate and add output data entities to the task, as specified in the KG schema
         self._add_outputs_to_task(task_entity)
 
         self.last_created_task = task_entity
         if task_entity.type == "CanvasTask":
             self.canvas_task_created = True
 
@@ -510,15 +500,15 @@
                 lambda m: m.iri == selected_property_and_method[1],
                 self.atomic_method_list,
             ),
             None,
         )
         # instantiate method and link it with the task using the appropriate selected_property_and_method[0] relation
         add_instance_from_parent_with_relation(
-            self.bottom_level_schema.namespace,
+            task_to_attach_to.namespace,
             self.output_kg,
             method_parent,
             selected_property_and_method[0],
             task_to_attach_to,
             name_instance(self.task_type_dict, self.method_type_dict, method_parent),
         )
 
@@ -543,15 +533,14 @@
         Handles the pipeline creation through CLI
         Args:
             pipeline_name: name for the pipeline
             input_data_path: path for the input data to be used by the pipeline's tasks
         """
         pipeline = create_pipeline_task(
             self.top_level_schema.namespace,
-            self.bottom_level_schema.namespace,
             self.pipeline,
             self.output_kg,
             pipeline_name,
             input_data_path,
         )
 
         self.last_created_task = pipeline
@@ -726,27 +715,7 @@
             if output:
                 task_output_dict.update(output)
 
             if next_task.type == "CanvasTask":
                 canvas_method = next_task
 
             next_task_iri = next_task.has_next_task
-
-    @staticmethod
-    def input_kg_schema_name() -> str:
-        """
-        Prompts the user to choose a schema by presenting the available schemas' names
-        Returns:
-            str: chosen schema name
-        """
-        kg_schema_names = list(KG_SCHEMAS.keys())
-        print(
-            "Choose a KG schema to use. Components of the Visualization schema can be used regardless of the chosen schema."
-        )
-        for i, kg_schema_name in enumerate(kg_schema_names):
-            if kg_schema_name == "Data Science":
-                continue
-            print(f"{i}: {kg_schema_name}")
-        selected_schema_i = int(input())
-        selected_schema_name = kg_schema_names[selected_schema_i]
-
-        return selected_schema_name
```

### Comparing `exe_kg_lib-1.1.2/exe_kg_lib/classes/kg_schema.py` & `exe_kg_lib-1.1.3/exe_kg_lib/classes/kg_schema.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-1.1.2/exe_kg_lib/classes/task.py` & `exe_kg_lib-1.1.3/exe_kg_lib/classes/task.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-1.1.2/exe_kg_lib/classes/tasks/README.md` & `exe_kg_lib-1.1.3/exe_kg_lib/classes/tasks/README.md`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-1.1.2/exe_kg_lib/classes/tasks/ml_tasks.py` & `exe_kg_lib-1.1.3/exe_kg_lib/classes/tasks/ml_tasks.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-1.1.2/exe_kg_lib/classes/tasks/statistic_tasks.py` & `exe_kg_lib-1.1.3/exe_kg_lib/classes/tasks/statistic_tasks.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-1.1.2/exe_kg_lib/classes/tasks/visual_tasks.py` & `exe_kg_lib-1.1.3/exe_kg_lib/classes/tasks/visual_tasks.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-1.1.2/exe_kg_lib/cli/main.py` & `exe_kg_lib-1.1.3/exe_kg_lib/cli/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,17 +13,16 @@
 
 app = typer.Typer(name="ML pipeline creation and execution", no_args_is_help=True)
 
 
 @app.command()
 def create_pipeline():
     pipeline_name, input_data_path = input_pipeline_info()
-    kg_schema_name = ExeKG.input_kg_schema_name()
 
-    exe_kg = ExeKG(kg_schema_name=kg_schema_name)
+    exe_kg = ExeKG()
     exe_kg.start_pipeline_creation(pipeline_name, input_data_path)
     exe_kg.save_created_kg(f"pipelines/{pipeline_name}.ttl")
 
 
 @app.command()
 def run_pipeline(path: str):
     exe_kg = ExeKG(input_exe_kg_path=path)
```

### Comparing `exe_kg_lib-1.1.2/exe_kg_lib/utils/cli_utils.py` & `exe_kg_lib-1.1.3/exe_kg_lib/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-1.1.2/exe_kg_lib/utils/kg_creation_utils.py` & `exe_kg_lib-1.1.3/exe_kg_lib/utils/kg_creation_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -190,33 +190,31 @@
     """
     add_data_entity_instance(kg, data, top_level_kg, top_level_schema_namespace, data_entity)
     add_relation(kg, task_entity, relation, data_entity)
 
 
 def create_pipeline_task(
     top_level_schema_namespace: Namespace,
-    bottom_level_schema_namespace: Namespace,
     parent_entity: Entity,
     kg: Graph,
     pipeline_name: str,
     input_data_path: str,
 ) -> Task:
     """
     Adds instance of pipeline task to kg
     Args:
         top_level_schema_namespace: namespace of the top-level KG schema
-        bottom_level_schema_namespace: namespace of the bottom-level KG schema
         parent_entity: parent entity of pipeline instance
         kg: Graph object to add to
         pipeline_name: name for the pipeline
         input_data_path: path for the input data to be used by the pipeline's tasks
 
     Returns:
         Task: created pipeline task
     """
-    pipeline = Task(bottom_level_schema_namespace + pipeline_name, parent_entity)
+    pipeline = Task(top_level_schema_namespace + pipeline_name, parent_entity)
     add_instance(kg, pipeline)
 
     input_data_path_literal = Literal(lexical_or_value=input_data_path, datatype=XSD.string)
     add_literal(kg, pipeline, top_level_schema_namespace.hasInputDataPath, input_data_path_literal)
 
     return pipeline
```

### Comparing `exe_kg_lib-1.1.2/exe_kg_lib/utils/query_utils.py` & `exe_kg_lib-1.1.3/exe_kg_lib/utils/query_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-1.1.2/exe_kg_lib/utils/string_utils.py` & `exe_kg_lib-1.1.3/exe_kg_lib/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-1.1.2/exe_kg_lib/utils/task_utils/ml_utils.py` & `exe_kg_lib-1.1.3/exe_kg_lib/utils/task_utils/ml_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-1.1.2/exe_kg_lib/utils/task_utils/statistic_utils.py` & `exe_kg_lib-1.1.3/exe_kg_lib/utils/task_utils/statistic_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-1.1.2/exe_kg_lib/utils/task_utils/visual_utils.py` & `exe_kg_lib-1.1.3/exe_kg_lib/utils/task_utils/visual_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-1.1.2/pyproject.toml` & `exe_kg_lib-1.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "exe-kg-lib"
-version = "1.1.2" # not used when bumping version via poe bump-version-tag or cd.yaml
+version = "1.1.3" # not used when bumping version via poe bump-version-tag or cd.yaml
 description = "Library for executable ML pipelines represented by KGs."
 license = "AGPL-3.0"
 authors = ["Antonis Klironomos <antonis.klironomos@de.bosch.com>", "Mohamed Gad-Elrab <mohamed.gad-elrab@de.bosch.com>"]
 
 classifiers = [
   "Development Status :: 1 - Planning",
   "Intended Audience :: Developers",
```

