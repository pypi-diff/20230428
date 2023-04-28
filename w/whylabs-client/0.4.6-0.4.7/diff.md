# Comparing `tmp/whylabs-client-0.4.6.tar.gz` & `tmp/whylabs-client-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylabs-client-0.4.6.tar", last modified: Wed Apr 19 16:58:31 2023, max compression
+gzip compressed data, was "whylabs-client-0.4.7.tar", last modified: Fri Apr 28 00:36:10 2023, max compression
```

## Comparing `whylabs-client-0.4.6.tar` & `whylabs-client-0.4.7.tar`

### file list

```diff
@@ -1,151 +1,154 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:58:31.307100 whylabs-client-0.4.6/
--rw-r--r--   0 root         (0) root         (0)     3358 2023-04-19 16:58:31.307100 whylabs-client-0.4.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    22425 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-19 16:58:31.307100 whylabs-client-0.4.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1269 2023-04-19 16:58:30.000000 whylabs-client-0.4.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:58:31.260098 whylabs-client-0.4.6/whylabs_client/
--rw-rw-rw-   0 root         (0) root         (0)      753 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:58:31.266098 whylabs-client-0.4.6/whylabs_client/api/
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15394 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api/dataset_metadata_api.py
--rw-rw-rw-   0 root         (0) root         (0)    18502 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api/dataset_profile_api.py
--rw-rw-rw-   0 root         (0) root         (0)    10632 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api/feature_weights_api.py
--rw-rw-rw-   0 root         (0) root         (0)    11520 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api/log_api.py
--rw-rw-rw-   0 root         (0) root         (0)    20727 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api/membership_api.py
--rw-rw-rw-   0 root         (0) root         (0)    67177 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api/models_api.py
--rw-rw-rw-   0 root         (0) root         (0)    52337 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api/monitor_api.py
--rw-rw-rw-   0 root         (0) root         (0)    48204 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api/notification_settings_api.py
--rw-rw-rw-   0 root         (0) root         (0)     5237 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api/schema_api.py
--rw-rw-rw-   0 root         (0) root         (0)    29965 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api/sessions_api.py
--rw-rw-rw-   0 root         (0) root         (0)    37575 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:58:31.266098 whylabs-client-0.4.6/whylabs_client/apis/
--rw-rw-rw-   0 root         (0) root         (0)     1038 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/apis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17084 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     5075 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:58:31.306100 whylabs-client-0.4.6/whylabs_client/model/
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11664 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/action_type.py
--rw-rw-rw-   0 root         (0) root         (0)    12110 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/add_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12005 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/async_log_response.py
--rw-rw-rw-   0 root         (0) root         (0)    13478 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/aws_marketplace_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11342 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/batch_log_reference_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11655 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/batch_log_session_reference_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12443 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/column_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    11118 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/create_session_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11207 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/create_session_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11136 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/create_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    13099 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/databricks_connection.py
--rw-rw-rw-   0 root         (0) root         (0)    11884 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dataset_request_monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11114 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/datatype_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11061 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/delete_analyzer_results_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11061 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/delete_dataset_profiles_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11368 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/distribution_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11275 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_auto_scale_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    13176 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_aws_attributes_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11715 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_aws_availability_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11665 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_cluster_log_conf_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11338 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_cron_schedule_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11082 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_dbfs_storage_info_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11745 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_ebs_volume_type_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11928 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_job_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12392 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_job_email_notifications_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    15918 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_job_settings_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    14946 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_new_cluster_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11591 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_notebook_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11909 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_spark_jar_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11493 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_spark_python_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11281 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dto_spark_submit_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12338 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/dtos3_storage_info_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11106 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/email_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    12313 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/entity_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    11862 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/entity_weight_record.py
--rw-rw-rw-   0 root         (0) root         (0)    11507 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/entity_weight_record_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11225 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/feature_flags.py
--rw-rw-rw-   0 root         (0) root         (0)    11574 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/get_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11411 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/get_connection_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11222 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/get_dataset_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11283 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/get_default_membership_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11431 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/get_marketplace_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11485 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/get_memberships_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11379 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/get_monitor_config_v2_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11417 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/get_notification_settings_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11334 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/get_session_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11559 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/list_jobs_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11260 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/list_jobs_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11496 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/list_models_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11530 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/list_organization_memberships_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11382 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/list_user_api_keys.py
--rw-rw-rw-   0 root         (0) root         (0)    11502 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/log_async_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11354 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/log_reference_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11858 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/log_reference_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11441 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/log_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12111 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/log_session_reference_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12015 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/marketplace_dimensions.py
--rw-rw-rw-   0 root         (0) root         (0)    12029 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/membership.py
--rw-rw-rw-   0 root         (0) root         (0)    11756 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/membership_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    12260 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/metric_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    11120 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/missing_recent_data_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11132 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/missing_recent_profiles_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11938 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/missing_values_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    12569 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/model_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12219 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/model_type.py
--rw-rw-rw-   0 root         (0) root         (0)    13063 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11473 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/monitor_config_version.py
--rw-rw-rw-   0 root         (0) root         (0)    12120 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/monitor_request_reference.py
--rw-rw-rw-   0 root         (0) root         (0)    11689 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/monitor_request_reference_type.py
--rw-rw-rw-   0 root         (0) root         (0)    11783 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    11982 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/notification_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    11979 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/notification_settings_day.py
--rw-rw-rw-   0 root         (0) root         (0)    11751 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/notification_sqs_message_cadence.py
--rw-rw-rw-   0 root         (0) root         (0)    14425 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/organization_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    13737 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/organization_summary.py
--rw-rw-rw-   0 root         (0) root         (0)    11215 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/pager_duty_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    12319 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/provided_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11680 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/provision_databricks_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11657 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/provision_databricks_connection_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11882 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/provision_new_aws_marketplace_user_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12226 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/provision_new_marketplace_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12422 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/provision_new_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11574 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/provision_new_user_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12315 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/reference_profile_item_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11188 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/refresh_access_token_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11444 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/refresh_connection_by_org_id_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11586 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/refresh_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    13668 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/register_databricks_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11112 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/register_databricks_connection_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11317 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/remove_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    13372 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/request_feature_monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    15325 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/request_monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11070 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/response.py
--rw-rw-rw-   0 root         (0) root         (0)    11580 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/role.py
--rw-rw-rw-   0 root         (0) root         (0)    11922 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/run_job_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11089 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/run_job_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11471 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/schema_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11833 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/seasonal_arima_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11197 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/segment.py
--rw-rw-rw-   0 root         (0) root         (0)    11192 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/segment_tag.py
--rw-rw-rw-   0 root         (0) root         (0)    11505 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/segment_weight.py
--rw-rw-rw-   0 root         (0) root         (0)    11948 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/session_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11350 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/set_default_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11193 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/slack_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    11652 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/subscription_tier.py
--rw-rw-rw-   0 root         (0) root         (0)    11670 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/time_period.py
--rw-rw-rw-   0 root         (0) root         (0)    12934 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/uber_notification_schedule.py
--rw-rw-rw-   0 root         (0) root         (0)    11917 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/unique_values_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11548 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/update_connection_changes.py
--rw-rw-rw-   0 root         (0) root         (0)    11816 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/update_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11650 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/update_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11747 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/user.py
--rw-rw-rw-   0 root         (0) root         (0)    13667 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/user_api_key.py
--rw-rw-rw-   0 root         (0) root         (0)    11220 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/user_api_key_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11805 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model/why_logs_metric.py
--rw-rw-rw-   0 root         (0) root         (0)    81897 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:58:31.306100 whylabs-client-0.4.6/whylabs_client/models/
--rw-rw-rw-   0 root         (0) root         (0)     9500 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14199 2023-04-19 16:58:20.000000 whylabs-client-0.4.6/whylabs_client/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:58:31.261098 whylabs-client-0.4.6/whylabs_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3358 2023-04-19 16:58:30.000000 whylabs-client-0.4.6/whylabs_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6453 2023-04-19 16:58:30.000000 whylabs-client-0.4.6/whylabs_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 16:58:30.000000 whylabs-client-0.4.6/whylabs_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-04-19 16:58:30.000000 whylabs-client-0.4.6/whylabs_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-19 16:58:30.000000 whylabs-client-0.4.6/whylabs_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 00:36:10.880926 whylabs-client-0.4.7/
+-rw-r--r--   0 root         (0) root         (0)     3358 2023-04-28 00:36:10.880926 whylabs-client-0.4.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    23249 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-28 00:36:10.881926 whylabs-client-0.4.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1269 2023-04-28 00:36:09.000000 whylabs-client-0.4.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 00:36:10.830922 whylabs-client-0.4.7/whylabs_client/
+-rw-rw-rw-   0 root         (0) root         (0)      753 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 00:36:10.836923 whylabs-client-0.4.7/whylabs_client/api/
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15394 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api/dataset_metadata_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    28878 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api/dataset_profile_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    10632 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api/feature_weights_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    11520 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api/log_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    20727 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api/membership_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    67177 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api/models_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    52337 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api/monitor_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    48204 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api/notification_settings_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     5237 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api/schema_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    29965 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api/sessions_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    37575 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 00:36:10.836923 whylabs-client-0.4.7/whylabs_client/apis/
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17084 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5075 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 00:36:10.880926 whylabs-client-0.4.7/whylabs_client/model/
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11664 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/action_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    12110 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/add_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12005 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/async_log_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    13478 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/aws_marketplace_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11342 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/batch_log_reference_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11655 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/batch_log_session_reference_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12443 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/column_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    11118 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/create_session_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11207 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/create_session_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11136 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/create_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    13099 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/databricks_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)    11884 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dataset_request_monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11114 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/datatype_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11061 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/delete_analyzer_results_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11061 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/delete_dataset_profiles_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11368 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/distribution_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11299 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_clusters_auto_scale_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    13257 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_clusters_aws_attributes_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11739 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_clusters_aws_availability_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11804 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_clusters_cluster_log_conf_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11106 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_clusters_dbfs_storage_info_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12362 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_clusters_s3_storage_info_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11745 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_ebs_volume_type_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11350 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_jobs_cron_schedule_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11934 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_jobs_data_security_mode_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11969 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_jobs_job_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12404 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_jobs_job_email_notifications_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    16133 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_jobs_job_settings_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    16932 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_jobs_new_cluster_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11603 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_jobs_notebook_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11707 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_jobs_spark_jar_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11505 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_jobs_spark_python_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11293 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/dto_jobs_spark_submit_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11106 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/email_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    12313 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/entity_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    12718 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/entity_search_result.py
+-rw-rw-rw-   0 root         (0) root         (0)    11862 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/entity_weight_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    11507 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/entity_weight_record_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11225 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/feature_flags.py
+-rw-rw-rw-   0 root         (0) root         (0)    11574 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/get_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11411 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/get_connection_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11222 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/get_dataset_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11283 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/get_default_membership_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11431 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/get_marketplace_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11485 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/get_memberships_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11379 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/get_monitor_config_v2_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11417 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/get_notification_settings_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11334 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/get_session_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11559 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/list_jobs_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11289 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/list_jobs_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11496 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/list_models_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11530 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/list_organization_memberships_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11382 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/list_user_api_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)    11502 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/log_async_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11354 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/log_reference_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11858 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/log_reference_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11441 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/log_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12111 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/log_session_reference_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12015 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/marketplace_dimensions.py
+-rw-rw-rw-   0 root         (0) root         (0)    12029 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/membership.py
+-rw-rw-rw-   0 root         (0) root         (0)    11756 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/membership_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    12260 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/metric_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    11120 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/missing_recent_data_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11132 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/missing_recent_profiles_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11938 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/missing_values_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    12569 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/model_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12219 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/model_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    13063 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11473 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/monitor_config_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    12120 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/monitor_request_reference.py
+-rw-rw-rw-   0 root         (0) root         (0)    11689 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/monitor_request_reference_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    11783 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    11982 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/notification_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    11979 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/notification_settings_day.py
+-rw-rw-rw-   0 root         (0) root         (0)    11751 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/notification_sqs_message_cadence.py
+-rw-rw-rw-   0 root         (0) root         (0)    14425 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/organization_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    13737 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/organization_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)    11215 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/pager_duty_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    12319 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/provided_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11680 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/provision_databricks_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11657 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/provision_databricks_connection_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11882 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/provision_new_aws_marketplace_user_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12226 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/provision_new_marketplace_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12422 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/provision_new_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11574 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/provision_new_user_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12387 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/reference_profile_item_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11188 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/refresh_access_token_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11444 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/refresh_connection_by_org_id_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11586 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/refresh_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    13668 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/register_databricks_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11112 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/register_databricks_connection_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11317 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/remove_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    13372 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/request_feature_monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15325 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/request_monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11070 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11580 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/role.py
+-rw-rw-rw-   0 root         (0) root         (0)    11922 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/run_job_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11089 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/run_job_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11471 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/schema_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11530 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/search_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11833 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/seasonal_arima_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11197 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/segment.py
+-rw-rw-rw-   0 root         (0) root         (0)    11192 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/segment_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)    11505 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/segment_weight.py
+-rw-rw-rw-   0 root         (0) root         (0)    11948 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/session_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11350 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/set_default_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11193 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/slack_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    11652 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/subscription_tier.py
+-rw-rw-rw-   0 root         (0) root         (0)    11670 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/time_period.py
+-rw-rw-rw-   0 root         (0) root         (0)    12934 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/uber_notification_schedule.py
+-rw-rw-rw-   0 root         (0) root         (0)    11917 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/unique_values_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11548 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/update_connection_changes.py
+-rw-rw-rw-   0 root         (0) root         (0)    11816 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/update_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11650 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/update_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11747 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/user.py
+-rw-rw-rw-   0 root         (0) root         (0)    13667 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/user_api_key.py
+-rw-rw-rw-   0 root         (0) root         (0)    11220 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/user_api_key_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11805 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model/why_logs_metric.py
+-rw-rw-rw-   0 root         (0) root         (0)    81897 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 00:36:10.880926 whylabs-client-0.4.7/whylabs_client/models/
+-rw-rw-rw-   0 root         (0) root         (0)     9913 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14199 2023-04-28 00:35:59.000000 whylabs-client-0.4.7/whylabs_client/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 00:36:10.832923 whylabs-client-0.4.7/whylabs_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3358 2023-04-28 00:36:10.000000 whylabs-client-0.4.7/whylabs_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6694 2023-04-28 00:36:10.000000 whylabs-client-0.4.7/whylabs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 00:36:10.000000 whylabs-client-0.4.7/whylabs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-28 00:36:10.000000 whylabs-client-0.4.7/whylabs_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-28 00:36:10.000000 whylabs-client-0.4.7/whylabs_client.egg-info/top_level.txt
```

### Comparing `whylabs-client-0.4.6/PKG-INFO` & `whylabs-client-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylabs-client
-Version: 0.4.6
+Version: 0.4.7
 Summary: WhyLabs API client
 Home-page: UNKNOWN
 Author: WhyLabs
 Author-email: support@whylabs.ai
 License: Apache License 2.0
 Keywords: OpenAPI,OpenAPI-Generator,WhyLabs API client
 Platform: UNKNOWN
