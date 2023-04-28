# Comparing `tmp/turms-0.4.0a1.tar.gz` & `tmp/turms-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turms-0.4.0a1.tar", max compression
+gzip compressed data, was "turms-0.4.1.tar", max compression
```

## Comparing `turms-0.4.0a1.tar` & `turms-0.4.1.tar`

### file list

```diff
@@ -1,41 +1,40 @@
--rw-r--r--   0        0        0     4881 2023-01-13 09:01:53.908215 turms-0.4.0a1/README.md
--rw-r--r--   0        0        0     1654 2023-04-28 14:12:02.202773 turms-0.4.0a1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-01-19 11:17:22.890244 turms-0.4.0a1/turms/__init__.py
--rw-r--r--   0        0        0        0 2022-01-20 10:23:20.654247 turms-0.4.0a1/turms/cli/__init__.py
--rw-r--r--   0        0        0     8622 2023-04-12 10:48:32.062124 turms-0.4.0a1/turms/cli/main.py
--rw-r--r--   0        0        0      621 2023-04-28 14:11:23.122644 turms-0.4.0a1/turms/cli/watch.py
--rw-r--r--   0        0        0    13305 2023-04-12 14:03:39.467970 turms-0.4.0a1/turms/config.py
--rw-r--r--   0        0        0     2153 2023-04-23 12:17:17.291356 turms-0.4.0a1/turms/directive_resolvers/variable/validator.py
--rw-r--r--   0        0        0      799 2022-12-01 14:27:27.458604 turms-0.4.0a1/turms/errors.py
--rw-r--r--   0        0        0     4520 2023-03-18 14:45:39.369557 turms-0.4.0a1/turms/helpers.py
--rw-r--r--   0        0        0      750 2022-07-25 16:54:58.579457 turms-0.4.0a1/turms/mocks.py
--rw-r--r--   0        0        0        0 2022-03-16 15:01:31.104480 turms-0.4.0a1/turms/parsers/__init__.py
--rw-r--r--   0        0        0      525 2022-12-01 14:27:27.458604 turms-0.4.0a1/turms/parsers/base.py
--rw-r--r--   0        0        0     2102 2022-12-01 14:27:27.458604 turms-0.4.0a1/turms/parsers/polyfill.py
--rw-r--r--   0        0        0        0 2023-04-12 13:45:47.588636 turms-0.4.0a1/turms/plugins/__init__.py
--rw-r--r--   0        0        0     1007 2023-03-18 14:45:39.369557 turms-0.4.0a1/turms/plugins/base.py
--rw-r--r--   0        0        0     3718 2023-03-18 14:45:39.369557 turms-0.4.0a1/turms/plugins/enums.py
--rw-r--r--   0        0        0    10361 2023-03-18 14:45:39.369557 turms-0.4.0a1/turms/plugins/fragments.py
--rw-r--r--   0        0        0    28213 2023-03-18 14:45:39.373557 turms-0.4.0a1/turms/plugins/funcs.py
--rw-r--r--   0        0        0     8477 2023-03-18 14:45:39.373557 turms-0.4.0a1/turms/plugins/inputs.py
--rw-r--r--   0        0        0    13761 2023-03-18 14:45:39.373557 turms-0.4.0a1/turms/plugins/objects.py
--rw-r--r--   0        0        0    11054 2023-04-12 13:58:28.221873 turms-0.4.0a1/turms/plugins/operations.py
--rw-r--r--   0        0        0    33581 2023-03-18 14:45:39.373557 turms-0.4.0a1/turms/plugins/strawberry.py
--rw-r--r--   0        0        0        0 2022-03-16 15:01:31.104480 turms-0.4.0a1/turms/processors/__init__.py
--rw-r--r--   0        0        0      685 2023-01-13 08:46:34.358681 turms-0.4.0a1/turms/processors/base.py
--rw-r--r--   0        0        0      751 2023-01-13 08:46:34.358681 turms-0.4.0a1/turms/processors/black.py
--rw-r--r--   0        0        0      968 2023-01-13 08:46:34.358681 turms-0.4.0a1/turms/processors/disclaimer.py
--rw-r--r--   0        0        0      573 2023-01-13 08:46:34.358681 turms-0.4.0a1/turms/processors/isort.py
--rw-r--r--   0        0        0     8277 2023-03-18 14:45:39.373557 turms-0.4.0a1/turms/processors/merge.py
--rw-r--r--   0        0        0    20783 2023-04-12 12:06:05.784888 turms-0.4.0a1/turms/recurse.py
--rw-r--r--   0        0        0     6502 2023-04-27 11:47:40.019614 turms-0.4.0a1/turms/referencer.py
--rw-r--r--   0        0        0    17396 2023-04-12 13:38:45.293543 turms-0.4.0a1/turms/registry.py
--rw-r--r--   0        0        0    14154 2023-04-12 13:35:54.104205 turms-0.4.0a1/turms/run.py
--rw-r--r--   0        0        0        0 2022-03-25 11:46:58.793385 turms-0.4.0a1/turms/stylers/__init__.py
--rw-r--r--   0        0        0     1112 2022-03-25 11:46:58.793385 turms-0.4.0a1/turms/stylers/appender.py
--rw-r--r--   0        0        0     2817 2022-12-01 14:27:27.458604 turms-0.4.0a1/turms/stylers/base.py
--rw-r--r--   0        0        0     1163 2022-12-01 14:27:27.458604 turms-0.4.0a1/turms/stylers/capitalize.py
--rw-r--r--   0        0        0     1438 2022-12-01 14:27:27.458604 turms-0.4.0a1/turms/stylers/default.py
--rw-r--r--   0        0        0      727 2022-12-01 14:27:27.458604 turms-0.4.0a1/turms/stylers/snake_case.py
--rw-r--r--   0        0        0    20341 2023-04-12 13:28:54.201249 turms-0.4.0a1/turms/utils.py
--rw-r--r--   0        0        0     6261 1970-01-01 00:00:00.000000 turms-0.4.0a1/PKG-INFO
+-rw-r--r--   0        0        0     4881 2023-03-18 12:48:25.735186 turms-0.4.1/README.md
+-rw-r--r--   0        0        0     1645 2023-03-18 14:56:18.070160 turms-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-18 12:48:25.744547 turms-0.4.1/turms/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-18 12:48:25.744647 turms-0.4.1/turms/cli/__init__.py
+-rw-r--r--   0        0        0     8574 2023-03-18 14:44:25.564848 turms-0.4.1/turms/cli/main.py
+-rw-r--r--   0        0        0      549 2023-03-18 14:44:25.565090 turms-0.4.1/turms/cli/watch.py
+-rw-r--r--   0        0        0    11698 2023-03-18 14:44:25.565234 turms-0.4.1/turms/config.py
+-rw-r--r--   0        0        0      799 2023-03-18 12:48:25.744917 turms-0.4.1/turms/errors.py
+-rw-r--r--   0        0        0     4520 2023-03-18 14:44:25.565351 turms-0.4.1/turms/helpers.py
+-rw-r--r--   0        0        0      750 2023-03-18 12:48:25.745032 turms-0.4.1/turms/mocks.py
+-rw-r--r--   0        0        0        0 2023-03-18 12:48:25.745083 turms-0.4.1/turms/parsers/__init__.py
+-rw-r--r--   0        0        0      525 2023-03-18 12:48:25.745145 turms-0.4.1/turms/parsers/base.py
+-rw-r--r--   0        0        0     2102 2023-03-18 12:48:25.745211 turms-0.4.1/turms/parsers/polyfill.py
+-rw-r--r--   0        0        0        0 2023-03-18 12:48:25.745260 turms-0.4.1/turms/plugins/__init__.py
+-rw-r--r--   0        0        0     1007 2023-03-18 14:44:25.565461 turms-0.4.1/turms/plugins/base.py
+-rw-r--r--   0        0        0     3718 2023-03-18 14:44:25.565640 turms-0.4.1/turms/plugins/enums.py
+-rw-r--r--   0        0        0    10361 2023-03-18 14:44:25.565767 turms-0.4.1/turms/plugins/fragments.py
+-rw-r--r--   0        0        0    28213 2023-03-18 14:44:25.566020 turms-0.4.1/turms/plugins/funcs.py
+-rw-r--r--   0        0        0     8477 2023-03-18 14:44:25.566166 turms-0.4.1/turms/plugins/inputs.py
+-rw-r--r--   0        0        0    13761 2023-03-18 14:44:25.566303 turms-0.4.1/turms/plugins/objects.py
+-rw-r--r--   0        0        0     9775 2023-03-18 14:44:25.566430 turms-0.4.1/turms/plugins/operations.py
+-rw-r--r--   0        0        0    33581 2023-03-18 14:44:25.566568 turms-0.4.1/turms/plugins/strawberry.py
+-rw-r--r--   0        0        0        0 2023-03-18 12:48:25.746147 turms-0.4.1/turms/processors/__init__.py
+-rw-r--r--   0        0        0      685 2023-03-18 12:48:25.746208 turms-0.4.1/turms/processors/base.py
+-rw-r--r--   0        0        0      751 2023-03-18 12:48:25.746259 turms-0.4.1/turms/processors/black.py
+-rw-r--r--   0        0        0      968 2023-03-18 12:48:25.746301 turms-0.4.1/turms/processors/disclaimer.py
+-rw-r--r--   0        0        0      573 2023-03-18 12:48:25.746348 turms-0.4.1/turms/processors/isort.py
+-rw-r--r--   0        0        0     8277 2023-03-18 14:44:25.566725 turms-0.4.1/turms/processors/merge.py
+-rw-r--r--   0        0        0    20443 2023-03-18 14:44:25.566832 turms-0.4.1/turms/recurse.py
+-rw-r--r--   0        0        0     6239 2023-03-18 14:44:25.567091 turms-0.4.1/turms/referencer.py
+-rw-r--r--   0        0        0    16522 2023-03-18 14:44:25.567350 turms-0.4.1/turms/registry.py
+-rw-r--r--   0        0        0    12975 2023-03-18 14:44:25.567666 turms-0.4.1/turms/run.py
+-rw-r--r--   0        0        0        0 2023-03-18 12:48:25.746858 turms-0.4.1/turms/stylers/__init__.py
+-rw-r--r--   0        0        0     1112 2023-03-18 12:48:25.746926 turms-0.4.1/turms/stylers/appender.py
+-rw-r--r--   0        0        0     2817 2023-03-18 12:48:25.746981 turms-0.4.1/turms/stylers/base.py
+-rw-r--r--   0        0        0     1163 2023-03-18 12:48:25.747037 turms-0.4.1/turms/stylers/capitalize.py
+-rw-r--r--   0        0        0     1438 2023-03-18 12:48:25.747085 turms-0.4.1/turms/stylers/default.py
+-rw-r--r--   0        0        0      727 2023-03-18 12:48:25.747135 turms-0.4.1/turms/stylers/snake_case.py
+-rw-r--r--   0        0        0    19484 2023-03-18 14:44:25.567814 turms-0.4.1/turms/utils.py
+-rw-r--r--   0        0        0     6259 1970-01-01 00:00:00.000000 turms-0.4.1/PKG-INFO
```

### Comparing `turms-0.4.0a1/README.md` & `turms-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `turms-0.4.0a1/pyproject.toml` & `turms-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "turms"
-version = "0.4.0a1"
+version = "0.4.1"
 description = "graphql-codegen powered by pydantic"
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 license = "CC BY-NC 3.0"
 readme = "README.md"
 packages = [{ include = "turms" }]
 homepage = "https://jhnnsrs.github.io/turms"
 repository = "https://github.com/jhnnsrs/turms"
@@ -45,15 +45,15 @@
 [tool.poetry.extras]
 watch = ["watchdog"]
 black = ["black"]
 isort = ["isort"]
 merge = ["libcst"]
 
 [tool.poetry.scripts]
-turms = "turms.cli.main:entrypoint"
+turms = "turms.cli.main:cli"
 
 [tool.poetry.group.dev.dependencies]
 libcst = "^0.4.9"
 ruff = "^0.0.257"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `turms-0.4.0a1/turms/cli/main.py` & `turms-0.4.1/turms/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,14 @@
                 write_code_to_file(
                     generated_code,
                     project.extensions.turms.out_dir,
                     project.extensions.turms.generated_name,
                 )
 
             except Exception as e:
