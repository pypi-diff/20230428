# Comparing `tmp/kedro_azureml-0.3.6.tar.gz` & `tmp/kedro_azureml-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro_azureml-0.3.6.tar", max compression
+gzip compressed data, was "kedro_azureml-0.4.0.tar", max compression
```

## Comparing `kedro_azureml-0.3.6.tar` & `kedro_azureml-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0    11338 2023-03-08 15:49:14.090430 kedro_azureml-0.3.6/LICENSE
--rw-r--r--   0        0        0     2441 2023-03-08 15:49:14.090430 kedro_azureml-0.3.6/README.md
--rw-r--r--   0        0        0       96 2023-03-08 15:49:14.098430 kedro_azureml-0.3.6/kedro_azureml/__init__.py
--rw-r--r--   0        0        0     8812 2023-03-08 15:49:14.098430 kedro_azureml-0.3.6/kedro_azureml/cli.py
--rw-r--r--   0        0        0     4771 2023-03-08 15:49:14.098430 kedro_azureml-0.3.6/kedro_azureml/cli_functions.py
--rw-r--r--   0        0        0     3270 2023-03-08 15:49:14.098430 kedro_azureml-0.3.6/kedro_azureml/client.py
--rw-r--r--   0        0        0     3901 2023-03-08 15:49:14.098430 kedro_azureml-0.3.6/kedro_azureml/config.py
--rw-r--r--   0        0        0      323 2023-03-08 15:49:14.098430 kedro_azureml-0.3.6/kedro_azureml/constants.py
--rw-r--r--   0        0        0      403 2023-03-08 15:49:14.098430 kedro_azureml-0.3.6/kedro_azureml/datasets/__init__.py
--rw-r--r--   0        0        0    10958 2023-03-08 15:49:14.098430 kedro_azureml-0.3.6/kedro_azureml/datasets/file_dataset.py
--rw-r--r--   0        0        0     5305 2023-03-08 15:49:14.098430 kedro_azureml-0.3.6/kedro_azureml/datasets/pandas_dataset.py
--rw-r--r--   0        0        0     2653 2023-03-08 15:49:14.098430 kedro_azureml-0.3.6/kedro_azureml/datasets/runner_dataset.py
--rw-r--r--   0        0        0      906 2023-03-08 15:49:14.098430 kedro_azureml-0.3.6/kedro_azureml/datasets/utils.py
--rw-r--r--   0        0        0      149 2023-03-08 15:49:14.102430 kedro_azureml-0.3.6/kedro_azureml/distributed/__init__.py
--rw-r--r--   0        0        0      453 2023-03-08 15:49:14.102430 kedro_azureml-0.3.6/kedro_azureml/distributed/config.py
--rw-r--r--   0        0        0      701 2023-03-08 15:49:14.102430 kedro_azureml-0.3.6/kedro_azureml/distributed/decorators.py
--rw-r--r--   0        0        0     1220 2023-03-08 15:49:14.102430 kedro_azureml-0.3.6/kedro_azureml/distributed/utils.py
--rw-r--r--   0        0        0    11543 2023-03-08 15:49:14.102430 kedro_azureml-0.3.6/kedro_azureml/generator.py
--rw-r--r--   0        0        0     2077 2023-03-08 15:49:14.102430 kedro_azureml-0.3.6/kedro_azureml/runner.py
--rw-r--r--   0        0        0     1166 2023-03-08 15:49:14.102430 kedro_azureml-0.3.6/kedro_azureml/utils.py
--rw-r--r--   0        0        0     1674 2023-03-08 15:49:14.102430 kedro_azureml-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     3835 1970-01-01 00:00:00.000000 kedro_azureml-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11338 2023-04-28 13:30:42.924832 kedro_azureml-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2441 2023-04-28 13:30:42.924832 kedro_azureml-0.4.0/README.md
+-rw-r--r--   0        0        0       96 2023-04-28 13:30:42.932833 kedro_azureml-0.4.0/kedro_azureml/__init__.py
+-rw-r--r--   0        0        0    10195 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/cli.py
+-rw-r--r--   0        0        0     5018 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/cli_functions.py
+-rw-r--r--   0        0        0     3270 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/client.py
+-rw-r--r--   0        0        0     4475 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/config.py
+-rw-r--r--   0        0        0      323 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/constants.py
+-rw-r--r--   0        0        0      508 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/datasets/__init__.py
+-rw-r--r--   0        0        0    10959 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/datasets/file_dataset.py
+-rw-r--r--   0        0        0     5305 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/datasets/pandas_dataset.py
+-rw-r--r--   0        0        0     4254 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/datasets/pipeline_dataset.py
+-rw-r--r--   0        0        0     2653 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/datasets/runner_dataset.py
+-rw-r--r--   0        0        0      906 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/datasets/utils.py
+-rw-r--r--   0        0        0      149 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/distributed/__init__.py
+-rw-r--r--   0        0        0      453 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/distributed/config.py
+-rw-r--r--   0        0        0      701 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/distributed/decorators.py
+-rw-r--r--   0        0        0     1220 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/distributed/utils.py
+-rw-r--r--   0        0        0    12385 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/generator.py
+-rw-r--r--   0        0        0     2784 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/manager.py
+-rw-r--r--   0        0        0     3509 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/runner.py
+-rw-r--r--   0        0        0      568 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/utils.py
+-rw-r--r--   0        0        0     1676 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3837 1970-01-01 00:00:00.000000 kedro_azureml-0.4.0/PKG-INFO
```

### Comparing `kedro_azureml-0.3.6/LICENSE` & `kedro_azureml-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.3.6/README.md` & `kedro_azureml-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.3.6/kedro_azureml/cli.py` & `kedro_azureml-0.4.0/kedro_azureml/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import logging
 import os
 from pathlib import Path
