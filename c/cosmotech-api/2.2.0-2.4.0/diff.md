# Comparing `tmp/cosmotech-api-2.2.0.tar.gz` & `tmp/cosmotech-api-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmotech-api-2.2.0.tar", last modified: Tue Jan 31 14:39:26 2023, max compression
+gzip compressed data, was "cosmotech-api-2.4.0.tar", last modified: Fri Apr 28 10:11:17 2023, max compression
```

## Comparing `cosmotech-api-2.2.0.tar` & `cosmotech-api-2.4.0.tar`

### file list

```diff
@@ -1,190 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-31 14:39:26.517958 cosmotech-api-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (116)     1134 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      330 2023-01-31 14:39:26.517958 cosmotech-api-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    27440 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-31 14:39:26.497958 cosmotech-api-2.2.0/cosmotech_api/
--rw-r--r--   0 runner    (1001) docker     (116)      735 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-31 14:39:26.497958 cosmotech-api-2.2.0/cosmotech_api/api/
--rw-r--r--   0 runner    (1001) docker     (116)      219 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    19220 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/api/connector_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    48253 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/api/dataset_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    56639 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/api/organization_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    98829 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/api/scenario_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    76314 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/api/scenariorun_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    84055 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/api/solution_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    21972 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/api/twingraph_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    46561 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    48794 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/api/validator_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    76537 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/api/workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    37652 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-31 14:39:26.497958 cosmotech-api-2.2.0/cosmotech_api/apis/
--rw-r--r--   0 runner    (1001) docker     (116)      922 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    16757 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)     5065 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-31 14:39:26.505958 cosmotech-api-2.2.0/cosmotech_api/model/
--rw-r--r--   0 runner    (1001) docker     (116)      348 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    11279 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/component_role_permissions.py
--rw-r--r--   0 runner    (1001) docker     (116)    15381 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/connector.py
--rw-r--r--   0 runner    (1001) docker     (116)    12494 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/connector_parameter.py
--rw-r--r--   0 runner    (1001) docker     (116)    11969 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/connector_parameter_group.py
--rw-r--r--   0 runner    (1001) docker     (116)    11355 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/container_resource_size_info.py
--rw-r--r--   0 runner    (1001) docker     (116)    11688 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/container_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (116)    13602 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/dataset.py
--rw-r--r--   0 runner    (1001) docker     (116)    11971 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/dataset_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (116)    11775 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/dataset_connector.py
--rw-r--r--   0 runner    (1001) docker     (116)    11824 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/dataset_copy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11208 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/dataset_search.py
--rw-r--r--   0 runner    (1001) docker     (116)    12173 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/delete_historical_data.py
--rw-r--r--   0 runner    (1001) docker     (116)    12396 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/organization.py
--rw-r--r--   0 runner    (1001) docker     (116)    11294 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/organization_access_control.py
--rw-r--r--   0 runner    (1001) docker     (116)    11097 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/organization_role.py
--rw-r--r--   0 runner    (1001) docker     (116)    11958 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/organization_security.py
--rw-r--r--   0 runner    (1001) docker     (116)    12597 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/organization_service.py
--rw-r--r--   0 runner    (1001) docker     (116)    12276 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/organization_services.py
--rw-r--r--   0 runner    (1001) docker     (116)    11802 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/organization_user.py
--rw-r--r--   0 runner    (1001) docker     (116)    11328 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/resource_size_info.py
--rw-r--r--   0 runner    (1001) docker     (116)    22090 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/run_template.py
--rw-r--r--   0 runner    (1001) docker     (116)    12198 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/run_template_handler_id.py
--rw-r--r--   0 runner    (1001) docker     (116)    13434 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/run_template_parameter.py
--rw-r--r--   0 runner    (1001) docker     (116)    12789 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/run_template_parameter_group.py
--rw-r--r--   0 runner    (1001) docker     (116)    11734 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/run_template_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (116)    11603 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/run_template_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (116)    11851 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/run_template_step_source.py
--rw-r--r--   0 runner    (1001) docker     (116)    18826 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario.py
--rw-r--r--   0 runner    (1001) docker     (116)    11282 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario_access_control.py
--rw-r--r--   0 runner    (1001) docker     (116)    12166 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario_changed_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (116)    12324 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario_comparison_result.py
--rw-r--r--   0 runner    (1001) docker     (116)    11543 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario_data_download_info.py
--rw-r--r--   0 runner    (1001) docker     (116)    11145 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario_data_download_job.py
--rw-r--r--   0 runner    (1001) docker     (116)    12066 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario_job_state.py
--rw-r--r--   0 runner    (1001) docker     (116)    11972 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario_last_run.py
--rw-r--r--   0 runner    (1001) docker     (116)    11594 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (116)    11077 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario_role.py
--rw-r--r--   0 runner    (1001) docker     (116)    19377 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario_run.py
--rw-r--r--   0 runner    (1001) docker     (116)    14031 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario_run_container.py
--rw-r--r--   0 runner    (1001) docker     (116)    11368 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario_run_container_artifact.py
--rw-r--r--   0 runner    (1001) docker     (116)    12044 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario_run_container_logs.py
--rw-r--r--   0 runner    (1001) docker     (116)    11759 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario_run_logs.py
--rw-r--r--   0 runner    (1001) docker     (116)    13624 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario_run_search.py
--rw-r--r--   0 runner    (1001) docker     (116)    12672 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario_run_start_containers.py
--rw-r--r--   0 runner    (1001) docker     (116)    12184 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario_run_state.py
--rw-r--r--   0 runner    (1001) docker     (116)    14602 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario_run_status.py
--rw-r--r--   0 runner    (1001) docker     (116)    13659 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario_run_status_node.py
--rw-r--r--   0 runner    (1001) docker     (116)    12120 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario_run_template_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (116)    11910 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario_security.py
--rw-r--r--   0 runner    (1001) docker     (116)    11622 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario_user.py
--rw-r--r--   0 runner    (1001) docker     (116)    11892 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/scenario_validation_status.py
--rw-r--r--   0 runner    (1001) docker     (116)    15484 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/solution.py
--rw-r--r--   0 runner    (1001) docker     (116)    12113 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/source_info.py
--rw-r--r--   0 runner    (1001) docker     (116)    10785 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/translated_labels.py
--rw-r--r--   0 runner    (1001) docker     (116)    12027 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/twin_graph_import.py
--rw-r--r--   0 runner    (1001) docker     (116)    11316 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/twin_graph_import_info.py
--rw-r--r--   0 runner    (1001) docker     (116)    11349 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/twin_graph_query.py
--rw-r--r--   0 runner    (1001) docker     (116)    12206 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/user.py
--rw-r--r--   0 runner    (1001) docker     (116)    12067 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/user_organization.py
--rw-r--r--   0 runner    (1001) docker     (116)    11582 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/user_workspace.py
--rw-r--r--   0 runner    (1001) docker     (116)    13045 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/validator.py
--rw-r--r--   0 runner    (1001) docker     (116)    13298 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/validator_run.py
--rw-r--r--   0 runner    (1001) docker     (116)    18581 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/workspace.py
--rw-r--r--   0 runner    (1001) docker     (116)    11285 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/workspace_access_control.py
--rw-r--r--   0 runner    (1001) docker     (116)    11085 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/workspace_file.py
--rw-r--r--   0 runner    (1001) docker     (116)    11082 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/workspace_role.py
--rw-r--r--   0 runner    (1001) docker     (116)    11195 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/workspace_secret.py
--rw-r--r--   0 runner    (1001) docker     (116)    11922 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/workspace_security.py
--rw-r--r--   0 runner    (1001) docker     (116)    12147 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/workspace_solution.py
--rw-r--r--   0 runner    (1001) docker     (116)    11653 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/workspace_user.py
--rw-r--r--   0 runner    (1001) docker     (116)    12036 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model/workspace_web_app.py
--rw-r--r--   0 runner    (1001) docker     (116)    82070 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-31 14:39:26.505958 cosmotech-api-2.2.0/cosmotech_api/models/
--rw-r--r--   0 runner    (1001) docker     (116)     4024 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    14188 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/cosmotech_api/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-31 14:39:26.497958 cosmotech-api-2.2.0/cosmotech_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      330 2023-01-31 14:39:26.000000 cosmotech-api-2.2.0/cosmotech_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6562 2023-01-31 14:39:26.000000 cosmotech-api-2.2.0/cosmotech_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-01-31 14:39:26.000000 cosmotech-api-2.2.0/cosmotech_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       32 2023-01-31 14:39:26.000000 cosmotech-api-2.2.0/cosmotech_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2023-01-31 14:39:26.000000 cosmotech-api-2.2.0/cosmotech_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       69 2023-01-31 14:39:26.517958 cosmotech-api-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1014 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-31 14:39:26.517958 cosmotech-api-2.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (116)      817 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_component_role_permissions.py
--rw-r--r--   0 runner    (1001) docker     (116)      864 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_connector.py
--rw-r--r--   0 runner    (1001) docker     (116)     1209 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_connector_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      783 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_connector_parameter.py
--rw-r--r--   0 runner    (1001) docker     (116)      943 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_connector_parameter_group.py
--rw-r--r--   0 runner    (1001) docker     (116)      825 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_container_resource_size_info.py
--rw-r--r--   0 runner    (1001) docker     (116)      964 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_container_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (116)      953 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (116)     2144 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_dataset_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      797 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_dataset_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (116)      769 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_dataset_connector.py
--rw-r--r--   0 runner    (1001) docker     (116)      805 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_dataset_copy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      748 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_dataset_search.py
--rw-r--r--   0 runner    (1001) docker     (116)      798 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_delete_historical_data.py
--rw-r--r--   0 runner    (1001) docker     (116)      988 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_organization.py
--rw-r--r--   0 runner    (1001) docker     (116)      824 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_organization_access_control.py
--rw-r--r--   0 runner    (1001) docker     (116)     2809 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_organization_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      760 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_organization_role.py
--rw-r--r--   0 runner    (1001) docker     (116)      941 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_organization_security.py
--rw-r--r--   0 runner    (1001) docker     (116)      790 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_organization_service.py
--rw-r--r--   0 runner    (1001) docker     (116)      925 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_organization_services.py
--rw-r--r--   0 runner    (1001) docker     (116)      769 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_organization_user.py
--rw-r--r--   0 runner    (1001) docker     (116)      761 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_resource_size_info.py
--rw-r--r--   0 runner    (1001) docker     (116)     1005 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_run_template.py
--rw-r--r--   0 runner    (1001) docker     (116)      799 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_run_template_handler_id.py
--rw-r--r--   0 runner    (1001) docker     (116)      914 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_run_template_parameter.py
--rw-r--r--   0 runner    (1001) docker     (116)      950 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_run_template_parameter_group.py
--rw-r--r--   0 runner    (1001) docker     (116)      834 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_run_template_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (116)      942 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_run_template_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (116)      806 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_run_template_step_source.py
--rw-r--r--   0 runner    (1001) docker     (116)     1378 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (116)      796 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_access_control.py
--rw-r--r--   0 runner    (1001) docker     (116)     3711 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      862 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_changed_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (116)      996 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_comparison_result.py
--rw-r--r--   0 runner    (1001) docker     (116)      944 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_data_download_info.py
--rw-r--r--   0 runner    (1001) docker     (116)      820 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_data_download_job.py
--rw-r--r--   0 runner    (1001) docker     (116)      770 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_job_state.py
--rw-r--r--   0 runner    (1001) docker     (116)      763 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_last_run.py
--rw-r--r--   0 runner    (1001) docker     (116)      920 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_resource_sizing.py
--rw-r--r--   0 runner    (1001) docker     (116)      732 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_role.py
--rw-r--r--   0 runner    (1001) docker     (116)     1138 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_run.py
--rw-r--r--   0 runner    (1001) docker     (116)      964 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_run_container.py
--rw-r--r--   0 runner    (1001) docker     (116)      855 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_run_container_artifact.py
--rw-r--r--   0 runner    (1001) docker     (116)      827 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_run_container_logs.py
--rw-r--r--   0 runner    (1001) docker     (116)      913 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_run_logs.py
--rw-r--r--   0 runner    (1001) docker     (116)      777 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_run_search.py
--rw-r--r--   0 runner    (1001) docker     (116)      974 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_run_start_containers.py
--rw-r--r--   0 runner    (1001) docker     (116)      770 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_run_state.py
--rw-r--r--   0 runner    (1001) docker     (116)     1032 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_run_status.py
--rw-r--r--   0 runner    (1001) docker     (116)      806 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_run_status_node.py
--rw-r--r--   0 runner    (1001) docker     (116)      891 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_run_template_parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (116)      897 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_security.py
--rw-r--r--   0 runner    (1001) docker     (116)      741 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_user.py
--rw-r--r--   0 runner    (1001) docker     (116)      826 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenario_validation_status.py
--rw-r--r--   0 runner    (1001) docker     (116)     3159 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_scenariorun_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1095 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_solution.py
--rw-r--r--   0 runner    (1001) docker     (116)     3382 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_solution_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      718 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_source_info.py
--rw-r--r--   0 runner    (1001) docker     (116)      769 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_translated_labels.py
--rw-r--r--   0 runner    (1001) docker     (116)      846 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_twin_graph_import.py
--rw-r--r--   0 runner    (1001) docker     (116)      783 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_twin_graph_import_info.py
--rw-r--r--   0 runner    (1001) docker     (116)      747 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_twin_graph_query.py
--rw-r--r--   0 runner    (1001) docker     (116)      925 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_twingraph_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      800 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_user.py
--rw-r--r--   0 runner    (1001) docker     (116)     2197 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      873 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_user_organization.py
--rw-r--r--   0 runner    (1001) docker     (116)      748 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_user_workspace.py
--rw-r--r--   0 runner    (1001) docker     (116)      719 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (116)     2000 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_validator_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      741 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_validator_run.py
--rw-r--r--   0 runner    (1001) docker     (116)     1056 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_workspace.py
--rw-r--r--   0 runner    (1001) docker     (116)      803 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_workspace_access_control.py
--rw-r--r--   0 runner    (1001) docker     (116)     3027 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      748 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_workspace_file.py
--rw-r--r--   0 runner    (1001) docker     (116)      739 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_workspace_role.py
--rw-r--r--   0 runner    (1001) docker     (116)      762 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_workspace_secret.py
--rw-r--r--   0 runner    (1001) docker     (116)      908 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_workspace_security.py
--rw-r--r--   0 runner    (1001) docker     (116)      776 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_workspace_solution.py
--rw-r--r--   0 runner    (1001) docker     (116)      748 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_workspace_user.py
--rw-r--r--   0 runner    (1001) docker     (116)      763 2023-01-31 14:39:12.000000 cosmotech-api-2.2.0/test/test_workspace_web_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:11:17.129549 cosmotech-api-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-28 10:11:17.129549 cosmotech-api-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34207 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:11:17.105549 cosmotech-api-2.4.0/cosmotech_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:11:17.109549 cosmotech-api-2.4.0/cosmotech_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24319 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api/connector_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54204 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api/dataset_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92962 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api/organization_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135364 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api/scenario_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83623 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api/scenariorun_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89623 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api/solution_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84630 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api/twingraph_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46553 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48790 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api/validator_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110590 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api/workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37648 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:11:17.109549 cosmotech-api-2.4.0/cosmotech_api/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16748 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:11:17.117549 cosmotech-api-2.4.0/cosmotech_api/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/component_role_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15377 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12490 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/connector_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/connector_parameter_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/container_resource_size_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/container_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14173 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/dataset_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/dataset_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/dataset_copy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/dataset_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/delete_historical_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/graph_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12549 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/organization_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/organization_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11963 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/organization_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/organization_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/organization_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/organization_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/resource_size_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22521 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/run_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12194 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/run_template_handler_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/run_template_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/run_template_parameter_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/run_template_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/run_template_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11847 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/run_template_step_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19743 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12162 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_changed_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_comparison_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_data_download_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_data_download_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_job_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_last_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11082 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_container_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_container_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13620 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_start_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14598 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_status_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_template_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11915 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/scenario_validation_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15825 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12118 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/source_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/translated_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/twin_graph_batch_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/twin_graph_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/twin_graph_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/twin_graph_import_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/twin_graph_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/user_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11574 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/user_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13041 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/validator_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19012 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11290 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/workspace_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/workspace_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/workspace_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11191 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/workspace_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/workspace_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/workspace_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/workspace_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-04-28 10:11:07.000000 cosmotech-api-2.4.0/cosmotech_api/model/workspace_web_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82066 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/cosmotech_api/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:11:17.117549 cosmotech-api-2.4.0/cosmotech_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/cosmotech_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14184 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/cosmotech_api/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:11:17.105549 cosmotech-api-2.4.0/cosmotech_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-28 10:11:17.000000 cosmotech-api-2.4.0/cosmotech_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-28 10:11:17.000000 cosmotech-api-2.4.0/cosmotech_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 10:11:17.000000 cosmotech-api-2.4.0/cosmotech_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 10:11:17.000000 cosmotech-api-2.4.0/cosmotech_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-28 10:11:17.000000 cosmotech-api-2.4.0/cosmotech_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-28 10:11:17.129549 cosmotech-api-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:11:17.129549 cosmotech-api-2.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_component_role_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_connector_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_connector_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_connector_parameter_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_container_resource_size_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_container_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_dataset_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_dataset_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_dataset_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_dataset_copy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_dataset_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_delete_historical_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_graph_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_organization_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_organization_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_organization_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_organization_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_organization_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_organization_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_organization_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_resource_size_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_run_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_run_template_handler_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_run_template_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_run_template_parameter_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_run_template_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_run_template_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_run_template_step_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_changed_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_comparison_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_data_download_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_data_download_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_job_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_last_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_resource_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_run_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_run_container_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_run_container_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_run_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_run_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_run_start_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_run_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_run_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_run_status_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_run_template_parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenario_validation_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_scenariorun_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_solution_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_source_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_translated_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_twin_graph_batch_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_twin_graph_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_twin_graph_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_twin_graph_import_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_twin_graph_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_twingraph_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_user_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_user_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_validator_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_validator_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_workspace_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_workspace_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_workspace_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_workspace_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_workspace_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_workspace_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_workspace_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-28 10:11:08.000000 cosmotech-api-2.4.0/test/test_workspace_web_app.py
```

### Comparing `cosmotech-api-2.2.0/LICENSE` & `cosmotech-api-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmotech-api-2.2.0/README.md` & `cosmotech-api-2.4.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # cosmotech-api
 Cosmo Tech Platform API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.1.3-SNAPSHOT
+- API version: 2.4.0-dev
 - Package version: 1.0.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://github.com/Cosmo-Tech/cosmotech-api](https://github.com/Cosmo-Tech/cosmotech-api)
 
 ## Requirements.
 
 Python >=3.6
@@ -70,187 +70,233 @@
 configuration.access_token = 'YOUR_ACCESS_TOKEN'
 
 
 # Enter a context with an instance of the API client
 with cosmotech_api.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = connector_api.ConnectorApi(api_client)
-    
+    page = 1 # int | page number to query (optional)
+size = 1 # int | amount of result by page (optional)
+
     try:
         # List all Connectors