-                get_console().print_exception()
                 project_tree.style = "red"
                 project_tree.label = f"{key} 💥"
                 project_tree.add(Tree(str(e), style="red"))
                 live.update(panel)
 
 
 def with_projects(func):
```

### Comparing `turms-0.4.0a1/turms/cli/watch.py` & `turms-0.4.1/turms/cli/watch.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,18 +6,15 @@
 class GraphQLFilter(BaseFilter):  # pragma: no cover
     def __call__(self, change, path: str) -> bool:
         x = super().__call__(change, path)
         if not x:
             return False
 
         x = os.path.basename(path)
-        try:
-            fileending = x.split(".")[1]
+        fileending = x.split(".")[1]
 
-            return fileending == "graphql"
-        except Exception:
-            return False
+        return fileending == "graphql"
 
 
 def stream_changes(folder: str):  # pragma: no cover
     for changes in watch(".", watch_filter=GraphQLFilter(), debounce=2000, step=500):
         yield changes
```

### Comparing `turms-0.4.0a1/turms/config.py` & `turms-0.4.1/turms/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import builtins
 from pydantic import AnyHttpUrl, BaseModel, BaseSettings, Field, validator
 from typing import Any, Dict, List, Optional, Union, Protocol, Literal, runtime_checkable
 from turms.helpers import import_string