```

### Comparing `whylabs-client-0.4.6/README.md` & `whylabs-client-0.4.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # whylabs-client
 WhyLabs API that enables end-to-end AI observability
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.1
-- Package version: 0.4.6
+- Package version: 0.4.7
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://whylabs.ai](https://whylabs.ai)
 
 ## Requirements.
 
 Python >= 3.6
 
@@ -93,14 +93,16 @@
 
 All URIs are relative to *http://localhost*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *DatasetProfileApi* | [**delete_analyzer_results**](docs/DatasetProfileApi.md#delete_analyzer_results) | **DELETE** /v0/organizations/{org_id}/dataset-profiles/models/{dataset_id}/analyzer-results | Deletes a set of analyzer results
 *DatasetProfileApi* | [**delete_dataset_profiles**](docs/DatasetProfileApi.md#delete_dataset_profiles) | **DELETE** /v0/organizations/{org_id}/dataset-profiles/models/{dataset_id} | Deletes a set of dataset profiles
+*DatasetProfileApi* | [**delete_reference_profile**](docs/DatasetProfileApi.md#delete_reference_profile) | **DELETE** /v0/organizations/{org_id}/dataset-profiles/models/{model_id}/reference-profiles/{reference_id} | Delete a single reference profile
+*DatasetProfileApi* | [**get_reference_profile**](docs/DatasetProfileApi.md#get_reference_profile) | **GET** /v0/organizations/{org_id}/dataset-profiles/models/{model_id}/reference-profiles/{reference_id} | Returns a single reference profile
 *DatasetProfileApi* | [**list_reference_profiles**](docs/DatasetProfileApi.md#list_reference_profiles) | **GET** /v0/organizations/{org_id}/dataset-profiles/models/{model_id}/reference-profiles | Returns a list for reference profiles
 *DatasetMetadataApi* | [**delete_dataset_metadata**](docs/DatasetMetadataApi.md#delete_dataset_metadata) | **DELETE** /v0/organizations/{org_id}/dataset/{dataset_id}/metadata | Delete dataset metadata for the specified dataset
 *DatasetMetadataApi* | [**get_dataset_metadata**](docs/DatasetMetadataApi.md#get_dataset_metadata) | **GET** /v0/organizations/{org_id}/dataset/{dataset_id}/metadata | Get dataset metadata for the specified dataset
 *DatasetMetadataApi* | [**put_dataset_metadata**](docs/DatasetMetadataApi.md#put_dataset_metadata) | **PUT** /v0/organizations/{org_id}/dataset/{dataset_id}/metadata | Put dataset metadata for the specified dataset
 *FeatureWeightsApi* | [**get_column_weights**](docs/FeatureWeightsApi.md#get_column_weights) | **GET** /v0/organizations/{org_id}/dataset/{dataset_id}/weights | Get column weights for the specified dataset
 *FeatureWeightsApi* | [**put_column_weights**](docs/FeatureWeightsApi.md#put_column_weights) | **PUT** /v0/organizations/{org_id}/dataset/{dataset_id}/weights | Put column weights for the specified dataset
 *LogApi* | [**log_async**](docs/LogApi.md#log_async) | **POST** /v0/organizations/{org_id}/log/async/{dataset_id} | Like /log, except this api doesn&#39;t take the actual profile content. It returns an upload link that can be used to upload the profile to.
@@ -159,38 +161,40 @@
  - [AsyncLogResponse](docs/AsyncLogResponse.md)
  - [BatchLogReferenceRequest](docs/BatchLogReferenceRequest.md)
  - [BatchLogSessionReferenceResponse](docs/BatchLogSessionReferenceResponse.md)
  - [ColumnSchema](docs/ColumnSchema.md)
  - [CreateSessionRequest](docs/CreateSessionRequest.md)
  - [CreateSessionResponse](docs/CreateSessionResponse.md)
  - [CreateUserRequest](docs/CreateUserRequest.md)
- - [DTOAutoScaleDTO](docs/DTOAutoScaleDTO.md)
- - [DTOAwsAttributesDTO](docs/DTOAwsAttributesDTO.md)
- - [DTOAwsAvailabilityDTO](docs/DTOAwsAvailabilityDTO.md)
- - [DTOClusterLogConfDTO](docs/DTOClusterLogConfDTO.md)
- - [DTOCronScheduleDTO](docs/DTOCronScheduleDTO.md)
- - [DTODbfsStorageInfoDTO](docs/DTODbfsStorageInfoDTO.md)
+ - [DTOClustersAutoScaleDTO](docs/DTOClustersAutoScaleDTO.md)
+ - [DTOClustersAwsAttributesDTO](docs/DTOClustersAwsAttributesDTO.md)
+ - [DTOClustersAwsAvailabilityDTO](docs/DTOClustersAwsAvailabilityDTO.md)
+ - [DTOClustersClusterLogConfDTO](docs/DTOClustersClusterLogConfDTO.md)
+ - [DTOClustersDbfsStorageInfoDTO](docs/DTOClustersDbfsStorageInfoDTO.md)
+ - [DTOClustersS3StorageInfoDTO](docs/DTOClustersS3StorageInfoDTO.md)
  - [DTOEbsVolumeTypeDTO](docs/DTOEbsVolumeTypeDTO.md)
- - [DTOJobDTO](docs/DTOJobDTO.md)
- - [DTOJobEmailNotificationsDTO](docs/DTOJobEmailNotificationsDTO.md)
- - [DTOJobSettingsDTO](docs/DTOJobSettingsDTO.md)
- - [DTONewClusterDTO](docs/DTONewClusterDTO.md)
- - [DTONotebookTaskDTO](docs/DTONotebookTaskDTO.md)
- - [DTOS3StorageInfoDTO](docs/DTOS3StorageInfoDTO.md)
- - [DTOSparkJarTaskDTO](docs/DTOSparkJarTaskDTO.md)
- - [DTOSparkPythonTaskDTO](docs/DTOSparkPythonTaskDTO.md)
- - [DTOSparkSubmitTaskDTO](docs/DTOSparkSubmitTaskDTO.md)
+ - [DTOJobsCronScheduleDTO](docs/DTOJobsCronScheduleDTO.md)
+ - [DTOJobsDataSecurityModeDTO](docs/DTOJobsDataSecurityModeDTO.md)
+ - [DTOJobsJobDTO](docs/DTOJobsJobDTO.md)
+ - [DTOJobsJobEmailNotificationsDTO](docs/DTOJobsJobEmailNotificationsDTO.md)
+ - [DTOJobsJobSettingsDTO](docs/DTOJobsJobSettingsDTO.md)
+ - [DTOJobsNewClusterDTO](docs/DTOJobsNewClusterDTO.md)
+ - [DTOJobsNotebookTaskDTO](docs/DTOJobsNotebookTaskDTO.md)
+ - [DTOJobsSparkJarTaskDTO](docs/DTOJobsSparkJarTaskDTO.md)
+ - [DTOJobsSparkPythonTaskDTO](docs/DTOJobsSparkPythonTaskDTO.md)
+ - [DTOJobsSparkSubmitTaskDTO](docs/DTOJobsSparkSubmitTaskDTO.md)
  - [DatabricksConnection](docs/DatabricksConnection.md)
  - [DatasetRequestMonitorConfig](docs/DatasetRequestMonitorConfig.md)
  - [DatatypeMonitorRequestConfig](docs/DatatypeMonitorRequestConfig.md)
  - [DeleteAnalyzerResultsResponse](docs/DeleteAnalyzerResultsResponse.md)
  - [DeleteDatasetProfilesResponse](docs/DeleteDatasetProfilesResponse.md)
  - [DistributionMonitorRequestConfig](docs/DistributionMonitorRequestConfig.md)
  - [EmailNotificationAction](docs/EmailNotificationAction.md)
  - [EntitySchema](docs/EntitySchema.md)
+ - [EntitySearchResult](docs/EntitySearchResult.md)
  - [EntityWeightRecord](docs/EntityWeightRecord.md)
  - [EntityWeightRecordMetadata](docs/EntityWeightRecordMetadata.md)
  - [FeatureFlags](docs/FeatureFlags.md)
  - [GetConnectionRequest](docs/GetConnectionRequest.md)
  - [GetConnectionResponse](docs/GetConnectionResponse.md)
  - [GetDatasetMetadataResponse](docs/GetDatasetMetadataResponse.md)
  - [GetDefaultMembershipResponse](docs/GetDefaultMembershipResponse.md)
@@ -246,14 +250,15 @@
  - [RequestFeatureMonitorConfig](docs/RequestFeatureMonitorConfig.md)
  - [RequestMonitorConfig](docs/RequestMonitorConfig.md)
  - [Response](docs/Response.md)
  - [Role](docs/Role.md)
  - [RunJobRequest](docs/RunJobRequest.md)
  - [RunJobResponse](docs/RunJobResponse.md)
  - [SchemaMetadata](docs/SchemaMetadata.md)
+ - [SearchResponse](docs/SearchResponse.md)
  - [SeasonalARIMARequestConfig](docs/SeasonalARIMARequestConfig.md)
  - [Segment](docs/Segment.md)
  - [SegmentTag](docs/SegmentTag.md)
  - [SegmentWeight](docs/SegmentWeight.md)
  - [SessionMetadata](docs/SessionMetadata.md)
  - [SetDefaultMembershipRequest](docs/SetDefaultMembershipRequest.md)
  - [SlackNotificationAction](docs/SlackNotificationAction.md)
```

### Comparing `whylabs-client-0.4.6/setup.py` & `whylabs-client-0.4.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from setuptools import setup, find_packages  # noqa: H301
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "RELEASE.md").read_text()
 
 NAME = "whylabs-client"
-VERSION = "0.4.6"
+VERSION = "0.4.7"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `whylabs-client-0.4.6/whylabs_client/__init__.py` & `whylabs-client-0.4.7/whylabs_client/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: 0.1
     Contact: support@whylabs.ai
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.4.6"
+__version__ = "0.4.7"
 
 # import ApiClient
 from whylabs_client.api_client import ApiClient
 
 # import Configuration
 from whylabs_client.configuration import Configuration
```

### Comparing `whylabs-client-0.4.6/whylabs_client/api/dataset_metadata_api.py` & `whylabs-client-0.4.7/whylabs_client/api/dataset_metadata_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/api/dataset_profile_api.py` & `whylabs-client-0.4.7/whylabs_client/api/dataset_profile_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -178,14 +178,140 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.delete_reference_profile_endpoint = _Endpoint(
+            settings={
+                'response_type': (bool,),
+                'auth': [
+                    'ApiKeyAuth'
+                ],
+                'endpoint_path': '/v0/organizations/{org_id}/dataset-profiles/models/{model_id}/reference-profiles/{reference_id}',
+                'operation_id': 'delete_reference_profile',
+                'http_method': 'DELETE',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'org_id',
+                    'model_id',
+                    'reference_id',
+                ],
+                'required': [
+                    'org_id',
+                    'model_id',
+                    'reference_id',
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
+                    'org_id':
+                        (str,),
+                    'model_id':
+                        (str,),
+                    'reference_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'org_id': 'org_id',
+                    'model_id': 'model_id',
+                    'reference_id': 'reference_id',
+                },
+                'location_map': {
+                    'org_id': 'path',
+                    'model_id': 'path',
+                    'reference_id': 'path',
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
+        self.get_reference_profile_endpoint = _Endpoint(
+            settings={
+                'response_type': (ReferenceProfileItemResponse,),
+                'auth': [
+                    'ApiKeyAuth'
+                ],
+                'endpoint_path': '/v0/organizations/{org_id}/dataset-profiles/models/{model_id}/reference-profiles/{reference_id}',
+                'operation_id': 'get_reference_profile',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'org_id',
+                    'model_id',
+                    'reference_id',
+                ],
+                'required': [
+                    'org_id',
+                    'model_id',
+                    'reference_id',
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
+                    'org_id':
+                        (str,),
+                    'model_id':
+                        (str,),
+                    'reference_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'org_id': 'org_id',
+                    'model_id': 'model_id',
+                    'reference_id': 'reference_id',
+                },
+                'location_map': {
+                    'org_id': 'path',
+                    'model_id': 'path',
+                    'reference_id': 'path',
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
         self.list_reference_profiles_endpoint = _Endpoint(
             settings={
                 'response_type': ([ReferenceProfileItemResponse],),
                 'auth': [
                     'ApiKeyAuth'
                 ],
                 'endpoint_path': '/v0/organizations/{org_id}/dataset-profiles/models/{model_id}/reference-profiles',
@@ -403,14 +529,172 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['org_id'] = \
             org_id
         kwargs['dataset_id'] = \
             dataset_id
         return self.delete_dataset_profiles_endpoint.call_with_http_info(**kwargs)
 
+    def delete_reference_profile(
+        self,
+        org_id,
+        model_id,
+        reference_id,
+        **kwargs
+    ):
+        """Delete a single reference profile  # noqa: E501
+
+        Delete a a Reference Profile. Returns false if the deletion encountered some error.            # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.delete_reference_profile(org_id, model_id, reference_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            org_id (str): Your company's unique organization ID
+            model_id (str): The unique model ID in your company.
+            reference_id (str): Unique reference Id.
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
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            bool
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
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['org_id'] = \
+            org_id
+        kwargs['model_id'] = \
+            model_id
+        kwargs['reference_id'] = \
+            reference_id
+        return self.delete_reference_profile_endpoint.call_with_http_info(**kwargs)
+
+    def get_reference_profile(
+        self,
+        org_id,
+        model_id,
+        reference_id,
+        **kwargs
+    ):
+        """Returns a single reference profile  # noqa: E501
+
+        Returns a Reference Profile.            # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_reference_profile(org_id, model_id, reference_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            org_id (str): Your company's unique organization ID
+            model_id (str): The unique model ID in your company.
+            reference_id (str): Unique reference Id.
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
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ReferenceProfileItemResponse
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
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['org_id'] = \
+            org_id
+        kwargs['model_id'] = \
+            model_id
+        kwargs['reference_id'] = \
+            reference_id
+        return self.get_reference_profile_endpoint.call_with_http_info(**kwargs)
+
     def list_reference_profiles(
         self,
         org_id,
         model_id,
         **kwargs
     ):
         """Returns a list for reference profiles  # noqa: E501
```

### Comparing `whylabs-client-0.4.6/whylabs_client/api/feature_weights_api.py` & `whylabs-client-0.4.7/whylabs_client/api/feature_weights_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/api/log_api.py` & `whylabs-client-0.4.7/whylabs_client/api/log_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/api/membership_api.py` & `whylabs-client-0.4.7/whylabs_client/api/membership_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/api/models_api.py` & `whylabs-client-0.4.7/whylabs_client/api/models_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/api/monitor_api.py` & `whylabs-client-0.4.7/whylabs_client/api/monitor_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/api/notification_settings_api.py` & `whylabs-client-0.4.7/whylabs_client/api/notification_settings_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/api/schema_api.py` & `whylabs-client-0.4.7/whylabs_client/api/schema_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/api/sessions_api.py` & `whylabs-client-0.4.7/whylabs_client/api/sessions_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/api_client.py` & `whylabs-client-0.4.7/whylabs_client/api_client.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/apis/__init__.py` & `whylabs-client-0.4.7/whylabs_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/configuration.py` & `whylabs-client-0.4.7/whylabs_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -406,15 +406,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1\n"\
-               "SDK Package Version: 0.4.6".\
+               "SDK Package Version: 0.4.7".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `whylabs-client-0.4.6/whylabs_client/exceptions.py` & `whylabs-client-0.4.7/whylabs_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/action_type.py` & `whylabs-client-0.4.7/whylabs_client/model/action_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/add_membership_request.py` & `whylabs-client-0.4.7/whylabs_client/model/add_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/async_log_response.py` & `whylabs-client-0.4.7/whylabs_client/model/async_log_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/aws_marketplace_metadata.py` & `whylabs-client-0.4.7/whylabs_client/model/aws_marketplace_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/batch_log_reference_request.py` & `whylabs-client-0.4.7/whylabs_client/model/batch_log_reference_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/batch_log_session_reference_response.py` & `whylabs-client-0.4.7/whylabs_client/model/batch_log_session_reference_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/column_schema.py` & `whylabs-client-0.4.7/whylabs_client/model/column_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/create_session_request.py` & `whylabs-client-0.4.7/whylabs_client/model/create_session_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/create_session_response.py` & `whylabs-client-0.4.7/whylabs_client/model/create_session_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/create_user_request.py` & `whylabs-client-0.4.7/whylabs_client/model/create_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/databricks_connection.py` & `whylabs-client-0.4.7/whylabs_client/model/databricks_connection.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/dataset_request_monitor_config.py` & `whylabs-client-0.4.7/whylabs_client/model/dataset_request_monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/datatype_monitor_request_config.py` & `whylabs-client-0.4.7/whylabs_client/model/datatype_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/delete_analyzer_results_response.py` & `whylabs-client-0.4.7/whylabs_client/model/delete_analyzer_results_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/delete_dataset_profiles_response.py` & `whylabs-client-0.4.7/whylabs_client/model/delete_dataset_profiles_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/distribution_monitor_request_config.py` & `whylabs-client-0.4.7/whylabs_client/model/distribution_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/dto_auto_scale_dto.py` & `whylabs-client-0.4.7/whylabs_client/model/dto_clusters_auto_scale_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class DTOAutoScaleDTO(ModelNormal):
+class DTOClustersAutoScaleDTO(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -100,15 +100,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """DTOAutoScaleDTO - a model defined in OpenAPI
+        """DTOClustersAutoScaleDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -183,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """DTOAutoScaleDTO - a model defined in OpenAPI
+        """DTOClustersAutoScaleDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `whylabs-client-0.4.6/whylabs_client/model/dto_aws_attributes_dto.py` & `whylabs-client-0.4.7/whylabs_client/model/dto_clusters_aws_attributes_dto.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,21 +27,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from whylabs_client.model.dto_aws_availability_dto import DTOAwsAvailabilityDTO
+    from whylabs_client.model.dto_clusters_aws_availability_dto import DTOClustersAwsAvailabilityDTO
     from whylabs_client.model.dto_ebs_volume_type_dto import DTOEbsVolumeTypeDTO
-    globals()['DTOAwsAvailabilityDTO'] = DTOAwsAvailabilityDTO
+    globals()['DTOClustersAwsAvailabilityDTO'] = DTOClustersAwsAvailabilityDTO
     globals()['DTOEbsVolumeTypeDTO'] = DTOEbsVolumeTypeDTO
 
 
-class DTOAwsAttributesDTO(ModelNormal):
+class DTOClustersAwsAttributesDTO(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -87,15 +87,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'first_on_demand': (int,),  # noqa: E501
-            'availability': (DTOAwsAvailabilityDTO,),  # noqa: E501
+            'availability': (DTOClustersAwsAvailabilityDTO,),  # noqa: E501
             'zone_id': (str,),  # noqa: E501
             'instance_profile_arn': (str,),  # noqa: E501
             'spot_bid_price_percent': (int,),  # noqa: E501
             'ebs_volume_type': (DTOEbsVolumeTypeDTO,),  # noqa: E501
             'ebs_volume_count': (int,),  # noqa: E501
             'ebs_volume_size': (int,),  # noqa: E501
         }
@@ -120,15 +120,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """DTOAwsAttributesDTO - a model defined in OpenAPI
+        """DTOClustersAwsAttributesDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -154,15 +154,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             first_on_demand (int): [optional]  # noqa: E501
-            availability (DTOAwsAvailabilityDTO): [optional]  # noqa: E501
+            availability (DTOClustersAwsAvailabilityDTO): [optional]  # noqa: E501
             zone_id (str): [optional]  # noqa: E501
             instance_profile_arn (str): [optional]  # noqa: E501
             spot_bid_price_percent (int): [optional]  # noqa: E501
             ebs_volume_type (DTOEbsVolumeTypeDTO): [optional]  # noqa: E501
             ebs_volume_count (int): [optional]  # noqa: E501
             ebs_volume_size (int): [optional]  # noqa: E501
         """
@@ -209,15 +209,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """DTOAwsAttributesDTO - a model defined in OpenAPI
+        """DTOClustersAwsAttributesDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -243,15 +243,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             first_on_demand (int): [optional]  # noqa: E501
-            availability (DTOAwsAvailabilityDTO): [optional]  # noqa: E501
+            availability (DTOClustersAwsAvailabilityDTO): [optional]  # noqa: E501
             zone_id (str): [optional]  # noqa: E501
             instance_profile_arn (str): [optional]  # noqa: E501
             spot_bid_price_percent (int): [optional]  # noqa: E501
             ebs_volume_type (DTOEbsVolumeTypeDTO): [optional]  # noqa: E501
             ebs_volume_count (int): [optional]  # noqa: E501
             ebs_volume_size (int): [optional]  # noqa: E501
         """
```

### Comparing `whylabs-client-0.4.6/whylabs_client/model/dto_aws_availability_dto.py` & `whylabs-client-0.4.7/whylabs_client/model/dto_clusters_aws_availability_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class DTOAwsAvailabilityDTO(ModelSimple):
+class DTOClustersAwsAvailabilityDTO(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -98,15 +98,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """DTOAwsAvailabilityDTO - a model defined in OpenAPI
+        """DTOClustersAwsAvailabilityDTO - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
             args[0] (str):, must be one of ["SPOT", "ON_DEMAND", "SPOT_WITH_FALLBACK", ]  # noqa: E501
 
         Keyword Args:
@@ -188,15 +188,15 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """DTOAwsAvailabilityDTO - a model defined in OpenAPI
+        """DTOClustersAwsAvailabilityDTO - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
             args[0] (str):, must be one of ["SPOT", "ON_DEMAND", "SPOT_WITH_FALLBACK", ]  # noqa: E501
 
         Keyword Args:
```

### Comparing `whylabs-client-0.4.6/whylabs_client/model/dto_cluster_log_conf_dto.py` & `whylabs-client-0.4.7/whylabs_client/model/dto_jobs_notebook_task_dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,22 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from whylabs_client.model.dto_dbfs_storage_info_dto import DTODbfsStorageInfoDTO
-    from whylabs_client.model.dtos3_storage_info_dto import DTOS3StorageInfoDTO
-    globals()['DTODbfsStorageInfoDTO'] = DTODbfsStorageInfoDTO
-    globals()['DTOS3StorageInfoDTO'] = DTOS3StorageInfoDTO
 
-
-class DTOClusterLogConfDTO(ModelNormal):
+class DTOJobsNotebookTaskDTO(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -69,54 +63,54 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'dbfs': (DTODbfsStorageInfoDTO,),  # noqa: E501
-            's3': (DTOS3StorageInfoDTO,),  # noqa: E501
+            'notebook_path': (str,),  # noqa: E501
+            'base_parameters': ({str: (str,)},),  # noqa: E501
+            'revision_timestamp': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'dbfs': 'dbfs',  # noqa: E501
-        's3': 's3',  # noqa: E501
+        'notebook_path': 'notebookPath',  # noqa: E501
+        'base_parameters': 'baseParameters',  # noqa: E501
+        'revision_timestamp': 'revisionTimestamp',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """DTOClusterLogConfDTO - a model defined in OpenAPI
+        """DTOJobsNotebookTaskDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -141,16 +135,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            dbfs (DTODbfsStorageInfoDTO): [optional]  # noqa: E501
-            s3 (DTOS3StorageInfoDTO): [optional]  # noqa: E501
+            notebook_path (str): [optional]  # noqa: E501
+            base_parameters ({str: (str,)}): [optional]  # noqa: E501
+            revision_timestamp (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -191,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """DTOClusterLogConfDTO - a model defined in OpenAPI
+        """DTOJobsNotebookTaskDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -224,16 +219,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            dbfs (DTODbfsStorageInfoDTO): [optional]  # noqa: E501
-            s3 (DTOS3StorageInfoDTO): [optional]  # noqa: E501
+            notebook_path (str): [optional]  # noqa: E501
+            base_parameters ({str: (str,)}): [optional]  # noqa: E501
+            revision_timestamp (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `whylabs-client-0.4.6/whylabs_client/model/dto_cron_schedule_dto.py` & `whylabs-client-0.4.7/whylabs_client/model/dto_jobs_cron_schedule_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class DTOCronScheduleDTO(ModelNormal):
+class DTOJobsCronScheduleDTO(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -100,15 +100,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """DTOCronScheduleDTO - a model defined in OpenAPI
+        """DTOJobsCronScheduleDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -183,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """DTOCronScheduleDTO - a model defined in OpenAPI
+        """DTOJobsCronScheduleDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `whylabs-client-0.4.6/whylabs_client/model/dto_dbfs_storage_info_dto.py` & `whylabs-client-0.4.7/whylabs_client/model/dto_clusters_dbfs_storage_info_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class DTODbfsStorageInfoDTO(ModelNormal):
+class DTOClustersDbfsStorageInfoDTO(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -98,15 +98,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """DTODbfsStorageInfoDTO - a model defined in OpenAPI
+        """DTOClustersDbfsStorageInfoDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -180,15 +180,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """DTODbfsStorageInfoDTO - a model defined in OpenAPI
+        """DTOClustersDbfsStorageInfoDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `whylabs-client-0.4.6/whylabs_client/model/dto_ebs_volume_type_dto.py` & `whylabs-client-0.4.7/whylabs_client/model/dto_ebs_volume_type_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/dto_job_dto.py` & `whylabs-client-0.4.7/whylabs_client/model/dto_jobs_job_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from whylabs_client.model.dto_job_settings_dto import DTOJobSettingsDTO
-    globals()['DTOJobSettingsDTO'] = DTOJobSettingsDTO
+    from whylabs_client.model.dto_jobs_job_settings_dto import DTOJobsJobSettingsDTO
+    globals()['DTOJobsJobSettingsDTO'] = DTOJobsJobSettingsDTO
 
 
-class DTOJobDTO(ModelNormal):
+class DTOJobsJobDTO(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,40 +85,40 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'job_id': (int,),  # noqa: E501
-            'settings': (DTOJobSettingsDTO,),  # noqa: E501
-            'created_time': (datetime,),  # noqa: E501
             'creator_user_name': (str,),  # noqa: E501
+            'settings': (DTOJobsJobSettingsDTO,),  # noqa: E501
+            'created_time': (datetime,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'job_id': 'jobId',  # noqa: E501
+        'creator_user_name': 'creatorUserName',  # noqa: E501
         'settings': 'settings',  # noqa: E501
         'created_time': 'createdTime',  # noqa: E501
-        'creator_user_name': 'creatorUserName',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """DTOJobDTO - a model defined in OpenAPI
+        """DTOJobsJobDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -144,17 +144,17 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             job_id (int): [optional]  # noqa: E501
-            settings (DTOJobSettingsDTO): [optional]  # noqa: E501
-            created_time (datetime): [optional]  # noqa: E501
             creator_user_name (str): [optional]  # noqa: E501
+            settings (DTOJobsJobSettingsDTO): [optional]  # noqa: E501
+            created_time (datetime): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,15 +195,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """DTOJobDTO - a model defined in OpenAPI
+        """DTOJobsJobDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -229,17 +229,17 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             job_id (int): [optional]  # noqa: E501
-            settings (DTOJobSettingsDTO): [optional]  # noqa: E501
-            created_time (datetime): [optional]  # noqa: E501
             creator_user_name (str): [optional]  # noqa: E501
+            settings (DTOJobsJobSettingsDTO): [optional]  # noqa: E501
+            created_time (datetime): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `whylabs-client-0.4.6/whylabs_client/model/dto_job_email_notifications_dto.py` & `whylabs-client-0.4.7/whylabs_client/model/dto_jobs_job_email_notifications_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class DTOJobEmailNotificationsDTO(ModelNormal):
+class DTOJobsJobEmailNotificationsDTO(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,41 +78,41 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'on_failure': ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}],),  # noqa: E501
             'on_start': ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}],),  # noqa: E501
             'on_success': ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}],),  # noqa: E501
+            'on_failure': ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}],),  # noqa: E501
             'no_alert_for_skipped_runs': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'on_failure': 'onFailure',  # noqa: E501
         'on_start': 'onStart',  # noqa: E501
         'on_success': 'onSuccess',  # noqa: E501
+        'on_failure': 'onFailure',  # noqa: E501
         'no_alert_for_skipped_runs': 'noAlertForSkippedRuns',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """DTOJobEmailNotificationsDTO - a model defined in OpenAPI
+        """DTOJobsJobEmailNotificationsDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,17 +137,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            on_failure ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
             on_start ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
             on_success ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
+            on_failure ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
             no_alert_for_skipped_runs (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -189,15 +189,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """DTOJobEmailNotificationsDTO - a model defined in OpenAPI
+        """DTOJobsJobEmailNotificationsDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -222,17 +222,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            on_failure ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
             on_start ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
             on_success ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
+            on_failure ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
             no_alert_for_skipped_runs (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `whylabs-client-0.4.6/whylabs_client/model/dto_job_settings_dto.py` & `whylabs-client-0.4.7/whylabs_client/model/dto_jobs_job_settings_dto.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,31 +27,31 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from whylabs_client.model.dto_cron_schedule_dto import DTOCronScheduleDTO
-    from whylabs_client.model.dto_job_email_notifications_dto import DTOJobEmailNotificationsDTO
-    from whylabs_client.model.dto_new_cluster_dto import DTONewClusterDTO
-    from whylabs_client.model.dto_notebook_task_dto import DTONotebookTaskDTO
-    from whylabs_client.model.dto_spark_jar_task_dto import DTOSparkJarTaskDTO
-    from whylabs_client.model.dto_spark_python_task_dto import DTOSparkPythonTaskDTO
-    from whylabs_client.model.dto_spark_submit_task_dto import DTOSparkSubmitTaskDTO
-    globals()['DTOCronScheduleDTO'] = DTOCronScheduleDTO
-    globals()['DTOJobEmailNotificationsDTO'] = DTOJobEmailNotificationsDTO
-    globals()['DTONewClusterDTO'] = DTONewClusterDTO
-    globals()['DTONotebookTaskDTO'] = DTONotebookTaskDTO
-    globals()['DTOSparkJarTaskDTO'] = DTOSparkJarTaskDTO
-    globals()['DTOSparkPythonTaskDTO'] = DTOSparkPythonTaskDTO
-    globals()['DTOSparkSubmitTaskDTO'] = DTOSparkSubmitTaskDTO
+    from whylabs_client.model.dto_jobs_cron_schedule_dto import DTOJobsCronScheduleDTO
+    from whylabs_client.model.dto_jobs_job_email_notifications_dto import DTOJobsJobEmailNotificationsDTO
+    from whylabs_client.model.dto_jobs_new_cluster_dto import DTOJobsNewClusterDTO
+    from whylabs_client.model.dto_jobs_notebook_task_dto import DTOJobsNotebookTaskDTO
+    from whylabs_client.model.dto_jobs_spark_jar_task_dto import DTOJobsSparkJarTaskDTO
+    from whylabs_client.model.dto_jobs_spark_python_task_dto import DTOJobsSparkPythonTaskDTO
+    from whylabs_client.model.dto_jobs_spark_submit_task_dto import DTOJobsSparkSubmitTaskDTO
+    globals()['DTOJobsCronScheduleDTO'] = DTOJobsCronScheduleDTO
+    globals()['DTOJobsJobEmailNotificationsDTO'] = DTOJobsJobEmailNotificationsDTO
+    globals()['DTOJobsNewClusterDTO'] = DTOJobsNewClusterDTO
+    globals()['DTOJobsNotebookTaskDTO'] = DTOJobsNotebookTaskDTO
+    globals()['DTOJobsSparkJarTaskDTO'] = DTOJobsSparkJarTaskDTO
+    globals()['DTOJobsSparkPythonTaskDTO'] = DTOJobsSparkPythonTaskDTO
+    globals()['DTOJobsSparkSubmitTaskDTO'] = DTOJobsSparkSubmitTaskDTO
 
 
-class DTOJobSettingsDTO(ModelNormal):
+class DTOJobsJobSettingsDTO(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -96,63 +96,63 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'name': (str,),  # noqa: E501
-            'new_cluster': (DTONewClusterDTO,),  # noqa: E501
             'existing_cluster_id': (str,),  # noqa: E501
-            'email_notifications': (DTOJobEmailNotificationsDTO,),  # noqa: E501
+            'new_cluster': (DTOJobsNewClusterDTO,),  # noqa: E501
+            'notebook_task': (DTOJobsNotebookTaskDTO,),  # noqa: E501
+            'spark_jar_task': (DTOJobsSparkJarTaskDTO,),  # noqa: E501
+            'spark_python_task': (DTOJobsSparkPythonTaskDTO,),  # noqa: E501
+            'spark_submit_task': (DTOJobsSparkSubmitTaskDTO,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'libraries': ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}],),  # noqa: E501
+            'email_notifications': (DTOJobsJobEmailNotificationsDTO,),  # noqa: E501
             'timeout_seconds': (int,),  # noqa: E501
-            'schedule': (DTOCronScheduleDTO,),  # noqa: E501
-            'notebook_task': (DTONotebookTaskDTO,),  # noqa: E501
-            'spark_jar_task': (DTOSparkJarTaskDTO,),  # noqa: E501
-            'spark_python_task': (DTOSparkPythonTaskDTO,),  # noqa: E501
-            'spark_submit_task': (DTOSparkSubmitTaskDTO,),  # noqa: E501
-            'retry_on_timeout': (bool,),  # noqa: E501
             'max_retries': (int,),  # noqa: E501
             'min_retry_interval_millis': (int,),  # noqa: E501
-            'libraries': ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}],),  # noqa: E501
+            'retry_on_timeout': (bool,),  # noqa: E501
+            'schedule': (DTOJobsCronScheduleDTO,),  # noqa: E501
             'max_concurrent_runs': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
-        'new_cluster': 'newCluster',  # noqa: E501
         'existing_cluster_id': 'existingClusterId',  # noqa: E501
-        'email_notifications': 'emailNotifications',  # noqa: E501
-        'timeout_seconds': 'timeoutSeconds',  # noqa: E501
-        'schedule': 'schedule',  # noqa: E501
+        'new_cluster': 'newCluster',  # noqa: E501
         'notebook_task': 'notebookTask',  # noqa: E501
         'spark_jar_task': 'sparkJarTask',  # noqa: E501
         'spark_python_task': 'sparkPythonTask',  # noqa: E501
         'spark_submit_task': 'sparkSubmitTask',  # noqa: E501
-        'retry_on_timeout': 'retryOnTimeout',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'libraries': 'libraries',  # noqa: E501
+        'email_notifications': 'emailNotifications',  # noqa: E501
+        'timeout_seconds': 'timeoutSeconds',  # noqa: E501
         'max_retries': 'maxRetries',  # noqa: E501
         'min_retry_interval_millis': 'minRetryIntervalMillis',  # noqa: E501
-        'libraries': 'libraries',  # noqa: E501
+        'retry_on_timeout': 'retryOnTimeout',  # noqa: E501
+        'schedule': 'schedule',  # noqa: E501
         'max_concurrent_runs': 'maxConcurrentRuns',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """DTOJobSettingsDTO - a model defined in OpenAPI
+        """DTOJobsJobSettingsDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -177,28 +177,28 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            new_cluster (DTONewClusterDTO): [optional]  # noqa: E501
             existing_cluster_id (str): [optional]  # noqa: E501
-            email_notifications (DTOJobEmailNotificationsDTO): [optional]  # noqa: E501
+            new_cluster (DTOJobsNewClusterDTO): [optional]  # noqa: E501
+            notebook_task (DTOJobsNotebookTaskDTO): [optional]  # noqa: E501
+            spark_jar_task (DTOJobsSparkJarTaskDTO): [optional]  # noqa: E501
+            spark_python_task (DTOJobsSparkPythonTaskDTO): [optional]  # noqa: E501
+            spark_submit_task (DTOJobsSparkSubmitTaskDTO): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            libraries ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
+            email_notifications (DTOJobsJobEmailNotificationsDTO): [optional]  # noqa: E501
             timeout_seconds (int): [optional]  # noqa: E501
-            schedule (DTOCronScheduleDTO): [optional]  # noqa: E501
-            notebook_task (DTONotebookTaskDTO): [optional]  # noqa: E501
-            spark_jar_task (DTOSparkJarTaskDTO): [optional]  # noqa: E501
-            spark_python_task (DTOSparkPythonTaskDTO): [optional]  # noqa: E501
-            spark_submit_task (DTOSparkSubmitTaskDTO): [optional]  # noqa: E501
-            retry_on_timeout (bool): [optional]  # noqa: E501
             max_retries (int): [optional]  # noqa: E501
             min_retry_interval_millis (int): [optional]  # noqa: E501
-            libraries ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
+            retry_on_timeout (bool): [optional]  # noqa: E501
+            schedule (DTOJobsCronScheduleDTO): [optional]  # noqa: E501
             max_concurrent_runs (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -240,15 +240,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """DTOJobSettingsDTO - a model defined in OpenAPI
+        """DTOJobsJobSettingsDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -273,28 +273,28 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            new_cluster (DTONewClusterDTO): [optional]  # noqa: E501
             existing_cluster_id (str): [optional]  # noqa: E501
-            email_notifications (DTOJobEmailNotificationsDTO): [optional]  # noqa: E501
+            new_cluster (DTOJobsNewClusterDTO): [optional]  # noqa: E501
+            notebook_task (DTOJobsNotebookTaskDTO): [optional]  # noqa: E501
+            spark_jar_task (DTOJobsSparkJarTaskDTO): [optional]  # noqa: E501
+            spark_python_task (DTOJobsSparkPythonTaskDTO): [optional]  # noqa: E501
+            spark_submit_task (DTOJobsSparkSubmitTaskDTO): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            libraries ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
+            email_notifications (DTOJobsJobEmailNotificationsDTO): [optional]  # noqa: E501
             timeout_seconds (int): [optional]  # noqa: E501
-            schedule (DTOCronScheduleDTO): [optional]  # noqa: E501
-            notebook_task (DTONotebookTaskDTO): [optional]  # noqa: E501
-            spark_jar_task (DTOSparkJarTaskDTO): [optional]  # noqa: E501
-            spark_python_task (DTOSparkPythonTaskDTO): [optional]  # noqa: E501
-            spark_submit_task (DTOSparkSubmitTaskDTO): [optional]  # noqa: E501
-            retry_on_timeout (bool): [optional]  # noqa: E501
             max_retries (int): [optional]  # noqa: E501
             min_retry_interval_millis (int): [optional]  # noqa: E501
-            libraries ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
+            retry_on_timeout (bool): [optional]  # noqa: E501
+            schedule (DTOJobsCronScheduleDTO): [optional]  # noqa: E501
             max_concurrent_runs (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `whylabs-client-0.4.6/whylabs_client/model/dto_new_cluster_dto.py` & `whylabs-client-0.4.7/whylabs_client/model/dto_jobs_new_cluster_dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,23 +27,25 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from whylabs_client.model.dto_auto_scale_dto import DTOAutoScaleDTO
-    from whylabs_client.model.dto_aws_attributes_dto import DTOAwsAttributesDTO
-    from whylabs_client.model.dto_cluster_log_conf_dto import DTOClusterLogConfDTO
-    globals()['DTOAutoScaleDTO'] = DTOAutoScaleDTO
-    globals()['DTOAwsAttributesDTO'] = DTOAwsAttributesDTO
-    globals()['DTOClusterLogConfDTO'] = DTOClusterLogConfDTO
+    from whylabs_client.model.dto_clusters_auto_scale_dto import DTOClustersAutoScaleDTO
+    from whylabs_client.model.dto_clusters_aws_attributes_dto import DTOClustersAwsAttributesDTO
+    from whylabs_client.model.dto_clusters_cluster_log_conf_dto import DTOClustersClusterLogConfDTO
+    from whylabs_client.model.dto_jobs_data_security_mode_dto import DTOJobsDataSecurityModeDTO
+    globals()['DTOClustersAutoScaleDTO'] = DTOClustersAutoScaleDTO
+    globals()['DTOClustersAwsAttributesDTO'] = DTOClustersAwsAttributesDTO
+    globals()['DTOClustersClusterLogConfDTO'] = DTOClustersClusterLogConfDTO
+    globals()['DTOJobsDataSecurityModeDTO'] = DTOJobsDataSecurityModeDTO
 
 
-class DTONewClusterDTO(ModelNormal):
+class DTOJobsNewClusterDTO(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -88,61 +90,73 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'spark_version': (str,),  # noqa: E501
-            'aws_attributes': (DTOAwsAttributesDTO,),  # noqa: E501
-            'node_type_id': (str,),  # noqa: E501
+            'policy_id': (str,),  # noqa: E501
+            'runtime_engine': (str,),  # noqa: E501
             'num_workers': (int,),  # noqa: E501
-            'auto_scale': (DTOAutoScaleDTO,),  # noqa: E501
+            'auto_scale': (DTOClustersAutoScaleDTO,),  # noqa: E501
             'cluster_name': (str,),  # noqa: E501
+            'spark_version': (str,),  # noqa: E501
             'spark_conf': ({str: (str,)},),  # noqa: E501
+            'aws_attributes': (DTOClustersAwsAttributesDTO,),  # noqa: E501
+            'node_type_id': (str,),  # noqa: E501
             'driver_node_type_id': (str,),  # noqa: E501
             'ssh_public_keys': ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}],),  # noqa: E501
             'custom_tags': ({str: (str,)},),  # noqa: E501
-            'cluster_log_conf': (DTOClusterLogConfDTO,),  # noqa: E501
+            'cluster_log_conf': (DTOClustersClusterLogConfDTO,),  # noqa: E501
+            'init_scripts': ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}],),  # noqa: E501
             'spark_env_vars': ({str: (str,)},),  # noqa: E501
-            'auto_termination_minutes': (int,),  # noqa: E501
             'enable_elastic_disk': (bool,),  # noqa: E501
+            'instance_pool_id': (str,),  # noqa: E501
+            'data_security_mode': (DTOJobsDataSecurityModeDTO,),  # noqa: E501
+            'auto_termination_minutes': (int,),  # noqa: E501
+            'artifact_paths': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'spark_version': 'sparkVersion',  # noqa: E501
-        'aws_attributes': 'awsAttributes',  # noqa: E501
-        'node_type_id': 'nodeTypeId',  # noqa: E501
+        'policy_id': 'policyId',  # noqa: E501
+        'runtime_engine': 'runtimeEngine',  # noqa: E501
         'num_workers': 'numWorkers',  # noqa: E501
         'auto_scale': 'autoScale',  # noqa: E501
         'cluster_name': 'clusterName',  # noqa: E501
+        'spark_version': 'sparkVersion',  # noqa: E501
         'spark_conf': 'sparkConf',  # noqa: E501
+        'aws_attributes': 'awsAttributes',  # noqa: E501
+        'node_type_id': 'nodeTypeId',  # noqa: E501
         'driver_node_type_id': 'driverNodeTypeId',  # noqa: E501
         'ssh_public_keys': 'sshPublicKeys',  # noqa: E501
         'custom_tags': 'customTags',  # noqa: E501
         'cluster_log_conf': 'clusterLogConf',  # noqa: E501
+        'init_scripts': 'initScripts',  # noqa: E501
         'spark_env_vars': 'sparkEnvVars',  # noqa: E501
-        'auto_termination_minutes': 'autoTerminationMinutes',  # noqa: E501
         'enable_elastic_disk': 'enableElasticDisk',  # noqa: E501
+        'instance_pool_id': 'instancePoolId',  # noqa: E501
+        'data_security_mode': 'dataSecurityMode',  # noqa: E501
+        'auto_termination_minutes': 'autoTerminationMinutes',  # noqa: E501
+        'artifact_paths': 'artifactPaths',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """DTONewClusterDTO - a model defined in OpenAPI
+        """DTOJobsNewClusterDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -167,28 +181,34 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            spark_version (str): [optional]  # noqa: E501
-            aws_attributes (DTOAwsAttributesDTO): [optional]  # noqa: E501
-            node_type_id (str): [optional]  # noqa: E501
+            policy_id (str): [optional]  # noqa: E501
+            runtime_engine (str): [optional]  # noqa: E501
             num_workers (int): [optional]  # noqa: E501
-            auto_scale (DTOAutoScaleDTO): [optional]  # noqa: E501
+            auto_scale (DTOClustersAutoScaleDTO): [optional]  # noqa: E501
             cluster_name (str): [optional]  # noqa: E501
+            spark_version (str): [optional]  # noqa: E501
             spark_conf ({str: (str,)}): [optional]  # noqa: E501
+            aws_attributes (DTOClustersAwsAttributesDTO): [optional]  # noqa: E501
+            node_type_id (str): [optional]  # noqa: E501
             driver_node_type_id (str): [optional]  # noqa: E501
             ssh_public_keys ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
             custom_tags ({str: (str,)}): [optional]  # noqa: E501
-            cluster_log_conf (DTOClusterLogConfDTO): [optional]  # noqa: E501
+            cluster_log_conf (DTOClustersClusterLogConfDTO): [optional]  # noqa: E501
+            init_scripts ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
             spark_env_vars ({str: (str,)}): [optional]  # noqa: E501
-            auto_termination_minutes (int): [optional]  # noqa: E501
             enable_elastic_disk (bool): [optional]  # noqa: E501
+            instance_pool_id (str): [optional]  # noqa: E501
+            data_security_mode (DTOJobsDataSecurityModeDTO): [optional]  # noqa: E501
+            auto_termination_minutes (int): [optional]  # noqa: E501
+            artifact_paths ([str]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -229,15 +249,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """DTONewClusterDTO - a model defined in OpenAPI
+        """DTOJobsNewClusterDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -262,28 +282,34 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            spark_version (str): [optional]  # noqa: E501
-            aws_attributes (DTOAwsAttributesDTO): [optional]  # noqa: E501
-            node_type_id (str): [optional]  # noqa: E501
+            policy_id (str): [optional]  # noqa: E501
+            runtime_engine (str): [optional]  # noqa: E501
             num_workers (int): [optional]  # noqa: E501
-            auto_scale (DTOAutoScaleDTO): [optional]  # noqa: E501
+            auto_scale (DTOClustersAutoScaleDTO): [optional]  # noqa: E501
             cluster_name (str): [optional]  # noqa: E501
+            spark_version (str): [optional]  # noqa: E501
             spark_conf ({str: (str,)}): [optional]  # noqa: E501
+            aws_attributes (DTOClustersAwsAttributesDTO): [optional]  # noqa: E501
+            node_type_id (str): [optional]  # noqa: E501
             driver_node_type_id (str): [optional]  # noqa: E501
             ssh_public_keys ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
             custom_tags ({str: (str,)}): [optional]  # noqa: E501
-            cluster_log_conf (DTOClusterLogConfDTO): [optional]  # noqa: E501
+            cluster_log_conf (DTOClustersClusterLogConfDTO): [optional]  # noqa: E501
+            init_scripts ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
             spark_env_vars ({str: (str,)}): [optional]  # noqa: E501
-            auto_termination_minutes (int): [optional]  # noqa: E501
             enable_elastic_disk (bool): [optional]  # noqa: E501
+            instance_pool_id (str): [optional]  # noqa: E501
+            data_security_mode (DTOJobsDataSecurityModeDTO): [optional]  # noqa: E501
+            auto_termination_minutes (int): [optional]  # noqa: E501
+            artifact_paths ([str]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `whylabs-client-0.4.6/whylabs_client/model/dto_notebook_task_dto.py` & `whylabs-client-0.4.7/whylabs_client/model/run_job_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class DTONotebookTaskDTO(ModelNormal):
+class RunJobRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,39 +78,42 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'notebook_path': (str,),  # noqa: E501
-            'base_parameters': ({str: (str,)},),  # noqa: E501
-            'revision_timestamp': (int,),  # noqa: E501
+            'job_id': (int,),  # noqa: E501
+            'org_id': (str, none_type,),  # noqa: E501
+            'workspace_id': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'notebook_path': 'notebookPath',  # noqa: E501
-        'base_parameters': 'baseParameters',  # noqa: E501
-        'revision_timestamp': 'revisionTimestamp',  # noqa: E501
+        'job_id': 'jobId',  # noqa: E501
+        'org_id': 'orgId',  # noqa: E501
+        'workspace_id': 'workspaceId',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """DTONotebookTaskDTO - a model defined in OpenAPI
+    def _from_openapi_data(cls, job_id, *args, **kwargs):  # noqa: E501
+        """RunJobRequest - a model defined in OpenAPI
+
+        Args:
+            job_id (int): The id of the job to run in the connected Databricks workspace.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,17 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            notebook_path (str): [optional]  # noqa: E501
-            base_parameters ({str: (str,)}): [optional]  # noqa: E501
-            revision_timestamp (int): [optional]  # noqa: E501
+            org_id (str, none_type): Look up a connection by the org that is connected to.. [optional]  # noqa: E501
+            workspace_id (str, none_type): Look up a connection by the workspace that it originates from.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -165,14 +167,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.job_id = job_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -185,16 +188,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """DTONotebookTaskDTO - a model defined in OpenAPI
+    def __init__(self, job_id, *args, **kwargs):  # noqa: E501
+        """RunJobRequest - a model defined in OpenAPI
+
+        Args:
+            job_id (int): The id of the job to run in the connected Databricks workspace.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,17 +225,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            notebook_path (str): [optional]  # noqa: E501
-            base_parameters ({str: (str,)}): [optional]  # noqa: E501
-            revision_timestamp (int): [optional]  # noqa: E501
+            org_id (str, none_type): Look up a connection by the org that is connected to.. [optional]  # noqa: E501
+            workspace_id (str, none_type): Look up a connection by the workspace that it originates from.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -247,14 +252,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.job_id = job_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.4.6/whylabs_client/model/dto_spark_jar_task_dto.py` & `whylabs-client-0.4.7/whylabs_client/model/dto_jobs_spark_python_task_dto.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class DTOSparkJarTaskDTO(ModelNormal):
+class DTOJobsSparkPythonTaskDTO(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,41 +78,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'jar_uri': (str,),  # noqa: E501
-            'main_class_name': (str,),  # noqa: E501
+            'python_file': (str,),  # noqa: E501
             'parameters': ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}],),  # noqa: E501
-            'run_as_repl': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'jar_uri': 'jarUri',  # noqa: E501
-        'main_class_name': 'mainClassName',  # noqa: E501
+        'python_file': 'pythonFile',  # noqa: E501
         'parameters': 'parameters',  # noqa: E501
-        'run_as_repl': 'runAsRepl',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """DTOSparkJarTaskDTO - a model defined in OpenAPI
+        """DTOJobsSparkPythonTaskDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,18 +133,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            jar_uri (str): [optional]  # noqa: E501
-            main_class_name (str): [optional]  # noqa: E501
+            python_file (str): [optional]  # noqa: E501
             parameters ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
-            run_as_repl (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -189,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """DTOSparkJarTaskDTO - a model defined in OpenAPI
+        """DTOJobsSparkPythonTaskDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -222,18 +216,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            jar_uri (str): [optional]  # noqa: E501
-            main_class_name (str): [optional]  # noqa: E501
+            python_file (str): [optional]  # noqa: E501
             parameters ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
-            run_as_repl (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `whylabs-client-0.4.6/whylabs_client/model/dto_spark_python_task_dto.py` & `whylabs-client-0.4.7/whylabs_client/model/log_reference_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class DTOSparkPythonTaskDTO(ModelNormal):
+class LogReferenceRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,37 +78,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'python_file': (str,),  # noqa: E501
-            'parameters': ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}],),  # noqa: E501
+            'alias': (str, none_type,),  # noqa: E501
+            'dataset_timestamp': (int, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'python_file': 'pythonFile',  # noqa: E501
-        'parameters': 'parameters',  # noqa: E501
+        'alias': 'alias',  # noqa: E501
+        'dataset_timestamp': 'datasetTimestamp',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """DTOSparkPythonTaskDTO - a model defined in OpenAPI
+        """LogReferenceRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,16 +133,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            python_file (str): [optional]  # noqa: E501
-            parameters ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
+            alias (str, none_type): [optional]  # noqa: E501
+            dataset_timestamp (int, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """DTOSparkPythonTaskDTO - a model defined in OpenAPI
+        """LogReferenceRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,16 +216,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            python_file (str): [optional]  # noqa: E501
-            parameters ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
+            alias (str, none_type): [optional]  # noqa: E501
+            dataset_timestamp (int, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `whylabs-client-0.4.6/whylabs_client/model/dto_spark_submit_task_dto.py` & `whylabs-client-0.4.7/whylabs_client/model/dto_jobs_spark_submit_task_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class DTOSparkSubmitTaskDTO(ModelNormal):
+class DTOJobsSparkSubmitTaskDTO(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -98,15 +98,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """DTOSparkSubmitTaskDTO - a model defined in OpenAPI
+        """DTOJobsSparkSubmitTaskDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -180,15 +180,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """DTOSparkSubmitTaskDTO - a model defined in OpenAPI
+        """DTOJobsSparkSubmitTaskDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `whylabs-client-0.4.6/whylabs_client/model/dtos3_storage_info_dto.py` & `whylabs-client-0.4.7/whylabs_client/model/dto_clusters_s3_storage_info_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class DTOS3StorageInfoDTO(ModelNormal):
+class DTOClustersS3StorageInfoDTO(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -110,15 +110,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """DTOS3StorageInfoDTO - a model defined in OpenAPI
+        """DTOClustersS3StorageInfoDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -198,15 +198,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """DTOS3StorageInfoDTO - a model defined in OpenAPI
+        """DTOClustersS3StorageInfoDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `whylabs-client-0.4.6/whylabs_client/model/email_notification_action.py` & `whylabs-client-0.4.7/whylabs_client/model/email_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/entity_schema.py` & `whylabs-client-0.4.7/whylabs_client/model/entity_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/entity_weight_record.py` & `whylabs-client-0.4.7/whylabs_client/model/entity_weight_record.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/entity_weight_record_metadata.py` & `whylabs-client-0.4.7/whylabs_client/model/entity_weight_record_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/feature_flags.py` & `whylabs-client-0.4.7/whylabs_client/model/feature_flags.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/get_connection_request.py` & `whylabs-client-0.4.7/whylabs_client/model/get_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/get_connection_response.py` & `whylabs-client-0.4.7/whylabs_client/model/get_connection_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/get_dataset_metadata_response.py` & `whylabs-client-0.4.7/whylabs_client/model/get_dataset_metadata_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/get_default_membership_response.py` & `whylabs-client-0.4.7/whylabs_client/model/get_default_membership_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/get_marketplace_metadata_response.py` & `whylabs-client-0.4.7/whylabs_client/model/get_marketplace_metadata_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/get_memberships_response.py` & `whylabs-client-0.4.7/whylabs_client/model/get_memberships_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/get_monitor_config_v2_response.py` & `whylabs-client-0.4.7/whylabs_client/model/get_monitor_config_v2_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/get_notification_settings_response.py` & `whylabs-client-0.4.7/whylabs_client/model/get_notification_settings_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/get_session_response.py` & `whylabs-client-0.4.7/whylabs_client/model/get_session_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/list_jobs_request.py` & `whylabs-client-0.4.7/whylabs_client/model/list_jobs_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/list_jobs_response.py` & `whylabs-client-0.4.7/whylabs_client/model/list_jobs_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from whylabs_client.model.dto_job_dto import DTOJobDTO
-    globals()['DTOJobDTO'] = DTOJobDTO
+    from whylabs_client.model.dto_jobs_job_dto import DTOJobsJobDTO
+    globals()['DTOJobsJobDTO'] = DTOJobsJobDTO
 
 
 class ListJobsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -84,15 +84,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'jobs': ([DTOJobDTO],),  # noqa: E501
+            'jobs': ([DTOJobsJobDTO],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -107,15 +107,15 @@
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, jobs, *args, **kwargs):  # noqa: E501
         """ListJobsResponse - a model defined in OpenAPI
 
         Args:
-            jobs ([DTOJobDTO]):
+            jobs ([DTOJobsJobDTO]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -192,15 +192,15 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, jobs, *args, **kwargs):  # noqa: E501
         """ListJobsResponse - a model defined in OpenAPI
 
         Args:
-            jobs ([DTOJobDTO]):
+            jobs ([DTOJobsJobDTO]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `whylabs-client-0.4.6/whylabs_client/model/list_models_response.py` & `whylabs-client-0.4.7/whylabs_client/model/list_models_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/list_organization_memberships_response.py` & `whylabs-client-0.4.7/whylabs_client/model/list_organization_memberships_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/list_user_api_keys.py` & `whylabs-client-0.4.7/whylabs_client/model/list_user_api_keys.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/log_async_request.py` & `whylabs-client-0.4.7/whylabs_client/model/log_async_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/log_reference_request.py` & `whylabs-client-0.4.7/whylabs_client/model/segment_weight.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from whylabs_client.model.segment import Segment
+    globals()['Segment'] = Segment
 
-class LogReferenceRequest(ModelNormal):
+
+class SegmentWeight(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,52 +67,54 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'alias': (str, none_type,),  # noqa: E501
-            'dataset_timestamp': (int, none_type,),  # noqa: E501
+            'segment': (Segment,),  # noqa: E501
+            'weights': ({str: (float,)},),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'alias': 'alias',  # noqa: E501
-        'dataset_timestamp': 'datasetTimestamp',  # noqa: E501
+        'segment': 'segment',  # noqa: E501
+        'weights': 'weights',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """LogReferenceRequest - a model defined in OpenAPI
+        """SegmentWeight - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,16 +139,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            alias (str, none_type): [optional]  # noqa: E501
-            dataset_timestamp (int, none_type): [optional]  # noqa: E501
+            segment (Segment): [optional]  # noqa: E501
+            weights ({str: (float,)}): Entity weight value for each entity. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +189,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """LogReferenceRequest - a model defined in OpenAPI
+        """SegmentWeight - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,16 +222,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            alias (str, none_type): [optional]  # noqa: E501
-            dataset_timestamp (int, none_type): [optional]  # noqa: E501
+            segment (Segment): [optional]  # noqa: E501
+            weights ({str: (float,)}): Entity weight value for each entity. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `whylabs-client-0.4.6/whylabs_client/model/log_reference_response.py` & `whylabs-client-0.4.7/whylabs_client/model/log_reference_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/log_response.py` & `whylabs-client-0.4.7/whylabs_client/model/log_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/log_session_reference_response.py` & `whylabs-client-0.4.7/whylabs_client/model/log_session_reference_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/marketplace_dimensions.py` & `whylabs-client-0.4.7/whylabs_client/model/marketplace_dimensions.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/membership.py` & `whylabs-client-0.4.7/whylabs_client/model/membership.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/membership_metadata.py` & `whylabs-client-0.4.7/whylabs_client/model/membership_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/metric_schema.py` & `whylabs-client-0.4.7/whylabs_client/model/metric_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/missing_recent_data_request_config.py` & `whylabs-client-0.4.7/whylabs_client/model/missing_recent_data_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/missing_recent_profiles_request_config.py` & `whylabs-client-0.4.7/whylabs_client/model/missing_recent_profiles_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/missing_values_monitor_request_config.py` & `whylabs-client-0.4.7/whylabs_client/model/missing_values_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/model_metadata_response.py` & `whylabs-client-0.4.7/whylabs_client/model/model_metadata_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/model_type.py` & `whylabs-client-0.4.7/whylabs_client/model/model_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/monitor_config.py` & `whylabs-client-0.4.7/whylabs_client/model/monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/monitor_config_version.py` & `whylabs-client-0.4.7/whylabs_client/model/monitor_config_version.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/monitor_request_reference.py` & `whylabs-client-0.4.7/whylabs_client/model/monitor_request_reference.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/monitor_request_reference_type.py` & `whylabs-client-0.4.7/whylabs_client/model/monitor_request_reference_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/notification_action.py` & `whylabs-client-0.4.7/whylabs_client/model/notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/notification_settings.py` & `whylabs-client-0.4.7/whylabs_client/model/notification_settings.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/notification_settings_day.py` & `whylabs-client-0.4.7/whylabs_client/model/notification_settings_day.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/notification_sqs_message_cadence.py` & `whylabs-client-0.4.7/whylabs_client/model/notification_sqs_message_cadence.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/organization_metadata.py` & `whylabs-client-0.4.7/whylabs_client/model/organization_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/organization_summary.py` & `whylabs-client-0.4.7/whylabs_client/model/organization_summary.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/pager_duty_notification_action.py` & `whylabs-client-0.4.7/whylabs_client/model/pager_duty_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/provided_config.py` & `whylabs-client-0.4.7/whylabs_client/model/provided_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/provision_databricks_connection_request.py` & `whylabs-client-0.4.7/whylabs_client/model/provision_databricks_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/provision_databricks_connection_response.py` & `whylabs-client-0.4.7/whylabs_client/model/provision_databricks_connection_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/provision_new_aws_marketplace_user_response.py` & `whylabs-client-0.4.7/whylabs_client/model/provision_new_aws_marketplace_user_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/provision_new_marketplace_user_request.py` & `whylabs-client-0.4.7/whylabs_client/model/provision_new_marketplace_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/provision_new_user_request.py` & `whylabs-client-0.4.7/whylabs_client/model/provision_new_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/provision_new_user_response.py` & `whylabs-client-0.4.7/whylabs_client/model/provision_new_user_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/reference_profile_item_response.py` & `whylabs-client-0.4.7/whylabs_client/model/reference_profile_item_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,30 +84,30 @@
         return {
             'org_id': (str,),  # noqa: E501
             'model_id': (str,),  # noqa: E501
             'alias': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'upload_timestamp': (int,),  # noqa: E501
             'dataset_timestamp': (int, none_type,),  # noqa: E501
-            'path': (str,),  # noqa: E501
+            'download_url': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'org_id': 'orgId',  # noqa: E501
         'model_id': 'modelId',  # noqa: E501
         'alias': 'alias',  # noqa: E501
         'id': 'id',  # noqa: E501
         'upload_timestamp': 'uploadTimestamp',  # noqa: E501
         'dataset_timestamp': 'datasetTimestamp',  # noqa: E501
-        'path': 'path',  # noqa: E501
+        'download_url': 'downloadUrl',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -149,15 +149,15 @@
                                 _visited_composed_classes = (Animal,)
             org_id (str): [optional]  # noqa: E501
             model_id (str): [optional]  # noqa: E501
             alias (str): [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
             upload_timestamp (int): [optional]  # noqa: E501
             dataset_timestamp (int, none_type): [optional]  # noqa: E501
-            path (str): [optional]  # noqa: E501
+            download_url (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -237,15 +237,15 @@
                                 _visited_composed_classes = (Animal,)
             org_id (str): [optional]  # noqa: E501
             model_id (str): [optional]  # noqa: E501
             alias (str): [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
             upload_timestamp (int): [optional]  # noqa: E501
             dataset_timestamp (int, none_type): [optional]  # noqa: E501
-            path (str): [optional]  # noqa: E501
+            download_url (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `whylabs-client-0.4.6/whylabs_client/model/refresh_access_token_request.py` & `whylabs-client-0.4.7/whylabs_client/model/refresh_access_token_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/refresh_connection_by_org_id_response.py` & `whylabs-client-0.4.7/whylabs_client/model/refresh_connection_by_org_id_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/refresh_connection_request.py` & `whylabs-client-0.4.7/whylabs_client/model/refresh_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/register_databricks_connection_request.py` & `whylabs-client-0.4.7/whylabs_client/model/register_databricks_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/register_databricks_connection_response.py` & `whylabs-client-0.4.7/whylabs_client/model/register_databricks_connection_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/remove_membership_request.py` & `whylabs-client-0.4.7/whylabs_client/model/remove_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/request_feature_monitor_config.py` & `whylabs-client-0.4.7/whylabs_client/model/request_feature_monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/request_monitor_config.py` & `whylabs-client-0.4.7/whylabs_client/model/request_monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/response.py` & `whylabs-client-0.4.7/whylabs_client/model/response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/role.py` & `whylabs-client-0.4.7/whylabs_client/model/role.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/run_job_request.py` & `whylabs-client-0.4.7/whylabs_client/model/search_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from whylabs_client.model.entity_search_result import EntitySearchResult
+    globals()['EntitySearchResult'] = EntitySearchResult
 
-class RunJobRequest(ModelNormal):
+
+class SearchResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,57 +67,54 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'job_id': (int,),  # noqa: E501
-            'org_id': (str, none_type,),  # noqa: E501
-            'workspace_id': (str, none_type,),  # noqa: E501
+            'request_id': (str, none_type,),  # noqa: E501
+            'results': ([EntitySearchResult],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'job_id': 'jobId',  # noqa: E501
-        'org_id': 'orgId',  # noqa: E501
-        'workspace_id': 'workspaceId',  # noqa: E501
+        'request_id': 'requestId',  # noqa: E501
+        'results': 'results',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, job_id, *args, **kwargs):  # noqa: E501
-        """RunJobRequest - a model defined in OpenAPI
-
-        Args:
-            job_id (int): The id of the job to run in the connected Databricks workspace.
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """SearchResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,16 +139,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            org_id (str, none_type): Look up a connection by the org that is connected to.. [optional]  # noqa: E501
-            workspace_id (str, none_type): Look up a connection by the workspace that it originates from.. [optional]  # noqa: E501
+            request_id (str, none_type): [optional]  # noqa: E501
+            results ([EntitySearchResult]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -167,15 +168,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.job_id = job_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -188,19 +188,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, job_id, *args, **kwargs):  # noqa: E501
-        """RunJobRequest - a model defined in OpenAPI
-
-        Args:
-            job_id (int): The id of the job to run in the connected Databricks workspace.
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """SearchResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -225,16 +222,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            org_id (str, none_type): Look up a connection by the org that is connected to.. [optional]  # noqa: E501
-            workspace_id (str, none_type): Look up a connection by the workspace that it originates from.. [optional]  # noqa: E501
+            request_id (str, none_type): [optional]  # noqa: E501
+            results ([EntitySearchResult]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -252,15 +249,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.job_id = job_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.4.6/whylabs_client/model/run_job_response.py` & `whylabs-client-0.4.7/whylabs_client/model/run_job_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/schema_metadata.py` & `whylabs-client-0.4.7/whylabs_client/model/schema_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/seasonal_arima_request_config.py` & `whylabs-client-0.4.7/whylabs_client/model/seasonal_arima_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/segment.py` & `whylabs-client-0.4.7/whylabs_client/model/segment.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/segment_tag.py` & `whylabs-client-0.4.7/whylabs_client/model/segment_tag.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/segment_weight.py` & `whylabs-client-0.4.7/whylabs_client/model/update_connection_changes.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from whylabs_client.model.segment import Segment
-    globals()['Segment'] = Segment
 
-
-class SegmentWeight(ModelNormal):
+class UpdateConnectionChanges(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,54 +63,54 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'segment': (Segment,),  # noqa: E501
-            'weights': ({str: (float,)},),  # noqa: E501
+            'org_id': (str, none_type,),  # noqa: E501
+            'connected': (bool, none_type,),  # noqa: E501
+            'demo': (bool, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'segment': 'segment',  # noqa: E501
-        'weights': 'weights',  # noqa: E501
+        'org_id': 'orgId',  # noqa: E501
+        'connected': 'connected',  # noqa: E501
+        'demo': 'demo',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SegmentWeight - a model defined in OpenAPI
+        """UpdateConnectionChanges - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,16 +135,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            segment (Segment): [optional]  # noqa: E501
-            weights ({str: (float,)}): Entity weight value for each entity. [optional]  # noqa: E501
+            org_id (str, none_type): [optional]  # noqa: E501
+            connected (bool, none_type): [optional]  # noqa: E501
+            demo (bool, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -189,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SegmentWeight - a model defined in OpenAPI
+        """UpdateConnectionChanges - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -222,16 +219,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            segment (Segment): [optional]  # noqa: E501
-            weights ({str: (float,)}): Entity weight value for each entity. [optional]  # noqa: E501
+            org_id (str, none_type): [optional]  # noqa: E501
+            connected (bool, none_type): [optional]  # noqa: E501
+            demo (bool, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `whylabs-client-0.4.6/whylabs_client/model/session_metadata.py` & `whylabs-client-0.4.7/whylabs_client/model/session_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/set_default_membership_request.py` & `whylabs-client-0.4.7/whylabs_client/model/set_default_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/slack_notification_action.py` & `whylabs-client-0.4.7/whylabs_client/model/slack_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/subscription_tier.py` & `whylabs-client-0.4.7/whylabs_client/model/subscription_tier.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/time_period.py` & `whylabs-client-0.4.7/whylabs_client/model/time_period.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/uber_notification_schedule.py` & `whylabs-client-0.4.7/whylabs_client/model/uber_notification_schedule.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/unique_values_monitor_request_config.py` & `whylabs-client-0.4.7/whylabs_client/model/unique_values_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/update_connection_changes.py` & `whylabs-client-0.4.7/whylabs_client/model/dto_jobs_spark_jar_task_dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class UpdateConnectionChanges(ModelNormal):
+class DTOJobsSparkJarTaskDTO(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,39 +78,39 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'org_id': (str, none_type,),  # noqa: E501
-            'connected': (bool, none_type,),  # noqa: E501
-            'demo': (bool, none_type,),  # noqa: E501
+            'jar_uri': (str,),  # noqa: E501
+            'main_class_name': (str,),  # noqa: E501
+            'parameters': ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'org_id': 'orgId',  # noqa: E501
-        'connected': 'connected',  # noqa: E501
-        'demo': 'demo',  # noqa: E501
+        'jar_uri': 'jarUri',  # noqa: E501
+        'main_class_name': 'mainClassName',  # noqa: E501
+        'parameters': 'parameters',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UpdateConnectionChanges - a model defined in OpenAPI
+        """DTOJobsSparkJarTaskDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,17 +135,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            org_id (str, none_type): [optional]  # noqa: E501
-            connected (bool, none_type): [optional]  # noqa: E501
-            demo (bool, none_type): [optional]  # noqa: E501
+            jar_uri (str): [optional]  # noqa: E501
+            main_class_name (str): [optional]  # noqa: E501
+            parameters ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """UpdateConnectionChanges - a model defined in OpenAPI
+        """DTOJobsSparkJarTaskDTO - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,17 +219,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            org_id (str, none_type): [optional]  # noqa: E501
-            connected (bool, none_type): [optional]  # noqa: E501
-            demo (bool, none_type): [optional]  # noqa: E501
+            jar_uri (str): [optional]  # noqa: E501
+            main_class_name (str): [optional]  # noqa: E501
+            parameters ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `whylabs-client-0.4.6/whylabs_client/model/update_connection_request.py` & `whylabs-client-0.4.7/whylabs_client/model/update_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/update_membership_request.py` & `whylabs-client-0.4.7/whylabs_client/model/update_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/user.py` & `whylabs-client-0.4.7/whylabs_client/model/user.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/user_api_key.py` & `whylabs-client-0.4.7/whylabs_client/model/user_api_key.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/user_api_key_response.py` & `whylabs-client-0.4.7/whylabs_client/model/user_api_key_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model/why_logs_metric.py` & `whylabs-client-0.4.7/whylabs_client/model/why_logs_metric.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/model_utils.py` & `whylabs-client-0.4.7/whylabs_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client/models/__init__.py` & `whylabs-client-0.4.7/whylabs_client/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,38 +15,40 @@
 from whylabs_client.model.async_log_response import AsyncLogResponse
 from whylabs_client.model.batch_log_reference_request import BatchLogReferenceRequest
 from whylabs_client.model.batch_log_session_reference_response import BatchLogSessionReferenceResponse
 from whylabs_client.model.column_schema import ColumnSchema
 from whylabs_client.model.create_session_request import CreateSessionRequest
 from whylabs_client.model.create_session_response import CreateSessionResponse
 from whylabs_client.model.create_user_request import CreateUserRequest
-from whylabs_client.model.dto_auto_scale_dto import DTOAutoScaleDTO
-from whylabs_client.model.dto_aws_attributes_dto import DTOAwsAttributesDTO
-from whylabs_client.model.dto_aws_availability_dto import DTOAwsAvailabilityDTO
-from whylabs_client.model.dto_cluster_log_conf_dto import DTOClusterLogConfDTO
-from whylabs_client.model.dto_cron_schedule_dto import DTOCronScheduleDTO
-from whylabs_client.model.dto_dbfs_storage_info_dto import DTODbfsStorageInfoDTO
+from whylabs_client.model.dto_clusters_auto_scale_dto import DTOClustersAutoScaleDTO
+from whylabs_client.model.dto_clusters_aws_attributes_dto import DTOClustersAwsAttributesDTO
+from whylabs_client.model.dto_clusters_aws_availability_dto import DTOClustersAwsAvailabilityDTO
+from whylabs_client.model.dto_clusters_cluster_log_conf_dto import DTOClustersClusterLogConfDTO
+from whylabs_client.model.dto_clusters_dbfs_storage_info_dto import DTOClustersDbfsStorageInfoDTO
+from whylabs_client.model.dto_clusters_s3_storage_info_dto import DTOClustersS3StorageInfoDTO
 from whylabs_client.model.dto_ebs_volume_type_dto import DTOEbsVolumeTypeDTO
-from whylabs_client.model.dto_job_dto import DTOJobDTO
-from whylabs_client.model.dto_job_email_notifications_dto import DTOJobEmailNotificationsDTO
-from whylabs_client.model.dto_job_settings_dto import DTOJobSettingsDTO
-from whylabs_client.model.dto_new_cluster_dto import DTONewClusterDTO
-from whylabs_client.model.dto_notebook_task_dto import DTONotebookTaskDTO
-from whylabs_client.model.dtos3_storage_info_dto import DTOS3StorageInfoDTO
-from whylabs_client.model.dto_spark_jar_task_dto import DTOSparkJarTaskDTO
-from whylabs_client.model.dto_spark_python_task_dto import DTOSparkPythonTaskDTO
-from whylabs_client.model.dto_spark_submit_task_dto import DTOSparkSubmitTaskDTO
+from whylabs_client.model.dto_jobs_cron_schedule_dto import DTOJobsCronScheduleDTO
+from whylabs_client.model.dto_jobs_data_security_mode_dto import DTOJobsDataSecurityModeDTO
+from whylabs_client.model.dto_jobs_job_dto import DTOJobsJobDTO
+from whylabs_client.model.dto_jobs_job_email_notifications_dto import DTOJobsJobEmailNotificationsDTO
+from whylabs_client.model.dto_jobs_job_settings_dto import DTOJobsJobSettingsDTO
+from whylabs_client.model.dto_jobs_new_cluster_dto import DTOJobsNewClusterDTO
+from whylabs_client.model.dto_jobs_notebook_task_dto import DTOJobsNotebookTaskDTO
+from whylabs_client.model.dto_jobs_spark_jar_task_dto import DTOJobsSparkJarTaskDTO
+from whylabs_client.model.dto_jobs_spark_python_task_dto import DTOJobsSparkPythonTaskDTO
+from whylabs_client.model.dto_jobs_spark_submit_task_dto import DTOJobsSparkSubmitTaskDTO
 from whylabs_client.model.databricks_connection import DatabricksConnection
 from whylabs_client.model.dataset_request_monitor_config import DatasetRequestMonitorConfig
 from whylabs_client.model.datatype_monitor_request_config import DatatypeMonitorRequestConfig
 from whylabs_client.model.delete_analyzer_results_response import DeleteAnalyzerResultsResponse
 from whylabs_client.model.delete_dataset_profiles_response import DeleteDatasetProfilesResponse
 from whylabs_client.model.distribution_monitor_request_config import DistributionMonitorRequestConfig
 from whylabs_client.model.email_notification_action import EmailNotificationAction
 from whylabs_client.model.entity_schema import EntitySchema
+from whylabs_client.model.entity_search_result import EntitySearchResult
 from whylabs_client.model.entity_weight_record import EntityWeightRecord
 from whylabs_client.model.entity_weight_record_metadata import EntityWeightRecordMetadata
 from whylabs_client.model.feature_flags import FeatureFlags
 from whylabs_client.model.get_connection_request import GetConnectionRequest
 from whylabs_client.model.get_connection_response import GetConnectionResponse
 from whylabs_client.model.get_dataset_metadata_response import GetDatasetMetadataResponse
 from whylabs_client.model.get_default_membership_response import GetDefaultMembershipResponse
@@ -102,14 +104,15 @@
 from whylabs_client.model.request_feature_monitor_config import RequestFeatureMonitorConfig
 from whylabs_client.model.request_monitor_config import RequestMonitorConfig
 from whylabs_client.model.response import Response
 from whylabs_client.model.role import Role
 from whylabs_client.model.run_job_request import RunJobRequest
 from whylabs_client.model.run_job_response import RunJobResponse
 from whylabs_client.model.schema_metadata import SchemaMetadata
+from whylabs_client.model.search_response import SearchResponse
 from whylabs_client.model.seasonal_arima_request_config import SeasonalARIMARequestConfig
 from whylabs_client.model.segment import Segment
 from whylabs_client.model.segment_tag import SegmentTag
 from whylabs_client.model.segment_weight import SegmentWeight
 from whylabs_client.model.session_metadata import SessionMetadata
 from whylabs_client.model.set_default_membership_request import SetDefaultMembershipRequest
 from whylabs_client.model.slack_notification_action import SlackNotificationAction
```

### Comparing `whylabs-client-0.4.6/whylabs_client/rest.py` & `whylabs-client-0.4.7/whylabs_client/rest.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.4.6/whylabs_client.egg-info/PKG-INFO` & `whylabs-client-0.4.7/whylabs_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylabs-client
-Version: 0.4.6
+Version: 0.4.7
 Summary: WhyLabs API client
 Home-page: UNKNOWN
 Author: WhyLabs
 Author-email: support@whylabs.ai
 License: Apache License 2.0
 Keywords: OpenAPI,OpenAPI-Generator,WhyLabs API client
 Platform: UNKNOWN
```

### Comparing `whylabs-client-0.4.6/whylabs_client.egg-info/SOURCES.txt` & `whylabs-client-0.4.7/whylabs_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,32 +37,34 @@
 whylabs_client/model/create_user_request.py
 whylabs_client/model/databricks_connection.py
 whylabs_client/model/dataset_request_monitor_config.py
 whylabs_client/model/datatype_monitor_request_config.py
 whylabs_client/model/delete_analyzer_results_response.py
 whylabs_client/model/delete_dataset_profiles_response.py
 whylabs_client/model/distribution_monitor_request_config.py
-whylabs_client/model/dto_auto_scale_dto.py
-whylabs_client/model/dto_aws_attributes_dto.py
-whylabs_client/model/dto_aws_availability_dto.py
-whylabs_client/model/dto_cluster_log_conf_dto.py
-whylabs_client/model/dto_cron_schedule_dto.py
-whylabs_client/model/dto_dbfs_storage_info_dto.py
+whylabs_client/model/dto_clusters_auto_scale_dto.py
+whylabs_client/model/dto_clusters_aws_attributes_dto.py
+whylabs_client/model/dto_clusters_aws_availability_dto.py
+whylabs_client/model/dto_clusters_cluster_log_conf_dto.py
+whylabs_client/model/dto_clusters_dbfs_storage_info_dto.py
+whylabs_client/model/dto_clusters_s3_storage_info_dto.py
 whylabs_client/model/dto_ebs_volume_type_dto.py
-whylabs_client/model/dto_job_dto.py
-whylabs_client/model/dto_job_email_notifications_dto.py
-whylabs_client/model/dto_job_settings_dto.py
-whylabs_client/model/dto_new_cluster_dto.py
-whylabs_client/model/dto_notebook_task_dto.py
-whylabs_client/model/dto_spark_jar_task_dto.py
-whylabs_client/model/dto_spark_python_task_dto.py
-whylabs_client/model/dto_spark_submit_task_dto.py
-whylabs_client/model/dtos3_storage_info_dto.py
+whylabs_client/model/dto_jobs_cron_schedule_dto.py
+whylabs_client/model/dto_jobs_data_security_mode_dto.py
+whylabs_client/model/dto_jobs_job_dto.py
+whylabs_client/model/dto_jobs_job_email_notifications_dto.py
+whylabs_client/model/dto_jobs_job_settings_dto.py
+whylabs_client/model/dto_jobs_new_cluster_dto.py
+whylabs_client/model/dto_jobs_notebook_task_dto.py
+whylabs_client/model/dto_jobs_spark_jar_task_dto.py
+whylabs_client/model/dto_jobs_spark_python_task_dto.py
+whylabs_client/model/dto_jobs_spark_submit_task_dto.py
 whylabs_client/model/email_notification_action.py
 whylabs_client/model/entity_schema.py
+whylabs_client/model/entity_search_result.py
 whylabs_client/model/entity_weight_record.py
 whylabs_client/model/entity_weight_record_metadata.py
 whylabs_client/model/feature_flags.py
 whylabs_client/model/get_connection_request.py
 whylabs_client/model/get_connection_response.py
 whylabs_client/model/get_dataset_metadata_response.py
 whylabs_client/model/get_default_membership_response.py
@@ -118,14 +120,15 @@
 whylabs_client/model/request_feature_monitor_config.py
 whylabs_client/model/request_monitor_config.py
 whylabs_client/model/response.py
 whylabs_client/model/role.py
 whylabs_client/model/run_job_request.py
 whylabs_client/model/run_job_response.py
 whylabs_client/model/schema_metadata.py
+whylabs_client/model/search_response.py
 whylabs_client/model/seasonal_arima_request_config.py
 whylabs_client/model/segment.py
 whylabs_client/model/segment_tag.py
 whylabs_client/model/segment_weight.py
 whylabs_client/model/session_metadata.py
 whylabs_client/model/set_default_membership_request.py
 whylabs_client/model/slack_notification_action.py
```