-        api_response = api_instance.find_all_connectors()
+        api_response = api_instance.find_all_connectors(page=page, size=size)
         pprint(api_response)
     except cosmotech_api.ApiException as e:
         print("Exception when calling ConnectorApi->find_all_connectors: %s\n" % e)
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://dev.api.cosmotech.com*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *ConnectorApi* | [**find_all_connectors**](docs/ConnectorApi.md#find_all_connectors) | **GET** /connectors | List all Connectors
 *ConnectorApi* | [**find_connector_by_id**](docs/ConnectorApi.md#find_connector_by_id) | **GET** /connectors/{connector_id} | Get the details of a connector
+*ConnectorApi* | [**import_connector**](docs/ConnectorApi.md#import_connector) | **POST** /connectors/import | Import existing connector
 *ConnectorApi* | [**register_connector**](docs/ConnectorApi.md#register_connector) | **POST** /connectors | Register a new connector
 *ConnectorApi* | [**unregister_connector**](docs/ConnectorApi.md#unregister_connector) | **DELETE** /connectors/{connector_id} | Unregister a connector
 *DatasetApi* | [**add_or_replace_dataset_compatibility_elements**](docs/DatasetApi.md#add_or_replace_dataset_compatibility_elements) | **POST** /organizations/{organization_id}/datasets/{dataset_id}/compatibility | Add Dataset Compatibility elements.
 *DatasetApi* | [**copy_dataset**](docs/DatasetApi.md#copy_dataset) | **POST** /organizations/{organization_id}/datasets/copy | Copy a Dataset to another Dataset. Source must have a read capable connector and Target a write capable connector.
 *DatasetApi* | [**create_dataset**](docs/DatasetApi.md#create_dataset) | **POST** /organizations/{organization_id}/datasets | Create a new Dataset
 *DatasetApi* | [**delete_dataset**](docs/DatasetApi.md#delete_dataset) | **DELETE** /organizations/{organization_id}/datasets/{dataset_id} | Delete a dataset
 *DatasetApi* | [**find_all_datasets**](docs/DatasetApi.md#find_all_datasets) | **GET** /organizations/{organization_id}/datasets | List all Datasets
 *DatasetApi* | [**find_dataset_by_id**](docs/DatasetApi.md#find_dataset_by_id) | **GET** /organizations/{organization_id}/datasets/{dataset_id} | Get the details of a Dataset
+*DatasetApi* | [**import_dataset**](docs/DatasetApi.md#import_dataset) | **POST** /organizations/{organization_id}/datasets/import | Import a new Dataset
 *DatasetApi* | [**remove_all_dataset_compatibility_elements**](docs/DatasetApi.md#remove_all_dataset_compatibility_elements) | **DELETE** /organizations/{organization_id}/datasets/{dataset_id}/compatibility | Remove all Dataset Compatibility elements from the Dataset specified
 *DatasetApi* | [**search_datasets**](docs/DatasetApi.md#search_datasets) | **POST** /organizations/{organization_id}/datasets/search | Search Datasets
 *DatasetApi* | [**update_dataset**](docs/DatasetApi.md#update_dataset) | **PATCH** /organizations/{organization_id}/datasets/{dataset_id} | Update a dataset
-*OrganizationApi* | [**add_or_replace_users_in_organization**](docs/OrganizationApi.md#add_or_replace_users_in_organization) | **POST** /organizations/{organization_id}/users | Add (or replace) users in the Organization specified
+*OrganizationApi* | [**add_organization_access_control**](docs/OrganizationApi.md#add_organization_access_control) | **POST** /organizations/{organization_id}/security/access | Add a control access to the Organization
 *OrganizationApi* | [**find_all_organizations**](docs/OrganizationApi.md#find_all_organizations) | **GET** /organizations | List all Organizations
 *OrganizationApi* | [**find_organization_by_id**](docs/OrganizationApi.md#find_organization_by_id) | **GET** /organizations/{organization_id} | Get the details of an Organization
+*OrganizationApi* | [**get_all_permissions**](docs/OrganizationApi.md#get_all_permissions) | **GET** /organizations/permissions | Get all permissions per components
+*OrganizationApi* | [**get_organization_access_control**](docs/OrganizationApi.md#get_organization_access_control) | **GET** /organizations/{organization_id}/security/access/{identity_id} | Get a control access for the Organization
+*OrganizationApi* | [**get_organization_permissions**](docs/OrganizationApi.md#get_organization_permissions) | **GET** /organizations/{organization_id}/permissions/{role} | Get the Organization permissions by given role
+*OrganizationApi* | [**get_organization_security**](docs/OrganizationApi.md#get_organization_security) | **GET** /organizations/{organization_id}/security | Get the Organization security information
+*OrganizationApi* | [**get_organization_security_users**](docs/OrganizationApi.md#get_organization_security_users) | **GET** /organizations/{organization_id}/security/users | Get the Organization security users list
+*OrganizationApi* | [**import_organization**](docs/OrganizationApi.md#import_organization) | **POST** /organizations/import | Import an organization
 *OrganizationApi* | [**register_organization**](docs/OrganizationApi.md#register_organization) | **POST** /organizations | Register a new organization
-*OrganizationApi* | [**remove_all_users_in_organization**](docs/OrganizationApi.md#remove_all_users_in_organization) | **DELETE** /organizations/{organization_id}/users | Remove all users from the Organization specified
-*OrganizationApi* | [**remove_user_from_organization**](docs/OrganizationApi.md#remove_user_from_organization) | **DELETE** /organizations/{organization_id}/users/{user_id} | Remove the specified user from the given Organization
+*OrganizationApi* | [**remove_organization_access_control**](docs/OrganizationApi.md#remove_organization_access_control) | **DELETE** /organizations/{organization_id}/security/access/{identity_id} | Remove the specified access from the given Organization
+*OrganizationApi* | [**set_organization_default_security**](docs/OrganizationApi.md#set_organization_default_security) | **POST** /organizations/{organization_id}/security/default | Set the Organization default security
 *OrganizationApi* | [**unregister_organization**](docs/OrganizationApi.md#unregister_organization) | **DELETE** /organizations/{organization_id} | Unregister an organization
 *OrganizationApi* | [**update_organization**](docs/OrganizationApi.md#update_organization) | **PATCH** /organizations/{organization_id} | Update an Organization
+*OrganizationApi* | [**update_organization_access_control**](docs/OrganizationApi.md#update_organization_access_control) | **PATCH** /organizations/{organization_id}/security/access/{identity_id} | Update the specified access to User for an Organization
 *OrganizationApi* | [**update_solutions_container_registry_by_organization_id**](docs/OrganizationApi.md#update_solutions_container_registry_by_organization_id) | **PATCH** /organizations/{organization_id}/services/solutionsContainerRegistry | Update the solutions container registry configuration for the Organization specified
 *OrganizationApi* | [**update_storage_by_organization_id**](docs/OrganizationApi.md#update_storage_by_organization_id) | **PATCH** /organizations/{organization_id}/services/storage | Update storage configuration for the Organization specified
 *OrganizationApi* | [**update_tenant_credentials_by_organization_id**](docs/OrganizationApi.md#update_tenant_credentials_by_organization_id) | **PATCH** /organizations/{organization_id}/services/tenantCredentials | Update tenant credentials for the Organization specified
 *ScenarioApi* | [**add_or_replace_scenario_parameter_values**](docs/ScenarioApi.md#add_or_replace_scenario_parameter_values) | **POST** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/parameterValues | Add (or replace) Parameter Values for the Scenario specified
-*ScenarioApi* | [**add_or_replace_users_in_scenario**](docs/ScenarioApi.md#add_or_replace_users_in_scenario) | **POST** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/users | Add (or replace) users in the Scenario specified
+*ScenarioApi* | [**add_scenario_access_control**](docs/ScenarioApi.md#add_scenario_access_control) | **POST** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/security/access | Add a control access to the Scenario
 *ScenarioApi* | [**compare_scenarios**](docs/ScenarioApi.md#compare_scenarios) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/compare/{compared_scenario_id} | Compare the Scenario with another one and returns the difference for parameters values
 *ScenarioApi* | [**create_scenario**](docs/ScenarioApi.md#create_scenario) | **POST** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios | Create a new Scenario
 *ScenarioApi* | [**delete_all_scenarios**](docs/ScenarioApi.md#delete_all_scenarios) | **DELETE** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios | Delete all Scenarios of the Workspace
 *ScenarioApi* | [**delete_scenario**](docs/ScenarioApi.md#delete_scenario) | **DELETE** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id} | Delete a scenario
 *ScenarioApi* | [**download_scenario_data**](docs/ScenarioApi.md#download_scenario_data) | **POST** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/downloads | Download Scenario data
 *ScenarioApi* | [**find_all_scenarios**](docs/ScenarioApi.md#find_all_scenarios) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios | List all Scenarios
 *ScenarioApi* | [**find_all_scenarios_by_validation_status**](docs/ScenarioApi.md#find_all_scenarios_by_validation_status) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/{validationStatus} | List all Scenarios by validation status
 *ScenarioApi* | [**find_scenario_by_id**](docs/ScenarioApi.md#find_scenario_by_id) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id} | Get the details of an scenario
+*ScenarioApi* | [**get_scenario_access_control**](docs/ScenarioApi.md#get_scenario_access_control) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/security/access/{identity_id} | Get a control access for the Scenario
 *ScenarioApi* | [**get_scenario_data_download_job_info**](docs/ScenarioApi.md#get_scenario_data_download_job_info) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/downloads/{download_id} | Get Scenario data download URL
+*ScenarioApi* | [**get_scenario_permissions**](docs/ScenarioApi.md#get_scenario_permissions) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/permissions/{role} | Get the Scenario permission by given role
+*ScenarioApi* | [**get_scenario_security**](docs/ScenarioApi.md#get_scenario_security) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/security | Get the Scenario security information
+*ScenarioApi* | [**get_scenario_security_users**](docs/ScenarioApi.md#get_scenario_security_users) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/security/users | Get the Scenario security users list
 *ScenarioApi* | [**get_scenario_validation_status_by_id**](docs/ScenarioApi.md#get_scenario_validation_status_by_id) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/ValidationStatus | Get the validation status of an scenario
 *ScenarioApi* | [**get_scenarios_tree**](docs/ScenarioApi.md#get_scenarios_tree) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/tree | Get the Scenarios Tree
+*ScenarioApi* | [**import_scenario**](docs/ScenarioApi.md#import_scenario) | **POST** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/import | Import Scenario
 *ScenarioApi* | [**remove_all_scenario_parameter_values**](docs/ScenarioApi.md#remove_all_scenario_parameter_values) | **DELETE** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/parameterValues | Remove all Parameter Values from the Scenario specified
-*ScenarioApi* | [**remove_all_users_of_scenario**](docs/ScenarioApi.md#remove_all_users_of_scenario) | **DELETE** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/users | Remove all users from the Scenario specified
-*ScenarioApi* | [**remove_user_from_scenario**](docs/ScenarioApi.md#remove_user_from_scenario) | **DELETE** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/users/{user_id} | Remove the specified user from the given Scenario
+*ScenarioApi* | [**remove_scenario_access_control**](docs/ScenarioApi.md#remove_scenario_access_control) | **DELETE** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/security/access/{identity_id} | Remove the specified access from the given Organization Scenario
+*ScenarioApi* | [**set_scenario_default_security**](docs/ScenarioApi.md#set_scenario_default_security) | **POST** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/security/default | Set the Scenario default security
 *ScenarioApi* | [**update_scenario**](docs/ScenarioApi.md#update_scenario) | **PATCH** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id} | Update a scenario
+*ScenarioApi* | [**update_scenario_access_control**](docs/ScenarioApi.md#update_scenario_access_control) | **PATCH** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/security/access/{identity_id} | Update the specified access to User for a Scenario
 *ScenariorunApi* | [**delete_historical_data_organization**](docs/ScenariorunApi.md#delete_historical_data_organization) | **DELETE** /organizations/{organization_id}/scenarioruns/historicaldata | Delete all historical ScenarioRuns in the Organization
 *ScenariorunApi* | [**delete_historical_data_scenario**](docs/ScenariorunApi.md#delete_historical_data_scenario) | **DELETE** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/scenarioruns/historicaldata | Delete all historical ScenarioRuns in the Scenario
 *ScenariorunApi* | [**delete_historical_data_workspace**](docs/ScenariorunApi.md#delete_historical_data_workspace) | **DELETE** /organizations/{organization_id}/workspaces/{workspace_id}/scenarioruns/historicaldata | Delete all historical ScenarioRuns in the Workspace
 *ScenariorunApi* | [**delete_scenario_run**](docs/ScenariorunApi.md#delete_scenario_run) | **DELETE** /organizations/{organization_id}/scenarioruns/{scenariorun_id} | Delete a scenariorun
 *ScenariorunApi* | [**find_scenario_run_by_id**](docs/ScenariorunApi.md#find_scenario_run_by_id) | **GET** /organizations/{organization_id}/scenarioruns/{scenariorun_id} | Get the details of a scenariorun
 *ScenariorunApi* | [**get_scenario_run_cumulated_logs**](docs/ScenariorunApi.md#get_scenario_run_cumulated_logs) | **GET** /organizations/{organization_id}/scenarioruns/{scenariorun_id}/cumulatedlogs | Get the cumulated logs of a scenariorun
 *ScenariorunApi* | [**get_scenario_run_logs**](docs/ScenariorunApi.md#get_scenario_run_logs) | **GET** /organizations/{organization_id}/scenarioruns/{scenariorun_id}/logs | get the logs for the ScenarioRun
 *ScenariorunApi* | [**get_scenario_run_status**](docs/ScenariorunApi.md#get_scenario_run_status) | **GET** /organizations/{organization_id}/scenarioruns/{scenariorun_id}/status | get the status for the ScenarioRun
 *ScenariorunApi* | [**get_scenario_runs**](docs/ScenariorunApi.md#get_scenario_runs) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/scenarioruns | get the list of ScenarioRuns for the Scenario
 *ScenariorunApi* | [**get_workspace_scenario_runs**](docs/ScenariorunApi.md#get_workspace_scenario_runs) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/scenarioruns | get the list of ScenarioRuns for the Workspace
+*ScenariorunApi* | [**import_scenario_run**](docs/ScenariorunApi.md#import_scenario_run) | **POST** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/run/import | import a ScenarioRun for the Scenario
 *ScenariorunApi* | [**run_scenario**](docs/ScenariorunApi.md#run_scenario) | **POST** /organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/run | run a ScenarioRun for the Scenario
 *ScenariorunApi* | [**search_scenario_runs**](docs/ScenariorunApi.md#search_scenario_runs) | **POST** /organizations/{organization_id}/scenarioruns/search | Search ScenarioRuns
 *ScenariorunApi* | [**start_scenario_run_containers**](docs/ScenariorunApi.md#start_scenario_run_containers) | **POST** /organizations/{organization_id}/scenarioruns/startcontainers | Start a new scenariorun with raw containers definition
 *ScenariorunApi* | [**stop_scenario_run**](docs/ScenariorunApi.md#stop_scenario_run) | **POST** /organizations/{organization_id}/scenarioruns/{scenariorun_id}/stop | stop a ScenarioRun for the Scenario
 *SolutionApi* | [**add_or_replace_parameter_groups**](docs/SolutionApi.md#add_or_replace_parameter_groups) | **POST** /organizations/{organization_id}/solutions/{solution_id}/parameterGroups | Add Parameter Groups. Any item with the same ID will be overwritten
 *SolutionApi* | [**add_or_replace_parameters**](docs/SolutionApi.md#add_or_replace_parameters) | **POST** /organizations/{organization_id}/solutions/{solution_id}/parameters | Add Parameters. Any item with the same ID will be overwritten
 *SolutionApi* | [**add_or_replace_run_templates**](docs/SolutionApi.md#add_or_replace_run_templates) | **POST** /organizations/{organization_id}/solutions/{solution_id}/runTemplates | Add Run Templates. Any item with the same ID will be overwritten
 *SolutionApi* | [**create_solution**](docs/SolutionApi.md#create_solution) | **POST** /organizations/{organization_id}/solutions | Register a new solution
 *SolutionApi* | [**delete_solution**](docs/SolutionApi.md#delete_solution) | **DELETE** /organizations/{organization_id}/solutions/{solution_id} | Delete a solution
 *SolutionApi* | [**delete_solution_run_template**](docs/SolutionApi.md#delete_solution_run_template) | **DELETE** /organizations/{organization_id}/solutions/{solution_id}/runTemplates/{run_template_id} | Remove the specified Solution Run Template
 *SolutionApi* | [**download_run_template_handler**](docs/SolutionApi.md#download_run_template_handler) | **GET** /organizations/{organization_id}/solutions/{solution_id}/runtemplates/{run_template_id}/handlers/{handler_id}/download | Download a Run Template step handler zip file
 *SolutionApi* | [**find_all_solutions**](docs/SolutionApi.md#find_all_solutions) | **GET** /organizations/{organization_id}/solutions | List all Solutions
 *SolutionApi* | [**find_solution_by_id**](docs/SolutionApi.md#find_solution_by_id) | **GET** /organizations/{organization_id}/solutions/{solution_id} | Get the details of a solution
+*SolutionApi* | [**import_solution**](docs/SolutionApi.md#import_solution) | **POST** /organizations/{organization_id}/solutions/import | Import a solution
 *SolutionApi* | [**remove_all_run_templates**](docs/SolutionApi.md#remove_all_run_templates) | **DELETE** /organizations/{organization_id}/solutions/{solution_id}/runTemplates | Remove all Run Templates from the Solution specified
 *SolutionApi* | [**remove_all_solution_parameter_groups**](docs/SolutionApi.md#remove_all_solution_parameter_groups) | **DELETE** /organizations/{organization_id}/solutions/{solution_id}/parameterGroups | Remove all Parameter Groups from the Solution specified
 *SolutionApi* | [**remove_all_solution_parameters**](docs/SolutionApi.md#remove_all_solution_parameters) | **DELETE** /organizations/{organization_id}/solutions/{solution_id}/parameters | Remove all Parameters from the Solution specified
 *SolutionApi* | [**update_solution**](docs/SolutionApi.md#update_solution) | **PATCH** /organizations/{organization_id}/solutions/{solution_id} | Update a solution
 *SolutionApi* | [**update_solution_run_template**](docs/SolutionApi.md#update_solution_run_template) | **PATCH** /organizations/{organization_id}/solutions/{solution_id}/runTemplates/{run_template_id} | Update the specified Solution Run Template
 *SolutionApi* | [**upload_run_template_handler**](docs/SolutionApi.md#upload_run_template_handler) | **POST** /organizations/{organization_id}/solutions/{solution_id}/runtemplates/{run_template_id}/handlers/{handler_id}/upload | Upload a Run Template step handler zip file
-*UserApi* | [**authorize_user**](docs/UserApi.md#authorize_user) | **GET** /oauth2/authorize | Authorize an User with OAuth2. Delegated to configured OAuth2 service
-*UserApi* | [**find_all_users**](docs/UserApi.md#find_all_users) | **GET** /users | List all Users
-*UserApi* | [**find_user_by_id**](docs/UserApi.md#find_user_by_id) | **GET** /users/{user_id} | Get the details of an user
-*UserApi* | [**get_current_user**](docs/UserApi.md#get_current_user) | **GET** /users/me | Get the details of the logged-in User
-*UserApi* | [**get_organization_current_user**](docs/UserApi.md#get_organization_current_user) | **GET** /organizations/{organization_id}/me | Get the details of a logged-in User with roles for an Organization
-*UserApi* | [**get_workspace_current_user**](docs/UserApi.md#get_workspace_current_user) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/me | Get the details of the logged-in user with roles for a Workspace
-*UserApi* | [**register_user**](docs/UserApi.md#register_user) | **POST** /users | Register a new user
-*UserApi* | [**test_platform**](docs/UserApi.md#test_platform) | **GET** /test | test platform API call
-*UserApi* | [**unregister_user**](docs/UserApi.md#unregister_user) | **DELETE** /users/{user_id} | Unregister an user
-*UserApi* | [**update_user**](docs/UserApi.md#update_user) | **PATCH** /users/{user_id} | Update a User
+*TwingraphApi* | [**batch_query**](docs/TwingraphApi.md#batch_query) | **POST** /organizations/{organization_id}/twingraph/{graph_id}/batch-query | 
+*TwingraphApi* | [**batch_upload_update**](docs/TwingraphApi.md#batch_upload_update) | **POST** /organizations/{organization_id}/twingraph/{graph_id}/batch | 
+*TwingraphApi* | [**create_entities**](docs/TwingraphApi.md#create_entities) | **POST** /organizations/{organization_id}/twingraph/{graph_id}/{modelType} | 
+*TwingraphApi* | [**create_graph**](docs/TwingraphApi.md#create_graph) | **POST** /organizations/{organization_id}/twingraph/{graph_id} | 
+*TwingraphApi* | [**delete**](docs/TwingraphApi.md#delete) | **DELETE** /organizations/{organization_id}/twingraph/{graph_id} | 
+*TwingraphApi* | [**delete_entities**](docs/TwingraphApi.md#delete_entities) | **DELETE** /organizations/{organization_id}/twingraph/{graph_id}/{modelType} | 
+*TwingraphApi* | [**download_graph**](docs/TwingraphApi.md#download_graph) | **GET** /organizations/{organization_id}/twingraph/bulk-query/download/{hash} | 
+*TwingraphApi* | [**find_all_twingraphs**](docs/TwingraphApi.md#find_all_twingraphs) | **GET** /organizations/{organization_id}/twingraphs | 
+*TwingraphApi* | [**get_entities**](docs/TwingraphApi.md#get_entities) | **GET** /organizations/{organization_id}/twingraph/{graph_id}/{modelType} | 
+*TwingraphApi* | [**get_graph_meta_data**](docs/TwingraphApi.md#get_graph_meta_data) | **GET** /organizations/{organization_id}/twingraph/{graph_id}/metadata | 
+*TwingraphApi* | [**import_graph**](docs/TwingraphApi.md#import_graph) | **POST** /organizations/{organization_id}/twingraph/import | 
+*TwingraphApi* | [**job_status**](docs/TwingraphApi.md#job_status) | **GET** /organizations/{organization_id}/job/{job_id}/status | 
+*TwingraphApi* | [**query**](docs/TwingraphApi.md#query) | **POST** /organizations/{organization_id}/twingraph/{graph_id}/query | 
+*TwingraphApi* | [**update_entities**](docs/TwingraphApi.md#update_entities) | **PATCH** /organizations/{organization_id}/twingraph/{graph_id}/{modelType} | 
+*TwingraphApi* | [**update_graph_meta_data**](docs/TwingraphApi.md#update_graph_meta_data) | **PATCH** /organizations/{organization_id}/twingraph/{graph_id}/metadata | 
 *ValidatorApi* | [**create_validator**](docs/ValidatorApi.md#create_validator) | **POST** /organizations/{organization_id}/datasets/validators | Register a new validator
 *ValidatorApi* | [**create_validator_run**](docs/ValidatorApi.md#create_validator_run) | **POST** /organizations/{organization_id}/datasets/validators/{validator_id}/history | Register a new validator run
 *ValidatorApi* | [**delete_validator**](docs/ValidatorApi.md#delete_validator) | **DELETE** /organizations/{organization_id}/datasets/validators/{validator_id} | Delete a validator
 *ValidatorApi* | [**delete_validator_run**](docs/ValidatorApi.md#delete_validator_run) | **DELETE** /organizations/{organization_id}/datasets/validators/{validator_id}/history/{validatorrun_id} | Delete a validator run
 *ValidatorApi* | [**find_all_validator_runs**](docs/ValidatorApi.md#find_all_validator_runs) | **GET** /organizations/{organization_id}/datasets/validators/{validator_id}/history | List all Validator Runs
 *ValidatorApi* | [**find_all_validators**](docs/ValidatorApi.md#find_all_validators) | **GET** /organizations/{organization_id}/datasets/validators | List all Validators
 *ValidatorApi* | [**find_validator_by_id**](docs/ValidatorApi.md#find_validator_by_id) | **GET** /organizations/{organization_id}/datasets/validators/{validator_id} | Get the details of a validator
 *ValidatorApi* | [**find_validator_run_by_id**](docs/ValidatorApi.md#find_validator_run_by_id) | **GET** /organizations/{organization_id}/datasets/validators/{validator_id}/history/{validatorrun_id} | Get the details of a validator run
 *ValidatorApi* | [**run_validator**](docs/ValidatorApi.md#run_validator) | **POST** /organizations/{organization_id}/datasets/validators/{validator_id}/run | Run a Validator
-*WorkspaceApi* | [**add_or_replace_users_in_organization_workspace**](docs/WorkspaceApi.md#add_or_replace_users_in_organization_workspace) | **POST** /organizations/{organization_id}/workspaces/{workspace_id}/users | Add (or replace) users to the Workspace specified
+*WorkspaceApi* | [**add_workspace_access_control**](docs/WorkspaceApi.md#add_workspace_access_control) | **POST** /organizations/{organization_id}/workspaces/{workspace_id}/security/access | Add a control access to the Workspace
 *WorkspaceApi* | [**create_secret**](docs/WorkspaceApi.md#create_secret) | **POST** /organizations/{organization_id}/workspaces/{workspace_id}/secret | Create a secret for the Workspace
 *WorkspaceApi* | [**create_workspace**](docs/WorkspaceApi.md#create_workspace) | **POST** /organizations/{organization_id}/workspaces | Create a new workspace
 *WorkspaceApi* | [**delete_all_workspace_files**](docs/WorkspaceApi.md#delete_all_workspace_files) | **DELETE** /organizations/{organization_id}/workspaces/{workspace_id}/files | Delete all Workspace files
 *WorkspaceApi* | [**delete_workspace**](docs/WorkspaceApi.md#delete_workspace) | **DELETE** /organizations/{organization_id}/workspaces/{workspace_id} | Delete a workspace
 *WorkspaceApi* | [**delete_workspace_file**](docs/WorkspaceApi.md#delete_workspace_file) | **DELETE** /organizations/{organization_id}/workspaces/{workspace_id}/files/delete | Delete a workspace file
 *WorkspaceApi* | [**download_workspace_file**](docs/WorkspaceApi.md#download_workspace_file) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/files/download | Download the Workspace File specified
 *WorkspaceApi* | [**find_all_workspace_files**](docs/WorkspaceApi.md#find_all_workspace_files) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/files | List all Workspace files
 *WorkspaceApi* | [**find_all_workspaces**](docs/WorkspaceApi.md#find_all_workspaces) | **GET** /organizations/{organization_id}/workspaces | List all Workspaces
 *WorkspaceApi* | [**find_workspace_by_id**](docs/WorkspaceApi.md#find_workspace_by_id) | **GET** /organizations/{organization_id}/workspaces/{workspace_id} | Get the details of an workspace
-*WorkspaceApi* | [**remove_all_users_of_workspace**](docs/WorkspaceApi.md#remove_all_users_of_workspace) | **DELETE** /organizations/{organization_id}/workspaces/{workspace_id}/users | Remove all users from the Workspace specified
-*WorkspaceApi* | [**remove_user_from_organization_workspace**](docs/WorkspaceApi.md#remove_user_from_organization_workspace) | **DELETE** /organizations/{organization_id}/workspaces/{workspace_id}/users/{user_id} | Remove the specified user from the given Organization Workspace
+*WorkspaceApi* | [**get_workspace_access_control**](docs/WorkspaceApi.md#get_workspace_access_control) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/security/access/{identity_id} | Get a control access for the Workspace
+*WorkspaceApi* | [**get_workspace_permissions**](docs/WorkspaceApi.md#get_workspace_permissions) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/permissions/{role} | Get the Workspace permission by given role
+*WorkspaceApi* | [**get_workspace_security**](docs/WorkspaceApi.md#get_workspace_security) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/security | Get the Workspace security information
+*WorkspaceApi* | [**get_workspace_security_users**](docs/WorkspaceApi.md#get_workspace_security_users) | **GET** /organizations/{organization_id}/workspaces/{workspace_id}/security/users | Get the Workspace security users list
+*WorkspaceApi* | [**import_workspace**](docs/WorkspaceApi.md#import_workspace) | **POST** /organizations/{organization_id}/workspaces/import | Import a workspace
+*WorkspaceApi* | [**remove_workspace_access_control**](docs/WorkspaceApi.md#remove_workspace_access_control) | **DELETE** /organizations/{organization_id}/workspaces/{workspace_id}/security/access/{identity_id} | Remove the specified access from the given Organization Workspace
+*WorkspaceApi* | [**set_workspace_default_security**](docs/WorkspaceApi.md#set_workspace_default_security) | **POST** /organizations/{organization_id}/workspaces/{workspace_id}/security/default | Set the Workspace default security
 *WorkspaceApi* | [**update_workspace**](docs/WorkspaceApi.md#update_workspace) | **PATCH** /organizations/{organization_id}/workspaces/{workspace_id} | Update a workspace
+*WorkspaceApi* | [**update_workspace_access_control**](docs/WorkspaceApi.md#update_workspace_access_control) | **PATCH** /organizations/{organization_id}/workspaces/{workspace_id}/security/access/{identity_id} | Update the specified access to User for a Workspace
 *WorkspaceApi* | [**upload_workspace_file**](docs/WorkspaceApi.md#upload_workspace_file) | **POST** /organizations/{organization_id}/workspaces/{workspace_id}/files | Upload a file for the Workspace
 
 
 ## Documentation For Models
 
+ - [ComponentRolePermissions](docs/ComponentRolePermissions.md)
  - [Connector](docs/Connector.md)
  - [ConnectorParameter](docs/ConnectorParameter.md)
  - [ConnectorParameterGroup](docs/ConnectorParameterGroup.md)
+ - [ContainerResourceSizeInfo](docs/ContainerResourceSizeInfo.md)
+ - [ContainerResourceSizing](docs/ContainerResourceSizing.md)
  - [Dataset](docs/Dataset.md)
  - [DatasetCompatibility](docs/DatasetCompatibility.md)
  - [DatasetConnector](docs/DatasetConnector.md)
  - [DatasetCopyParameters](docs/DatasetCopyParameters.md)
  - [DatasetSearch](docs/DatasetSearch.md)
  - [DeleteHistoricalData](docs/DeleteHistoricalData.md)
+ - [GraphProperties](docs/GraphProperties.md)
  - [Organization](docs/Organization.md)
+ - [OrganizationAccessControl](docs/OrganizationAccessControl.md)
+ - [OrganizationRole](docs/OrganizationRole.md)
+ - [OrganizationSecurity](docs/OrganizationSecurity.md)
  - [OrganizationService](docs/OrganizationService.md)
  - [OrganizationServices](docs/OrganizationServices.md)
- - [OrganizationUser](docs/OrganizationUser.md)
+ - [ResourceSizeInfo](docs/ResourceSizeInfo.md)
  - [RunTemplate](docs/RunTemplate.md)
  - [RunTemplateHandlerId](docs/RunTemplateHandlerId.md)
  - [RunTemplateParameter](docs/RunTemplateParameter.md)
  - [RunTemplateParameterGroup](docs/RunTemplateParameterGroup.md)
  - [RunTemplateParameterValue](docs/RunTemplateParameterValue.md)
+ - [RunTemplateResourceSizing](docs/RunTemplateResourceSizing.md)
  - [RunTemplateStepSource](docs/RunTemplateStepSource.md)
  - [Scenario](docs/Scenario.md)
+ - [ScenarioAccessControl](docs/ScenarioAccessControl.md)
  - [ScenarioChangedParameterValue](docs/ScenarioChangedParameterValue.md)
  - [ScenarioComparisonResult](docs/ScenarioComparisonResult.md)
  - [ScenarioDataDownloadInfo](docs/ScenarioDataDownloadInfo.md)
  - [ScenarioDataDownloadJob](docs/ScenarioDataDownloadJob.md)
  - [ScenarioJobState](docs/ScenarioJobState.md)
  - [ScenarioLastRun](docs/ScenarioLastRun.md)
+ - [ScenarioResourceSizing](docs/ScenarioResourceSizing.md)
+ - [ScenarioRole](docs/ScenarioRole.md)
  - [ScenarioRun](docs/ScenarioRun.md)
  - [ScenarioRunContainer](docs/ScenarioRunContainer.md)
  - [ScenarioRunContainerArtifact](docs/ScenarioRunContainerArtifact.md)
  - [ScenarioRunContainerLogs](docs/ScenarioRunContainerLogs.md)
  - [ScenarioRunLogs](docs/ScenarioRunLogs.md)
  - [ScenarioRunSearch](docs/ScenarioRunSearch.md)
  - [ScenarioRunStartContainers](docs/ScenarioRunStartContainers.md)
  - [ScenarioRunState](docs/ScenarioRunState.md)
  - [ScenarioRunStatus](docs/ScenarioRunStatus.md)
  - [ScenarioRunStatusNode](docs/ScenarioRunStatusNode.md)
  - [ScenarioRunTemplateParameterValue](docs/ScenarioRunTemplateParameterValue.md)
- - [ScenarioUser](docs/ScenarioUser.md)
+ - [ScenarioSecurity](docs/ScenarioSecurity.md)
  - [ScenarioValidationStatus](docs/ScenarioValidationStatus.md)
  - [Solution](docs/Solution.md)
+ - [SourceInfo](docs/SourceInfo.md)
  - [TranslatedLabels](docs/TranslatedLabels.md)
- - [User](docs/User.md)
- - [UserOrganization](docs/UserOrganization.md)
- - [UserWorkspace](docs/UserWorkspace.md)
+ - [TwinGraphBatchResult](docs/TwinGraphBatchResult.md)
+ - [TwinGraphHash](docs/TwinGraphHash.md)
+ - [TwinGraphImport](docs/TwinGraphImport.md)
+ - [TwinGraphImportInfo](docs/TwinGraphImportInfo.md)
+ - [TwinGraphQuery](docs/TwinGraphQuery.md)
  - [Validator](docs/Validator.md)
  - [ValidatorRun](docs/ValidatorRun.md)
  - [Workspace](docs/Workspace.md)
+ - [WorkspaceAccessControl](docs/WorkspaceAccessControl.md)
  - [WorkspaceFile](docs/WorkspaceFile.md)
+ - [WorkspaceRole](docs/WorkspaceRole.md)
  - [WorkspaceSecret](docs/WorkspaceSecret.md)
+ - [WorkspaceSecurity](docs/WorkspaceSecurity.md)
  - [WorkspaceSolution](docs/WorkspaceSolution.md)
- - [WorkspaceUser](docs/WorkspaceUser.md)
  - [WorkspaceWebApp](docs/WorkspaceWebApp.md)
 
 
 ## Documentation For Authorization
 
 
 ## oAuth2AuthCode
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/__init__.py` & `cosmotech-api-2.4.0/cosmotech_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 __version__ = "1.0.0"
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/api/connector_api.py` & `cosmotech-api-2.4.0/cosmotech_api/api/connector_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -45,14 +45,16 @@
                 'endpoint_path': '/connectors',
                 'operation_id': 'find_all_connectors',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
+                    'page',
+                    'size',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -60,18 +62,26 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
+                    'page':
+                        (int,),
+                    'size':
+                        (int,),
                 },
                 'attribute_map': {
+                    'page': 'page',
+                    'size': 'size',
                 },
                 'location_map': {
+                    'page': 'query',
+                    'size': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -127,14 +137,66 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.import_connector_endpoint = _Endpoint(
+            settings={
+                'response_type': (Connector,),
+                'auth': [
+                    'oAuth2AuthCode'
+                ],
+                'endpoint_path': '/connectors/import',
+                'operation_id': 'import_connector',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'connector',
+                ],
+                'required': [
+                    'connector',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'connector':
+                        (Connector,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'connector': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.register_connector_endpoint = _Endpoint(
             settings={
                 'response_type': (Connector,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
                 'endpoint_path': '/connectors',
@@ -244,14 +306,16 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.find_all_connectors(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
+            page (int): page number to query. [optional]
+            size (int): amount of result by page. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -379,14 +443,91 @@
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['connector_id'] = \
             connector_id
         return self.find_connector_by_id_endpoint.call_with_http_info(**kwargs)
 
+    def import_connector(
+        self,
+        connector,
+        **kwargs
+    ):
+        """Import existing connector  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.import_connector(connector, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            connector (Connector): the Connector to import
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            Connector
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['connector'] = \
+            connector
+        return self.import_connector_endpoint.call_with_http_info(**kwargs)
+
     def register_connector(
         self,
         connector,
         **kwargs
     ):
         """Register a new connector  # noqa: E501
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/api/dataset_api.py` & `cosmotech-api-2.4.0/cosmotech_api/api/dataset_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -286,14 +286,16 @@
                 'operation_id': 'find_all_datasets',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
+                    'page',
+                    'size',
                 ],
                 'required': [
                     'organization_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -305,20 +307,28 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'organization_id':
                         (str,),
+                    'page':
+                        (int,),
+                    'size':
+                        (int,),
                 },
                 'attribute_map': {
                     'organization_id': 'organization_id',
+                    'page': 'page',
+                    'size': 'size',
                 },
                 'location_map': {
                     'organization_id': 'path',
+                    'page': 'query',
+                    'size': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -380,14 +390,72 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.import_dataset_endpoint = _Endpoint(
+            settings={
+                'response_type': (Dataset,),
+                'auth': [
+                    'oAuth2AuthCode'
+                ],
+                'endpoint_path': '/organizations/{organization_id}/datasets/import',
+                'operation_id': 'import_dataset',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'organization_id',
+                    'dataset',
+                ],
+                'required': [
+                    'organization_id',
+                    'dataset',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'organization_id':
+                        (str,),
+                    'dataset':
+                        (Dataset,),
+                },
+                'attribute_map': {
+                    'organization_id': 'organization_id',
+                },
+                'location_map': {
+                    'organization_id': 'path',
+                    'dataset': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.remove_all_dataset_compatibility_elements_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'oAuth2AuthCode'
                 ],
                 'endpoint_path': '/organizations/{organization_id}/datasets/{dataset_id}/compatibility',
@@ -450,14 +518,16 @@
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
                     'dataset_search',
+                    'page',
+                    'size',
                 ],
                 'required': [
                     'organization_id',
                     'dataset_search',
                 ],
                 'nullable': [
                 ],
@@ -472,21 +542,29 @@
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'organization_id':
                         (str,),
                     'dataset_search':
                         (DatasetSearch,),
+                    'page':
+                        (int,),
+                    'size':
+                        (int,),
                 },
                 'attribute_map': {
                     'organization_id': 'organization_id',
+                    'page': 'page',
+                    'size': 'size',
                 },
                 'location_map': {
                     'organization_id': 'path',
                     'dataset_search': 'body',
+                    'page': 'query',
+                    'size': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -905,14 +983,16 @@
         >>> thread = api.find_all_datasets(organization_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             organization_id (str): the Organization identifier
 
         Keyword Args:
+            page (int): page number to query. [optional]
+            size (int): amount of result by page. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1046,14 +1126,95 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['organization_id'] = \
             organization_id
         kwargs['dataset_id'] = \
             dataset_id
         return self.find_dataset_by_id_endpoint.call_with_http_info(**kwargs)
 
+    def import_dataset(
+        self,
+        organization_id,
+        dataset,
+        **kwargs
+    ):
+        """Import a new Dataset  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.import_dataset(organization_id, dataset, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            organization_id (str): the Organization identifier
+            dataset (Dataset): the Dataset to import
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            Dataset
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['organization_id'] = \
+            organization_id
+        kwargs['dataset'] = \
+            dataset
+        return self.import_dataset_endpoint.call_with_http_info(**kwargs)
+
     def remove_all_dataset_compatibility_elements(
         self,
         organization_id,
         dataset_id,
         **kwargs
     ):
         """Remove all Dataset Compatibility elements from the Dataset specified  # noqa: E501
@@ -1146,14 +1307,16 @@
         >>> result = thread.get()
 
         Args:
             organization_id (str): the Organization identifier
             dataset_search (DatasetSearch): the Dataset search parameters
 
         Keyword Args:
+            page (int): page number to query. [optional]
+            size (int): amount of result by page. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/api/organization_api.py` & `cosmotech-api-2.4.0/cosmotech_api/api/user_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.3.7
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -18,96 +18,78 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from cosmotech_api.model.organization import Organization
-from cosmotech_api.model.organization_service import OrganizationService
-from cosmotech_api.model.organization_user import OrganizationUser
+from cosmotech_api.model.user import User
 
 
-class OrganizationApi(object):
+class UserApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.add_or_replace_users_in_organization_endpoint = _Endpoint(
+        self.authorize_user_endpoint = _Endpoint(
             settings={
-                'response_type': ([OrganizationUser],),
+                'response_type': None,
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/organizations/{organization_id}/users',
-                'operation_id': 'add_or_replace_users_in_organization',
-                'http_method': 'POST',
+                'endpoint_path': '/oauth2/authorize',
+                'operation_id': 'authorize_user',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'organization_id',
-                    'organization_user',
-                ],
-                'required': [
-                    'organization_id',
-                    'organization_user',
                 ],
+                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'organization_id':
-                        (str,),
-                    'organization_user':
-                        ([OrganizationUser],),
                 },
                 'attribute_map': {
-                    'organization_id': 'organization_id',
                 },
                 'location_map': {
-                    'organization_id': 'path',
-                    'organization_user': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [
-                    'application/json'
-                ]
+                'accept': [],
+                'content_type': [],
             },
             api_client=api_client
         )
-        self.find_all_organizations_endpoint = _Endpoint(
+        self.find_all_users_endpoint = _Endpoint(
             settings={
-                'response_type': ([Organization],),
+                'response_type': ([User],),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/organizations',
-                'operation_id': 'find_all_organizations',
+                'endpoint_path': '/users',
+                'operation_id': 'find_all_users',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                 ],
                 'required': [],
@@ -136,127 +118,118 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.find_organization_by_id_endpoint = _Endpoint(
+        self.find_user_by_id_endpoint = _Endpoint(
             settings={
-                'response_type': (Organization,),
+                'response_type': (User,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/organizations/{organization_id}',
-                'operation_id': 'find_organization_by_id',
+                'endpoint_path': '/users/{user_id}',
+                'operation_id': 'find_user_by_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'organization_id',
+                    'user_id',
                 ],
                 'required': [
-                    'organization_id',
+                    'user_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'organization_id':
+                    'user_id':
                         (str,),
                 },
                 'attribute_map': {
-                    'organization_id': 'organization_id',
+                    'user_id': 'user_id',
                 },
                 'location_map': {
-                    'organization_id': 'path',
+                    'user_id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.register_organization_endpoint = _Endpoint(
+        self.get_current_user_endpoint = _Endpoint(
             settings={
-                'response_type': (Organization,),
+                'response_type': (User,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/organizations',
-                'operation_id': 'register_organization',
-                'http_method': 'POST',
+                'endpoint_path': '/users/me',
+                'operation_id': 'get_current_user',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'organization',
-                ],
-                'required': [
-                    'organization',
                 ],
+                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'organization':
-                        (Organization,),
                 },
                 'attribute_map': {
                 },
                 'location_map': {
-                    'organization': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [
-                    'application/json',
-                    'application/yaml'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
-        self.remove_all_users_in_organization_endpoint = _Endpoint(
+        self.get_organization_current_user_endpoint = _Endpoint(
             settings={
-                'response_type': None,
+                'response_type': (User,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/organizations/{organization_id}/users',
-                'operation_id': 'remove_all_users_in_organization',
-                'http_method': 'DELETE',
+                'endpoint_path': '/organizations/{organization_id}/me',
+                'operation_id': 'get_organization_current_user',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
                 ],
                 'required': [
@@ -284,38 +257,40 @@
                 'location_map': {
                     'organization_id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [],
+                'accept': [
+                    'application/json'
+                ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.remove_user_from_organization_endpoint = _Endpoint(
+        self.get_workspace_current_user_endpoint = _Endpoint(
             settings={
-                'response_type': None,
+                'response_type': (User,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/organizations/{organization_id}/users/{user_id}',
-                'operation_id': 'remove_user_from_organization',
-                'http_method': 'DELETE',
+                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/me',
+                'operation_id': 'get_workspace_current_user',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
-                    'user_id',
+                    'workspace_id',
                 ],
                 'required': [
                     'organization_id',
-                    'user_id',
+                    'workspace_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
@@ -324,127 +299,74 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'organization_id':
                         (str,),
-                    'user_id':
+                    'workspace_id':
                         (str,),
                 },
                 'attribute_map': {
                     'organization_id': 'organization_id',
-                    'user_id': 'user_id',
+                    'workspace_id': 'workspace_id',
                 },
                 'location_map': {
                     'organization_id': 'path',
-                    'user_id': 'path',
+                    'workspace_id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-        self.unregister_organization_endpoint = _Endpoint(
-            settings={
-                'response_type': None,
-                'auth': [
-                    'oAuth2AuthCode'
-                ],
-                'endpoint_path': '/organizations/{organization_id}',
-                'operation_id': 'unregister_organization',
-                'http_method': 'DELETE',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'organization_id',
-                ],
-                'required': [
-                    'organization_id',
-                ],
-                'nullable': [
-                ],
-                'enum': [
+                'accept': [
+                    'application/json'
                 ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'organization_id':
-                        (str,),
-                },
-                'attribute_map': {
-                    'organization_id': 'organization_id',
-                },
-                'location_map': {
-                    'organization_id': 'path',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.update_organization_endpoint = _Endpoint(
+        self.register_user_endpoint = _Endpoint(
             settings={
-                'response_type': (Organization,),
+                'response_type': (User,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/organizations/{organization_id}',
-                'operation_id': 'update_organization',
-                'http_method': 'PATCH',
+                'endpoint_path': '/users',
+                'operation_id': 'register_user',
+                'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'organization_id',
-                    'organization',
+                    'user',
                 ],
                 'required': [
-                    'organization_id',
-                    'organization',
+                    'user',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'organization_id':
-                        (str,),
-                    'organization':
-                        (Organization,),
+                    'user':
+                        (User,),
                 },
                 'attribute_map': {
-                    'organization_id': 'organization_id',
                 },
                 'location_map': {
-                    'organization_id': 'path',
-                    'organization': 'body',
+                    'user': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -452,208 +374,179 @@
                 'content_type': [
                     'application/json',
                     'application/yaml'
                 ]
             },
             api_client=api_client
         )
-        self.update_solutions_container_registry_by_organization_id_endpoint = _Endpoint(
+        self.test_platform_endpoint = _Endpoint(
             settings={
-                'response_type': (OrganizationService,),
+                'response_type': (str,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/organizations/{organization_id}/services/solutionsContainerRegistry',
-                'operation_id': 'update_solutions_container_registry_by_organization_id',
-                'http_method': 'PATCH',
+                'endpoint_path': '/test',
+                'operation_id': 'test_platform',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'organization_id',
-                    'organization_service',
-                ],
-                'required': [
-                    'organization_id',
-                    'organization_service',
                 ],
+                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'organization_id':
-                        (str,),
-                    'organization_service':
-                        (OrganizationService,),
                 },
                 'attribute_map': {
-                    'organization_id': 'organization_id',
                 },
                 'location_map': {
-                    'organization_id': 'path',
-                    'organization_service': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
-                    'application/json'
+                    'text/plain'
                 ],
-                'content_type': [
-                    'application/json',
-                    'application/yaml'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
-        self.update_storage_by_organization_id_endpoint = _Endpoint(
+        self.unregister_user_endpoint = _Endpoint(
             settings={
-                'response_type': (OrganizationService,),
+                'response_type': None,
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/organizations/{organization_id}/services/storage',
-                'operation_id': 'update_storage_by_organization_id',
-                'http_method': 'PATCH',
+                'endpoint_path': '/users/{user_id}',
+                'operation_id': 'unregister_user',
+                'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'organization_id',
-                    'organization_service',
+                    'user_id',
                 ],
                 'required': [
-                    'organization_id',
-                    'organization_service',
+                    'user_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'organization_id':
+                    'user_id':
                         (str,),
-                    'organization_service':
-                        (OrganizationService,),
                 },
                 'attribute_map': {
-                    'organization_id': 'organization_id',
+                    'user_id': 'user_id',
                 },
                 'location_map': {
-                    'organization_id': 'path',
-                    'organization_service': 'body',
+                    'user_id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [
-                    'application/json',
-                    'application/yaml'
-                ]
+                'accept': [],
+                'content_type': [],
             },
             api_client=api_client
         )
-        self.update_tenant_credentials_by_organization_id_endpoint = _Endpoint(
+        self.update_user_endpoint = _Endpoint(
             settings={
-                'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
+                'response_type': (User,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/organizations/{organization_id}/services/tenantCredentials',
-                'operation_id': 'update_tenant_credentials_by_organization_id',
+                'endpoint_path': '/users/{user_id}',
+                'operation_id': 'update_user',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'organization_id',
-                    'request_body',
+                    'user_id',
+                    'user',
                 ],
                 'required': [
-                    'organization_id',
-                    'request_body',
+                    'user_id',
+                    'user',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'organization_id':
+                    'user_id':
                         (str,),
-                    'request_body':
-                        ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
+                    'user':
+                        (User,),
                 },
                 'attribute_map': {
-                    'organization_id': 'organization_id',
+                    'user_id': 'user_id',
                 },
                 'location_map': {
-                    'organization_id': 'path',
-                    'request_body': 'body',
+                    'user_id': 'path',
+                    'user': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [
-                    'application/json'
+                    'application/json',
+                    'application/yaml'
                 ]
             },
             api_client=api_client
         )
 
-    def add_or_replace_users_in_organization(
+    def authorize_user(
         self,
-        organization_id,
-        organization_user,
         **kwargs
     ):
-        """Add (or replace) users in the Organization specified  # noqa: E501
+        """Authorize an User with OAuth2. Delegated to configured OAuth2 service  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.add_or_replace_users_in_organization(organization_id, organization_user, async_req=True)
+        >>> thread = api.authorize_user(async_req=True)
         >>> result = thread.get()
 
-        Args:
-            organization_id (str): the Organization identifier
-            organization_user ([OrganizationUser]): the Users to add. Any User with the same ID is overwritten
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -676,91 +569,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            [OrganizationUser]
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['organization_id'] = \
-            organization_id
-        kwargs['organization_user'] = \
-            organization_user
-        return self.add_or_replace_users_in_organization_endpoint.call_with_http_info(**kwargs)
-
-    def find_all_organizations(
-        self,
-        **kwargs
-    ):
-        """List all Organizations  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.find_all_organizations(async_req=True)
-        >>> result = thread.get()
-
-
-        Keyword Args:
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            [Organization]
+            None
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -780,31 +597,28 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        return self.find_all_organizations_endpoint.call_with_http_info(**kwargs)
+        return self.authorize_user_endpoint.call_with_http_info(**kwargs)
 
-    def find_organization_by_id(
+    def find_all_users(
         self,
-        organization_id,
         **kwargs
     ):
-        """Get the details of an Organization  # noqa: E501
+        """List all Users  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_organization_by_id(organization_id, async_req=True)
+        >>> thread = api.find_all_users(async_req=True)
         >>> result = thread.get()
 
-        Args:
-            organization_id (str): the Organization identifier
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -827,15 +641,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            Organization
+            [User]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -855,33 +669,31 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['organization_id'] = \
-            organization_id
-        return self.find_organization_by_id_endpoint.call_with_http_info(**kwargs)
+        return self.find_all_users_endpoint.call_with_http_info(**kwargs)
 
-    def register_organization(
+    def find_user_by_id(
         self,
-        organization,
+        user_id,
         **kwargs
     ):
-        """Register a new organization  # noqa: E501
+        """Get the details of an user  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.register_organization(organization, async_req=True)
+        >>> thread = api.find_user_by_id(user_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            organization (Organization): the Organization to register
+            user_id (str): the User identifier
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -904,15 +716,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            Organization
+            User
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -932,33 +744,30 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['organization'] = \
-            organization
-        return self.register_organization_endpoint.call_with_http_info(**kwargs)
+        kwargs['user_id'] = \
+            user_id
+        return self.find_user_by_id_endpoint.call_with_http_info(**kwargs)
 
-    def remove_all_users_in_organization(
+    def get_current_user(
         self,
-        organization_id,
         **kwargs
     ):
-        """Remove all users from the Organization specified  # noqa: E501
+        """Get the details of the logged-in User  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.remove_all_users_in_organization(organization_id, async_req=True)
+        >>> thread = api.get_current_user(async_req=True)
         >>> result = thread.get()
 
-        Args:
-            organization_id (str): the Organization identifier
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -981,15 +790,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            None
+            User
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1009,35 +818,31 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['organization_id'] = \
-            organization_id
-        return self.remove_all_users_in_organization_endpoint.call_with_http_info(**kwargs)
+        return self.get_current_user_endpoint.call_with_http_info(**kwargs)
 
-    def remove_user_from_organization(
+    def get_organization_current_user(
         self,
         organization_id,
-        user_id,
         **kwargs
     ):
-        """Remove the specified user from the given Organization  # noqa: E501
+        """Get the details of a logged-in User with roles for an Organization  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.remove_user_from_organization(organization_id, user_id, async_req=True)
+        >>> thread = api.get_organization_current_user(organization_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             organization_id (str): the Organization identifier
-            user_id (str): the User identifier
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1060,15 +865,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            None
+            User
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1090,33 +895,33 @@
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['organization_id'] = \
             organization_id
-        kwargs['user_id'] = \
-            user_id
-        return self.remove_user_from_organization_endpoint.call_with_http_info(**kwargs)
+        return self.get_organization_current_user_endpoint.call_with_http_info(**kwargs)
 
-    def unregister_organization(
+    def get_workspace_current_user(
         self,
         organization_id,
+        workspace_id,
         **kwargs
     ):
-        """Unregister an organization  # noqa: E501
+        """Get the details of the logged-in user with roles for a Workspace  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.unregister_organization(organization_id, async_req=True)
+        >>> thread = api.get_workspace_current_user(organization_id, workspace_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             organization_id (str): the Organization identifier
+            workspace_id (str): the Workspace identifier
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1139,15 +944,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            None
+            User
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1169,33 +974,33 @@
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['organization_id'] = \
             organization_id
-        return self.unregister_organization_endpoint.call_with_http_info(**kwargs)
+        kwargs['workspace_id'] = \
+            workspace_id
+        return self.get_workspace_current_user_endpoint.call_with_http_info(**kwargs)
 
-    def update_organization(
+    def register_user(
         self,
-        organization_id,
-        organization,
+        user,
         **kwargs
     ):
-        """Update an Organization  # noqa: E501
+        """Register a new user  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_organization(organization_id, organization, async_req=True)
+        >>> thread = api.register_user(user, async_req=True)
         >>> result = thread.get()
 
         Args:
-            organization_id (str): the Organization identifier
-            organization (Organization): the new Organization details
+            user (User): the User to register
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1218,15 +1023,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            Organization
+            User
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1246,37 +1051,30 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['organization_id'] = \
-            organization_id
-        kwargs['organization'] = \
-            organization
-        return self.update_organization_endpoint.call_with_http_info(**kwargs)
+        kwargs['user'] = \
+            user
+        return self.register_user_endpoint.call_with_http_info(**kwargs)
 
-    def update_solutions_container_registry_by_organization_id(
+    def test_platform(
         self,
-        organization_id,
-        organization_service,
         **kwargs
     ):
-        """Update the solutions container registry configuration for the Organization specified  # noqa: E501
+        """test platform API call  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_solutions_container_registry_by_organization_id(organization_id, organization_service, async_req=True)
+        >>> thread = api.test_platform(async_req=True)
         >>> result = thread.get()
 
-        Args:
-            organization_id (str): the Organization identifier
-            organization_service (OrganizationService): the new solutions container registry configuration to use
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1299,15 +1097,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            OrganizationService
+            str
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1327,37 +1125,31 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['organization_id'] = \
-            organization_id
-        kwargs['organization_service'] = \
-            organization_service
-        return self.update_solutions_container_registry_by_organization_id_endpoint.call_with_http_info(**kwargs)
+        return self.test_platform_endpoint.call_with_http_info(**kwargs)
 
-    def update_storage_by_organization_id(
+    def unregister_user(
         self,
-        organization_id,
-        organization_service,
+        user_id,
         **kwargs
     ):
-        """Update storage configuration for the Organization specified  # noqa: E501
+        """Unregister an user  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_storage_by_organization_id(organization_id, organization_service, async_req=True)
+        >>> thread = api.unregister_user(user_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            organization_id (str): the Organization identifier
-            organization_service (OrganizationService): the new Storage configuration to use
+            user_id (str): the User identifier
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1380,15 +1172,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            OrganizationService
+            None
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1408,37 +1200,35 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['organization_id'] = \
-            organization_id
-        kwargs['organization_service'] = \
-            organization_service
-        return self.update_storage_by_organization_id_endpoint.call_with_http_info(**kwargs)
+        kwargs['user_id'] = \
+            user_id
+        return self.unregister_user_endpoint.call_with_http_info(**kwargs)
 
-    def update_tenant_credentials_by_organization_id(
+    def update_user(
         self,
-        organization_id,
-        request_body,
+        user_id,
+        user,
         **kwargs
     ):
-        """Update tenant credentials for the Organization specified  # noqa: E501
+        """Update a User  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_tenant_credentials_by_organization_id(organization_id, request_body, async_req=True)
+        >>> thread = api.update_user(user_id, user, async_req=True)
         >>> result = thread.get()
 
         Args:
-            organization_id (str): the Organization identifier
-            request_body ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): the new Tenant Credentials to use
+            user_id (str): the User identifier
+            user (User): the new User details. Organization membership is handled via the /organizations endpoint.
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1461,15 +1251,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+            User
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1489,13 +1279,13 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['organization_id'] = \
-            organization_id
-        kwargs['request_body'] = \
-            request_body
-        return self.update_tenant_credentials_by_organization_id_endpoint.call_with_http_info(**kwargs)
+        kwargs['user_id'] = \
+            user_id
+        kwargs['user'] = \
+            user
+        return self.update_user_endpoint.call_with_http_info(**kwargs)
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/api/scenario_api.py` & `cosmotech-api-2.4.0/cosmotech_api/api/scenario_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -19,19 +19,21 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from cosmotech_api.model.scenario import Scenario
+from cosmotech_api.model.scenario_access_control import ScenarioAccessControl
 from cosmotech_api.model.scenario_comparison_result import ScenarioComparisonResult
 from cosmotech_api.model.scenario_data_download_info import ScenarioDataDownloadInfo
 from cosmotech_api.model.scenario_data_download_job import ScenarioDataDownloadJob
+from cosmotech_api.model.scenario_role import ScenarioRole
 from cosmotech_api.model.scenario_run_template_parameter_value import ScenarioRunTemplateParameterValue
-from cosmotech_api.model.scenario_user import ScenarioUser
+from cosmotech_api.model.scenario_security import ScenarioSecurity
 from cosmotech_api.model.scenario_validation_status import ScenarioValidationStatus
 
 
 class ScenarioApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
@@ -108,37 +110,37 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.add_or_replace_users_in_scenario_endpoint = _Endpoint(
+        self.add_scenario_access_control_endpoint = _Endpoint(
             settings={
-                'response_type': ([ScenarioUser],),
+                'response_type': (ScenarioAccessControl,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/users',
-                'operation_id': 'add_or_replace_users_in_scenario',
+                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/security/access',
+                'operation_id': 'add_scenario_access_control',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
                     'workspace_id',
                     'scenario_id',
-                    'scenario_user',
+                    'scenario_access_control',
                 ],
                 'required': [
                     'organization_id',
                     'workspace_id',
                     'scenario_id',
-                    'scenario_user',
+                    'scenario_access_control',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
@@ -151,37 +153,38 @@
                 'openapi_types': {
                     'organization_id':
                         (str,),
                     'workspace_id':
                         (str,),
                     'scenario_id':
                         (str,),
-                    'scenario_user':
-                        ([ScenarioUser],),
+                    'scenario_access_control':
+                        (ScenarioAccessControl,),
                 },
                 'attribute_map': {
                     'organization_id': 'organization_id',
                     'workspace_id': 'workspace_id',
                     'scenario_id': 'scenario_id',
                 },
                 'location_map': {
                     'organization_id': 'path',
                     'workspace_id': 'path',
                     'scenario_id': 'path',
-                    'scenario_user': 'body',
+                    'scenario_access_control': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [
-                    'application/json'
+                    'application/json',
+                    'application/yaml'
                 ]
             },
             api_client=api_client
         )
         self.compare_scenarios_endpoint = _Endpoint(
             settings={
                 'response_type': (ScenarioComparisonResult,),
@@ -511,14 +514,16 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
                     'workspace_id',
+                    'page',
+                    'size',
                 ],
                 'required': [
                     'organization_id',
                     'workspace_id',
                 ],
                 'nullable': [
                 ],
@@ -533,22 +538,30 @@
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'organization_id':
                         (str,),
                     'workspace_id':
                         (str,),
+                    'page':
+                        (int,),
+                    'size':
+                        (int,),
                 },
                 'attribute_map': {
                     'organization_id': 'organization_id',
                     'workspace_id': 'workspace_id',
+                    'page': 'page',
+                    'size': 'size',
                 },
                 'location_map': {
                     'organization_id': 'path',
                     'workspace_id': 'path',
+                    'page': 'query',
+                    'size': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -569,14 +582,16 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
                     'workspace_id',
                     'validation_status',
+                    'page',
+                    'size',
                 ],
                 'required': [
                     'organization_id',
                     'workspace_id',
                     'validation_status',
                 ],
                 'nullable': [
@@ -594,24 +609,32 @@
                 'openapi_types': {
                     'organization_id':
                         (str,),
                     'workspace_id':
                         (str,),
                     'validation_status':
                         (ScenarioValidationStatus,),
+                    'page':
+                        (int,),
+                    'size':
+                        (int,),
                 },
                 'attribute_map': {
                     'organization_id': 'organization_id',
                     'workspace_id': 'workspace_id',
                     'validation_status': 'validationStatus',
+                    'page': 'page',
+                    'size': 'size',
                 },
                 'location_map': {
                     'organization_id': 'path',
                     'workspace_id': 'path',
                     'validation_status': 'path',
+                    'page': 'query',
+                    'size': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -679,14 +702,83 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.get_scenario_access_control_endpoint = _Endpoint(
+            settings={
+                'response_type': (ScenarioAccessControl,),
+                'auth': [
+                    'oAuth2AuthCode'
+                ],
+                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/security/access/{identity_id}',
+                'operation_id': 'get_scenario_access_control',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'organization_id',
+                    'workspace_id',
+                    'scenario_id',
+                    'identity_id',
+                ],
+                'required': [
+                    'organization_id',
+                    'workspace_id',
+                    'scenario_id',
+                    'identity_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'organization_id':
+                        (str,),
+                    'workspace_id':
+                        (str,),
+                    'scenario_id':
+                        (str,),
+                    'identity_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'organization_id': 'organization_id',
+                    'workspace_id': 'workspace_id',
+                    'scenario_id': 'scenario_id',
+                    'identity_id': 'identity_id',
+                },
+                'location_map': {
+                    'organization_id': 'path',
+                    'workspace_id': 'path',
+                    'scenario_id': 'path',
+                    'identity_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.get_scenario_data_download_job_info_endpoint = _Endpoint(
             settings={
                 'response_type': (ScenarioDataDownloadInfo,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
                 'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/downloads/{download_id}',
@@ -748,14 +840,203 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.get_scenario_permissions_endpoint = _Endpoint(
+            settings={
+                'response_type': ([str],),
+                'auth': [
+                    'oAuth2AuthCode'
+                ],
+                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/scenarios/permissions/{role}',
+                'operation_id': 'get_scenario_permissions',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'organization_id',
+                    'workspace_id',
+                    'role',
+                ],
+                'required': [
+                    'organization_id',
+                    'workspace_id',
+                    'role',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'organization_id':
+                        (str,),
+                    'workspace_id':
+                        (str,),
+                    'role':
+                        (str,),
+                },
+                'attribute_map': {
+                    'organization_id': 'organization_id',
+                    'workspace_id': 'workspace_id',
+                    'role': 'role',
+                },
+                'location_map': {
+                    'organization_id': 'path',
+                    'workspace_id': 'path',
+                    'role': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.get_scenario_security_endpoint = _Endpoint(
+            settings={
+                'response_type': (ScenarioSecurity,),
+                'auth': [
+                    'oAuth2AuthCode'
+                ],
+                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/security',
+                'operation_id': 'get_scenario_security',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'organization_id',
+                    'workspace_id',
+                    'scenario_id',
+                ],
+                'required': [
+                    'organization_id',
+                    'workspace_id',
+                    'scenario_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'organization_id':
+                        (str,),
+                    'workspace_id':
+                        (str,),
+                    'scenario_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'organization_id': 'organization_id',
+                    'workspace_id': 'workspace_id',
+                    'scenario_id': 'scenario_id',
+                },
+                'location_map': {
+                    'organization_id': 'path',
+                    'workspace_id': 'path',
+                    'scenario_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.get_scenario_security_users_endpoint = _Endpoint(
+            settings={
+                'response_type': ([str],),
+                'auth': [
+                    'oAuth2AuthCode'
+                ],
+                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/security/users',
+                'operation_id': 'get_scenario_security_users',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'organization_id',
+                    'workspace_id',
+                    'scenario_id',
+                ],
+                'required': [
+                    'organization_id',
+                    'workspace_id',
+                    'scenario_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'organization_id':
+                        (str,),
+                    'workspace_id':
+                        (str,),
+                    'scenario_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'organization_id': 'organization_id',
+                    'workspace_id': 'workspace_id',
+                    'scenario_id': 'scenario_id',
+                },
+                'location_map': {
+                    'organization_id': 'path',
+                    'workspace_id': 'path',
+                    'scenario_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.get_scenario_validation_status_by_id_endpoint = _Endpoint(
             settings={
                 'response_type': (ScenarioValidationStatus,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
                 'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/ValidationStatus',
@@ -868,14 +1149,78 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.import_scenario_endpoint = _Endpoint(
+            settings={
+                'response_type': (Scenario,),
+                'auth': [
+                    'oAuth2AuthCode'
+                ],
+                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/scenarios/import',
+                'operation_id': 'import_scenario',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'organization_id',
+                    'workspace_id',
+                    'scenario',
+                ],
+                'required': [
+                    'organization_id',
+                    'workspace_id',
+                    'scenario',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'organization_id':
+                        (str,),
+                    'workspace_id':
+                        (str,),
+                    'scenario':
+                        (Scenario,),
+                },
+                'attribute_map': {
+                    'organization_id': 'organization_id',
+                    'workspace_id': 'workspace_id',
+                },
+                'location_map': {
+                    'organization_id': 'path',
+                    'workspace_id': 'path',
+                    'scenario': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.remove_all_scenario_parameter_values_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'oAuth2AuthCode'
                 ],
                 'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/parameterValues',
@@ -929,35 +1274,37 @@
             },
             headers_map={
                 'accept': [],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.remove_all_users_of_scenario_endpoint = _Endpoint(
+        self.remove_scenario_access_control_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/users',
-                'operation_id': 'remove_all_users_of_scenario',
+                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/security/access/{identity_id}',
+                'operation_id': 'remove_scenario_access_control',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
                     'workspace_id',
                     'scenario_id',
+                    'identity_id',
                 ],
                 'required': [
                     'organization_id',
                     'workspace_id',
                     'scenario_id',
+                    'identity_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
@@ -970,57 +1317,61 @@
                 'openapi_types': {
                     'organization_id':
                         (str,),
                     'workspace_id':
                         (str,),
                     'scenario_id':
                         (str,),
+                    'identity_id':
+                        (str,),
                 },
                 'attribute_map': {
                     'organization_id': 'organization_id',
                     'workspace_id': 'workspace_id',
                     'scenario_id': 'scenario_id',
+                    'identity_id': 'identity_id',
                 },
                 'location_map': {
                     'organization_id': 'path',
                     'workspace_id': 'path',
                     'scenario_id': 'path',
+                    'identity_id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.remove_user_from_scenario_endpoint = _Endpoint(
+        self.set_scenario_default_security_endpoint = _Endpoint(
             settings={
-                'response_type': None,
+                'response_type': (ScenarioSecurity,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/users/{user_id}',
-                'operation_id': 'remove_user_from_scenario',
-                'http_method': 'DELETE',
+                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/security/default',
+                'operation_id': 'set_scenario_default_security',
+                'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
                     'workspace_id',
                     'scenario_id',
-                    'user_id',
+                    'scenario_role',
                 ],
                 'required': [
                     'organization_id',
                     'workspace_id',
                     'scenario_id',
-                    'user_id',
+                    'scenario_role',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
@@ -1033,35 +1384,39 @@
                 'openapi_types': {
                     'organization_id':
                         (str,),
                     'workspace_id':
                         (str,),
                     'scenario_id':
                         (str,),
-                    'user_id':
-                        (str,),
+                    'scenario_role':
+                        (ScenarioRole,),
                 },
                 'attribute_map': {
                     'organization_id': 'organization_id',
                     'workspace_id': 'workspace_id',
                     'scenario_id': 'scenario_id',
-                    'user_id': 'user_id',
                 },
                 'location_map': {
                     'organization_id': 'path',
                     'workspace_id': 'path',
                     'scenario_id': 'path',
-                    'user_id': 'path',
+                    'scenario_role': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [],
-                'content_type': [],
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json',
+                    'application/yaml'
+                ]
             },
             api_client=api_client
         )
         self.update_scenario_endpoint = _Endpoint(
             settings={
                 'response_type': (Scenario,),
                 'auth': [
@@ -1128,14 +1483,90 @@
                 'content_type': [
                     'application/json',
                     'application/yaml'
                 ]
             },
             api_client=api_client
         )
+        self.update_scenario_access_control_endpoint = _Endpoint(
+            settings={
+                'response_type': (ScenarioAccessControl,),
+                'auth': [
+                    'oAuth2AuthCode'
+                ],
+                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/security/access/{identity_id}',
+                'operation_id': 'update_scenario_access_control',
+                'http_method': 'PATCH',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'organization_id',
+                    'workspace_id',
+                    'scenario_id',
+                    'identity_id',
+                    'scenario_role',
+                ],
+                'required': [
+                    'organization_id',
+                    'workspace_id',
+                    'scenario_id',
+                    'identity_id',
+                    'scenario_role',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'organization_id':
+                        (str,),
+                    'workspace_id':
+                        (str,),
+                    'scenario_id':
+                        (str,),
+                    'identity_id':
+                        (str,),
+                    'scenario_role':
+                        (ScenarioRole,),
+                },
+                'attribute_map': {
+                    'organization_id': 'organization_id',
+                    'workspace_id': 'workspace_id',
+                    'scenario_id': 'scenario_id',
+                    'identity_id': 'identity_id',
+                },
+                'location_map': {
+                    'organization_id': 'path',
+                    'workspace_id': 'path',
+                    'scenario_id': 'path',
+                    'identity_id': 'path',
+                    'scenario_role': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
 
     def add_or_replace_scenario_parameter_values(
         self,
         organization_id,
         workspace_id,
         scenario_id,
         scenario_run_template_parameter_value,
@@ -1218,35 +1649,35 @@
             workspace_id
         kwargs['scenario_id'] = \
             scenario_id
         kwargs['scenario_run_template_parameter_value'] = \
             scenario_run_template_parameter_value
         return self.add_or_replace_scenario_parameter_values_endpoint.call_with_http_info(**kwargs)
 
-    def add_or_replace_users_in_scenario(
+    def add_scenario_access_control(
         self,
         organization_id,
         workspace_id,
         scenario_id,
-        scenario_user,
+        scenario_access_control,
         **kwargs
     ):
-        """Add (or replace) users in the Scenario specified  # noqa: E501
+        """Add a control access to the Scenario  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.add_or_replace_users_in_scenario(organization_id, workspace_id, scenario_id, scenario_user, async_req=True)
+        >>> thread = api.add_scenario_access_control(organization_id, workspace_id, scenario_id, scenario_access_control, async_req=True)
         >>> result = thread.get()
 
         Args:
             organization_id (str): the Organization identifier
             workspace_id (str): the Workspace identifier
             scenario_id (str): the Scenario identifier
-            scenario_user ([ScenarioUser]): the Users to add. Any User with the same ID is overwritten
+            scenario_access_control (ScenarioAccessControl): the new Scenario security access to add.
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1269,15 +1700,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            [ScenarioUser]
+            ScenarioAccessControl
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1303,17 +1734,17 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['organization_id'] = \
             organization_id
         kwargs['workspace_id'] = \
             workspace_id
         kwargs['scenario_id'] = \
             scenario_id
-        kwargs['scenario_user'] = \
-            scenario_user
-        return self.add_or_replace_users_in_scenario_endpoint.call_with_http_info(**kwargs)
+        kwargs['scenario_access_control'] = \
+            scenario_access_control
+        return self.add_scenario_access_control_endpoint.call_with_http_info(**kwargs)
 
     def compare_scenarios(
         self,
         organization_id,
         workspace_id,
         scenario_id,
         compared_scenario_id,
@@ -1752,14 +2183,16 @@
         >>> result = thread.get()
 
         Args:
             organization_id (str): the Organization identifier
             workspace_id (str): the Workspace identifier
 
         Keyword Args:
+            page (int): page number to query. [optional]
+            size (int): amount of result by page. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1835,14 +2268,16 @@
 
         Args:
             organization_id (str): the Organization identifier
             workspace_id (str): the Workspace identifier
             validation_status (ScenarioValidationStatus): the Scenario Validation Status
 
         Keyword Args:
+            page (int): page number to query. [optional]
+            size (int): amount of result by page. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1984,14 +2419,103 @@
             organization_id
         kwargs['workspace_id'] = \
             workspace_id
         kwargs['scenario_id'] = \
             scenario_id
         return self.find_scenario_by_id_endpoint.call_with_http_info(**kwargs)
 
+    def get_scenario_access_control(
+        self,
+        organization_id,
+        workspace_id,
+        scenario_id,
+        identity_id,
+        **kwargs
+    ):
+        """Get a control access for the Scenario  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_scenario_access_control(organization_id, workspace_id, scenario_id, identity_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            organization_id (str): the Organization identifier
+            workspace_id (str): the Workspace identifier
+            scenario_id (str): the Scenario identifier
+            identity_id (str): the User identifier
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ScenarioAccessControl
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['organization_id'] = \
+            organization_id
+        kwargs['workspace_id'] = \
+            workspace_id
+        kwargs['scenario_id'] = \
+            scenario_id
+        kwargs['identity_id'] = \
+            identity_id
+        return self.get_scenario_access_control_endpoint.call_with_http_info(**kwargs)
+
     def get_scenario_data_download_job_info(
         self,
         organization_id,
         workspace_id,
         scenario_id,
         download_id,
         **kwargs
@@ -2073,14 +2597,269 @@
             workspace_id
         kwargs['scenario_id'] = \
             scenario_id
         kwargs['download_id'] = \
             download_id
         return self.get_scenario_data_download_job_info_endpoint.call_with_http_info(**kwargs)
 
+    def get_scenario_permissions(
+        self,
+        organization_id,
+        workspace_id,
+        role,
+        **kwargs
+    ):
+        """Get the Scenario permission by given role  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_scenario_permissions(organization_id, workspace_id, role, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            organization_id (str): the Organization identifier
+            workspace_id (str): the Workspace identifier
+            role (str): the Role
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            [str]
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['organization_id'] = \
+            organization_id
+        kwargs['workspace_id'] = \
+            workspace_id
+        kwargs['role'] = \
+            role
+        return self.get_scenario_permissions_endpoint.call_with_http_info(**kwargs)
+
+    def get_scenario_security(
+        self,
+        organization_id,
+        workspace_id,
+        scenario_id,
+        **kwargs
+    ):
+        """Get the Scenario security information  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_scenario_security(organization_id, workspace_id, scenario_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            organization_id (str): the Organization identifier
+            workspace_id (str): the Workspace identifier
+            scenario_id (str): the Scenario identifier
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ScenarioSecurity
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['organization_id'] = \
+            organization_id
+        kwargs['workspace_id'] = \
+            workspace_id
+        kwargs['scenario_id'] = \
+            scenario_id
+        return self.get_scenario_security_endpoint.call_with_http_info(**kwargs)
+
+    def get_scenario_security_users(
+        self,
+        organization_id,
+        workspace_id,
+        scenario_id,
+        **kwargs
+    ):
+        """Get the Scenario security users list  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_scenario_security_users(organization_id, workspace_id, scenario_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            organization_id (str): the Organization identifier
+            workspace_id (str): the Workspace identifier
+            scenario_id (str): the Scenario identifier
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            [str]
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['organization_id'] = \
+            organization_id
+        kwargs['workspace_id'] = \
+            workspace_id
+        kwargs['scenario_id'] = \
+            scenario_id
+        return self.get_scenario_security_users_endpoint.call_with_http_info(**kwargs)
+
     def get_scenario_validation_status_by_id(
         self,
         organization_id,
         workspace_id,
         scenario_id,
         **kwargs
     ):
@@ -2239,14 +3018,99 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['organization_id'] = \
             organization_id
         kwargs['workspace_id'] = \
             workspace_id
         return self.get_scenarios_tree_endpoint.call_with_http_info(**kwargs)
 
+    def import_scenario(
+        self,
+        organization_id,
+        workspace_id,
+        scenario,
+        **kwargs
+    ):
+        """Import Scenario  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.import_scenario(organization_id, workspace_id, scenario, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            organization_id (str): the Organization identifier
+            workspace_id (str): the Workspace identifier
+            scenario (Scenario): the Scenario to import
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            Scenario
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['organization_id'] = \
+            organization_id
+        kwargs['workspace_id'] = \
+            workspace_id
+        kwargs['scenario'] = \
+            scenario
+        return self.import_scenario_endpoint.call_with_http_info(**kwargs)
+
     def remove_all_scenario_parameter_values(
         self,
         organization_id,
         workspace_id,
         scenario_id,
         **kwargs
     ):
@@ -2324,33 +3188,35 @@
             organization_id
         kwargs['workspace_id'] = \
             workspace_id
         kwargs['scenario_id'] = \
             scenario_id
         return self.remove_all_scenario_parameter_values_endpoint.call_with_http_info(**kwargs)
 
-    def remove_all_users_of_scenario(
+    def remove_scenario_access_control(
         self,
         organization_id,
         workspace_id,
         scenario_id,
+        identity_id,
         **kwargs
     ):
-        """Remove all users from the Scenario specified  # noqa: E501
+        """Remove the specified access from the given Organization Scenario  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.remove_all_users_of_scenario(organization_id, workspace_id, scenario_id, async_req=True)
+        >>> thread = api.remove_scenario_access_control(organization_id, workspace_id, scenario_id, identity_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             organization_id (str): the Organization identifier
             workspace_id (str): the Workspace identifier
             scenario_id (str): the Scenario identifier
+            identity_id (str): the User identifier
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -2407,37 +3273,39 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['organization_id'] = \
             organization_id
         kwargs['workspace_id'] = \
             workspace_id
         kwargs['scenario_id'] = \
             scenario_id
-        return self.remove_all_users_of_scenario_endpoint.call_with_http_info(**kwargs)
+        kwargs['identity_id'] = \
+            identity_id
+        return self.remove_scenario_access_control_endpoint.call_with_http_info(**kwargs)
 
-    def remove_user_from_scenario(
+    def set_scenario_default_security(
         self,
         organization_id,
         workspace_id,
         scenario_id,
-        user_id,
+        scenario_role,
         **kwargs
     ):
-        """Remove the specified user from the given Scenario  # noqa: E501
+        """Set the Scenario default security  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.remove_user_from_scenario(organization_id, workspace_id, scenario_id, user_id, async_req=True)
+        >>> thread = api.set_scenario_default_security(organization_id, workspace_id, scenario_id, scenario_role, async_req=True)
         >>> result = thread.get()
 
         Args:
             organization_id (str): the Organization identifier
             workspace_id (str): the Workspace identifier
             scenario_id (str): the Scenario identifier
-            user_id (str): the User identifier
+            scenario_role (ScenarioRole): the new Scenario default security.
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -2460,15 +3328,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            None
+            ScenarioSecurity
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -2494,17 +3362,17 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['organization_id'] = \
             organization_id
         kwargs['workspace_id'] = \
             workspace_id
         kwargs['scenario_id'] = \
             scenario_id
-        kwargs['user_id'] = \
-            user_id
-        return self.remove_user_from_scenario_endpoint.call_with_http_info(**kwargs)
+        kwargs['scenario_role'] = \
+            scenario_role
+        return self.set_scenario_default_security_endpoint.call_with_http_info(**kwargs)
 
     def update_scenario(
         self,
         organization_id,
         workspace_id,
         scenario_id,
         scenario,
@@ -2587,7 +3455,100 @@
             workspace_id
         kwargs['scenario_id'] = \
             scenario_id
         kwargs['scenario'] = \
             scenario
         return self.update_scenario_endpoint.call_with_http_info(**kwargs)
 
+    def update_scenario_access_control(
+        self,
+        organization_id,
+        workspace_id,
+        scenario_id,
+        identity_id,
+        scenario_role,
+        **kwargs
+    ):
+        """Update the specified access to User for a Scenario  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.update_scenario_access_control(organization_id, workspace_id, scenario_id, identity_id, scenario_role, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            organization_id (str): the Organization identifier
+            workspace_id (str): the Workspace identifier
+            scenario_id (str): the Scenario identifier
+            identity_id (str): the User identifier
+            scenario_role (ScenarioRole): The new Scenario Access Control
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ScenarioAccessControl
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['organization_id'] = \
+            organization_id
+        kwargs['workspace_id'] = \
+            workspace_id
+        kwargs['scenario_id'] = \
+            scenario_id
+        kwargs['identity_id'] = \
+            identity_id
+        kwargs['scenario_role'] = \
+            scenario_role
+        return self.update_scenario_access_control_endpoint.call_with_http_info(**kwargs)
+
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/api/scenariorun_api.py` & `cosmotech-api-2.4.0/cosmotech_api/api/scenariorun_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -515,14 +515,16 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
                     'workspace_id',
                     'scenario_id',
+                    'page',
+                    'size',
                 ],
                 'required': [
                     'organization_id',
                     'workspace_id',
                     'scenario_id',
                 ],
                 'nullable': [
@@ -540,24 +542,32 @@
                 'openapi_types': {
                     'organization_id':
                         (str,),
                     'workspace_id':
                         (str,),
                     'scenario_id':
                         (str,),
+                    'page':
+                        (int,),
+                    'size':
+                        (int,),
                 },
                 'attribute_map': {
                     'organization_id': 'organization_id',
                     'workspace_id': 'workspace_id',
                     'scenario_id': 'scenario_id',
+                    'page': 'page',
+                    'size': 'size',
                 },
                 'location_map': {
                     'organization_id': 'path',
                     'workspace_id': 'path',
                     'scenario_id': 'path',
+                    'page': 'query',
+                    'size': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -577,14 +587,16 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
                     'workspace_id',
+                    'page',
+                    'size',
                 ],
                 'required': [
                     'organization_id',
                     'workspace_id',
                 ],
                 'nullable': [
                 ],
@@ -599,34 +611,112 @@
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'organization_id':
                         (str,),
                     'workspace_id':
                         (str,),
+                    'page':
+                        (int,),
+                    'size':
+                        (int,),
                 },
                 'attribute_map': {
                     'organization_id': 'organization_id',
                     'workspace_id': 'workspace_id',
+                    'page': 'page',
+                    'size': 'size',
                 },
                 'location_map': {
                     'organization_id': 'path',
                     'workspace_id': 'path',
+                    'page': 'query',
+                    'size': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.import_scenario_run_endpoint = _Endpoint(
+            settings={
+                'response_type': (ScenarioRun,),
+                'auth': [
+                    'oAuth2AuthCode'
+                ],
+                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/run/import',
+                'operation_id': 'import_scenario_run',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'organization_id',
+                    'workspace_id',
+                    'scenario_id',
+                    'scenario_run',
+                ],
+                'required': [
+                    'organization_id',
+                    'workspace_id',
+                    'scenario_id',
+                    'scenario_run',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'organization_id':
+                        (str,),
+                    'workspace_id':
+                        (str,),
+                    'scenario_id':
+                        (str,),
+                    'scenario_run':
+                        (ScenarioRun,),
+                },
+                'attribute_map': {
+                    'organization_id': 'organization_id',
+                    'workspace_id': 'workspace_id',
+                    'scenario_id': 'scenario_id',
+                },
+                'location_map': {
+                    'organization_id': 'path',
+                    'workspace_id': 'path',
+                    'scenario_id': 'path',
+                    'scenario_run': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.run_scenario_endpoint = _Endpoint(
             settings={
                 'response_type': (ScenarioRun,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
                 'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/scenarios/{scenario_id}/run',
@@ -697,14 +787,16 @@
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
                     'scenario_run_search',
+                    'page',
+                    'size',
                 ],
                 'required': [
                     'organization_id',
                     'scenario_run_search',
                 ],
                 'nullable': [
                 ],
@@ -719,21 +811,29 @@
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'organization_id':
                         (str,),
                     'scenario_run_search':
                         (ScenarioRunSearch,),
+                    'page':
+                        (int,),
+                    'size':
+                        (int,),
                 },
                 'attribute_map': {
                     'organization_id': 'organization_id',
+                    'page': 'page',
+                    'size': 'size',
                 },
                 'location_map': {
                     'organization_id': 'path',
                     'scenario_run_search': 'body',
+                    'page': 'query',
+                    'size': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -1530,14 +1630,16 @@
 
         Args:
             organization_id (str): the Organization identifier
             workspace_id (str): the Workspace identifier
             scenario_id (str): the Scenario identifier
 
         Keyword Args:
+            page (int): page number to query. [optional]
+            size (int): amount of result by page. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1613,14 +1715,16 @@
         >>> result = thread.get()
 
         Args:
             organization_id (str): the Organization identifier
             workspace_id (str): the Workspace identifier
 
         Keyword Args:
+            page (int): page number to query. [optional]
+            size (int): amount of result by page. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1675,14 +1779,103 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['organization_id'] = \
             organization_id
         kwargs['workspace_id'] = \
             workspace_id
         return self.get_workspace_scenario_runs_endpoint.call_with_http_info(**kwargs)
 
+    def import_scenario_run(
+        self,
+        organization_id,
+        workspace_id,
+        scenario_id,
+        scenario_run,
+        **kwargs
+    ):
+        """import a ScenarioRun for the Scenario  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.import_scenario_run(organization_id, workspace_id, scenario_id, scenario_run, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            organization_id (str): the Organization identifier
+            workspace_id (str): the Workspace identifier
+            scenario_id (str): the Scenario identifier
+            scenario_run (ScenarioRun): the ScenarioRun to import
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ScenarioRun
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['organization_id'] = \
+            organization_id
+        kwargs['workspace_id'] = \
+            workspace_id
+        kwargs['scenario_id'] = \
+            scenario_id
+        kwargs['scenario_run'] = \
+            scenario_run
+        return self.import_scenario_run_endpoint.call_with_http_info(**kwargs)
+
     def run_scenario(
         self,
         organization_id,
         workspace_id,
         scenario_id,
         **kwargs
     ):
@@ -1779,14 +1972,16 @@
         >>> result = thread.get()
 
         Args:
             organization_id (str): the Organization identifier
             scenario_run_search (ScenarioRunSearch): the ScenarioRun search parameters
 
         Keyword Args:
+            page (int): page number to query. [optional]
+            size (int): amount of result by page. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/api/solution_api.py` & `cosmotech-api-2.4.0/cosmotech_api/api/solution_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -486,14 +486,16 @@
                 'operation_id': 'find_all_solutions',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
+                    'page',
+                    'size',
                 ],
                 'required': [
                     'organization_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -505,20 +507,28 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'organization_id':
                         (str,),
+                    'page':
+                        (int,),
+                    'size':
+                        (int,),
                 },
                 'attribute_map': {
                     'organization_id': 'organization_id',
+                    'page': 'page',
+                    'size': 'size',
                 },
                 'location_map': {
                     'organization_id': 'path',
+                    'page': 'query',
+                    'size': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -580,14 +590,73 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.import_solution_endpoint = _Endpoint(
+            settings={
+                'response_type': (Solution,),
+                'auth': [
+                    'oAuth2AuthCode'
+                ],
+                'endpoint_path': '/organizations/{organization_id}/solutions/import',
+                'operation_id': 'import_solution',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'organization_id',
+                    'solution',
+                ],
+                'required': [
+                    'organization_id',
+                    'solution',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'organization_id':
+                        (str,),
+                    'solution':
+                        (Solution,),
+                },
+                'attribute_map': {
+                    'organization_id': 'organization_id',
+                },
+                'location_map': {
+                    'organization_id': 'path',
+                    'solution': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json',
+                    'application/yaml'
+                ]
+            },
+            api_client=api_client
+        )
         self.remove_all_run_templates_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'oAuth2AuthCode'
                 ],
                 'endpoint_path': '/organizations/{organization_id}/solutions/{solution_id}/runTemplates',
@@ -1569,14 +1638,16 @@
         >>> thread = api.find_all_solutions(organization_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             organization_id (str): the Organization identifier
 
         Keyword Args:
+            page (int): page number to query. [optional]
+            size (int): amount of result by page. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1710,14 +1781,95 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['organization_id'] = \
             organization_id
         kwargs['solution_id'] = \
             solution_id
         return self.find_solution_by_id_endpoint.call_with_http_info(**kwargs)
 
+    def import_solution(
+        self,
+        organization_id,
+        solution,
+        **kwargs
+    ):
+        """Import a solution  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.import_solution(organization_id, solution, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            organization_id (str): the Organization identifier
+            solution (Solution): the Solution to import
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            Solution
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['organization_id'] = \
+            organization_id
+        kwargs['solution'] = \
+            solution
+        return self.import_solution_endpoint.call_with_http_info(**kwargs)
+
     def remove_all_run_templates(
         self,
         organization_id,
         solution_id,
         **kwargs
     ):
         """Remove all Run Templates from the Solution specified  # noqa: E501
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/api/user_api.py` & `cosmotech-api-2.4.0/cosmotech_api/api/validator_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -18,226 +18,229 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from cosmotech_api.model.user import User
+from cosmotech_api.model.validator import Validator
+from cosmotech_api.model.validator_run import ValidatorRun
 
 
-class UserApi(object):
+class ValidatorApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.authorize_user_endpoint = _Endpoint(
+        self.create_validator_endpoint = _Endpoint(
             settings={
-                'response_type': None,
+                'response_type': (Validator,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/oauth2/authorize',
-                'operation_id': 'authorize_user',
-                'http_method': 'GET',
+                'endpoint_path': '/organizations/{organization_id}/datasets/validators',
+                'operation_id': 'create_validator',
+                'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
+                    'organization_id',
+                    'validator',
                 ],
-                'required': [],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                },
-                'attribute_map': {
-                },
-                'location_map': {
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-        self.find_all_users_endpoint = _Endpoint(
-            settings={
-                'response_type': ([User],),
-                'auth': [
-                    'oAuth2AuthCode'
-                ],
-                'endpoint_path': '/users',
-                'operation_id': 'find_all_users',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
+                'required': [
+                    'organization_id',
+                    'validator',
                 ],
-                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
+                    'organization_id':
+                        (str,),
+                    'validator':
+                        (Validator,),
                 },
                 'attribute_map': {
+                    'organization_id': 'organization_id',
                 },
                 'location_map': {
+                    'organization_id': 'path',
+                    'validator': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [],
+                'content_type': [
+                    'application/json',
+                    'application/yaml'
+                ]
             },
             api_client=api_client
         )
-        self.find_user_by_id_endpoint = _Endpoint(
+        self.create_validator_run_endpoint = _Endpoint(
             settings={
-                'response_type': (User,),
+                'response_type': (ValidatorRun,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/users/{user_id}',
-                'operation_id': 'find_user_by_id',
-                'http_method': 'GET',
+                'endpoint_path': '/organizations/{organization_id}/datasets/validators/{validator_id}/history',
+                'operation_id': 'create_validator_run',
+                'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'user_id',
+                    'organization_id',
+                    'validator_id',
+                    'validator_run',
                 ],
                 'required': [
-                    'user_id',
+                    'organization_id',
+                    'validator_id',
+                    'validator_run',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'user_id':
+                    'organization_id':
                         (str,),
+                    'validator_id':
+                        (str,),
+                    'validator_run':
+                        (ValidatorRun,),
                 },
                 'attribute_map': {
-                    'user_id': 'user_id',
+                    'organization_id': 'organization_id',
+                    'validator_id': 'validator_id',
                 },
                 'location_map': {
-                    'user_id': 'path',
+                    'organization_id': 'path',
+                    'validator_id': 'path',
+                    'validator_run': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [],
+                'content_type': [
+                    'application/json',
+                    'application/yaml'
+                ]
             },
             api_client=api_client
         )
-        self.get_current_user_endpoint = _Endpoint(
+        self.delete_validator_endpoint = _Endpoint(
             settings={
-                'response_type': (User,),
+                'response_type': None,
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/users/me',
-                'operation_id': 'get_current_user',
-                'http_method': 'GET',
+                'endpoint_path': '/organizations/{organization_id}/datasets/validators/{validator_id}',
+                'operation_id': 'delete_validator',
+                'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
+                    'organization_id',
+                    'validator_id',
+                ],
+                'required': [
+                    'organization_id',
+                    'validator_id',
                 ],
-                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
+                    'organization_id':
+                        (str,),
+                    'validator_id':
+                        (str,),
                 },
                 'attribute_map': {
+                    'organization_id': 'organization_id',
+                    'validator_id': 'validator_id',
                 },
                 'location_map': {
+                    'organization_id': 'path',
+                    'validator_id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [
-                    'application/json'
-                ],
+                'accept': [],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_organization_current_user_endpoint = _Endpoint(
+        self.delete_validator_run_endpoint = _Endpoint(
             settings={
-                'response_type': (User,),
+                'response_type': None,
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/organizations/{organization_id}/me',
-                'operation_id': 'get_organization_current_user',
-                'http_method': 'GET',
+                'endpoint_path': '/organizations/{organization_id}/datasets/validators/{validator_id}/history/{validatorrun_id}',
+                'operation_id': 'delete_validator_run',
+                'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
+                    'validator_id',
+                    'validatorrun_id',
                 ],
                 'required': [
                     'organization_id',
+                    'validator_id',
+                    'validatorrun_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
@@ -246,51 +249,57 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'organization_id':
                         (str,),
+                    'validator_id':
+                        (str,),
+                    'validatorrun_id':
+                        (str,),
                 },
                 'attribute_map': {
                     'organization_id': 'organization_id',
+                    'validator_id': 'validator_id',
+                    'validatorrun_id': 'validatorrun_id',
                 },
                 'location_map': {
                     'organization_id': 'path',
+                    'validator_id': 'path',
+                    'validatorrun_id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [
-                    'application/json'
-                ],
+                'accept': [],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_workspace_current_user_endpoint = _Endpoint(
+        self.find_all_validator_runs_endpoint = _Endpoint(
             settings={
-                'response_type': (User,),
+                'response_type': ([ValidatorRun],),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/me',
-                'operation_id': 'get_workspace_current_user',
+                'endpoint_path': '/organizations/{organization_id}/datasets/validators/{validator_id}/history',
+                'operation_id': 'find_all_validator_runs',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
-                    'workspace_id',
+                    'validator_id',
                 ],
                 'required': [
                     'organization_id',
-                    'workspace_id',
+                    'validator_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
@@ -299,226 +308,257 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'organization_id':
                         (str,),
-                    'workspace_id':
+                    'validator_id':
                         (str,),
                 },
                 'attribute_map': {
                     'organization_id': 'organization_id',
-                    'workspace_id': 'workspace_id',
+                    'validator_id': 'validator_id',
                 },
                 'location_map': {
                     'organization_id': 'path',
-                    'workspace_id': 'path',
+                    'validator_id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.register_user_endpoint = _Endpoint(
+        self.find_all_validators_endpoint = _Endpoint(
             settings={
-                'response_type': (User,),
+                'response_type': ([Validator],),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/users',
-                'operation_id': 'register_user',
-                'http_method': 'POST',
+                'endpoint_path': '/organizations/{organization_id}/datasets/validators',
+                'operation_id': 'find_all_validators',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'user',
+                    'organization_id',
                 ],
                 'required': [
-                    'user',
+                    'organization_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'user':
-                        (User,),
+                    'organization_id':
+                        (str,),
                 },
                 'attribute_map': {
+                    'organization_id': 'organization_id',
                 },
                 'location_map': {
-                    'user': 'body',
+                    'organization_id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [
-                    'application/json',
-                    'application/yaml'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
-        self.test_platform_endpoint = _Endpoint(
+        self.find_validator_by_id_endpoint = _Endpoint(
             settings={
-                'response_type': (str,),
+                'response_type': (Validator,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/test',
-                'operation_id': 'test_platform',
+                'endpoint_path': '/organizations/{organization_id}/datasets/validators/{validator_id}',
+                'operation_id': 'find_validator_by_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
+                    'organization_id',
+                    'validator_id',
+                ],
+                'required': [
+                    'organization_id',
+                    'validator_id',
                 ],
-                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
+                    'organization_id':
+                        (str,),
+                    'validator_id':
+                        (str,),
                 },
                 'attribute_map': {
+                    'organization_id': 'organization_id',
+                    'validator_id': 'validator_id',
                 },
                 'location_map': {
+                    'organization_id': 'path',
+                    'validator_id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
-                    'text/plain'
+                    'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.unregister_user_endpoint = _Endpoint(
+        self.find_validator_run_by_id_endpoint = _Endpoint(
             settings={
-                'response_type': None,
+                'response_type': (ValidatorRun,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/users/{user_id}',
-                'operation_id': 'unregister_user',
-                'http_method': 'DELETE',
+                'endpoint_path': '/organizations/{organization_id}/datasets/validators/{validator_id}/history/{validatorrun_id}',
+                'operation_id': 'find_validator_run_by_id',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'user_id',
+                    'organization_id',
+                    'validator_id',
+                    'validatorrun_id',
                 ],
                 'required': [
-                    'user_id',
+                    'organization_id',
+                    'validator_id',
+                    'validatorrun_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'user_id':
+                    'organization_id':
+                        (str,),
+                    'validator_id':
+                        (str,),
+                    'validatorrun_id':
                         (str,),
                 },
                 'attribute_map': {
-                    'user_id': 'user_id',
+                    'organization_id': 'organization_id',
+                    'validator_id': 'validator_id',
+                    'validatorrun_id': 'validatorrun_id',
                 },
                 'location_map': {
-                    'user_id': 'path',
+                    'organization_id': 'path',
+                    'validator_id': 'path',
+                    'validatorrun_id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [],
+                'accept': [
+                    'application/json'
+                ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.update_user_endpoint = _Endpoint(
+        self.run_validator_endpoint = _Endpoint(
             settings={
-                'response_type': (User,),
+                'response_type': (ValidatorRun,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/users/{user_id}',
-                'operation_id': 'update_user',
-                'http_method': 'PATCH',
+                'endpoint_path': '/organizations/{organization_id}/datasets/validators/{validator_id}/run',
+                'operation_id': 'run_validator',
+                'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'user_id',
-                    'user',
+                    'organization_id',
+                    'validator_id',
+                    'validator_run',
                 ],
                 'required': [
-                    'user_id',
-                    'user',
+                    'organization_id',
+                    'validator_id',
+                    'validator_run',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'user_id':
+                    'organization_id':
                         (str,),
-                    'user':
-                        (User,),
+                    'validator_id':
+                        (str,),
+                    'validator_run':
+                        (ValidatorRun,),
                 },
                 'attribute_map': {
-                    'user_id': 'user_id',
+                    'organization_id': 'organization_id',
+                    'validator_id': 'validator_id',
                 },
                 'location_map': {
-                    'user_id': 'path',
-                    'user': 'body',
+                    'organization_id': 'path',
+                    'validator_id': 'path',
+                    'validator_run': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -527,98 +567,31 @@
                     'application/json',
                     'application/yaml'
                 ]
             },
             api_client=api_client
         )
 
-    def authorize_user(
-        self,
-        **kwargs
-    ):
-        """Authorize an User with OAuth2. Delegated to configured OAuth2 service  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.authorize_user(async_req=True)
-        >>> result = thread.get()
-
-
-        Keyword Args:
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            None
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        return self.authorize_user_endpoint.call_with_http_info(**kwargs)
-
-    def find_all_users(
+    def create_validator(
         self,
+        organization_id,
+        validator,
         **kwargs
     ):
-        """List all Users  # noqa: E501
+        """Register a new validator  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_all_users(async_req=True)
+        >>> thread = api.create_validator(organization_id, validator, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            organization_id (str): the Organization identifier
+            validator (Validator): the Validator to create
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -641,15 +614,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            [User]
+            Validator
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -669,31 +642,39 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        return self.find_all_users_endpoint.call_with_http_info(**kwargs)
+        kwargs['organization_id'] = \
+            organization_id
+        kwargs['validator'] = \
+            validator
+        return self.create_validator_endpoint.call_with_http_info(**kwargs)
 
-    def find_user_by_id(
+    def create_validator_run(
         self,
-        user_id,
+        organization_id,
+        validator_id,
+        validator_run,
         **kwargs
     ):
-        """Get the details of an user  # noqa: E501
+        """Register a new validator run  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_user_by_id(user_id, async_req=True)
+        >>> thread = api.create_validator_run(organization_id, validator_id, validator_run, async_req=True)
         >>> result = thread.get()
 
         Args:
-            user_id (str): the User identifier
+            organization_id (str): the Organization identifier
+            validator_id (str): the ValidatorRun identifier
+            validator_run (ValidatorRun): the Validator Run to create
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -716,15 +697,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            User
+            ValidatorRun
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -744,30 +725,39 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['user_id'] = \
-            user_id
-        return self.find_user_by_id_endpoint.call_with_http_info(**kwargs)
+        kwargs['organization_id'] = \
+            organization_id
+        kwargs['validator_id'] = \
+            validator_id
+        kwargs['validator_run'] = \
+            validator_run
+        return self.create_validator_run_endpoint.call_with_http_info(**kwargs)
 
-    def get_current_user(
+    def delete_validator(
         self,
+        organization_id,
+        validator_id,
         **kwargs
     ):
-        """Get the details of the logged-in User  # noqa: E501
+        """Delete a validator  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_current_user(async_req=True)
+        >>> thread = api.delete_validator(organization_id, validator_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            organization_id (str): the Organization identifier
+            validator_id (str): the Validator identifier
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -790,15 +780,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            User
+            None
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -818,31 +808,39 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        return self.get_current_user_endpoint.call_with_http_info(**kwargs)
+        kwargs['organization_id'] = \
+            organization_id
+        kwargs['validator_id'] = \
+            validator_id
+        return self.delete_validator_endpoint.call_with_http_info(**kwargs)
 
-    def get_organization_current_user(
+    def delete_validator_run(
         self,
         organization_id,
+        validator_id,
+        validatorrun_id,
         **kwargs
     ):
-        """Get the details of a logged-in User with roles for an Organization  # noqa: E501
+        """Delete a validator run  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_organization_current_user(organization_id, async_req=True)
+        >>> thread = api.delete_validator_run(organization_id, validator_id, validatorrun_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             organization_id (str): the Organization identifier
+            validator_id (str): the Validator identifier
+            validatorrun_id (str): the Validator Run identifier
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -865,15 +863,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            User
+            None
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -895,33 +893,37 @@
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['organization_id'] = \
             organization_id
-        return self.get_organization_current_user_endpoint.call_with_http_info(**kwargs)
+        kwargs['validator_id'] = \
+            validator_id
+        kwargs['validatorrun_id'] = \
+            validatorrun_id
+        return self.delete_validator_run_endpoint.call_with_http_info(**kwargs)
 
-    def get_workspace_current_user(
+    def find_all_validator_runs(
         self,
         organization_id,
-        workspace_id,
+        validator_id,
         **kwargs
     ):
-        """Get the details of the logged-in user with roles for a Workspace  # noqa: E501
+        """List all Validator Runs  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_workspace_current_user(organization_id, workspace_id, async_req=True)
+        >>> thread = api.find_all_validator_runs(organization_id, validator_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             organization_id (str): the Organization identifier
-            workspace_id (str): the Workspace identifier
+            validator_id (str): the ValidatorRun identifier
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -944,15 +946,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            User
+            [ValidatorRun]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -974,33 +976,33 @@
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['organization_id'] = \
             organization_id
-        kwargs['workspace_id'] = \
-            workspace_id
-        return self.get_workspace_current_user_endpoint.call_with_http_info(**kwargs)
+        kwargs['validator_id'] = \
+            validator_id
+        return self.find_all_validator_runs_endpoint.call_with_http_info(**kwargs)
 
-    def register_user(
+    def find_all_validators(
         self,
-        user,
+        organization_id,
         **kwargs
     ):
-        """Register a new user  # noqa: E501
+        """List all Validators  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.register_user(user, async_req=True)
+        >>> thread = api.find_all_validators(organization_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            user (User): the User to register
+            organization_id (str): the Organization identifier
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1023,15 +1025,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            User
+            [Validator]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1051,30 +1053,35 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['user'] = \
-            user
-        return self.register_user_endpoint.call_with_http_info(**kwargs)
+        kwargs['organization_id'] = \
+            organization_id
+        return self.find_all_validators_endpoint.call_with_http_info(**kwargs)
 
-    def test_platform(
+    def find_validator_by_id(
         self,
+        organization_id,
+        validator_id,
         **kwargs
     ):
-        """test platform API call  # noqa: E501
+        """Get the details of a validator  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.test_platform(async_req=True)
+        >>> thread = api.find_validator_by_id(organization_id, validator_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            organization_id (str): the Organization identifier
+            validator_id (str): the Validator identifier
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1097,15 +1104,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            str
+            Validator
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1125,31 +1132,39 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        return self.test_platform_endpoint.call_with_http_info(**kwargs)
+        kwargs['organization_id'] = \
+            organization_id
+        kwargs['validator_id'] = \
+            validator_id
+        return self.find_validator_by_id_endpoint.call_with_http_info(**kwargs)
 
-    def unregister_user(
+    def find_validator_run_by_id(
         self,
-        user_id,
+        organization_id,
+        validator_id,
+        validatorrun_id,
         **kwargs
     ):
-        """Unregister an user  # noqa: E501
+        """Get the details of a validator run  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.unregister_user(user_id, async_req=True)
+        >>> thread = api.find_validator_run_by_id(organization_id, validator_id, validatorrun_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            user_id (str): the User identifier
+            organization_id (str): the Organization identifier
+            validator_id (str): the Validator identifier
+            validatorrun_id (str): the Validator Run identifier
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1172,15 +1187,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            None
+            ValidatorRun
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1200,35 +1215,41 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['user_id'] = \
-            user_id
-        return self.unregister_user_endpoint.call_with_http_info(**kwargs)
+        kwargs['organization_id'] = \
+            organization_id
+        kwargs['validator_id'] = \
+            validator_id
+        kwargs['validatorrun_id'] = \
+            validatorrun_id
+        return self.find_validator_run_by_id_endpoint.call_with_http_info(**kwargs)
 
-    def update_user(
+    def run_validator(
         self,
-        user_id,
-        user,
+        organization_id,
+        validator_id,
+        validator_run,
         **kwargs
     ):
-        """Update a User  # noqa: E501
+        """Run a Validator  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_user(user_id, user, async_req=True)
+        >>> thread = api.run_validator(organization_id, validator_id, validator_run, async_req=True)
         >>> result = thread.get()
 
         Args:
-            user_id (str): the User identifier
-            user (User): the new User details. Organization membership is handled via the /organizations endpoint.
+            organization_id (str): the Organization identifier
+            validator_id (str): the ValidatorRun identifier
+            validator_run (ValidatorRun): the Validator to run
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1251,15 +1272,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            User
+            ValidatorRun
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1279,13 +1300,15 @@
         )
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['user_id'] = \
-            user_id
-        kwargs['user'] = \
-            user
-        return self.update_user_endpoint.call_with_http_info(**kwargs)
+        kwargs['organization_id'] = \
+            organization_id
+        kwargs['validator_id'] = \
+            validator_id
+        kwargs['validator_run'] = \
+            validator_run
+        return self.run_validator_endpoint.call_with_http_info(**kwargs)
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/api/workspace_api.py` & `cosmotech-api-2.4.0/cosmotech_api/api/workspace_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -19,51 +19,53 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from cosmotech_api.model.workspace import Workspace
+from cosmotech_api.model.workspace_access_control import WorkspaceAccessControl
 from cosmotech_api.model.workspace_file import WorkspaceFile
+from cosmotech_api.model.workspace_role import WorkspaceRole
 from cosmotech_api.model.workspace_secret import WorkspaceSecret
-from cosmotech_api.model.workspace_user import WorkspaceUser
+from cosmotech_api.model.workspace_security import WorkspaceSecurity
 
 
 class WorkspaceApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.add_or_replace_users_in_organization_workspace_endpoint = _Endpoint(
+        self.add_workspace_access_control_endpoint = _Endpoint(
             settings={
-                'response_type': ([WorkspaceUser],),
+                'response_type': (WorkspaceAccessControl,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/users',
-                'operation_id': 'add_or_replace_users_in_organization_workspace',
+                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/security/access',
+                'operation_id': 'add_workspace_access_control',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
                     'workspace_id',
-                    'workspace_user',
+                    'workspace_access_control',
                 ],
                 'required': [
                     'organization_id',
                     'workspace_id',
-                    'workspace_user',
+                    'workspace_access_control',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
@@ -74,35 +76,36 @@
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'organization_id':
                         (str,),
                     'workspace_id':
                         (str,),
-                    'workspace_user':
-                        ([WorkspaceUser],),
+                    'workspace_access_control':
+                        (WorkspaceAccessControl,),
                 },
                 'attribute_map': {
                     'organization_id': 'organization_id',
                     'workspace_id': 'workspace_id',
                 },
                 'location_map': {
                     'organization_id': 'path',
                     'workspace_id': 'path',
-                    'workspace_user': 'body',
+                    'workspace_access_control': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [
-                    'application/json'
+                    'application/json',
+                    'application/yaml'
                 ]
             },
             api_client=api_client
         )
         self.create_secret_endpoint = _Endpoint(
             settings={
                 'response_type': None,
@@ -528,14 +531,16 @@
                 'operation_id': 'find_all_workspaces',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
+                    'page',
+                    'size',
                 ],
                 'required': [
                     'organization_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -547,20 +552,28 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'organization_id':
                         (str,),
+                    'page':
+                        (int,),
+                    'size':
+                        (int,),
                 },
                 'attribute_map': {
                     'organization_id': 'organization_id',
+                    'page': 'page',
+                    'size': 'size',
                 },
                 'location_map': {
                     'organization_id': 'path',
+                    'page': 'query',
+                    'size': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -622,33 +635,35 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.remove_all_users_of_workspace_endpoint = _Endpoint(
+        self.get_workspace_access_control_endpoint = _Endpoint(
             settings={
-                'response_type': None,
+                'response_type': (WorkspaceAccessControl,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/users',
-                'operation_id': 'remove_all_users_of_workspace',
-                'http_method': 'DELETE',
+                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/security/access/{identity_id}',
+                'operation_id': 'get_workspace_access_control',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
                     'workspace_id',
+                    'identity_id',
                 ],
                 'required': [
                     'organization_id',
                     'workspace_id',
+                    'identity_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
@@ -659,53 +674,295 @@
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'organization_id':
                         (str,),
                     'workspace_id':
                         (str,),
+                    'identity_id':
+                        (str,),
                 },
                 'attribute_map': {
                     'organization_id': 'organization_id',
                     'workspace_id': 'workspace_id',
+                    'identity_id': 'identity_id',
                 },
                 'location_map': {
                     'organization_id': 'path',
                     'workspace_id': 'path',
+                    'identity_id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [],
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.get_workspace_permissions_endpoint = _Endpoint(
+            settings={
+                'response_type': ([str],),
+                'auth': [
+                    'oAuth2AuthCode'
+                ],
+                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/permissions/{role}',
+                'operation_id': 'get_workspace_permissions',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'organization_id',
+                    'workspace_id',
+                    'role',
+                ],
+                'required': [
+                    'organization_id',
+                    'workspace_id',
+                    'role',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'organization_id':
+                        (str,),
+                    'workspace_id':
+                        (str,),
+                    'role':
+                        (str,),
+                },
+                'attribute_map': {
+                    'organization_id': 'organization_id',
+                    'workspace_id': 'workspace_id',
+                    'role': 'role',
+                },
+                'location_map': {
+                    'organization_id': 'path',
+                    'workspace_id': 'path',
+                    'role': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.remove_user_from_organization_workspace_endpoint = _Endpoint(
+        self.get_workspace_security_endpoint = _Endpoint(
+            settings={
+                'response_type': (WorkspaceSecurity,),
+                'auth': [
+                    'oAuth2AuthCode'
+                ],
+                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/security',
+                'operation_id': 'get_workspace_security',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'organization_id',
+                    'workspace_id',
+                ],
+                'required': [
+                    'organization_id',
+                    'workspace_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'organization_id':
+                        (str,),
+                    'workspace_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'organization_id': 'organization_id',
+                    'workspace_id': 'workspace_id',
+                },
+                'location_map': {
+                    'organization_id': 'path',
+                    'workspace_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.get_workspace_security_users_endpoint = _Endpoint(
+            settings={
+                'response_type': ([str],),
+                'auth': [
+                    'oAuth2AuthCode'
+                ],
+                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/security/users',
+                'operation_id': 'get_workspace_security_users',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'organization_id',
+                    'workspace_id',
+                ],
+                'required': [
+                    'organization_id',
+                    'workspace_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'organization_id':
+                        (str,),
+                    'workspace_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'organization_id': 'organization_id',
+                    'workspace_id': 'workspace_id',
+                },
+                'location_map': {
+                    'organization_id': 'path',
+                    'workspace_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.import_workspace_endpoint = _Endpoint(
+            settings={
+                'response_type': (Workspace,),
+                'auth': [
+                    'oAuth2AuthCode'
+                ],
+                'endpoint_path': '/organizations/{organization_id}/workspaces/import',
+                'operation_id': 'import_workspace',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'organization_id',
+                    'workspace',
+                ],
+                'required': [
+                    'organization_id',
+                    'workspace',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'organization_id':
+                        (str,),
+                    'workspace':
+                        (Workspace,),
+                },
+                'attribute_map': {
+                    'organization_id': 'organization_id',
+                },
+                'location_map': {
+                    'organization_id': 'path',
+                    'workspace': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json',
+                    'application/yaml'
+                ]
+            },
+            api_client=api_client
+        )
+        self.remove_workspace_access_control_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'oAuth2AuthCode'
                 ],
-                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/users/{user_id}',
-                'operation_id': 'remove_user_from_organization_workspace',
+                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/security/access/{identity_id}',
+                'operation_id': 'remove_workspace_access_control',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'organization_id',
                     'workspace_id',
-                    'user_id',
+                    'identity_id',
                 ],
                 'required': [
                     'organization_id',
                     'workspace_id',
-                    'user_id',
+                    'identity_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
@@ -716,36 +973,101 @@
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'organization_id':
                         (str,),
                     'workspace_id':
                         (str,),
-                    'user_id':
+                    'identity_id':
                         (str,),
                 },
                 'attribute_map': {
                     'organization_id': 'organization_id',
                     'workspace_id': 'workspace_id',
-                    'user_id': 'user_id',
+                    'identity_id': 'identity_id',
                 },
                 'location_map': {
                     'organization_id': 'path',
                     'workspace_id': 'path',
-                    'user_id': 'path',
+                    'identity_id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.set_workspace_default_security_endpoint = _Endpoint(
+            settings={
+                'response_type': (WorkspaceSecurity,),
+                'auth': [
+                    'oAuth2AuthCode'
+                ],
+                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/security/default',
+                'operation_id': 'set_workspace_default_security',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'organization_id',
+                    'workspace_id',
+                    'workspace_role',
+                ],
+                'required': [
+                    'organization_id',
+                    'workspace_id',
+                    'workspace_role',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'organization_id':
+                        (str,),
+                    'workspace_id':
+                        (str,),
+                    'workspace_role':
+                        (WorkspaceRole,),
+                },
+                'attribute_map': {
+                    'organization_id': 'organization_id',
+                    'workspace_id': 'workspace_id',
+                },
+                'location_map': {
+                    'organization_id': 'path',
+                    'workspace_id': 'path',
+                    'workspace_role': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json',
+                    'application/yaml'
+                ]
+            },
+            api_client=api_client
+        )
         self.update_workspace_endpoint = _Endpoint(
             settings={
                 'response_type': (Workspace,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
                 'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}',
@@ -803,14 +1125,84 @@
                 'content_type': [
                     'application/json',
                     'application/yaml'
                 ]
             },
             api_client=api_client
         )
+        self.update_workspace_access_control_endpoint = _Endpoint(
+            settings={
+                'response_type': (WorkspaceAccessControl,),
+                'auth': [
+                    'oAuth2AuthCode'
+                ],
+                'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/security/access/{identity_id}',
+                'operation_id': 'update_workspace_access_control',
+                'http_method': 'PATCH',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'organization_id',
+                    'workspace_id',
+                    'identity_id',
+                    'workspace_role',
+                ],
+                'required': [
+                    'organization_id',
+                    'workspace_id',
+                    'identity_id',
+                    'workspace_role',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'organization_id':
+                        (str,),
+                    'workspace_id':
+                        (str,),
+                    'identity_id':
+                        (str,),
+                    'workspace_role':
+                        (WorkspaceRole,),
+                },
+                'attribute_map': {
+                    'organization_id': 'organization_id',
+                    'workspace_id': 'workspace_id',
+                    'identity_id': 'identity_id',
+                },
+                'location_map': {
+                    'organization_id': 'path',
+                    'workspace_id': 'path',
+                    'identity_id': 'path',
+                    'workspace_role': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.upload_workspace_file_endpoint = _Endpoint(
             settings={
                 'response_type': (WorkspaceFile,),
                 'auth': [
                     'oAuth2AuthCode'
                 ],
                 'endpoint_path': '/organizations/{organization_id}/workspaces/{workspace_id}/files',
@@ -879,33 +1271,33 @@
                 'content_type': [
                     'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
 
-    def add_or_replace_users_in_organization_workspace(
+    def add_workspace_access_control(
         self,
         organization_id,
         workspace_id,
-        workspace_user,
+        workspace_access_control,
         **kwargs
     ):
-        """Add (or replace) users to the Workspace specified  # noqa: E501
+        """Add a control access to the Workspace  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.add_or_replace_users_in_organization_workspace(organization_id, workspace_id, workspace_user, async_req=True)
+        >>> thread = api.add_workspace_access_control(organization_id, workspace_id, workspace_access_control, async_req=True)
         >>> result = thread.get()
 
         Args:
             organization_id (str): the Organization identifier
             workspace_id (str): the Workspace identifier
-            workspace_user ([WorkspaceUser]): the Users to add. Any User with the same ID is overwritten
+            workspace_access_control (WorkspaceAccessControl): the new Workspace security access to add.
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -928,15 +1320,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            [WorkspaceUser]
+            WorkspaceAccessControl
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -960,17 +1352,17 @@
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['organization_id'] = \
             organization_id
         kwargs['workspace_id'] = \
             workspace_id
-        kwargs['workspace_user'] = \
-            workspace_user
-        return self.add_or_replace_users_in_organization_workspace_endpoint.call_with_http_info(**kwargs)
+        kwargs['workspace_access_control'] = \
+            workspace_access_control
+        return self.add_workspace_access_control_endpoint.call_with_http_info(**kwargs)
 
     def create_secret(
         self,
         organization_id,
         workspace_id,
         workspace_secret,
         **kwargs
@@ -1560,14 +1952,16 @@
         >>> thread = api.find_all_workspaces(organization_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             organization_id (str): the Organization identifier
 
         Keyword Args:
+            page (int): page number to query. [optional]
+            size (int): amount of result by page. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1701,31 +2095,33 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['organization_id'] = \
             organization_id
         kwargs['workspace_id'] = \
             workspace_id
         return self.find_workspace_by_id_endpoint.call_with_http_info(**kwargs)
 
-    def remove_all_users_of_workspace(
+    def get_workspace_access_control(
         self,
         organization_id,
         workspace_id,
+        identity_id,
         **kwargs
     ):
-        """Remove all users from the Workspace specified  # noqa: E501
+        """Get a control access for the Workspace  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.remove_all_users_of_workspace(organization_id, workspace_id, async_req=True)
+        >>> thread = api.get_workspace_access_control(organization_id, workspace_id, identity_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             organization_id (str): the Organization identifier
             workspace_id (str): the Workspace identifier
+            identity_id (str): the User identifier
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1748,15 +2144,183 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            None
+            WorkspaceAccessControl
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['organization_id'] = \
+            organization_id
+        kwargs['workspace_id'] = \
+            workspace_id
+        kwargs['identity_id'] = \
+            identity_id
+        return self.get_workspace_access_control_endpoint.call_with_http_info(**kwargs)
+
+    def get_workspace_permissions(
+        self,
+        organization_id,
+        workspace_id,
+        role,
+        **kwargs
+    ):
+        """Get the Workspace permission by given role  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_workspace_permissions(organization_id, workspace_id, role, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            organization_id (str): the Organization identifier
+            workspace_id (str): the Workspace identifier
+            role (str): the Role
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            [str]
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['organization_id'] = \
+            organization_id
+        kwargs['workspace_id'] = \
+            workspace_id
+        kwargs['role'] = \
+            role
+        return self.get_workspace_permissions_endpoint.call_with_http_info(**kwargs)
+
+    def get_workspace_security(
+        self,
+        organization_id,
+        workspace_id,
+        **kwargs
+    ):
+        """Get the Workspace security information  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_workspace_security(organization_id, workspace_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            organization_id (str): the Organization identifier
+            workspace_id (str): the Workspace identifier
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            WorkspaceSecurity
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1780,35 +2344,197 @@
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['organization_id'] = \
             organization_id
         kwargs['workspace_id'] = \
             workspace_id
-        return self.remove_all_users_of_workspace_endpoint.call_with_http_info(**kwargs)
+        return self.get_workspace_security_endpoint.call_with_http_info(**kwargs)
+
+    def get_workspace_security_users(
+        self,
+        organization_id,
+        workspace_id,
+        **kwargs
+    ):
+        """Get the Workspace security users list  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_workspace_security_users(organization_id, workspace_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            organization_id (str): the Organization identifier
+            workspace_id (str): the Workspace identifier
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            [str]
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['organization_id'] = \
+            organization_id
+        kwargs['workspace_id'] = \
+            workspace_id
+        return self.get_workspace_security_users_endpoint.call_with_http_info(**kwargs)
+
+    def import_workspace(
+        self,
+        organization_id,
+        workspace,
+        **kwargs
+    ):
+        """Import a workspace  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.import_workspace(organization_id, workspace, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            organization_id (str): the Organization identifier
+            workspace (Workspace): the Workspace to import
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            Workspace
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['organization_id'] = \
+            organization_id
+        kwargs['workspace'] = \
+            workspace
+        return self.import_workspace_endpoint.call_with_http_info(**kwargs)
 
-    def remove_user_from_organization_workspace(
+    def remove_workspace_access_control(
         self,
         organization_id,
         workspace_id,
-        user_id,
+        identity_id,
         **kwargs
     ):
-        """Remove the specified user from the given Organization Workspace  # noqa: E501
+        """Remove the specified access from the given Organization Workspace  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.remove_user_from_organization_workspace(organization_id, workspace_id, user_id, async_req=True)
+        >>> thread = api.remove_workspace_access_control(organization_id, workspace_id, identity_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             organization_id (str): the Organization identifier
             workspace_id (str): the Workspace identifier
-            user_id (str): the User identifier
+            identity_id (str): the User identifier
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1863,17 +2589,102 @@
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['organization_id'] = \
             organization_id
         kwargs['workspace_id'] = \
             workspace_id
-        kwargs['user_id'] = \
-            user_id
-        return self.remove_user_from_organization_workspace_endpoint.call_with_http_info(**kwargs)
+        kwargs['identity_id'] = \
+            identity_id
+        return self.remove_workspace_access_control_endpoint.call_with_http_info(**kwargs)
+
+    def set_workspace_default_security(
+        self,
+        organization_id,
+        workspace_id,
+        workspace_role,
+        **kwargs
+    ):
+        """Set the Workspace default security  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.set_workspace_default_security(organization_id, workspace_id, workspace_role, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            organization_id (str): the Organization identifier
+            workspace_id (str): the Workspace identifier
+            workspace_role (WorkspaceRole): the new Workspace default security.
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            WorkspaceSecurity
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['organization_id'] = \
+            organization_id
+        kwargs['workspace_id'] = \
+            workspace_id
+        kwargs['workspace_role'] = \
+            workspace_role
+        return self.set_workspace_default_security_endpoint.call_with_http_info(**kwargs)
 
     def update_workspace(
         self,
         organization_id,
         workspace_id,
         workspace,
         **kwargs
@@ -1885,15 +2696,15 @@
 
         >>> thread = api.update_workspace(organization_id, workspace_id, workspace, async_req=True)
         >>> result = thread.get()
 
         Args:
             organization_id (str): the Organization identifier
             workspace_id (str): the Workspace identifier
-            workspace (Workspace): the new Workspace details.
+            workspace (Workspace): The new Workspace details.
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1952,14 +2763,103 @@
             organization_id
         kwargs['workspace_id'] = \
             workspace_id
         kwargs['workspace'] = \
             workspace
         return self.update_workspace_endpoint.call_with_http_info(**kwargs)
 
+    def update_workspace_access_control(
+        self,
+        organization_id,
+        workspace_id,
+        identity_id,
+        workspace_role,
+        **kwargs
+    ):
+        """Update the specified access to User for a Workspace  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.update_workspace_access_control(organization_id, workspace_id, identity_id, workspace_role, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            organization_id (str): the Organization identifier
+            workspace_id (str): the Workspace identifier
+            identity_id (str): the User identifier
+            workspace_role (WorkspaceRole): The new Workspace Access Control
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            WorkspaceAccessControl
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['organization_id'] = \
+            organization_id
+        kwargs['workspace_id'] = \
+            workspace_id
+        kwargs['identity_id'] = \
+            identity_id
+        kwargs['workspace_role'] = \
+            workspace_role
+        return self.update_workspace_access_control_endpoint.call_with_http_info(**kwargs)
+
     def upload_workspace_file(
         self,
         organization_id,
         workspace_id,
         file,
         **kwargs
     ):
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/api_client.py` & `cosmotech-api-2.4.0/cosmotech_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/apis/__init__.py` & `cosmotech-api-2.4.0/cosmotech_api/apis/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,10 +16,10 @@
 # Import APIs into API package:
 from cosmotech_api.api.connector_api import ConnectorApi
 from cosmotech_api.api.dataset_api import DatasetApi
 from cosmotech_api.api.organization_api import OrganizationApi
 from cosmotech_api.api.scenario_api import ScenarioApi
 from cosmotech_api.api.scenariorun_api import ScenariorunApi
 from cosmotech_api.api.solution_api import SolutionApi
-from cosmotech_api.api.user_api import UserApi
+from cosmotech_api.api.twingraph_api import TwingraphApi
 from cosmotech_api.api.validator_api import ValidatorApi
 from cosmotech_api.api.workspace_api import WorkspaceApi
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/configuration.py` & `cosmotech-api-2.4.0/cosmotech_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
@@ -384,15 +384,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.1.3-SNAPSHOT\n"\
+               "Version of the API: 2.4.0-dev\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/exceptions.py` & `cosmotech-api-2.4.0/cosmotech_api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/component_role_permissions.py` & `cosmotech-api-2.4.0/cosmotech_api/model/component_role_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/connector.py` & `cosmotech-api-2.4.0/cosmotech_api/model/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/connector_parameter.py` & `cosmotech-api-2.4.0/cosmotech_api/model/connector_parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/connector_parameter_group.py` & `cosmotech-api-2.4.0/cosmotech_api/model/connector_parameter_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/container_resource_size_info.py` & `cosmotech-api-2.4.0/cosmotech_api/model/container_resource_size_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/container_resource_sizing.py` & `cosmotech-api-2.4.0/cosmotech_api/model/container_resource_sizing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/dataset.py` & `cosmotech-api-2.4.0/cosmotech_api/model/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -90,16 +90,17 @@
         """
         lazy_import()
         return {
             'id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'owner_id': (str,),  # noqa: E501
+            'organization_id': (str,),  # noqa: E501
             'tags': ([str],),  # noqa: E501
-            'connector': (DatasetConnector,),  # noqa: E501
+            'connector': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'fragments_ids': ([str],),  # noqa: E501
             'validator_id': (str,),  # noqa: E501
             'compatibility': ([DatasetCompatibility],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
@@ -107,24 +108,26 @@
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'name': 'name',  # noqa: E501
         'description': 'description',  # noqa: E501
         'owner_id': 'ownerId',  # noqa: E501
+        'organization_id': 'organizationId',  # noqa: E501
         'tags': 'tags',  # noqa: E501
         'connector': 'connector',  # noqa: E501
         'fragments_ids': 'fragmentsIds',  # noqa: E501
         'validator_id': 'validatorId',  # noqa: E501
         'compatibility': 'compatibility',  # noqa: E501
     }
 
     read_only_vars = {
         'id',  # noqa: E501
         'owner_id',  # noqa: E501
+        'organization_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
@@ -161,16 +164,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): the Dataset unique identifier. [optional]  # noqa: E501
             name (str): the Dataset name. [optional]  # noqa: E501
             description (str): the Dataset description. [optional]  # noqa: E501
             owner_id (str): the User id which own this Dataset. [optional]  # noqa: E501
+            organization_id (str): the Organization Id related to this Dataset. [optional]  # noqa: E501
             tags ([str]): the list of tags. [optional]  # noqa: E501
-            connector (DatasetConnector): [optional]  # noqa: E501
+            connector (bool, date, datetime, dict, float, int, list, str, none_type): the Connector setup bound to a Dataset. [optional]  # noqa: E501
             fragments_ids ([str]): the list of other Datasets ids to compose as fragments. [optional]  # noqa: E501
             validator_id (str): the validator id. [optional]  # noqa: E501
             compatibility ([DatasetCompatibility]): the list of compatible Solutions versions. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -251,16 +255,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): the Dataset unique identifier. [optional]  # noqa: E501
             name (str): the Dataset name. [optional]  # noqa: E501
             description (str): the Dataset description. [optional]  # noqa: E501
             owner_id (str): the User id which own this Dataset. [optional]  # noqa: E501
+            organization_id (str): the Organization Id related to this Dataset. [optional]  # noqa: E501
             tags ([str]): the list of tags. [optional]  # noqa: E501
-            connector (DatasetConnector): [optional]  # noqa: E501
+            connector (bool, date, datetime, dict, float, int, list, str, none_type): the Connector setup bound to a Dataset. [optional]  # noqa: E501
             fragments_ids ([str]): the list of other Datasets ids to compose as fragments. [optional]  # noqa: E501
             validator_id (str): the validator id. [optional]  # noqa: E501
             compatibility ([DatasetCompatibility]): the list of compatible Solutions versions. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/dataset_compatibility.py` & `cosmotech-api-2.4.0/cosmotech_api/model/dataset_compatibility.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/dataset_connector.py` & `cosmotech-api-2.4.0/cosmotech_api/model/dataset_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/dataset_copy_parameters.py` & `cosmotech-api-2.4.0/cosmotech_api/model/dataset_copy_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/dataset_search.py` & `cosmotech-api-2.4.0/cosmotech_api/model/dataset_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/delete_historical_data.py` & `cosmotech-api-2.4.0/cosmotech_api/model/delete_historical_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/organization.py` & `cosmotech-api-2.4.0/cosmotech_api/model/organization.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,18 +27,18 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from cosmotech_api.exceptions import ApiAttributeError
 
 
 def lazy_import():
+    from cosmotech_api.model.organization_security import OrganizationSecurity
     from cosmotech_api.model.organization_services import OrganizationServices
-    from cosmotech_api.model.organization_user import OrganizationUser
+    globals()['OrganizationSecurity'] = OrganizationSecurity
     globals()['OrganizationServices'] = OrganizationServices
-    globals()['OrganizationUser'] = OrganizationUser
 
 
 class Organization(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -89,29 +89,29 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'owner_id': (str,),  # noqa: E501
-            'users': ([OrganizationUser],),  # noqa: E501
             'services': (OrganizationServices,),  # noqa: E501
+            'security': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'name': 'name',  # noqa: E501
         'owner_id': 'ownerId',  # noqa: E501
-        'users': 'users',  # noqa: E501
         'services': 'services',  # noqa: E501
+        'security': 'security',  # noqa: E501
     }
 
     read_only_vars = {
         'id',  # noqa: E501
         'owner_id',  # noqa: E501
     }
 
@@ -152,16 +152,16 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): the Organization unique identifier. [optional]  # noqa: E501
             name (str): the Organization name. [optional]  # noqa: E501
             owner_id (str): the Owner User Id. [optional]  # noqa: E501
-            users ([OrganizationUser]): [optional]  # noqa: E501
             services (OrganizationServices): [optional]  # noqa: E501
+            security (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -238,16 +238,16 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): the Organization unique identifier. [optional]  # noqa: E501
             name (str): the Organization name. [optional]  # noqa: E501
             owner_id (str): the Owner User Id. [optional]  # noqa: E501
-            users ([OrganizationUser]): [optional]  # noqa: E501
             services (OrganizationServices): [optional]  # noqa: E501
+            security (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/organization_access_control.py` & `cosmotech-api-2.4.0/cosmotech_api/model/organization_access_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/organization_role.py` & `cosmotech-api-2.4.0/cosmotech_api/model/organization_role.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/organization_security.py` & `cosmotech-api-2.4.0/cosmotech_api/model/organization_security.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/organization_service.py` & `cosmotech-api-2.4.0/cosmotech_api/model/organization_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/organization_services.py` & `cosmotech-api-2.4.0/cosmotech_api/model/organization_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/organization_user.py` & `cosmotech-api-2.4.0/cosmotech_api/model/organization_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Plaform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.3.4-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/resource_size_info.py` & `cosmotech-api-2.4.0/cosmotech_api/model/resource_size_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/run_template.py` & `cosmotech-api-2.4.0/cosmotech_api/model/run_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -28,16 +28,18 @@
     OpenApiModel
 )
 from cosmotech_api.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from cosmotech_api.model.delete_historical_data import DeleteHistoricalData
+    from cosmotech_api.model.run_template_resource_sizing import RunTemplateResourceSizing
     from cosmotech_api.model.run_template_step_source import RunTemplateStepSource
     globals()['DeleteHistoricalData'] = DeleteHistoricalData
+    globals()['RunTemplateResourceSizing'] = RunTemplateResourceSizing
     globals()['RunTemplateStepSource'] = RunTemplateStepSource
 
 
 class RunTemplate(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -92,14 +94,15 @@
         return {
             'id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'csm_simulation': (str,),  # noqa: E501
             'tags': ([str],),  # noqa: E501
             'compute_size': (str,),  # noqa: E501
+            'run_sizing': (RunTemplateResourceSizing,),  # noqa: E501
             'no_data_ingestion_state': (bool,),  # noqa: E501
             'fetch_datasets': (bool,),  # noqa: E501
             'scenario_data_download_transform': (bool,),  # noqa: E501
             'fetch_scenario_parameters': (bool,),  # noqa: E501
             'apply_parameters': (bool,),  # noqa: E501
             'validate_data': (bool,),  # noqa: E501
             'send_datasets_to_data_warehouse': (bool,),  # noqa: E501
@@ -131,14 +134,15 @@
     attribute_map = {
         'id': 'id',  # noqa: E501
         'name': 'name',  # noqa: E501
         'description': 'description',  # noqa: E501
         'csm_simulation': 'csmSimulation',  # noqa: E501
         'tags': 'tags',  # noqa: E501
         'compute_size': 'computeSize',  # noqa: E501
+        'run_sizing': 'runSizing',  # noqa: E501
         'no_data_ingestion_state': 'noDataIngestionState',  # noqa: E501
         'fetch_datasets': 'fetchDatasets',  # noqa: E501
         'scenario_data_download_transform': 'scenarioDataDownloadTransform',  # noqa: E501
         'fetch_scenario_parameters': 'fetchScenarioParameters',  # noqa: E501
         'apply_parameters': 'applyParameters',  # noqa: E501
         'validate_data': 'validateData',  # noqa: E501
         'send_datasets_to_data_warehouse': 'sendDatasetsToDataWarehouse',  # noqa: E501
@@ -207,14 +211,15 @@
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             name (str): the Run Template name. [optional]  # noqa: E501
             description (str): the Run Template description. [optional]  # noqa: E501
             csm_simulation (str): the Cosmo Tech simulation name. This information is send to the Engine. Mandatory information if no Engine is defined. [optional]  # noqa: E501
             tags ([str]): the list of Run Template tags. [optional]  # noqa: E501
             compute_size (str): the compute size needed for this Run Template. Standard sizes are basic and highcpu. Default is basic. [optional]  # noqa: E501
+            run_sizing (RunTemplateResourceSizing): [optional]  # noqa: E501
             no_data_ingestion_state (bool): set to true if the run template does not want to check data ingestion state (no probes or not control plane). [optional]  # noqa: E501
             fetch_datasets (bool): whether or not the fetch dataset step is done. [optional]  # noqa: E501
             scenario_data_download_transform (bool): whether or not the scenario data download transform step step is done. [optional]  # noqa: E501
             fetch_scenario_parameters (bool): whether or not the fetch parameters step is done. [optional]  # noqa: E501
             apply_parameters (bool): whether or not the apply parameter step is done. [optional]  # noqa: E501
             validate_data (bool): whether or not the validate step is done. [optional]  # noqa: E501
             send_datasets_to_data_warehouse (bool): whether or not the Datasets values are send to the DataWarehouse prior to Simulation Run. If not set follow the Workspace setting. [optional]  # noqa: E501
@@ -322,14 +327,15 @@
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             name (str): the Run Template name. [optional]  # noqa: E501
             description (str): the Run Template description. [optional]  # noqa: E501
             csm_simulation (str): the Cosmo Tech simulation name. This information is send to the Engine. Mandatory information if no Engine is defined. [optional]  # noqa: E501
             tags ([str]): the list of Run Template tags. [optional]  # noqa: E501
             compute_size (str): the compute size needed for this Run Template. Standard sizes are basic and highcpu. Default is basic. [optional]  # noqa: E501
+            run_sizing (RunTemplateResourceSizing): [optional]  # noqa: E501
             no_data_ingestion_state (bool): set to true if the run template does not want to check data ingestion state (no probes or not control plane). [optional]  # noqa: E501
             fetch_datasets (bool): whether or not the fetch dataset step is done. [optional]  # noqa: E501
             scenario_data_download_transform (bool): whether or not the scenario data download transform step step is done. [optional]  # noqa: E501
             fetch_scenario_parameters (bool): whether or not the fetch parameters step is done. [optional]  # noqa: E501
             apply_parameters (bool): whether or not the apply parameter step is done. [optional]  # noqa: E501
             validate_data (bool): whether or not the validate step is done. [optional]  # noqa: E501
             send_datasets_to_data_warehouse (bool): whether or not the Datasets values are send to the DataWarehouse prior to Simulation Run. If not set follow the Workspace setting. [optional]  # noqa: E501
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/run_template_handler_id.py` & `cosmotech-api-2.4.0/cosmotech_api/model/run_template_handler_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/run_template_parameter.py` & `cosmotech-api-2.4.0/cosmotech_api/model/run_template_parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/run_template_parameter_group.py` & `cosmotech-api-2.4.0/cosmotech_api/model/run_template_parameter_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/run_template_parameter_value.py` & `cosmotech-api-2.4.0/cosmotech_api/model/run_template_parameter_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/run_template_resource_sizing.py` & `cosmotech-api-2.4.0/cosmotech_api/model/run_template_resource_sizing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/run_template_step_source.py` & `cosmotech-api-2.4.0/cosmotech_api/model/run_template_step_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -29,21 +29,23 @@
 )
 from cosmotech_api.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from cosmotech_api.model.scenario_job_state import ScenarioJobState
     from cosmotech_api.model.scenario_last_run import ScenarioLastRun
+    from cosmotech_api.model.scenario_resource_sizing import ScenarioResourceSizing
     from cosmotech_api.model.scenario_run_template_parameter_value import ScenarioRunTemplateParameterValue
-    from cosmotech_api.model.scenario_user import ScenarioUser
+    from cosmotech_api.model.scenario_security import ScenarioSecurity
     from cosmotech_api.model.scenario_validation_status import ScenarioValidationStatus
     globals()['ScenarioJobState'] = ScenarioJobState
     globals()['ScenarioLastRun'] = ScenarioLastRun
+    globals()['ScenarioResourceSizing'] = ScenarioResourceSizing
     globals()['ScenarioRunTemplateParameterValue'] = ScenarioRunTemplateParameterValue
-    globals()['ScenarioUser'] = ScenarioUser
+    globals()['ScenarioSecurity'] = ScenarioSecurity
     globals()['ScenarioValidationStatus'] = ScenarioValidationStatus
 
 
 class Scenario(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -101,28 +103,30 @@
             'description': (str,),  # noqa: E501
             'tags': ([str],),  # noqa: E501
             'parent_id': (str,),  # noqa: E501
             'owner_id': (str,),  # noqa: E501
             'root_id': (str,),  # noqa: E501
             'solution_id': (str,),  # noqa: E501
             'run_template_id': (str,),  # noqa: E501
+            'organization_id': (str,),  # noqa: E501
             'workspace_id': (str,),  # noqa: E501
-            'users': ([ScenarioUser],),  # noqa: E501
             'state': (ScenarioJobState,),  # noqa: E501
-            'creation_date': (datetime,),  # noqa: E501
-            'last_update': (datetime,),  # noqa: E501
+            'creation_date': (int,),  # noqa: E501
+            'last_update': (int,),  # noqa: E501
             'owner_name': (str,),  # noqa: E501
             'solution_name': (str,),  # noqa: E501
             'run_template_name': (str,),  # noqa: E501
             'dataset_list': ([str],),  # noqa: E501
+            'run_sizing': (ScenarioResourceSizing,),  # noqa: E501
             'parameters_values': ([ScenarioRunTemplateParameterValue],),  # noqa: E501
             'last_run': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'parent_last_run': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'root_last_run': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'validation_status': (ScenarioValidationStatus,),  # noqa: E501
+            'validation_status': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'security': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -132,35 +136,38 @@
         'description': 'description',  # noqa: E501
         'tags': 'tags',  # noqa: E501
         'parent_id': 'parentId',  # noqa: E501
         'owner_id': 'ownerId',  # noqa: E501
         'root_id': 'rootId',  # noqa: E501
         'solution_id': 'solutionId',  # noqa: E501
         'run_template_id': 'runTemplateId',  # noqa: E501
+        'organization_id': 'organizationId',  # noqa: E501
         'workspace_id': 'workspaceId',  # noqa: E501
-        'users': 'users',  # noqa: E501
         'state': 'state',  # noqa: E501
         'creation_date': 'creationDate',  # noqa: E501
         'last_update': 'lastUpdate',  # noqa: E501
         'owner_name': 'ownerName',  # noqa: E501
         'solution_name': 'solutionName',  # noqa: E501
         'run_template_name': 'runTemplateName',  # noqa: E501
         'dataset_list': 'datasetList',  # noqa: E501
+        'run_sizing': 'runSizing',  # noqa: E501
         'parameters_values': 'parametersValues',  # noqa: E501
         'last_run': 'lastRun',  # noqa: E501
         'parent_last_run': 'parentLastRun',  # noqa: E501
         'root_last_run': 'rootLastRun',  # noqa: E501
         'validation_status': 'validationStatus',  # noqa: E501
+        'security': 'security',  # noqa: E501
     }
 
     read_only_vars = {
         'id',  # noqa: E501
         'owner_id',  # noqa: E501
         'root_id',  # noqa: E501
         'solution_id',  # noqa: E501
+        'organization_id',  # noqa: E501
         'workspace_id',  # noqa: E501
         'creation_date',  # noqa: E501
         'last_update',  # noqa: E501
         'owner_name',  # noqa: E501
         'solution_name',  # noqa: E501
         'run_template_name',  # noqa: E501
     }
@@ -208,28 +215,30 @@
             description (str): the Scenario description. [optional]  # noqa: E501
             tags ([str]): the list of tags. [optional]  # noqa: E501
             parent_id (str): the Scenario parent id. [optional]  # noqa: E501
             owner_id (str): the user id which own this Scenario. [optional]  # noqa: E501
             root_id (str): the scenario root id. [optional]  # noqa: E501
             solution_id (str): the Solution Id associated with this Scenario. [optional]  # noqa: E501
             run_template_id (str): the Solution Run Template Id associated with this Scenario. [optional]  # noqa: E501
+            organization_id (str): the associated Organization Id. [optional]  # noqa: E501
             workspace_id (str): the associated Workspace Id. [optional]  # noqa: E501
-            users ([ScenarioUser]): the list of users Id with their role. [optional]  # noqa: E501
             state (ScenarioJobState): [optional]  # noqa: E501
-            creation_date (datetime): the Scenario creation date. [optional]  # noqa: E501
-            last_update (datetime): the last time a Scenario was updated. [optional]  # noqa: E501
+            creation_date (int): the Scenario creation date. [optional]  # noqa: E501
+            last_update (int): the last time a Scenario was updated. [optional]  # noqa: E501
             owner_name (str): the name of the owner. [optional]  # noqa: E501
             solution_name (str): the Solution name. [optional]  # noqa: E501
             run_template_name (str): the Solution Run Template name associated with this Scenario. [optional]  # noqa: E501
             dataset_list ([str]): the list of Dataset Id associated to this Scenario Run Template. [optional]  # noqa: E501
+            run_sizing (ScenarioResourceSizing): [optional]  # noqa: E501
             parameters_values ([ScenarioRunTemplateParameterValue]): the list of Solution Run Template parameters values. [optional]  # noqa: E501
             last_run (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             parent_last_run (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             root_last_run (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            validation_status (ScenarioValidationStatus): [optional]  # noqa: E501
+            validation_status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            security (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -312,28 +321,30 @@
             description (str): the Scenario description. [optional]  # noqa: E501
             tags ([str]): the list of tags. [optional]  # noqa: E501
             parent_id (str): the Scenario parent id. [optional]  # noqa: E501
             owner_id (str): the user id which own this Scenario. [optional]  # noqa: E501
             root_id (str): the scenario root id. [optional]  # noqa: E501
             solution_id (str): the Solution Id associated with this Scenario. [optional]  # noqa: E501
             run_template_id (str): the Solution Run Template Id associated with this Scenario. [optional]  # noqa: E501
+            organization_id (str): the associated Organization Id. [optional]  # noqa: E501
             workspace_id (str): the associated Workspace Id. [optional]  # noqa: E501
-            users ([ScenarioUser]): the list of users Id with their role. [optional]  # noqa: E501
             state (ScenarioJobState): [optional]  # noqa: E501
-            creation_date (datetime): the Scenario creation date. [optional]  # noqa: E501
-            last_update (datetime): the last time a Scenario was updated. [optional]  # noqa: E501
+            creation_date (int): the Scenario creation date. [optional]  # noqa: E501
+            last_update (int): the last time a Scenario was updated. [optional]  # noqa: E501
             owner_name (str): the name of the owner. [optional]  # noqa: E501
             solution_name (str): the Solution name. [optional]  # noqa: E501
             run_template_name (str): the Solution Run Template name associated with this Scenario. [optional]  # noqa: E501
             dataset_list ([str]): the list of Dataset Id associated to this Scenario Run Template. [optional]  # noqa: E501
+            run_sizing (ScenarioResourceSizing): [optional]  # noqa: E501
             parameters_values ([ScenarioRunTemplateParameterValue]): the list of Solution Run Template parameters values. [optional]  # noqa: E501
             last_run (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             parent_last_run (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             root_last_run (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            validation_status (ScenarioValidationStatus): [optional]  # noqa: E501
+            validation_status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            security (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario_access_control.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario_access_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario_changed_parameter_value.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario_changed_parameter_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario_comparison_result.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario_comparison_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario_data_download_info.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario_data_download_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario_data_download_job.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario_data_download_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario_job_state.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario_job_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario_last_run.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario_last_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario_resource_sizing.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario_resource_sizing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario_role.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario_run.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -89,15 +89,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'id': (str,),  # noqa: E501
-            'state': (ScenarioRunState,),  # noqa: E501
+            'state': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'organization_id': (str,),  # noqa: E501
             'workflow_id': (str,),  # noqa: E501
             'csm_simulation_run': (str,),  # noqa: E501
             'generate_name': (str,),  # noqa: E501
             'workflow_name': (str,),  # noqa: E501
             'owner_id': (str,),  # noqa: E501
             'workspace_id': (str,),  # noqa: E501
@@ -198,15 +198,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): the ScenarioRun. [optional]  # noqa: E501
-            state (ScenarioRunState): [optional]  # noqa: E501
+            state (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             organization_id (str): the Organization id. [optional]  # noqa: E501
             workflow_id (str): the Cosmo Tech compute cluster Argo Workflow Id to search. [optional]  # noqa: E501
             csm_simulation_run (str): the Cosmo Tech Simulation Run Id. [optional]  # noqa: E501
             generate_name (str): the base name for workflow name generation. [optional]  # noqa: E501
             workflow_name (str): the Cosmo Tech compute cluster Argo Workflow Name. [optional]  # noqa: E501
             owner_id (str): the user id which own this scenariorun. [optional]  # noqa: E501
             workspace_id (str): the Workspace Id. [optional]  # noqa: E501
@@ -301,15 +301,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): the ScenarioRun. [optional]  # noqa: E501
-            state (ScenarioRunState): [optional]  # noqa: E501
+            state (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             organization_id (str): the Organization id. [optional]  # noqa: E501
             workflow_id (str): the Cosmo Tech compute cluster Argo Workflow Id to search. [optional]  # noqa: E501
             csm_simulation_run (str): the Cosmo Tech Simulation Run Id. [optional]  # noqa: E501
             generate_name (str): the base name for workflow name generation. [optional]  # noqa: E501
             workflow_name (str): the Cosmo Tech compute cluster Argo Workflow Name. [optional]  # noqa: E501
             owner_id (str): the user id which own this scenariorun. [optional]  # noqa: E501
             workspace_id (str): the Workspace Id. [optional]  # noqa: E501
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario_run_container.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_container.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,15 +27,17 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from cosmotech_api.exceptions import ApiAttributeError
 
 
 def lazy_import():
+    from cosmotech_api.model.container_resource_sizing import ContainerResourceSizing
     from cosmotech_api.model.scenario_run_container_artifact import ScenarioRunContainerArtifact
+    globals()['ContainerResourceSizing'] = ContainerResourceSizing
     globals()['ScenarioRunContainerArtifact'] = ScenarioRunContainerArtifact
 
 
 class ScenarioRunContainer(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -93,14 +95,16 @@
             'id': (str,),  # noqa: E501
             'labels': ({str: (str,)},),  # noqa: E501
             'env_vars': ({str: (str,)},),  # noqa: E501
             'entrypoint': (str,),  # noqa: E501
             'run_args': ([str],),  # noqa: E501
             'dependencies': ([str],),  # noqa: E501
             'solution_container': (bool,),  # noqa: E501
+            'node_label': (str,),  # noqa: E501
+            'run_sizing': (ContainerResourceSizing,),  # noqa: E501
             'artifacts': ([ScenarioRunContainerArtifact],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -111,14 +115,16 @@
         'id': 'id',  # noqa: E501
         'labels': 'labels',  # noqa: E501
         'env_vars': 'envVars',  # noqa: E501
         'entrypoint': 'entrypoint',  # noqa: E501
         'run_args': 'runArgs',  # noqa: E501
         'dependencies': 'dependencies',  # noqa: E501
         'solution_container': 'solutionContainer',  # noqa: E501
+        'node_label': 'nodeLabel',  # noqa: E501
+        'run_sizing': 'runSizing',  # noqa: E501
         'artifacts': 'artifacts',  # noqa: E501
     }
 
     read_only_vars = {
         'id',  # noqa: E501
         'solution_container',  # noqa: E501
     }
@@ -168,14 +174,16 @@
             id (str): the container Id. [optional]  # noqa: E501
             labels ({str: (str,)}): the metadata labels. [optional]  # noqa: E501
             env_vars ({str: (str,)}): environment variable map. [optional]  # noqa: E501
             entrypoint (str): the container entry point. [optional]  # noqa: E501
             run_args ([str]): the list of run arguments for the container. [optional]  # noqa: E501
             dependencies ([str]): the list of dependencies container name to run this container. [optional]  # noqa: E501
             solution_container (bool): whether or not this container is a Cosmo Tech solution container. [optional]  # noqa: E501
+            node_label (str): the node label request. [optional]  # noqa: E501
+            run_sizing (ContainerResourceSizing): [optional]  # noqa: E501
             artifacts ([ScenarioRunContainerArtifact]): the list of artifacts. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -263,14 +271,16 @@
             id (str): the container Id. [optional]  # noqa: E501
             labels ({str: (str,)}): the metadata labels. [optional]  # noqa: E501
             env_vars ({str: (str,)}): environment variable map. [optional]  # noqa: E501
             entrypoint (str): the container entry point. [optional]  # noqa: E501
             run_args ([str]): the list of run arguments for the container. [optional]  # noqa: E501
             dependencies ([str]): the list of dependencies container name to run this container. [optional]  # noqa: E501
             solution_container (bool): whether or not this container is a Cosmo Tech solution container. [optional]  # noqa: E501
+            node_label (str): the node label request. [optional]  # noqa: E501
+            run_sizing (ContainerResourceSizing): [optional]  # noqa: E501
             artifacts ([ScenarioRunContainerArtifact]): the list of artifacts. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario_run_container_artifact.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_container_artifact.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario_run_container_logs.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_container_logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario_run_logs.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario_run_search.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario_run_start_containers.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_start_containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario_run_state.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario_run_status.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario_run_status_node.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_status_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario_run_template_parameter_value.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario_run_template_parameter_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario_security.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario_security.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario_user.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Plaform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.3.4-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/scenario_validation_status.py` & `cosmotech-api-2.4.0/cosmotech_api/model/scenario_validation_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/solution.py` & `cosmotech-api-2.4.0/cosmotech_api/model/solution.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -89,14 +89,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'id': (str,),  # noqa: E501
+            'organization_id': (str,),  # noqa: E501
             'key': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'repository': (str,),  # noqa: E501
             'csm_simulator': (str,),  # noqa: E501
             'version': (str,),  # noqa: E501
             'owner_id': (str,),  # noqa: E501
@@ -111,14 +112,15 @@
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
+        'organization_id': 'organizationId',  # noqa: E501
         'key': 'key',  # noqa: E501
         'name': 'name',  # noqa: E501
         'description': 'description',  # noqa: E501
         'repository': 'repository',  # noqa: E501
         'csm_simulator': 'csmSimulator',  # noqa: E501
         'version': 'version',  # noqa: E501
         'owner_id': 'ownerId',  # noqa: E501
@@ -128,14 +130,15 @@
         'parameters': 'parameters',  # noqa: E501
         'parameter_groups': 'parameterGroups',  # noqa: E501
         'run_templates': 'runTemplates',  # noqa: E501
     }
 
     read_only_vars = {
         'id',  # noqa: E501
+        'organization_id',  # noqa: E501
         'owner_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
@@ -170,14 +173,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): the Solution version unique identifier. [optional]  # noqa: E501
+            organization_id (str): the Organization unique identifier. [optional]  # noqa: E501
             key (str): the Solution key which group Solution versions. [optional]  # noqa: E501
             name (str): the Solution name. [optional]  # noqa: E501
             description (str): the Solution description. [optional]  # noqa: E501
             repository (str): the registry repository containing the image. [optional]  # noqa: E501
             csm_simulator (str): the main Cosmo Tech simulator name used in standard Run Template. [optional]  # noqa: E501
             version (str): the Solution version MAJOR.MINOR.PATCH. Must be aligned with an existing repository tag. [optional]  # noqa: E501
             owner_id (str): the User id which own this Solution. [optional]  # noqa: E501
@@ -265,14 +269,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): the Solution version unique identifier. [optional]  # noqa: E501
+            organization_id (str): the Organization unique identifier. [optional]  # noqa: E501
             key (str): the Solution key which group Solution versions. [optional]  # noqa: E501
             name (str): the Solution name. [optional]  # noqa: E501
             description (str): the Solution description. [optional]  # noqa: E501
             repository (str): the registry repository containing the image. [optional]  # noqa: E501
             csm_simulator (str): the main Cosmo Tech simulator name used in standard Run Template. [optional]  # noqa: E501
             version (str): the Solution version MAJOR.MINOR.PATCH. Must be aligned with an existing repository tag. [optional]  # noqa: E501
             owner_id (str): the User id which own this Solution. [optional]  # noqa: E501
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/source_info.py` & `cosmotech-api-2.4.0/cosmotech_api/model/source_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/translated_labels.py` & `cosmotech-api-2.4.0/cosmotech_api/model/translated_labels.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/twin_graph_import.py` & `cosmotech-api-2.4.0/cosmotech_api/model/twin_graph_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/twin_graph_import_info.py` & `cosmotech-api-2.4.0/cosmotech_api/model/twin_graph_import_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/twin_graph_query.py` & `cosmotech-api-2.4.0/cosmotech_api/model/twin_graph_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/user.py` & `cosmotech-api-2.4.0/cosmotech_api/model/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.3.7
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/user_organization.py` & `cosmotech-api-2.4.0/cosmotech_api/model/user_organization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.3.7
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/user_workspace.py` & `cosmotech-api-2.4.0/cosmotech_api/model/user_workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.3.7
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/validator.py` & `cosmotech-api-2.4.0/cosmotech_api/model/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/validator_run.py` & `cosmotech-api-2.4.0/cosmotech_api/model/validator_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/workspace.py` & `cosmotech-api-2.4.0/cosmotech_api/model/workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from cosmotech_api.exceptions import ApiAttributeError
 
 
 def lazy_import():
+    from cosmotech_api.model.workspace_security import WorkspaceSecurity
     from cosmotech_api.model.workspace_solution import WorkspaceSolution
-    from cosmotech_api.model.workspace_user import WorkspaceUser
     from cosmotech_api.model.workspace_web_app import WorkspaceWebApp
+    globals()['WorkspaceSecurity'] = WorkspaceSecurity
     globals()['WorkspaceSolution'] = WorkspaceSolution
-    globals()['WorkspaceUser'] = WorkspaceUser
     globals()['WorkspaceWebApp'] = WorkspaceWebApp
 
 
 class Workspace(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -92,54 +92,57 @@
         """
         lazy_import()
         return {
             'key': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'solution': (WorkspaceSolution,),  # noqa: E501
             'id': (str,),  # noqa: E501
+            'organization_id': (str,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'version': (str,),  # noqa: E501
             'tags': ([str],),  # noqa: E501
             'owner_id': (str,),  # noqa: E501
-            'users': ([WorkspaceUser],),  # noqa: E501
             'web_app': (WorkspaceWebApp,),  # noqa: E501
             'send_input_to_data_warehouse': (bool,),  # noqa: E501
             'use_dedicated_event_hub_namespace': (bool,),  # noqa: E501
             'dedicated_event_hub_sas_key_name': (str,),  # noqa: E501
             'dedicated_event_hub_authentication_strategy': (str,),  # noqa: E501
             'send_scenario_run_to_event_hub': (bool,),  # noqa: E501
             'send_scenario_metadata_to_event_hub': (bool,),  # noqa: E501
+            'security': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'key': 'key',  # noqa: E501
         'name': 'name',  # noqa: E501
         'solution': 'solution',  # noqa: E501
         'id': 'id',  # noqa: E501
+        'organization_id': 'organizationId',  # noqa: E501
         'description': 'description',  # noqa: E501
         'version': 'version',  # noqa: E501
         'tags': 'tags',  # noqa: E501
         'owner_id': 'ownerId',  # noqa: E501
-        'users': 'users',  # noqa: E501
         'web_app': 'webApp',  # noqa: E501
         'send_input_to_data_warehouse': 'sendInputToDataWarehouse',  # noqa: E501
         'use_dedicated_event_hub_namespace': 'useDedicatedEventHubNamespace',  # noqa: E501
         'dedicated_event_hub_sas_key_name': 'dedicatedEventHubSasKeyName',  # noqa: E501
         'dedicated_event_hub_authentication_strategy': 'dedicatedEventHubAuthenticationStrategy',  # noqa: E501
         'send_scenario_run_to_event_hub': 'sendScenarioRunToEventHub',  # noqa: E501
         'send_scenario_metadata_to_event_hub': 'sendScenarioMetadataToEventHub',  # noqa: E501
+        'security': 'security',  # noqa: E501
     }
 
     read_only_vars = {
         'id',  # noqa: E501
+        'organization_id',  # noqa: E501
         'owner_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
@@ -179,26 +182,27 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): the Workspace version unique identifier. [optional]  # noqa: E501
+            organization_id (str): the Organization unique identifier. [optional]  # noqa: E501
             description (str): the Workspace description. [optional]  # noqa: E501
             version (str): the Workspace version MAJOR.MINOR.PATCH.. [optional]  # noqa: E501
             tags ([str]): the list of tags. [optional]  # noqa: E501
             owner_id (str): the user id which own this workspace. [optional]  # noqa: E501
-            users ([WorkspaceUser]): the list of users Id with their role. [optional]  # noqa: E501
             web_app (WorkspaceWebApp): [optional]  # noqa: E501
             send_input_to_data_warehouse (bool): default setting for all Scenarios and Run Templates to set whether or not the Dataset values and the input parameters values are send to the DataWarehouse prior to the ScenarioRun. [optional]  # noqa: E501
             use_dedicated_event_hub_namespace (bool): Set this property to true to use a dedicated Azure Event Hub Namespace for this Workspace. The Event Hub Namespace must be named \\'<organization_id\\>-<workspace_id\\>\\' (in lower case). This Namespace must also contain two Event Hubs named \\'probesmeasures\\' and \\'scenariorun\\'.. [optional] if omitted the server will use the default value of False  # noqa: E501
             dedicated_event_hub_sas_key_name (str): the Dedicated Event Hub SAS key name, default to RootManageSharedAccessKey. Use the /secret endpoint to set the key value. [optional]  # noqa: E501
             dedicated_event_hub_authentication_strategy (str): the Event Hub authentication strategy, SHARED_ACCESS_POLICY or TENANT_CLIENT_CREDENTIALS. Default to the one defined for the tenant.. [optional]  # noqa: E501
             send_scenario_run_to_event_hub (bool): default setting for all Scenarios and Run Templates to set whether or not the ScenarioRun is send to the Event Hub. [optional] if omitted the server will use the default value of True  # noqa: E501
             send_scenario_metadata_to_event_hub (bool): Set this property to false to not send scenario metada to Azure Event Hub Namespace for this Workspace. The Event Hub Namespace must be named \\'<organization_id\\>-<workspace_id\\>\\' (in lower case). This Namespace must also contain two Event Hubs named \\'scenariometadata\\' and \\'scenariorunmetadata\\'.. [optional] if omitted the server will use the default value of False  # noqa: E501
+            security (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -281,26 +285,27 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): the Workspace version unique identifier. [optional]  # noqa: E501
+            organization_id (str): the Organization unique identifier. [optional]  # noqa: E501
             description (str): the Workspace description. [optional]  # noqa: E501
             version (str): the Workspace version MAJOR.MINOR.PATCH.. [optional]  # noqa: E501
             tags ([str]): the list of tags. [optional]  # noqa: E501
             owner_id (str): the user id which own this workspace. [optional]  # noqa: E501
-            users ([WorkspaceUser]): the list of users Id with their role. [optional]  # noqa: E501
             web_app (WorkspaceWebApp): [optional]  # noqa: E501
             send_input_to_data_warehouse (bool): default setting for all Scenarios and Run Templates to set whether or not the Dataset values and the input parameters values are send to the DataWarehouse prior to the ScenarioRun. [optional]  # noqa: E501
             use_dedicated_event_hub_namespace (bool): Set this property to true to use a dedicated Azure Event Hub Namespace for this Workspace. The Event Hub Namespace must be named \\'<organization_id\\>-<workspace_id\\>\\' (in lower case). This Namespace must also contain two Event Hubs named \\'probesmeasures\\' and \\'scenariorun\\'.. [optional] if omitted the server will use the default value of False  # noqa: E501
             dedicated_event_hub_sas_key_name (str): the Dedicated Event Hub SAS key name, default to RootManageSharedAccessKey. Use the /secret endpoint to set the key value. [optional]  # noqa: E501
             dedicated_event_hub_authentication_strategy (str): the Event Hub authentication strategy, SHARED_ACCESS_POLICY or TENANT_CLIENT_CREDENTIALS. Default to the one defined for the tenant.. [optional]  # noqa: E501
             send_scenario_run_to_event_hub (bool): default setting for all Scenarios and Run Templates to set whether or not the ScenarioRun is send to the Event Hub. [optional] if omitted the server will use the default value of True  # noqa: E501
             send_scenario_metadata_to_event_hub (bool): Set this property to false to not send scenario metada to Azure Event Hub Namespace for this Workspace. The Event Hub Namespace must be named \\'<organization_id\\>-<workspace_id\\>\\' (in lower case). This Namespace must also contain two Event Hubs named \\'scenariometadata\\' and \\'scenariorunmetadata\\'.. [optional] if omitted the server will use the default value of False  # noqa: E501
+            security (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/workspace_access_control.py` & `cosmotech-api-2.4.0/cosmotech_api/model/workspace_access_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/workspace_file.py` & `cosmotech-api-2.4.0/cosmotech_api/model/workspace_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/workspace_role.py` & `cosmotech-api-2.4.0/cosmotech_api/model/workspace_role.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/workspace_secret.py` & `cosmotech-api-2.4.0/cosmotech_api/model/workspace_secret.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/workspace_security.py` & `cosmotech-api-2.4.0/cosmotech_api/model/workspace_security.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/workspace_solution.py` & `cosmotech-api-2.4.0/cosmotech_api/model/workspace_solution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/workspace_user.py` & `cosmotech-api-2.4.0/cosmotech_api/model/workspace_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Plaform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.3.4-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model/workspace_web_app.py` & `cosmotech-api-2.4.0/cosmotech_api/model/workspace_web_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/model_utils.py` & `cosmotech-api-2.4.0/cosmotech_api/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/models/__init__.py` & `cosmotech-api-2.4.0/cosmotech_api/models/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,59 +5,75 @@
 # raise a RecursionError
 # to avoid this, import only the models that you directly need like:
 # from from cosmotech_api.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
+from cosmotech_api.model.component_role_permissions import ComponentRolePermissions
 from cosmotech_api.model.connector import Connector
 from cosmotech_api.model.connector_parameter import ConnectorParameter
 from cosmotech_api.model.connector_parameter_group import ConnectorParameterGroup
+from cosmotech_api.model.container_resource_size_info import ContainerResourceSizeInfo
+from cosmotech_api.model.container_resource_sizing import ContainerResourceSizing
 from cosmotech_api.model.dataset import Dataset
 from cosmotech_api.model.dataset_compatibility import DatasetCompatibility
 from cosmotech_api.model.dataset_connector import DatasetConnector
 from cosmotech_api.model.dataset_copy_parameters import DatasetCopyParameters
 from cosmotech_api.model.dataset_search import DatasetSearch
 from cosmotech_api.model.delete_historical_data import DeleteHistoricalData
+from cosmotech_api.model.graph_properties import GraphProperties
 from cosmotech_api.model.organization import Organization
+from cosmotech_api.model.organization_access_control import OrganizationAccessControl
+from cosmotech_api.model.organization_role import OrganizationRole
+from cosmotech_api.model.organization_security import OrganizationSecurity
 from cosmotech_api.model.organization_service import OrganizationService
 from cosmotech_api.model.organization_services import OrganizationServices
-from cosmotech_api.model.organization_user import OrganizationUser
+from cosmotech_api.model.resource_size_info import ResourceSizeInfo
 from cosmotech_api.model.run_template import RunTemplate
 from cosmotech_api.model.run_template_handler_id import RunTemplateHandlerId
 from cosmotech_api.model.run_template_parameter import RunTemplateParameter
 from cosmotech_api.model.run_template_parameter_group import RunTemplateParameterGroup
 from cosmotech_api.model.run_template_parameter_value import RunTemplateParameterValue
+from cosmotech_api.model.run_template_resource_sizing import RunTemplateResourceSizing
 from cosmotech_api.model.run_template_step_source import RunTemplateStepSource
 from cosmotech_api.model.scenario import Scenario
+from cosmotech_api.model.scenario_access_control import ScenarioAccessControl
 from cosmotech_api.model.scenario_changed_parameter_value import ScenarioChangedParameterValue
 from cosmotech_api.model.scenario_comparison_result import ScenarioComparisonResult
 from cosmotech_api.model.scenario_data_download_info import ScenarioDataDownloadInfo
 from cosmotech_api.model.scenario_data_download_job import ScenarioDataDownloadJob
 from cosmotech_api.model.scenario_job_state import ScenarioJobState
 from cosmotech_api.model.scenario_last_run import ScenarioLastRun
+from cosmotech_api.model.scenario_resource_sizing import ScenarioResourceSizing
+from cosmotech_api.model.scenario_role import ScenarioRole
 from cosmotech_api.model.scenario_run import ScenarioRun
 from cosmotech_api.model.scenario_run_container import ScenarioRunContainer
 from cosmotech_api.model.scenario_run_container_artifact import ScenarioRunContainerArtifact
 from cosmotech_api.model.scenario_run_container_logs import ScenarioRunContainerLogs
 from cosmotech_api.model.scenario_run_logs import ScenarioRunLogs
 from cosmotech_api.model.scenario_run_search import ScenarioRunSearch
 from cosmotech_api.model.scenario_run_start_containers import ScenarioRunStartContainers
 from cosmotech_api.model.scenario_run_state import ScenarioRunState
 from cosmotech_api.model.scenario_run_status import ScenarioRunStatus
 from cosmotech_api.model.scenario_run_status_node import ScenarioRunStatusNode
 from cosmotech_api.model.scenario_run_template_parameter_value import ScenarioRunTemplateParameterValue
-from cosmotech_api.model.scenario_user import ScenarioUser
+from cosmotech_api.model.scenario_security import ScenarioSecurity
 from cosmotech_api.model.scenario_validation_status import ScenarioValidationStatus
 from cosmotech_api.model.solution import Solution
+from cosmotech_api.model.source_info import SourceInfo
 from cosmotech_api.model.translated_labels import TranslatedLabels
-from cosmotech_api.model.user import User
-from cosmotech_api.model.user_organization import UserOrganization
-from cosmotech_api.model.user_workspace import UserWorkspace
+from cosmotech_api.model.twin_graph_batch_result import TwinGraphBatchResult
+from cosmotech_api.model.twin_graph_hash import TwinGraphHash
+from cosmotech_api.model.twin_graph_import import TwinGraphImport
+from cosmotech_api.model.twin_graph_import_info import TwinGraphImportInfo
+from cosmotech_api.model.twin_graph_query import TwinGraphQuery
 from cosmotech_api.model.validator import Validator
 from cosmotech_api.model.validator_run import ValidatorRun
 from cosmotech_api.model.workspace import Workspace
+from cosmotech_api.model.workspace_access_control import WorkspaceAccessControl
 from cosmotech_api.model.workspace_file import WorkspaceFile
+from cosmotech_api.model.workspace_role import WorkspaceRole
 from cosmotech_api.model.workspace_secret import WorkspaceSecret
+from cosmotech_api.model.workspace_security import WorkspaceSecurity
 from cosmotech_api.model.workspace_solution import WorkspaceSolution
-from cosmotech_api.model.workspace_user import WorkspaceUser
 from cosmotech_api.model.workspace_web_app import WorkspaceWebApp
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api/rest.py` & `cosmotech-api-2.4.0/cosmotech_api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
```

### Comparing `cosmotech-api-2.2.0/cosmotech_api.egg-info/SOURCES.txt` & `cosmotech-api-2.4.0/cosmotech_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 cosmotech_api/model/container_resource_sizing.py
 cosmotech_api/model/dataset.py
 cosmotech_api/model/dataset_compatibility.py
 cosmotech_api/model/dataset_connector.py
 cosmotech_api/model/dataset_copy_parameters.py
 cosmotech_api/model/dataset_search.py
 cosmotech_api/model/delete_historical_data.py
+cosmotech_api/model/graph_properties.py
 cosmotech_api/model/organization.py
 cosmotech_api/model/organization_access_control.py
 cosmotech_api/model/organization_role.py
 cosmotech_api/model/organization_security.py
 cosmotech_api/model/organization_service.py
 cosmotech_api/model/organization_services.py
 cosmotech_api/model/organization_user.py
@@ -76,14 +77,16 @@
 cosmotech_api/model/scenario_run_template_parameter_value.py
 cosmotech_api/model/scenario_security.py
 cosmotech_api/model/scenario_user.py
 cosmotech_api/model/scenario_validation_status.py
 cosmotech_api/model/solution.py
 cosmotech_api/model/source_info.py
 cosmotech_api/model/translated_labels.py
+cosmotech_api/model/twin_graph_batch_result.py
+cosmotech_api/model/twin_graph_hash.py
 cosmotech_api/model/twin_graph_import.py
 cosmotech_api/model/twin_graph_import_info.py
 cosmotech_api/model/twin_graph_query.py
 cosmotech_api/model/user.py
 cosmotech_api/model/user_organization.py
 cosmotech_api/model/user_workspace.py
 cosmotech_api/model/validator.py
@@ -108,14 +111,15 @@
 test/test_dataset.py
 test/test_dataset_api.py
 test/test_dataset_compatibility.py
 test/test_dataset_connector.py
 test/test_dataset_copy_parameters.py
 test/test_dataset_search.py
 test/test_delete_historical_data.py
+test/test_graph_properties.py
 test/test_organization.py
 test/test_organization_access_control.py
 test/test_organization_api.py
 test/test_organization_role.py
 test/test_organization_security.py
 test/test_organization_service.py
 test/test_organization_services.py
@@ -154,14 +158,16 @@
 test/test_scenario_user.py
 test/test_scenario_validation_status.py
 test/test_scenariorun_api.py
 test/test_solution.py
 test/test_solution_api.py
 test/test_source_info.py
 test/test_translated_labels.py
+test/test_twin_graph_batch_result.py
+test/test_twin_graph_hash.py
 test/test_twin_graph_import.py
 test/test_twin_graph_import_info.py
 test/test_twin_graph_query.py
 test/test_twingraph_api.py
 test/test_user.py
 test/test_user_api.py
 test/test_user_organization.py
```

### Comparing `cosmotech-api-2.2.0/setup.py` & `cosmotech-api-2.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "cosmotech-api"
-VERSION = "2.2.0"
+VERSION = "2.4.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -24,19 +24,19 @@
   "urllib3 >= 1.25.3",
   "python-dateutil",
 ]
 
 setup(
     name=NAME,
     version=VERSION,
-    description="Cosmo Tech Plaform API",
+    description="Cosmo Tech Platform API",
     author="Repository",
     author_email="platform@cosmotech.com",
     url="",
-    keywords=["OpenAPI", "OpenAPI-Generator", "Cosmo Tech Plaform API"],
+    keywords=["OpenAPI", "OpenAPI-Generator", "Cosmo Tech Platform API"],
     python_requires=">=3.6",
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     license="MIT License",
     long_description="""\
     Cosmo Tech Platform API  # noqa: E501
```

### Comparing `cosmotech-api-2.2.0/test/test_component_role_permissions.py` & `cosmotech-api-2.4.0/test/test_component_role_permissions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_connector.py` & `cosmotech-api-2.4.0/test/test_connector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_connector_api.py` & `cosmotech-api-2.4.0/test/test_connector_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
@@ -34,14 +34,21 @@
     def test_find_connector_by_id(self):
         """Test case for find_connector_by_id
 
         Get the details of a connector  # noqa: E501
         """
         pass
 
+    def test_import_connector(self):
+        """Test case for import_connector
+
+        Import existing connector  # noqa: E501
+        """
+        pass
+
     def test_register_connector(self):
         """Test case for register_connector
 
         Register a new connector  # noqa: E501
         """
         pass
```

### Comparing `cosmotech-api-2.2.0/test/test_connector_parameter.py` & `cosmotech-api-2.4.0/test/test_connector_parameter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_connector_parameter_group.py` & `cosmotech-api-2.4.0/test/test_connector_parameter_group.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_container_resource_size_info.py` & `cosmotech-api-2.4.0/test/test_container_resource_size_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_container_resource_sizing.py` & `cosmotech-api-2.4.0/test/test_container_resource_sizing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_dataset.py` & `cosmotech-api-2.4.0/test/test_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_dataset_api.py` & `cosmotech-api-2.4.0/test/test_dataset_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
@@ -62,14 +62,21 @@
     def test_find_dataset_by_id(self):
         """Test case for find_dataset_by_id
 
         Get the details of a Dataset  # noqa: E501
         """
         pass
 
+    def test_import_dataset(self):
+        """Test case for import_dataset
+
+        Import a new Dataset  # noqa: E501
+        """
+        pass
+
     def test_remove_all_dataset_compatibility_elements(self):
         """Test case for remove_all_dataset_compatibility_elements
 
         Remove all Dataset Compatibility elements from the Dataset specified  # noqa: E501
         """
         pass
```

### Comparing `cosmotech-api-2.2.0/test/test_dataset_compatibility.py` & `cosmotech-api-2.4.0/test/test_dataset_compatibility.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_dataset_connector.py` & `cosmotech-api-2.4.0/test/test_dataset_connector.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_dataset_copy_parameters.py` & `cosmotech-api-2.4.0/test/test_dataset_copy_parameters.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_dataset_search.py` & `cosmotech-api-2.4.0/test/test_dataset_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_delete_historical_data.py` & `cosmotech-api-2.4.0/test/test_delete_historical_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_organization.py` & `cosmotech-api-2.4.0/test/test_organization_services.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
+from cosmotech_api.model.organization_service import OrganizationService
+globals()['OrganizationService'] = OrganizationService
 from cosmotech_api.model.organization_services import OrganizationServices
-from cosmotech_api.model.organization_user import OrganizationUser
-globals()['OrganizationServices'] = OrganizationServices
-globals()['OrganizationUser'] = OrganizationUser
-from cosmotech_api.model.organization import Organization
 
 
-class TestOrganization(unittest.TestCase):
-    """Organization unit test stubs"""
+class TestOrganizationServices(unittest.TestCase):
+    """OrganizationServices unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testOrganization(self):
-        """Test Organization"""
+    def testOrganizationServices(self):
+        """Test OrganizationServices"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Organization()  # noqa: E501
+        # model = OrganizationServices()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.2.0/test/test_organization_access_control.py` & `cosmotech-api-2.4.0/test/test_organization_access_control.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_organization_api.py` & `cosmotech-api-2.4.0/test/test_organization_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
@@ -20,18 +20,18 @@
 
     def setUp(self):
         self.api = OrganizationApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_add_or_replace_users_in_organization(self):
-        """Test case for add_or_replace_users_in_organization
+    def test_add_organization_access_control(self):
+        """Test case for add_organization_access_control
 
-        Add (or replace) users in the Organization specified  # noqa: E501
+        Add a control access to the Organization  # noqa: E501
         """
         pass
 
     def test_find_all_organizations(self):
         """Test case for find_all_organizations
 
         List all Organizations  # noqa: E501
@@ -41,32 +41,74 @@
     def test_find_organization_by_id(self):
         """Test case for find_organization_by_id
 
         Get the details of an Organization  # noqa: E501
         """
         pass
 
+    def test_get_all_permissions(self):
+        """Test case for get_all_permissions
+
+        Get all permissions per components  # noqa: E501
+        """
+        pass
+
+    def test_get_organization_access_control(self):
+        """Test case for get_organization_access_control
+
+        Get a control access for the Organization  # noqa: E501
+        """
+        pass
+
+    def test_get_organization_permissions(self):
+        """Test case for get_organization_permissions
+
+        Get the Organization permissions by given role  # noqa: E501
+        """
+        pass
+
+    def test_get_organization_security(self):
+        """Test case for get_organization_security
+
+        Get the Organization security information  # noqa: E501
+        """
+        pass
+
+    def test_get_organization_security_users(self):
+        """Test case for get_organization_security_users
+
+        Get the Organization security users list  # noqa: E501
+        """
+        pass
+
+    def test_import_organization(self):
+        """Test case for import_organization
+
+        Import an organization  # noqa: E501
+        """
+        pass
+
     def test_register_organization(self):
         """Test case for register_organization
 
         Register a new organization  # noqa: E501
         """
         pass
 
-    def test_remove_all_users_in_organization(self):
-        """Test case for remove_all_users_in_organization
+    def test_remove_organization_access_control(self):
+        """Test case for remove_organization_access_control
 
-        Remove all users from the Organization specified  # noqa: E501
+        Remove the specified access from the given Organization  # noqa: E501
         """
         pass
 
-    def test_remove_user_from_organization(self):
-        """Test case for remove_user_from_organization
+    def test_set_organization_default_security(self):
+        """Test case for set_organization_default_security
 
-        Remove the specified user from the given Organization  # noqa: E501
+        Set the Organization default security  # noqa: E501
         """
         pass
 
     def test_unregister_organization(self):
         """Test case for unregister_organization
 
         Unregister an organization  # noqa: E501
@@ -76,14 +118,21 @@
     def test_update_organization(self):
         """Test case for update_organization
 
         Update an Organization  # noqa: E501
         """
         pass
 
+    def test_update_organization_access_control(self):
+        """Test case for update_organization_access_control
+
+        Update the specified access to User for an Organization  # noqa: E501
+        """
+        pass
+
     def test_update_solutions_container_registry_by_organization_id(self):
         """Test case for update_solutions_container_registry_by_organization_id
 
         Update the solutions container registry configuration for the Organization specified  # noqa: E501
         """
         pass
```

### Comparing `cosmotech-api-2.2.0/test/test_organization_role.py` & `cosmotech-api-2.4.0/test/test_organization_role.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_organization_security.py` & `cosmotech-api-2.4.0/test/test_organization_security.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_organization_service.py` & `cosmotech-api-2.4.0/test/test_organization_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_organization_user.py` & `cosmotech-api-2.4.0/test/test_organization_user.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Cosmo Tech Plaform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.3.4-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_resource_size_info.py` & `cosmotech-api-2.4.0/test/test_scenario_resource_sizing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
 from cosmotech_api.model.resource_size_info import ResourceSizeInfo
+globals()['ResourceSizeInfo'] = ResourceSizeInfo
+from cosmotech_api.model.scenario_resource_sizing import ScenarioResourceSizing
 
 
-class TestResourceSizeInfo(unittest.TestCase):
-    """ResourceSizeInfo unit test stubs"""
+class TestScenarioResourceSizing(unittest.TestCase):
+    """ScenarioResourceSizing unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testResourceSizeInfo(self):
-        """Test ResourceSizeInfo"""
+    def testScenarioResourceSizing(self):
+        """Test ScenarioResourceSizing"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ResourceSizeInfo()  # noqa: E501
+        # model = ScenarioResourceSizing()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.2.0/test/test_run_template.py` & `cosmotech-api-2.4.0/test/test_run_template.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
 from cosmotech_api.model.delete_historical_data import DeleteHistoricalData
+from cosmotech_api.model.run_template_resource_sizing import RunTemplateResourceSizing
 from cosmotech_api.model.run_template_step_source import RunTemplateStepSource
 globals()['DeleteHistoricalData'] = DeleteHistoricalData
+globals()['RunTemplateResourceSizing'] = RunTemplateResourceSizing
 globals()['RunTemplateStepSource'] = RunTemplateStepSource
 from cosmotech_api.model.run_template import RunTemplate
 
 
 class TestRunTemplate(unittest.TestCase):
     """RunTemplate unit test stubs"""
```

### Comparing `cosmotech-api-2.2.0/test/test_run_template_handler_id.py` & `cosmotech-api-2.4.0/test/test_run_template_handler_id.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_run_template_parameter.py` & `cosmotech-api-2.4.0/test/test_run_template_parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_run_template_parameter_group.py` & `cosmotech-api-2.4.0/test/test_run_template_parameter_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_run_template_parameter_value.py` & `cosmotech-api-2.4.0/test/test_run_template_parameter_value.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_run_template_resource_sizing.py` & `cosmotech-api-2.4.0/test/test_run_template_resource_sizing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_run_template_step_source.py` & `cosmotech-api-2.4.0/test/test_run_template_step_source.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_access_control.py` & `cosmotech-api-2.4.0/test/test_scenario_access_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_api.py` & `cosmotech-api-2.4.0/test/test_scenario_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
@@ -27,18 +27,18 @@
     def test_add_or_replace_scenario_parameter_values(self):
         """Test case for add_or_replace_scenario_parameter_values
 
         Add (or replace) Parameter Values for the Scenario specified  # noqa: E501
         """
         pass
 
-    def test_add_or_replace_users_in_scenario(self):
-        """Test case for add_or_replace_users_in_scenario
+    def test_add_scenario_access_control(self):
+        """Test case for add_scenario_access_control
 
-        Add (or replace) users in the Scenario specified  # noqa: E501
+        Add a control access to the Scenario  # noqa: E501
         """
         pass
 
     def test_compare_scenarios(self):
         """Test case for compare_scenarios
 
         Compare the Scenario with another one and returns the difference for parameters values  # noqa: E501
@@ -90,59 +90,101 @@
     def test_find_scenario_by_id(self):
         """Test case for find_scenario_by_id
 
         Get the details of an scenario  # noqa: E501
         """
         pass
 
+    def test_get_scenario_access_control(self):
+        """Test case for get_scenario_access_control
+
+        Get a control access for the Scenario  # noqa: E501
+        """
+        pass
+
     def test_get_scenario_data_download_job_info(self):
         """Test case for get_scenario_data_download_job_info
 
         Get Scenario data download URL  # noqa: E501
         """
         pass
 
+    def test_get_scenario_permissions(self):
+        """Test case for get_scenario_permissions
+
+        Get the Scenario permission by given role  # noqa: E501
+        """
+        pass
+
+    def test_get_scenario_security(self):
+        """Test case for get_scenario_security
+
+        Get the Scenario security information  # noqa: E501
+        """
+        pass
+
+    def test_get_scenario_security_users(self):
+        """Test case for get_scenario_security_users
+
+        Get the Scenario security users list  # noqa: E501
+        """
+        pass
+
     def test_get_scenario_validation_status_by_id(self):
         """Test case for get_scenario_validation_status_by_id
 
         Get the validation status of an scenario  # noqa: E501
         """
         pass
 
     def test_get_scenarios_tree(self):
         """Test case for get_scenarios_tree
 
         Get the Scenarios Tree  # noqa: E501
         """
         pass
 
+    def test_import_scenario(self):
+        """Test case for import_scenario
+
+        Import Scenario  # noqa: E501
+        """
+        pass
+
     def test_remove_all_scenario_parameter_values(self):
         """Test case for remove_all_scenario_parameter_values
 
         Remove all Parameter Values from the Scenario specified  # noqa: E501
         """
         pass
 
-    def test_remove_all_users_of_scenario(self):
-        """Test case for remove_all_users_of_scenario
+    def test_remove_scenario_access_control(self):
+        """Test case for remove_scenario_access_control
 
-        Remove all users from the Scenario specified  # noqa: E501
+        Remove the specified access from the given Organization Scenario  # noqa: E501
         """
         pass
 
-    def test_remove_user_from_scenario(self):
-        """Test case for remove_user_from_scenario
+    def test_set_scenario_default_security(self):
+        """Test case for set_scenario_default_security
 
-        Remove the specified user from the given Scenario  # noqa: E501
+        Set the Scenario default security  # noqa: E501
         """
         pass
 
     def test_update_scenario(self):
         """Test case for update_scenario
 
         Update a scenario  # noqa: E501
         """
         pass
 
+    def test_update_scenario_access_control(self):
+        """Test case for update_scenario_access_control
+
+        Update the specified access to User for a Scenario  # noqa: E501
+        """
+        pass
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_changed_parameter_value.py` & `cosmotech-api-2.4.0/test/test_scenario_changed_parameter_value.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_comparison_result.py` & `cosmotech-api-2.4.0/test/test_scenario_comparison_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_data_download_info.py` & `cosmotech-api-2.4.0/test/test_scenario_data_download_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_data_download_job.py` & `cosmotech-api-2.4.0/test/test_workspace_access_control.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.scenario_data_download_job import ScenarioDataDownloadJob
+from cosmotech_api.model.workspace_access_control import WorkspaceAccessControl
 
 
-class TestScenarioDataDownloadJob(unittest.TestCase):
-    """ScenarioDataDownloadJob unit test stubs"""
+class TestWorkspaceAccessControl(unittest.TestCase):
+    """WorkspaceAccessControl unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScenarioDataDownloadJob(self):
-        """Test ScenarioDataDownloadJob"""
+    def testWorkspaceAccessControl(self):
+        """Test WorkspaceAccessControl"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ScenarioDataDownloadJob()  # noqa: E501
+        # model = WorkspaceAccessControl()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_job_state.py` & `cosmotech-api-2.4.0/test/test_scenario_job_state.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_last_run.py` & `cosmotech-api-2.4.0/test/test_scenario_last_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_resource_sizing.py` & `cosmotech-api-2.4.0/test/test_workspace_user.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """
     Cosmo Tech Plaform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.3.4-SNAPSHOT
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.resource_size_info import ResourceSizeInfo
-globals()['ResourceSizeInfo'] = ResourceSizeInfo
-from cosmotech_api.model.scenario_resource_sizing import ScenarioResourceSizing
+from cosmotech_api.model.workspace_user import WorkspaceUser
 
 
-class TestScenarioResourceSizing(unittest.TestCase):
-    """ScenarioResourceSizing unit test stubs"""
+class TestWorkspaceUser(unittest.TestCase):
+    """WorkspaceUser unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScenarioResourceSizing(self):
-        """Test ScenarioResourceSizing"""
+    def testWorkspaceUser(self):
+        """Test WorkspaceUser"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ScenarioResourceSizing()  # noqa: E501
+        # model = WorkspaceUser()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_role.py` & `cosmotech-api-2.4.0/test/test_scenario_role.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_run.py` & `cosmotech-api-2.4.0/test/test_scenario_run.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_run_container.py` & `cosmotech-api-2.4.0/test/test_scenario_run_container.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
+from cosmotech_api.model.container_resource_sizing import ContainerResourceSizing
 from cosmotech_api.model.scenario_run_container_artifact import ScenarioRunContainerArtifact
+globals()['ContainerResourceSizing'] = ContainerResourceSizing
 globals()['ScenarioRunContainerArtifact'] = ScenarioRunContainerArtifact
 from cosmotech_api.model.scenario_run_container import ScenarioRunContainer
 
 
 class TestScenarioRunContainer(unittest.TestCase):
     """ScenarioRunContainer unit test stubs"""
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_run_container_artifact.py` & `cosmotech-api-2.4.0/test/test_scenario_run_container_artifact.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_run_container_logs.py` & `cosmotech-api-2.4.0/test/test_scenario_run_logs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
 from cosmotech_api.model.scenario_run_container_logs import ScenarioRunContainerLogs
+globals()['ScenarioRunContainerLogs'] = ScenarioRunContainerLogs
+from cosmotech_api.model.scenario_run_logs import ScenarioRunLogs
 
 
-class TestScenarioRunContainerLogs(unittest.TestCase):
-    """ScenarioRunContainerLogs unit test stubs"""
+class TestScenarioRunLogs(unittest.TestCase):
+    """ScenarioRunLogs unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScenarioRunContainerLogs(self):
-        """Test ScenarioRunContainerLogs"""
+    def testScenarioRunLogs(self):
+        """Test ScenarioRunLogs"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ScenarioRunContainerLogs()  # noqa: E501
+        # model = ScenarioRunLogs()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_run_logs.py` & `cosmotech-api-2.4.0/test/test_scenario_run_container_logs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
 from cosmotech_api.model.scenario_run_container_logs import ScenarioRunContainerLogs
-globals()['ScenarioRunContainerLogs'] = ScenarioRunContainerLogs
-from cosmotech_api.model.scenario_run_logs import ScenarioRunLogs
 
 
-class TestScenarioRunLogs(unittest.TestCase):
-    """ScenarioRunLogs unit test stubs"""
+class TestScenarioRunContainerLogs(unittest.TestCase):
+    """ScenarioRunContainerLogs unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScenarioRunLogs(self):
-        """Test ScenarioRunLogs"""
+    def testScenarioRunContainerLogs(self):
+        """Test ScenarioRunContainerLogs"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ScenarioRunLogs()  # noqa: E501
+        # model = ScenarioRunContainerLogs()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_run_search.py` & `cosmotech-api-2.4.0/test/test_scenario_run_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_run_start_containers.py` & `cosmotech-api-2.4.0/test/test_scenario_run_start_containers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_run_state.py` & `cosmotech-api-2.4.0/test/test_scenario_run_status.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
 from cosmotech_api.model.scenario_run_state import ScenarioRunState
+from cosmotech_api.model.scenario_run_status_node import ScenarioRunStatusNode
+globals()['ScenarioRunState'] = ScenarioRunState
+globals()['ScenarioRunStatusNode'] = ScenarioRunStatusNode
+from cosmotech_api.model.scenario_run_status import ScenarioRunStatus
 
 
-class TestScenarioRunState(unittest.TestCase):
-    """ScenarioRunState unit test stubs"""
+class TestScenarioRunStatus(unittest.TestCase):
+    """ScenarioRunStatus unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScenarioRunState(self):
-        """Test ScenarioRunState"""
+    def testScenarioRunStatus(self):
+        """Test ScenarioRunStatus"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ScenarioRunState()  # noqa: E501
+        # model = ScenarioRunStatus()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_run_status.py` & `cosmotech-api-2.4.0/test/test_graph_properties.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.scenario_run_state import ScenarioRunState
-from cosmotech_api.model.scenario_run_status_node import ScenarioRunStatusNode
-globals()['ScenarioRunState'] = ScenarioRunState
-globals()['ScenarioRunStatusNode'] = ScenarioRunStatusNode
-from cosmotech_api.model.scenario_run_status import ScenarioRunStatus
+from cosmotech_api.model.graph_properties import GraphProperties
 
 
-class TestScenarioRunStatus(unittest.TestCase):
-    """ScenarioRunStatus unit test stubs"""
+class TestGraphProperties(unittest.TestCase):
+    """GraphProperties unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScenarioRunStatus(self):
-        """Test ScenarioRunStatus"""
+    def testGraphProperties(self):
+        """Test GraphProperties"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ScenarioRunStatus()  # noqa: E501
+        # model = GraphProperties()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_run_status_node.py` & `cosmotech-api-2.4.0/test/test_scenario_run_status_node.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_run_template_parameter_value.py` & `cosmotech-api-2.4.0/test/test_solution.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.scenario_run_template_parameter_value import ScenarioRunTemplateParameterValue
+from cosmotech_api.model.run_template import RunTemplate
+from cosmotech_api.model.run_template_parameter import RunTemplateParameter
+from cosmotech_api.model.run_template_parameter_group import RunTemplateParameterGroup
+globals()['RunTemplate'] = RunTemplate
+globals()['RunTemplateParameter'] = RunTemplateParameter
+globals()['RunTemplateParameterGroup'] = RunTemplateParameterGroup
+from cosmotech_api.model.solution import Solution
 
 
-class TestScenarioRunTemplateParameterValue(unittest.TestCase):
-    """ScenarioRunTemplateParameterValue unit test stubs"""
+class TestSolution(unittest.TestCase):
+    """Solution unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScenarioRunTemplateParameterValue(self):
-        """Test ScenarioRunTemplateParameterValue"""
+    def testSolution(self):
+        """Test Solution"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ScenarioRunTemplateParameterValue()  # noqa: E501
+        # model = Solution()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_security.py` & `cosmotech-api-2.4.0/test/test_scenario_security.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_user.py` & `cosmotech-api-2.4.0/test/test_source_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.scenario_user import ScenarioUser
+from cosmotech_api.model.source_info import SourceInfo
 
 
-class TestScenarioUser(unittest.TestCase):
-    """ScenarioUser unit test stubs"""
+class TestSourceInfo(unittest.TestCase):
+    """SourceInfo unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScenarioUser(self):
-        """Test ScenarioUser"""
+    def testSourceInfo(self):
+        """Test SourceInfo"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ScenarioUser()  # noqa: E501
+        # model = SourceInfo()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.2.0/test/test_scenario_validation_status.py` & `cosmotech-api-2.4.0/test/test_scenario_validation_status.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_scenariorun_api.py` & `cosmotech-api-2.4.0/test/test_scenariorun_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
@@ -90,14 +90,21 @@
     def test_get_workspace_scenario_runs(self):
         """Test case for get_workspace_scenario_runs
 
         get the list of ScenarioRuns for the Workspace  # noqa: E501
         """
         pass
 
+    def test_import_scenario_run(self):
+        """Test case for import_scenario_run
+
+        import a ScenarioRun for the Scenario  # noqa: E501
+        """
+        pass
+
     def test_run_scenario(self):
         """Test case for run_scenario
 
         run a ScenarioRun for the Scenario  # noqa: E501
         """
         pass
```

### Comparing `cosmotech-api-2.2.0/test/test_solution_api.py` & `cosmotech-api-2.4.0/test/test_solution_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
@@ -83,14 +83,21 @@
     def test_find_solution_by_id(self):
         """Test case for find_solution_by_id
 
         Get the details of a solution  # noqa: E501
         """
         pass
 
+    def test_import_solution(self):
+        """Test case for import_solution
+
+        Import a solution  # noqa: E501
+        """
+        pass
+
     def test_remove_all_run_templates(self):
         """Test case for remove_all_run_templates
 
         Remove all Run Templates from the Solution specified  # noqa: E501
         """
         pass
```

### Comparing `cosmotech-api-2.2.0/test/test_source_info.py` & `cosmotech-api-2.4.0/test/test_validator_run.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.source_info import SourceInfo
+from cosmotech_api.model.validator_run import ValidatorRun
 
 
-class TestSourceInfo(unittest.TestCase):
-    """SourceInfo unit test stubs"""
+class TestValidatorRun(unittest.TestCase):
+    """ValidatorRun unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSourceInfo(self):
-        """Test SourceInfo"""
+    def testValidatorRun(self):
+        """Test ValidatorRun"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = SourceInfo()  # noqa: E501
+        # model = ValidatorRun()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.2.0/test/test_translated_labels.py` & `cosmotech-api-2.4.0/test/test_translated_labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_twin_graph_import.py` & `cosmotech-api-2.4.0/test/test_twin_graph_import_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.source_info import SourceInfo
-globals()['SourceInfo'] = SourceInfo
-from cosmotech_api.model.twin_graph_import import TwinGraphImport
+from cosmotech_api.model.twin_graph_import_info import TwinGraphImportInfo
 
 
-class TestTwinGraphImport(unittest.TestCase):
-    """TwinGraphImport unit test stubs"""
+class TestTwinGraphImportInfo(unittest.TestCase):
+    """TwinGraphImportInfo unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTwinGraphImport(self):
-        """Test TwinGraphImport"""
+    def testTwinGraphImportInfo(self):
+        """Test TwinGraphImportInfo"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TwinGraphImport()  # noqa: E501
+        # model = TwinGraphImportInfo()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.2.0/test/test_twin_graph_import_info.py` & `cosmotech-api-2.4.0/test/test_twin_graph_hash.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.twin_graph_import_info import TwinGraphImportInfo
+from cosmotech_api.model.twin_graph_hash import TwinGraphHash
 
 
-class TestTwinGraphImportInfo(unittest.TestCase):
-    """TwinGraphImportInfo unit test stubs"""
+class TestTwinGraphHash(unittest.TestCase):
+    """TwinGraphHash unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTwinGraphImportInfo(self):
-        """Test TwinGraphImportInfo"""
+    def testTwinGraphHash(self):
+        """Test TwinGraphHash"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TwinGraphImportInfo()  # noqa: E501
+        # model = TwinGraphHash()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.2.0/test/test_twin_graph_query.py` & `cosmotech-api-2.4.0/test/test_twin_graph_query.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_user.py` & `cosmotech-api-2.4.0/test/test_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.3.7
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_user_api.py` & `cosmotech-api-2.4.0/test/test_user_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.3.7
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_user_organization.py` & `cosmotech-api-2.4.0/test/test_user_organization.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.3.7
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_user_workspace.py` & `cosmotech-api-2.4.0/test/test_user_workspace.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.3.7
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_validator.py` & `cosmotech-api-2.4.0/test/test_workspace_role.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.validator import Validator
+from cosmotech_api.model.workspace_role import WorkspaceRole
 
 
-class TestValidator(unittest.TestCase):
-    """Validator unit test stubs"""
+class TestWorkspaceRole(unittest.TestCase):
+    """WorkspaceRole unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testValidator(self):
-        """Test Validator"""
+    def testWorkspaceRole(self):
+        """Test WorkspaceRole"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Validator()  # noqa: E501
+        # model = WorkspaceRole()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.2.0/test/test_validator_api.py` & `cosmotech-api-2.4.0/test/test_validator_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_validator_run.py` & `cosmotech-api-2.4.0/test/test_workspace_web_app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.validator_run import ValidatorRun
+from cosmotech_api.model.workspace_web_app import WorkspaceWebApp
 
 
-class TestValidatorRun(unittest.TestCase):
-    """ValidatorRun unit test stubs"""
+class TestWorkspaceWebApp(unittest.TestCase):
+    """WorkspaceWebApp unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testValidatorRun(self):
-        """Test ValidatorRun"""
+    def testWorkspaceWebApp(self):
+        """Test WorkspaceWebApp"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ValidatorRun()  # noqa: E501
+        # model = WorkspaceWebApp()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.2.0/test/test_workspace.py` & `cosmotech-api-2.4.0/test/test_workspace_secret.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.workspace_solution import WorkspaceSolution
-from cosmotech_api.model.workspace_user import WorkspaceUser
-from cosmotech_api.model.workspace_web_app import WorkspaceWebApp
-globals()['WorkspaceSolution'] = WorkspaceSolution
-globals()['WorkspaceUser'] = WorkspaceUser
-globals()['WorkspaceWebApp'] = WorkspaceWebApp
-from cosmotech_api.model.workspace import Workspace
+from cosmotech_api.model.workspace_secret import WorkspaceSecret
 
 
-class TestWorkspace(unittest.TestCase):
-    """Workspace unit test stubs"""
+class TestWorkspaceSecret(unittest.TestCase):
+    """WorkspaceSecret unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testWorkspace(self):
-        """Test Workspace"""
+    def testWorkspaceSecret(self):
+        """Test WorkspaceSecret"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Workspace()  # noqa: E501
+        # model = WorkspaceSecret()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.2.0/test/test_workspace_api.py` & `cosmotech-api-2.4.0/test/test_workspace_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
@@ -20,18 +20,18 @@
 
     def setUp(self):
         self.api = WorkspaceApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_add_or_replace_users_in_organization_workspace(self):
-        """Test case for add_or_replace_users_in_organization_workspace
+    def test_add_workspace_access_control(self):
+        """Test case for add_workspace_access_control
 
-        Add (or replace) users to the Workspace specified  # noqa: E501
+        Add a control access to the Workspace  # noqa: E501
         """
         pass
 
     def test_create_secret(self):
         """Test case for create_secret
 
         Create a secret for the Workspace  # noqa: E501
@@ -90,35 +90,77 @@
     def test_find_workspace_by_id(self):
         """Test case for find_workspace_by_id
 
         Get the details of an workspace  # noqa: E501
         """
         pass
 
-    def test_remove_all_users_of_workspace(self):
-        """Test case for remove_all_users_of_workspace
+    def test_get_workspace_access_control(self):
+        """Test case for get_workspace_access_control
 
-        Remove all users from the Workspace specified  # noqa: E501
+        Get a control access for the Workspace  # noqa: E501
         """
         pass
 
-    def test_remove_user_from_organization_workspace(self):
-        """Test case for remove_user_from_organization_workspace
+    def test_get_workspace_permissions(self):
+        """Test case for get_workspace_permissions
 
-        Remove the specified user from the given Organization Workspace  # noqa: E501
+        Get the Workspace permission by given role  # noqa: E501
+        """
+        pass
+
+    def test_get_workspace_security(self):
+        """Test case for get_workspace_security
+
+        Get the Workspace security information  # noqa: E501
+        """
+        pass
+
+    def test_get_workspace_security_users(self):
+        """Test case for get_workspace_security_users
+
+        Get the Workspace security users list  # noqa: E501
+        """
+        pass
+
+    def test_import_workspace(self):
+        """Test case for import_workspace
+
+        Import a workspace  # noqa: E501
+        """
+        pass
+
+    def test_remove_workspace_access_control(self):
+        """Test case for remove_workspace_access_control
+
+        Remove the specified access from the given Organization Workspace  # noqa: E501
+        """
+        pass
+
+    def test_set_workspace_default_security(self):
+        """Test case for set_workspace_default_security
+
+        Set the Workspace default security  # noqa: E501
         """
         pass
 
     def test_update_workspace(self):
         """Test case for update_workspace
 
         Update a workspace  # noqa: E501
         """
         pass
 
+    def test_update_workspace_access_control(self):
+        """Test case for update_workspace_access_control
+
+        Update the specified access to User for a Workspace  # noqa: E501
+        """
+        pass
+
     def test_upload_workspace_file(self):
         """Test case for upload_workspace_file
 
         Upload a file for the Workspace  # noqa: E501
         """
         pass
```

### Comparing `cosmotech-api-2.2.0/test/test_workspace_file.py` & `cosmotech-api-2.4.0/test/test_workspace_file.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_workspace_role.py` & `cosmotech-api-2.4.0/test/test_workspace.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.workspace_role import WorkspaceRole
+from cosmotech_api.model.workspace_security import WorkspaceSecurity
+from cosmotech_api.model.workspace_solution import WorkspaceSolution
+from cosmotech_api.model.workspace_web_app import WorkspaceWebApp
+globals()['WorkspaceSecurity'] = WorkspaceSecurity
+globals()['WorkspaceSolution'] = WorkspaceSolution
+globals()['WorkspaceWebApp'] = WorkspaceWebApp
+from cosmotech_api.model.workspace import Workspace
 
 
-class TestWorkspaceRole(unittest.TestCase):
-    """WorkspaceRole unit test stubs"""
+class TestWorkspace(unittest.TestCase):
+    """Workspace unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testWorkspaceRole(self):
-        """Test WorkspaceRole"""
+    def testWorkspace(self):
+        """Test Workspace"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = WorkspaceRole()  # noqa: E501
+        # model = Workspace()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.2.0/test/test_workspace_secret.py` & `cosmotech-api-2.4.0/test/test_workspace_solution.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.workspace_secret import WorkspaceSecret
+from cosmotech_api.model.workspace_solution import WorkspaceSolution
 
 
-class TestWorkspaceSecret(unittest.TestCase):
-    """WorkspaceSecret unit test stubs"""
+class TestWorkspaceSolution(unittest.TestCase):
+    """WorkspaceSolution unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testWorkspaceSecret(self):
-        """Test WorkspaceSecret"""
+    def testWorkspaceSolution(self):
+        """Test WorkspaceSolution"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = WorkspaceSecret()  # noqa: E501
+        # model = WorkspaceSolution()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.2.0/test/test_workspace_security.py` & `cosmotech-api-2.4.0/test/test_workspace_security.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 2.2.0
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `cosmotech-api-2.2.0/test/test_workspace_solution.py` & `cosmotech-api-2.4.0/test/test_validator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.workspace_solution import WorkspaceSolution
+from cosmotech_api.model.validator import Validator
 
 
-class TestWorkspaceSolution(unittest.TestCase):
-    """WorkspaceSolution unit test stubs"""
+class TestValidator(unittest.TestCase):
+    """Validator unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testWorkspaceSolution(self):
-        """Test WorkspaceSolution"""
+    def testValidator(self):
+        """Test Validator"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = WorkspaceSolution()  # noqa: E501
+        # model = Validator()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cosmotech-api-2.2.0/test/test_workspace_web_app.py` & `cosmotech-api-2.4.0/test/test_scenario_run_state.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
-    Cosmo Tech Plaform API
+    Cosmo Tech Platform API
 
     Cosmo Tech Platform API  # noqa: E501
 
-    The version of the OpenAPI document: 1.1.3-SNAPSHOT
+    The version of the OpenAPI document: 2.4.0-dev
     Contact: platform@cosmotech.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import cosmotech_api
-from cosmotech_api.model.workspace_web_app import WorkspaceWebApp
+from cosmotech_api.model.scenario_run_state import ScenarioRunState
 
 
-class TestWorkspaceWebApp(unittest.TestCase):
-    """WorkspaceWebApp unit test stubs"""
+class TestScenarioRunState(unittest.TestCase):
+    """ScenarioRunState unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testWorkspaceWebApp(self):
-        """Test WorkspaceWebApp"""
+    def testScenarioRunState(self):
+        """Test ScenarioRunState"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = WorkspaceWebApp()  # noqa: E501
+        # model = ScenarioRunState()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