-from graphql import DirectiveLocation
 from enum import Enum
 
 
 class ConfigProxy(BaseModel):
     type: str
 
     class Config:
         extra = "allow"
 
+
 class ImportableFunctionMixin(Protocol):
     @classmethod
     def __get_validators__(cls):
         # one or more validators may be yielded which will be called in the
         # order to validate the input, each validator will receive as an input
         # the value returned from the previous validator
         yield cls.validate
@@ -67,18 +67,14 @@
 
 @runtime_checkable
 class LogFunction(Protocol):
 
     def __call__(self, message, level: LogLevel = LogLevel.INFO):
         pass
 
-@runtime_checkable
-class DirectiveFunction(ImportableFunctionMixin, Protocol):
-    pass
-
 
 class FreezeConfig(BaseSettings):
     """Configuration for freezing the generated pydantic
     models
 
     This is useful for when you want to generate the models
     that are faux immutable and hashable by default. The configuration
@@ -157,36 +153,14 @@
     )
     """List of types to exclude from setting this option"""
     include: Optional[List[str]] = Field(
         description="List of types to include in setting these options"
     )
     """The types to freeze"""
 
-DescriptionLocation = Literal["field", "docstring", "both"]
-ArgType = Literal["string", "int", "float"]
-
-class TurmsDirective(BaseModel):
-    """A directive resolver"""
-
-    type: DirectiveFunction
-    """The type of the resolver"""
-    locations: List[DirectiveLocation] = Field(
-        [], description="The location of the directive"
-    )
-    args: Optional[Dict[str, ArgType]] = Field(
-        default_factory=dict, description="The arguments of the directive"
-    )
-    trim: bool = Field(
-        True, description="This directive will be exluded and not send to the server"
-    )
-
-    
-
-
-
 
 class GeneratorConfig(BaseSettings):
     """Configuration for the generator
 
     This is the main generator configuration that allows you to
     customize the way the models are generated.
 