-from typing import Optional, Tuple
+from typing import List, Optional, Tuple
 
 import click
 from kedro.framework.startup import ProjectMetadata
 
 from kedro_azureml.cli_functions import (
     get_context_and_pipeline,
     parse_extra_env_params,
@@ -17,16 +17,17 @@
 from kedro_azureml.client import AzureMLPipelinesClient
 from kedro_azureml.config import CONFIG_TEMPLATE_YAML
 from kedro_azureml.constants import (
     AZURE_SUBSCRIPTION_ID,
     KEDRO_AZURE_BLOB_TEMP_DIR_NAME,
 )
 from kedro_azureml.distributed.utils import is_distributed_master_node
+from kedro_azureml.manager import KedroContextManager
 from kedro_azureml.runner import AzurePipelinesRunner
-from kedro_azureml.utils import CliContext, KedroContextManager
+from kedro_azureml.utils import CliContext
 
 logger = logging.getLogger(__name__)
 
 
 @click.group("AzureML")
 def commands():
     """Kedro plugin adding support for Azure ML Pipelines"""
@@ -52,43 +53,56 @@
 
 @azureml_group.command()
 @click.argument("subscription_id")
 @click.argument("resource_group")
 @click.argument("workspace_name")
 @click.argument("experiment_name")
 @click.argument("cluster_name")
-@click.argument("storage_account_name")
-@click.argument("storage_container")
 @click.argument("environment_name")
+@click.option("-a", "--storage_account_name")
+@click.option("-c", "--storage_container")
+@click.option("--use-pipeline-data-passing", is_flag=True, default=False)
 @click.pass_obj
 def init(
     ctx: CliContext,
     subscription_id,
     resource_group,
     workspace_name,
     experiment_name,
     cluster_name,
+    environment_name,
     storage_account_name,
     storage_container,
-    environment_name,
+    use_pipeline_data_passing: bool,
 ):
     """
     Creates basic configuration for Kedro AzureML plugin
     """
+
+    if (
+        not (storage_account_name and storage_container)
+        and not use_pipeline_data_passing
+    ):
+        raise click.UsageError(
+            "You need to specify storage account (-a) and container name (-c) "
+            "or enable pipeline data passing (--use-pipeline-data-passing)"
+        )
+
     target_path = Path.cwd().joinpath("conf/base/azureml.yml")
     cfg = CONFIG_TEMPLATE_YAML.format(
         **{
             "subscription_id": subscription_id,
             "resource_group": resource_group,
             "workspace_name": workspace_name,
             "experiment_name": experiment_name,
             "cluster_name": cluster_name,
-            "storage_account_name": storage_account_name,
-            "storage_container": storage_container,
+            "storage_account_name": storage_account_name or "~",
+            "storage_container": storage_container or "~",
             "environment_name": environment_name,
+            "pipeline_data_passing": use_pipeline_data_passing,
         }
     )
     target_path.write_text(cfg)
 
     click.echo(f"Configuration generated in {target_path}")
 
     click.echo(
@@ -286,32 +300,54 @@
 @click.option(
     "--params",
     "params",
     type=str,
     help="Parameters override in form of `key=value`",
 )
 @click.option(
+    "--az-input",
+    "azure_inputs",
+    type=(str, click.Path(exists=True, file_okay=False, dir_okay=True)),
+    multiple=True,
+    help="Name and path of Azure ML Pipeline input",
+)
+@click.option(
     "--az-output",
     "azure_outputs",
-    type=str,
+    type=(str, click.Path(exists=True, file_okay=False, dir_okay=True)),
     multiple=True,
-    help="Paths of Azure ML Pipeline outputs to save dummy data into",
+    help="Name and path of Azure ML Pipeline output",
 )
 @click.pass_obj
 def execute(
-    ctx: CliContext, pipeline: str, node: str, params: str, azure_outputs: Tuple[str]
+    ctx: CliContext,
+    pipeline: str,
+    node: str,
+    params: str,
+    azure_inputs: List[Tuple[str, str]],
+    azure_outputs: List[Tuple[str, str]],
 ):
     # 1. Run kedro
     parameters = parse_extra_params(params)
+    azure_inputs = {ds_name: data_path for ds_name, data_path in azure_inputs}
+    azure_outputs = {ds_name: data_path for ds_name, data_path in azure_outputs}
+    data_paths = {**azure_inputs, **azure_outputs}
+
     with KedroContextManager(
         ctx.metadata.package_name, env=ctx.env, extra_params=parameters
     ) as mgr:
-        runner = AzurePipelinesRunner()
+        pipeline_data_passing = (
+            mgr.plugin_config.azure.pipeline_data_passing is not None
+            and mgr.plugin_config.azure.pipeline_data_passing.enabled
+        )
+        runner = AzurePipelinesRunner(
+            data_paths=data_paths, pipeline_data_passing=pipeline_data_passing
+        )
         mgr.session.run(pipeline, node_names=[node], runner=runner)
 
     # 2. Save dummy outputs
     # In distributed computing, it will only happen on nodes with rank 0
-    if is_distributed_master_node():
-        for dummy_output in azure_outputs:
-            (Path(dummy_output) / "output.txt").write_text("#getindata")
+    if not pipeline_data_passing and is_distributed_master_node():
+        for data_path in azure_outputs.values():
+            (Path(data_path) / "output.txt").write_text("#getindata")
     else:
         logger.info("Skipping saving Azure outputs on non-master distributed nodes")
```

### Comparing `kedro_azureml-0.3.6/kedro_azureml/cli_functions.py` & `kedro_azureml-0.4.0/kedro_azureml/cli_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Dict, Optional
 
 import click
 
 from kedro_azureml.generator import AzureMLPipelineGenerator
-from kedro_azureml.utils import CliContext, KedroContextManager
+from kedro_azureml.manager import KedroContextManager
+from kedro_azureml.utils import CliContext
 
 logger = logging.getLogger()
 
 
 @contextmanager
 def get_context_and_pipeline(
     ctx: CliContext,
@@ -23,15 +24,19 @@
     aml_env: Optional[str] = None,
     extra_env: Dict[str, str] = {},
 ):
     with KedroContextManager(
         ctx.metadata.package_name, ctx.env, parse_extra_params(params, True)
     ) as mgr:
         storage_account_key = os.getenv("AZURE_STORAGE_ACCOUNT_KEY", "")
-        if not storage_account_key:
+        pipeline_data_passing = (
+            mgr.plugin_config.azure.pipeline_data_passing is not None
+            and mgr.plugin_config.azure.pipeline_data_passing.enabled
+        )
+        if not pipeline_data_passing and not storage_account_key:
             click.echo(
                 click.style(
                     "Environment variable AZURE_STORAGE_ACCOUNT_KEY not set, falling back to CLI prompt",
                     fg="yellow",
                 )
             )
             storage_account_key = click.prompt(
```

### Comparing `kedro_azureml-0.3.6/kedro_azureml/client.py` & `kedro_azureml-0.4.0/kedro_azureml/client.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.3.6/kedro_azureml/config.py` & `kedro_azureml-0.4.0/kedro_azureml/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 from collections import defaultdict
 from typing import Dict, Optional, Type
 
 import yaml
 from pydantic import BaseModel, validator
 
+from kedro_azureml.utils import update_dict
+
 
 class DefaultConfigDict(defaultdict):
     def __getitem__(self, key):
         defaults: BaseModel = super().__getitem__("__default__")
         this: BaseModel = super().__getitem__(key)
         return defaults.copy(update=this.dict(exclude_none=True)) if defaults else this
 
 
 class AzureTempStorageConfig(BaseModel):
-    account_name: str
-    container: str
+    account_name: Optional[str] = None
+    container: Optional[str] = None
 
 
 class ComputeConfig(BaseModel):
     cluster_name: str
 
 
 class DockerConfig(BaseModel):
     image: Optional[str] = None
 
 
+class PipelineDataPassingConfig(BaseModel):
+    enabled: bool = False
+
+
 class AzureMLConfig(BaseModel):
     @staticmethod
     def _create_default_dict_with(
         value: dict, default, dict_cls: Type = DefaultConfigDict
     ):
         default_value = (value := value or {}).get("__default__", default)
         return dict_cls(lambda: default_value, value)
@@ -40,18 +46,19 @@
         )
 
     subscription_id: str
     resource_group: str
     workspace_name: str
     experiment_name: str
     compute: Optional[Dict[str, ComputeConfig]]
-    temporary_storage: AzureTempStorageConfig
+    temporary_storage: Optional[AzureTempStorageConfig]
     environment_name: Optional[str]
     code_directory: Optional[str]
     working_directory: Optional[str]
+    pipeline_data_passing: Optional[PipelineDataPassingConfig] = None
 
 
 class KedroAzureMLConfig(BaseModel):
     azure: AzureMLConfig
     docker: Optional[DockerConfig] = None
 
 
@@ -75,25 +82,28 @@
   # Azure ML Environment to use during pipeline execution
   environment_name: "{environment_name}"
   # Path to directory to upload, or null to disable code upload
   code_directory: "."
   # Path to the directory in the Docker image to run the code from
   # Ignored when code_directory is set
   working_directory: /home/kedro_docker
+  # Use Azure ML pipeline data passing instead of temporary storage
+  pipeline_data_passing:
+    enabled: {pipeline_data_passing} # disabled by default
 
   # Temporary storage settings - this is used to pass some data between steps
   # if the data is not specified in the catalog directly
   temporary_storage:
     # Azure Storage account name, where the temp data should be stored
     # It's recommended to set Lifecycle management rule for storage container, to avoid costs of long-term storage
     # of the temporary data. Temporary data will be stored under abfs://<containter>/kedro-azureml-temp path
     # See https://docs.microsoft.com/en-us/azure/storage/blobs/lifecycle-management-policy-configure?tabs=azure-portal
-    account_name: "{storage_account_name}"
+    account_name: {storage_account_name}
     # Name of the storage container
-    container: "{storage_container}"
+    container: {storage_container}
   compute:
     # Azure compute used for running kedro jobs.
     # Additional compute cluster can be defined here. Individual nodes can reference specific compute clusters by adding
     # the section title (e.g. <your_node_tag>) as a node_tag to their tags list. Nodes without a tag will run on
     # __default__ cluster.
     __default__:
       cluster_name: "{cluster_name}"
@@ -104,8 +114,15 @@
   # We suggest using the Azure environment instead
   # See https://kedro-azureml.readthedocs.io/en/0.2.1/source/03_quickstart.html
   # Docker image to use during pipeline execution
   image: ~
 """.strip()
 
 # This auto-validates the template above during import
-_CONFIG_TEMPLATE = KedroAzureMLConfig.parse_obj(yaml.safe_load(CONFIG_TEMPLATE_YAML))
+_CONFIG_TEMPLATE = KedroAzureMLConfig.parse_obj(
+    update_dict(
+        yaml.safe_load(CONFIG_TEMPLATE_YAML),
+        ("azure.pipeline_data_passing.enabled", False),
+        ("azure.temporary_storage.container", ""),
+        ("azure.temporary_storage.account_name", ""),
+    )
+)
```

### Comparing `kedro_azureml-0.3.6/kedro_azureml/datasets/file_dataset.py` & `kedro_azureml-0.4.0/kedro_azureml/datasets/file_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         abstract_dataset.abstractdataset?view=azure-ml-py#azureml-data-abstract-dataset-abstractdataset-register
     .. _`azureml.core.Dataset.get_by_name`: https://learn.microsoft.com/en-us/python/api/azureml-core/azureml.core.
         dataset.dataset?view=azure-ml-py#azureml-core-dataset-dataset-get-by-name
 
     Example
     -------
 
-    Example of a catalog.yml enry:
+    Example of a catalog.yml entry:
 
     .. code-block:: yaml
 
         processed_images:
           type: kedro_azureml.datasets.AzureMLFileDataSet
           dataset: pillow.ImageDataSet
           filename_suffix: '.png'
```

### Comparing `kedro_azureml-0.3.6/kedro_azureml/datasets/pandas_dataset.py` & `kedro_azureml-0.4.0/kedro_azureml/datasets/pandas_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.3.6/kedro_azureml/datasets/runner_dataset.py` & `kedro_azureml-0.4.0/kedro_azureml/datasets/runner_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.3.6/kedro_azureml/datasets/utils.py` & `kedro_azureml-0.4.0/kedro_azureml/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.3.6/kedro_azureml/distributed/decorators.py` & `kedro_azureml-0.4.0/kedro_azureml/distributed/decorators.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.3.6/kedro_azureml/distributed/utils.py` & `kedro_azureml-0.4.0/kedro_azureml/distributed/utils.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.3.6/kedro_azureml/generator.py` & `kedro_azureml-0.4.0/kedro_azureml/generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -169,39 +169,46 @@
         self,
         pipeline: Pipeline,
         node: Node,
         kedro_azure_run_id: str,
     ):
         command_kwargs = {}
         command_kwargs.update(self._get_distributed_azure_command_kwargs(node))
+        pipeline_data_passing = (
+            self.config.azure.pipeline_data_passing is not None
+            and self.config.azure.pipeline_data_passing.enabled
+        )
 
         return command(
             name=self._sanitize_azure_name(node.name),
             display_name=node.name,
-            command=self._prepare_command(node),
+            command=self._prepare_command(node, pipeline),
             compute=self.get_target_resource_from_node_tags(node).cluster_name,
             environment_variables={
                 KEDRO_AZURE_RUNNER_CONFIG: KedroAzureRunnerConfig(
                     temporary_storage=self.config.azure.temporary_storage,
                     run_id=kedro_azure_run_id,
                     storage_account_key=self.storage_account_key,
-                ).json(),
+                ).json()
+                if not pipeline_data_passing
+                else "",
                 **self.extra_env,
             },
             environment=self._resolve_azure_environment(),  # TODO: check whether Environment exists
             inputs={
                 self._sanitize_param_name(name): (
                     Input(type="string") if name in pipeline.inputs() else Input()
                 )
                 for name in node.inputs
             },
             outputs={
                 self._sanitize_param_name(name): Output() for name in node.outputs
             },
             code=self.config.azure.code_directory,
+            is_deterministic=False,  # TODO: allow setting this to true per node (e.g. by tags as for resources)
             **command_kwargs,
         )
 
     def _get_distributed_azure_command_kwargs(self, node) -> dict:
         azure_command_kwargs = {}
         if hasattr(node.func, DISTRIBUTED_CONFIG_FIELD) and isinstance(
             distributed_config := getattr(node.func, DISTRIBUTED_CONFIG_FIELD),
@@ -280,27 +287,42 @@
                     azure_inputs[sanitized_input_name] = azure_output
                 else:
                     # 2. if not found, provide dummy input
                     azure_inputs[sanitized_input_name] = node_input
             invoked_components[node.name] = commands[node.name](**azure_inputs)
         return invoked_components
 
-    def _prepare_command(self, node):
-        azure_outputs = (
+    def _prepare_command(self, node, pipeline):
+        input_data_paths = (
+            [
+                f"--az-input={name} "
+                + "${{inputs."
+                + self._sanitize_param_name(name)
+                + "}}"
+                for name in node.inputs
+                if not name.startswith("params:") and name not in pipeline.inputs()
+            ]
+            if node.inputs
+            else []
+        )
+        output_data_paths = (
             [
-                "--az-output=${{outputs." + self._sanitize_param_name(name) + "}}"
+                f"--az-output={name} "
+                + "${{outputs."
+                + self._sanitize_param_name(name)
+                + "}}"
                 for name in node.outputs
             ]
             if node.outputs
             else []
         )
         return (
             (
                 f"cd {self.config.azure.working_directory} && "
                 if self.config.azure.working_directory is not None
                 and self.config.azure.code_directory is None
                 else ""
             )
             + f"kedro azureml -e {self.kedro_environment} execute --pipeline={self.pipeline_name} --node={node.name} "  # noqa
-            + " ".join(azure_outputs)
+            + " ".join(input_data_paths + output_data_paths)
             + (f" --params='{self.params}'" if self.params else "")
         ).strip()
```

### Comparing `kedro_azureml-0.3.6/kedro_azureml/runner.py` & `kedro_azureml-0.4.0/kedro_azureml/runner.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,89 @@
 import logging
 import os
-from typing import Any, Dict
+from pathlib import Path
+from typing import Any, Dict, Optional
 
+from kedro.extras.datasets.pickle import PickleDataSet
 from kedro.io import AbstractDataSet, DataCatalog
 from kedro.pipeline import Pipeline
 from kedro.runner import SequentialRunner
 from pluggy import PluginManager
 
 from kedro_azureml.config import KedroAzureRunnerConfig
 from kedro_azureml.constants import KEDRO_AZURE_RUNNER_CONFIG
 from kedro_azureml.datasets import (
+    AzureMLPipelineDataSet,
     KedroAzureRunnerDataset,
     KedroAzureRunnerDistributedDataset,
 )
 from kedro_azureml.distributed.utils import is_distributed_environment
 
 logger = logging.getLogger(__name__)
 
 
 class AzurePipelinesRunner(SequentialRunner):
-    def __init__(self, is_async: bool = False):
+    def __init__(
+        self,
+        is_async: bool = False,
+        data_paths: Optional[Dict[str, str]] = None,
+        pipeline_data_passing: bool = False,
+    ):
         super().__init__(is_async)
+        self.pipeline_data_passing = pipeline_data_passing
         self.runner_config_raw = os.environ.get(KEDRO_AZURE_RUNNER_CONFIG)
-        self.runner_config: KedroAzureRunnerConfig = KedroAzureRunnerConfig.parse_raw(
-            self.runner_config_raw
+        self.runner_config: KedroAzureRunnerConfig = (
+            KedroAzureRunnerConfig.parse_raw(self.runner_config_raw)
+            if not self.pipeline_data_passing
+            else None
         )
+        self.data_paths = data_paths if data_paths is not None else {}
 
     def run(
         self,
         pipeline: Pipeline,
         catalog: DataCatalog,
         hook_manager: PluginManager = None,
         session_id: str = None,
     ) -> Dict[str, Any]:
+        catalog = catalog.shallow_copy()
+        catalog_set = set(catalog.list())
+
+        # Loop over datasets in arguments to set their paths
+        for ds_name, azure_dataset_folder in self.data_paths.items():
+            if ds_name in catalog_set:
+                ds = catalog._get_dataset(ds_name)
+                if isinstance(ds, AzureMLPipelineDataSet):
+                    file_name = Path(ds.path).name
+                    ds.path = str(Path(azure_dataset_folder) / file_name)
+                    catalog.add(ds_name, ds, replace=True)
+            else:
+                catalog.add(ds_name, self.create_default_data_set(ds_name))
+
+        # Loop over remaining input datasets to add them to the catalog
         unsatisfied = pipeline.inputs() - set(catalog.list())
         for ds_name in unsatisfied:
-            catalog = catalog.shallow_copy()
             catalog.add(ds_name, self.create_default_data_set(ds_name))
 
         return super().run(pipeline, catalog, hook_manager, session_id)
 
     def create_default_data_set(self, ds_name: str) -> AbstractDataSet:
-        # TODO: handle credentials better (probably with built-in Kedro credentials
-        #  via ConfigLoader (but it's not available here...)
-        dataset_cls = KedroAzureRunnerDataset
-        if is_distributed_environment():
-            logger.info("Using distributed dataset class as a default")
-            dataset_cls = KedroAzureRunnerDistributedDataset
-
-        return dataset_cls(
-            self.runner_config.temporary_storage.account_name,
-            self.runner_config.temporary_storage.container,
-            self.runner_config.storage_account_key,
-            ds_name,
-            self.runner_config.run_id,
-        )
+        if self.pipeline_data_passing:
+            path = str(Path(self.data_paths[ds_name]) / f"{ds_name}.pickle")
+            return AzureMLPipelineDataSet(
+                {"type": PickleDataSet, "backend": "cloudpickle", "filepath": path}
+            )
+        else:
+            # TODO: handle credentials better (probably with built-in Kedro credentials
+            #  via ConfigLoader (but it's not available here...)
+            dataset_cls = KedroAzureRunnerDataset
+            if is_distributed_environment():
+                logger.info("Using distributed dataset class as a default")
+                dataset_cls = KedroAzureRunnerDistributedDataset
+
+            return dataset_cls(
+                self.runner_config.temporary_storage.account_name,
+                self.runner_config.temporary_storage.container,
+                self.runner_config.storage_account_key,
+                ds_name,
+                self.runner_config.run_id,
+            )
```

### Comparing `kedro_azureml-0.3.6/pyproject.toml` & `kedro_azureml-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kedro-azureml"
-version = "0.3.6"
+version = "0.4.0"
 description = "Kedro plugin with Azure ML Pipelines support"
 readme = "README.md"
 authors = ['marcin.zablocki <marcin.zablocki@getindata.com>']
 maintainers = ['GetInData MLOPS <mlops@getindata.com>']
 homepage = "https://github.com/getindata/kedro-azureml"
 repository = "https://github.com/getindata/kedro-azureml"
 documentation = "https://kedro-azureml.readthedocs.io/"
@@ -29,15 +29,15 @@
 ]
 
 [tool.isort]
 known_third_party = ["azure", "tabulate", "pydantic","semver","setuptools"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
-kedro = ">=0.18.2,<0.19"
+kedro = ">=0.18.5,<0.19.0"
 cloudpickle = "^2.1.0"
 adlfs = ">=2022.2.0"
 azure-ai-ml = ">=1.2.0"
 azureml-mlflow = { version = ">=1.42.0", optional = true}
 pydantic = "~=1.9.1"
 mlflow = {version = "^1.27.0", optional = true}
 backoff = "^2.2.1"
```

### Comparing `kedro_azureml-0.3.6/PKG-INFO` & `kedro_azureml-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-azureml
-Version: 0.3.6
+Version: 0.4.0
 Summary: Kedro plugin with Azure ML Pipelines support
 Home-page: https://github.com/getindata/kedro-azureml
 License: Apache-2.0
 Keywords: kedro,mlops,azureml,machinelearning
 Author: marcin.zablocki
 Author-email: marcin.zablocki@getindata.com
 Maintainer: GetInData MLOPS
@@ -21,15 +21,15 @@
 Requires-Dist: azure-ai-ml (>=1.2.0)
 Requires-Dist: azure-core (>=1.26.1)
 Requires-Dist: azureml-core (>=1.49.0,<2.0.0)
 Requires-Dist: azureml-dataset-runtime (>=1.49.0,<2.0.0)
 Requires-Dist: azureml-mlflow (>=1.42.0) ; extra == "mlflow"
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: cloudpickle (>=2.1.0,<3.0.0)
-Requires-Dist: kedro (>=0.18.2,<0.19)
+Requires-Dist: kedro (>=0.18.5,<0.19.0)
 Requires-Dist: mlflow (>=1.27.0,<2.0.0) ; extra == "mlflow"
 Requires-Dist: pydantic (>=1.9.1,<1.10.0)
 Project-URL: Documentation, https://kedro-azureml.readthedocs.io/
 Project-URL: Repository, https://github.com/getindata/kedro-azureml
 Description-Content-Type: text/markdown
 
 # Kedro Azure ML Pipelines plugin
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: kedro-azureml Version: 0.3.6 Summary: Kedro plugin
+Metadata-Version: 2.1 Name: kedro-azureml Version: 0.4.0 Summary: Kedro plugin
 with Azure ML Pipelines support Home-page: https://github.com/getindata/kedro-
 azureml License: Apache-2.0 Keywords: kedro,mlops,azureml,machinelearning
 Author: marcin.zablocki Author-email: marcin.zablocki@getindata.com Maintainer:
 GetInData MLOPS Maintainer-email: mlops@getindata.com Requires-Python:
 >=3.8,<3.11 Classifier: Development Status :: 4 - Beta Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Provides-Extra: mlflow Requires-Dist: adlfs (>=2022.2.0)
 Requires-Dist: azure-ai-ml (>=1.2.0) Requires-Dist: azure-core (>=1.26.1)
 Requires-Dist: azureml-core (>=1.49.0,<2.0.0) Requires-Dist: azureml-dataset-
 runtime (>=1.49.0,<2.0.0) Requires-Dist: azureml-mlflow (>=1.42.0) ; extra ==
 "mlflow" Requires-Dist: backoff (>=2.2.1,<3.0.0) Requires-Dist: cloudpickle
-(>=2.1.0,<3.0.0) Requires-Dist: kedro (>=0.18.2,<0.19) Requires-Dist: mlflow
+(>=2.1.0,<3.0.0) Requires-Dist: kedro (>=0.18.5,<0.19.0) Requires-Dist: mlflow
 (>=1.27.0,<2.0.0) ; extra == "mlflow" Requires-Dist: pydantic (>=1.9.1,<1.10.0)
 Project-URL: Documentation, https://kedro-azureml.readthedocs.io/ Project-URL:
 Repository, https://github.com/getindata/kedro-azureml Description-Content-
 Type: text/markdown # Kedro Azure ML Pipelines plugin [![Python Version](https:
 //img.shields.io/pypi/pyversions/kedro-azureml)](https://github.com/getindata/
 kedro-azureml) [![License](https://img.shields.io/badge/license-Apache%202.0-
 blue.svg)](https://opensource.org/licenses/Apache-2.0) [![SemVer](https://
```