@@ -205,38 +179,24 @@
     """The documents to parse. Setting this will overwrite the documents in the graphql config"""
     verbose: bool = False
     """Enable verbose logging"""
 
     allow_introspection: bool = True
     """Allow introspection queries"""
 
-    description: DescriptionLocation = "docstring"
-    turms_directives: Dict[str, TurmsDirective] = Field(
-        default_factory=dict,
-        description="Mapping directives to a resolver e.g @upper: path.to.upper_resolver, @lower: path.to.lower_resolver",
-    )
-
-
     object_bases: List[str] = ["pydantic.BaseModel"]
     """The base classes for the generated objects. This is useful if you want to change the base class from BaseModel to something else"""
 
     interface_bases: Optional[List[str]] = None
     """List of base classes for interfaces"""
     always_resolve_interfaces: bool = True
     """Always resolve interfaces to concrete types"""
     exclude_typenames: bool = False
     """Exclude __typename from generated models when calling dict or json"""
-    default_factories: Dict[str, PythonType] = Field(
-        default_factory=dict,
-        description="Mapping arguments to a default factories e.g ID: uuid.uuid4, Date: datetime.date.today, if you want to generated a default value for a list of a Type you can use standard graphql syntax like [Date]: path.to.list.factory",
-    )
-    argument_validators: Dict[str, PythonType] = Field(
-        default_factory=dict,
-        description="Will generate a validator for arguments that will always be called. This is useful for validating arguments that are not part of the schema. e.g. ID: path.to.validator",
-    )
+
     scalar_definitions: Dict[str, PythonType] = Field(
         default_factory=dict,
         description="Additional config for mapping scalars to python types (e.g. ID: str). Can use dotted paths to import types from other modules.",
     )
     """Additional config for mapping scalars to python types (e.g. ID: str). Can use dotted paths to import types from other modules."""
     freeze: FreezeConfig = Field(
         default_factory=FreezeConfig,
```

### Comparing `turms-0.4.0a1/turms/errors.py` & `turms-0.4.1/turms/errors.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.0a1/turms/helpers.py` & `turms-0.4.1/turms/helpers.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.0a1/turms/mocks.py` & `turms-0.4.1/turms/mocks.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.0a1/turms/parsers/base.py` & `turms-0.4.1/turms/parsers/base.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.0a1/turms/parsers/polyfill.py` & `turms-0.4.1/turms/parsers/polyfill.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.0a1/turms/plugins/base.py` & `turms-0.4.1/turms/plugins/base.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.0a1/turms/plugins/enums.py` & `turms-0.4.1/turms/plugins/enums.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.0a1/turms/plugins/fragments.py` & `turms-0.4.1/turms/plugins/fragments.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.0a1/turms/plugins/funcs.py` & `turms-0.4.1/turms/plugins/funcs.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.0a1/turms/plugins/inputs.py` & `turms-0.4.1/turms/plugins/inputs.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.0a1/turms/plugins/objects.py` & `turms-0.4.1/turms/plugins/objects.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.0a1/turms/plugins/operations.py` & `turms-0.4.1/turms/plugins/operations.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 from turms.recurse import type_field_node
 from turms.plugins.base import Plugin, PluginConfig
 from pydantic import Field
 from graphql.language.ast import (
     FieldNode,
     OperationDefinitionNode,
     OperationType,
-    VariableDefinitionNode,
-    NamedTypeNode,
-    ListTypeNode,
 )
 from graphql.utilities.build_client_schema import GraphQLSchema
 from graphql.utilities.get_operation_root_type import get_operation_root_type
 from graphql.utilities.type_info import get_field_def
 
 import re
 from graphql import NonNullTypeNode, language
@@ -26,15 +23,15 @@
     inspect_operation_for_documentation,
     parse_documents,
     recurse_type_annotation,
     replace_iteratively,
     parse_value_node,
 )
 import logging
-from turms.utils import print_operation
+
 
 logger = logging.getLogger(__name__)
 fragment_searcher = re.compile(r"\.\.\.(?P<fragment>[a-zA-Z]*)")
 
 
 class OperationsPluginConfig(PluginConfig):
     type = "turms.plugins.operations.OperationsPlugin"
@@ -142,23 +139,14 @@
 
             return [
                 ast.Name(id=base.split(".")[-1], ctx=ast.Load())
                 for base in config.object_bases
             ]
 
 
-def represent_variable_definition(x: VariableDefinitionNode)-> str:
-    if isinstance(x, NamedTypeNode):
-        return x.name.value
-    if isinstance(x, NonNullTypeNode):
-        return f"{represent_variable_definition(x.type)}!"
-    if isinstance(x, ListTypeNode):
-        return f"[{represent_variable_definition(x.type)}]"
-    raise Exception(f"Unknown type {type(x)}")
-
 def generate_operation(
     o: OperationDefinitionNode,
     client_schema: GraphQLSchema,
     config: GeneratorConfig,
     plugin_config: OperationsPluginConfig,
     registry: ClassRegistry,
 ):
@@ -205,81 +193,54 @@
                 client_schema,
                 config,
                 tree,
                 registry,
             ),
         ]
 
-    merged_document = print_operation(o, config, registry)
+    query_document = language.print_ast(o)
+    merged_document = replace_iteratively(query_document, registry)
 
     if plugin_config.create_arguments:
 
         arguments_body = []
-        validators_body = []
 
         for v in o.variable_definitions:
-
-            variable_def_body = []
-
-            type = v.type
-
-            keywords = []
-
-            if v.default_value:
-                keywords.append(ast.keyword(arg="default", value=ast.Constant(v.default_value.value, ctx=ast.Load())))
-                
-
-            if keywords:
-                registry.register_import("pydantic.Field")
-                variable_def_body += [
+            if isinstance(v.type, NonNullTypeNode) and not v.default_value:
+                arguments_body += [
                     ast.AnnAssign(
                         target=ast.Name(
                             id=registry.generate_parameter_name(v.variable.name.value),
                             ctx=ast.Store(),
                         ),
-                        annotation=recurse_type_annotation(
-                            v.type,
-                            registry,
-                        ),
-                        value=ast.Call(
-                            func=ast.Name(id="Field", ctx=ast.Load()),
-                            args=[],
-                            keywords=keywords,
-                        ),
+                        annotation=recurse_type_annotation(v.type, registry),
                         simple=1,
                     )
                 ]
-                
-            else:
-                variable_def_body += [
+
+            if not isinstance(v.type, NonNullTypeNode) or v.default_value:
+                arguments_body += [
                     ast.AnnAssign(
                         target=ast.Name(
                             id=registry.generate_parameter_name(v.variable.name.value),
                             ctx=ast.Store(),
                         ),
-                        annotation=recurse_type_annotation(v.type, registry),
+                        annotation=recurse_type_annotation(
+                            v.type,
+                            registry,
+                        ),
+                        value=ast.Constant(
+                            value=parse_value_node(v.default_value)
+                            if v.default_value
+                            else None
+                        ),
                         simple=1,
                     )
                 ]
 
-            for directive in v.directives:
-                directive_name = directive.name.value
-                directive_def = registry.get_directive(directive_name)
-                if directive_def:
-                    variable_def_body = directive_def.type(
-                        v,
-                        variable_def_body,
-                        registry,
-                        **{arg.name.value: arg.value.value for arg in directive.arguments}
-                    )
-                    
-            arguments_body += variable_def_body
-
-        arguments_body += validators_body
-
         class_body_fields += [
             ast.ClassDef(
                 "Arguments",
                 bases=get_arguments_bases(config, plugin_config, registry=registry),
                 decorator_list=[],
                 keywords=[],
                 body=arguments_body or [ast.Pass()],
```

### Comparing `turms-0.4.0a1/turms/plugins/strawberry.py` & `turms-0.4.1/turms/plugins/strawberry.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.0a1/turms/processors/base.py` & `turms-0.4.1/turms/processors/base.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.0a1/turms/processors/black.py` & `turms-0.4.1/turms/processors/black.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.0a1/turms/processors/disclaimer.py` & `turms-0.4.1/turms/processors/disclaimer.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.0a1/turms/processors/isort.py` & `turms-0.4.1/turms/processors/isort.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.0a1/turms/processors/merge.py` & `turms-0.4.1/turms/processors/merge.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.0a1/turms/recurse.py` & `turms-0.4.1/turms/recurse.py`

 * *Files 3% similar despite different names*

```diff
@@ -514,15 +514,14 @@
                     config,
                     subtree,
                     registry,
                 )
             )
 
 
-
 def type_field_node(
     node: FieldNode,
     parent: str,
     field: GraphQLField,
     client_schema: GraphQLSchema,
     config: GeneratorConfig,
     subtree: ast.AST,
@@ -546,34 +545,15 @@
     Returns:
         _type_: _description_
     """
 
     target = target_from_node(node)
     field_name = registry.generate_node_name(target)
 
-    potential_comment = (
-        field.description
-        if not field.deprecation_reason
-        else f"DEPRECATED {field.deprecation_reason}: : {field.description} "
-    )
-
-    keywords = []
-
-    if field.deprecation_reason:
-        registry.warn(
-            f"Field {node.name.value} on {parent} is deprecated: {field.deprecation_reason}"
-        )
-
-    if config.description == "both" or config.description == "field" and potential_comment:
-        keywords.append(ast.keyword(arg="description", value=ast.Constant(value=potential_comment)))
-
     if target != field_name:
-        keywords.append(ast.keyword(arg="alias", value=ast.Constant(value=target)))
-
-    if keywords:
         registry.register_import("pydantic.Field")
         assign = ast.AnnAssign(
             target=ast.Name(field_name, ctx=ast.Store()),
             annotation=recurse_annotation(
                 node,
                 parent,
                 field.type,
@@ -582,15 +562,15 @@
                 subtree,
                 registry,
                 is_optional=is_optional,
             ),
             value=ast.Call(
                 func=ast.Name(id="Field", ctx=ast.Load()),
                 args=[],
-                keywords=keywords,
+                keywords=[ast.keyword(arg="alias", value=ast.Constant(value=target))],
             ),
             simple=1,
         )
     else:
         assign = ast.AnnAssign(
             target=ast.Name(target, ctx=ast.Store()),
             annotation=recurse_annotation(
@@ -602,13 +582,22 @@
                 subtree,
                 registry,
                 is_optional=is_optional,
             ),
             simple=1,
         )
 
-    
+    potential_comment = (
+        field.description
+        if not field.deprecation_reason
+        else f"DEPRECATED {field.deprecation_reason}: : {field.description} "
+    )
+
+    if field.deprecation_reason:
+        registry.warn(
+            f"Field {node.name.value} on {parent} is deprecated: {field.deprecation_reason}"
+        )
 
-    if config.description == "both" or config.description == "docstring" and potential_comment:
+    if potential_comment:
         return [assign, ast.Expr(value=ast.Constant(value=potential_comment))]
 
     return [assign]
```

### Comparing `turms-0.4.0a1/turms/referencer.py` & `turms-0.4.1/turms/referencer.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,61 +56,58 @@
     client_schema: GraphQLSchema,
     registry: ReferenceRegistry,
     is_optional=True,
 ):
     if isinstance(
         graphql_type, (GraphQLUnionType, GraphQLObjectType, GraphQLInterfaceType)
     ):
+
         for sub_node in node.selection_set.selections:
+
             if isinstance(sub_node, FragmentSpreadNode):
                 registry.register_fragment(sub_node.name.value)
 
-            elif isinstance(sub_node, InlineFragmentNode):
+            if isinstance(sub_node, InlineFragmentNode):
                 for sub_sub_node in sub_node.selection_set.selections:
+
                     if isinstance(sub_sub_node, FieldNode):
                         sub_sub_node_type = client_schema.get_type(
                             sub_node.type_condition.name.value
                         )
 
                         if sub_sub_node.name.value == "__typename":
                             continue
 
                         field_type = sub_sub_node_type.fields[sub_sub_node.name.value]
-                        recurse_find_references(
+                        return recurse_find_references(
                             sub_sub_node,
                             field_type.type,
                             client_schema,
                             registry,
                         )
 
-            else:
-                field_type = graphql_type.fields[sub_node.name.value]
-                recurse_find_references(
-                    sub_node,
-                    field_type.type,
-                    client_schema,
-                    registry,
-                )
-
     elif isinstance(graphql_type, GraphQLScalarType):
+
         registry.register_scalar(graphql_type.name)
 
     elif isinstance(graphql_type, GraphQLEnumType):
+
         registry.register_enum(graphql_type.name)
 
     elif isinstance(graphql_type, GraphQLNonNull):
         recurse_find_references(
             node,
             graphql_type.of_type,
             client_schema,
             registry,
             is_optional=False,
         )
 
     elif isinstance(graphql_type, GraphQLList):
+
         recurse_find_references(
             node,
             graphql_type.of_type,
             client_schema,
             registry,
             is_optional=False,
         )
@@ -120,23 +117,25 @@
 
 def recurse_type_annotation(
     graphql_type: NamedTypeNode,
     schema: GraphQLSchema,
     registry: ReferenceRegistry,
     optional=True,
 ):
+
     if isinstance(graphql_type, NonNullTypeNode):
         return recurse_type_annotation(
             graphql_type.type, schema, registry, optional=False
         )
 
     elif isinstance(graphql_type, ListTypeNode):
         recurse_type_annotation(graphql_type.type, schema, registry)
 
     elif isinstance(graphql_type, NamedTypeNode):
+
         z = schema.get_type(graphql_type.name.value)
         if isinstance(z, GraphQLScalarType):
             registry.register_scalar(z.name)
 
         elif isinstance(z, GraphQLInputObjectType):
             registry.register_input(z.name)
 
@@ -163,36 +162,40 @@
     for definition in document.definitions:
         if isinstance(definition, FragmentDefinitionNode):
             fragments[definition.name.value] = definition
         if isinstance(definition, OperationDefinitionNode):
             operations[definition.name.value] = definition
 
     for fragment in fragments.values():
+
         type = schema.get_type(fragment.type_condition.name.value)
         for selection in fragment.selection_set.selections:
+
             if isinstance(selection, FieldNode):
                 # definition
                 if selection.name.value == "__typename":
                     continue
                 this_type = type.fields[selection.name.value]
 
                 recurse_find_references(
                     selection,
                     this_type.type,
                     schema,
                     registry,
                 )
 
     for operation in operations.values():
+
         type = schema.get_root_type(operation.operation)
 
         for argument in operation.variable_definitions:
             recurse_type_annotation(argument.type, schema, registry)
 
         for selection in operation.selection_set.selections:
+
             if isinstance(selection, FieldNode):
                 # definition
                 if selection.name.value == "__typename":
                     continue
                 this_type = type.fields[selection.name.value]
 
                 recurse_find_references(
```

### Comparing `turms-0.4.0a1/turms/registry.py` & `turms-0.4.1/turms/registry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import ast
-from typing import Dict, List, Optional
-from turms.config import GeneratorConfig, LogFunction, TurmsDirective
+from typing import Dict, List
+from turms.config import GeneratorConfig, LogFunction
 from keyword import iskeyword
 from turms.errors import (
     NoEnumFound,
     NoInputTypeFound,
     NoScalarFound,
     RegistryError,
 )
@@ -80,17 +80,14 @@
     def __init__(self, config: GeneratorConfig, stylers: List[Styler], log: LogFunction):
         self.stylers = stylers
         self._imports = set()
         self._builtins = set()
         self.config = config
 
         self.scalar_map = {**SCALAR_DEFAULTS, **config.scalar_definitions}
-        self.factory_map = config.default_factories
-        self.validator_map = config.argument_validators
-        self.directive_map = config.turms_directives
 
         self.fragment_document_map = {}
 
         self.enum_class_map = {}
         self.inputtype_class_map = {}
         self.object_class_map = {}
         self.interface_reference_map = {}
@@ -103,33 +100,14 @@
         self.mutation_class_map = {}
 
         self.forward_references = set()
 
         self.interfacefragments_class_map = {}
         self.log = log
 
-    def get_default_factory(self, typename: str) -> Optional[str]:
-        if typename in self.factory_map:
-            factory = self.factory_map[typename]
-            self.register_import(factory)
-            return factory.split(".")[-1]
-        
-    def get_validator(self, typename: str) -> Optional[str]:
-        if typename in self.validator_map:
-            factory = self.validator_map[typename]
-            self.register_import(factory)
-            return factory.split(".")[-1]
-        
-    def get_directive(self, directive_name: str) -> Optional[TurmsDirective]:
-        if directive_name in self.directive_map:
-            return self.directive_map[directive_name]
-    
-
-
-
     def style_inputtype_class(self, typename: str):
         for styler in self.stylers:
             typename = styler.style_input_name(typename)
         if iskeyword(typename):
             typename += "_"
         return typename
```

### Comparing `turms-0.4.0a1/turms/run.py` & `turms-0.4.1/turms/run.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ast
 import os
 from typing import Dict, List, Optional, Callable
 
 import yaml
-from graphql import GraphQLSchema, parse, build_ast_schema, build_client_schema, GraphQLDirective, DirectiveLocation, print_schema, GraphQLArgument, GraphQLString, GraphQLInt
+from graphql import GraphQLSchema, parse, build_ast_schema, build_client_schema
 from pydantic import AnyHttpUrl, ValidationError
 from rich import get_console
 
 from turms.config import (
     GeneratorConfig,
     GraphQLConfigMultiple,
     GraphQLConfigSingle,
@@ -302,52 +302,14 @@
                 intropection = load_introspection_from_glob(schema)
                 return build_client_schema(intropection)
             raise e
 
     raise GenerationError("Could not build schema with type " + str(type(schema)))
 
 
-
-
-
-def expand_schema(schema: GraphQLSchema, project: GraphQLProject) -> GraphQLSchema:
-    """Expands a schema with the schema extensions
-
-    Args:
-        schema (GraphQLSchema): The schema
-        project (GraphQLProject): The project
-
-    Returns:
-        GraphQLSchema: The expanded schema
-    """
-    additional_directives = []
-    for key, directive in project.extensions.turms.turms_directives.items():
-
-        additional_directives.append(GraphQLDirective(
-            name=key,
-            locations=directive.locations,
-            args={
-                arg: GraphQLArgument(
-                    GraphQLString if value == "string" else GraphQLInt,
-                    description="A custom argument for the directive. Faked for now.",
-                )
-                for arg, value in directive.args.items()
-            },
-            description="Marks an element of a GraphQL schema as no longer supported.",
-        ))
-
-
-    schema.directives = tuple(additional_directives) + schema.directives
-
-
-    return schema
-
-    
-
-
 def generate(project: GraphQLProject, log: Optional[LogFunction] = None) -> str:
     """Genrates the code according to the configugration
 
     The code is generated in the following order:
         1. Introspect the schema (either url or locally)
         2. Generate the of grapqhl.ast from this schema
         3. Instantiate all plugins/parsers/stylers
@@ -369,15 +331,14 @@
 
     gen_config = project.extensions.turms
 
     schema = build_schema_from_schema_type(
         project.schema_url,
         allow_introspection=project.extensions.turms.allow_introspection,
     )
-    scehma = expand_schema(schema, project)
 
     gen_config.documents = gen_config.documents or project.documents
     verbose = gen_config.verbose
 
     plugins = []
     stylers = []
     parsers = []
```

### Comparing `turms-0.4.0a1/turms/stylers/appender.py` & `turms-0.4.1/turms/stylers/appender.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.0a1/turms/stylers/base.py` & `turms-0.4.1/turms/stylers/base.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.0a1/turms/stylers/capitalize.py` & `turms-0.4.1/turms/stylers/capitalize.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.0a1/turms/stylers/default.py` & `turms-0.4.1/turms/stylers/default.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.0a1/turms/stylers/snake_case.py` & `turms-0.4.1/turms/stylers/snake_case.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.0a1/turms/utils.py` & `turms-0.4.1/turms/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,17 +31,14 @@
 from turms.registry import ClassRegistry
 from turms.errors import (
     GenerationError,
     NoEnumFound,
     NoInputTypeFound,
     NoScalarFound,
 )
-from copy import copy
-
-from graphql import NonNullTypeNode, language
 from .config import GraphQLTypes
 import re
 
 
 commentline_regex = re.compile(r"^.*#(.*)")
 
 
@@ -336,36 +333,14 @@
         nested_interface
         for other_interface in other_interfaces
         for nested_interface in other_interface.interfaces
     }
     return interface in interfaces_implemented_by_other_interfaces
 
 
-def print_operation(operation: OperationDefinitionNode, config: GeneratorConfig, registry: ClassRegistry) -> str:
-
-    directive_resolvers = list(config.turms_directives.keys())
-    
-    new_variables = []
-    for variable in operation.variable_definitions:
-        new_variable = copy(variable)
-        if variable.directives:
-            new_variable.directives = tuple(dir for dir in variable.directives if dir.name.value not in directive_resolvers)
-        new_variables.append(new_variable)
-
-    new_operation = copy(operation)
-    new_operation.variable_definitions = tuple(new_variables)
-
-
-    query_document = language.print_ast(new_operation)
-    return replace_iteratively(query_document, registry)
-
-
-
-
-
 def recurse_type_annotation(
     type: NamedTypeNode,
     registry: ClassRegistry,
     optional=True,
     overwrite_final: Optional[str] = None,
 ):
 
@@ -399,26 +374,26 @@
     if isinstance(type, NamedTypeNode):
         x = None
         if overwrite_final is not None:
             x = ast.Name(id=overwrite_final, ctx=ast.Load())
         else:
             try:
                 x = registry.reference_scalar(type.name.value)
-            except NoScalarFound as scalar_error:
+            except NoScalarFound:
                 try:
                     x = registry.reference_inputtype(
                         type.name.value, "", allow_forward=False
                     )
                 except NoInputTypeFound:
                     try:
                         x = registry.reference_enum(
                             type.name.value, "", allow_forward=False
                         )
                     except NoEnumFound:
-                        raise NotImplementedError("Could not find correspondig Type for " + type.name.value) from scalar_error
+                        raise NotImplementedError("Not implemented")
 
         if not x:
             raise Exception(f"Could not set value for {type}")
 
         if optional:
             registry.register_import("typing.Optional")
             return ast.Subscript(
```

### Comparing `turms-0.4.0a1/PKG-INFO` & `turms-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turms
-Version: 0.4.0a1
+Version: 0.4.1
 Summary: graphql-codegen powered by pydantic
 Home-page: https://jhnnsrs.github.io/turms
 License: CC BY-NC 3.0
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 6 - Mature
```

