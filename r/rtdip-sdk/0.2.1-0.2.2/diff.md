# Comparing `tmp/rtdip_sdk-0.2.1-py3-none-any.whl.zip` & `tmp/rtdip_sdk-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,81 +1,86 @@
-Zip file size: 92459 bytes, number of entries: 79
--rw-r--r--  2.0 unx      571 b- defN 23-Apr-21 15:32 rtdip_sdk/__init__.py
--rw-r--r--  2.0 unx      571 b- defN 23-Apr-21 15:32 rtdip_sdk/authentication/__init__.py
--rw-r--r--  2.0 unx     7210 b- defN 23-Apr-21 15:32 rtdip_sdk/authentication/authenticate.py
--rw-r--r--  2.0 unx      571 b- defN 23-Apr-21 15:32 rtdip_sdk/functions/__init__.py
--rw-r--r--  2.0 unx     8746 b- defN 23-Apr-21 15:32 rtdip_sdk/functions/_query_builder.py
--rw-r--r--  2.0 unx     2908 b- defN 23-Apr-21 15:32 rtdip_sdk/functions/interpolate.py
--rw-r--r--  2.0 unx     2293 b- defN 23-Apr-21 15:32 rtdip_sdk/functions/metadata.py
--rw-r--r--  2.0 unx     2786 b- defN 23-Apr-21 15:32 rtdip_sdk/functions/raw.py
--rw-r--r--  2.0 unx     3052 b- defN 23-Apr-21 15:32 rtdip_sdk/functions/resample.py
--rw-r--r--  2.0 unx     8921 b- defN 23-Apr-21 15:32 rtdip_sdk/functions/time_weighted_average.py
--rw-r--r--  2.0 unx      571 b- defN 23-Apr-21 15:32 rtdip_sdk/odbc/__init__.py
--rw-r--r--  2.0 unx      934 b- defN 23-Apr-21 15:32 rtdip_sdk/odbc/connection_interface.py
--rw-r--r--  2.0 unx      952 b- defN 23-Apr-21 15:32 rtdip_sdk/odbc/cursor_interface.py
--rw-r--r--  2.0 unx     3498 b- defN 23-Apr-21 15:32 rtdip_sdk/odbc/db_sql_connector.py
--rw-r--r--  2.0 unx     4228 b- defN 23-Apr-21 15:32 rtdip_sdk/odbc/pyodbc_sql_connector.py
--rw-r--r--  2.0 unx     4432 b- defN 23-Apr-21 15:32 rtdip_sdk/odbc/turbodbc_sql_connector.py
--rw-r--r--  2.0 unx      569 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/__init__.py
--rw-r--r--  2.0 unx     1035 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/interfaces.py
--rw-r--r--  2.0 unx      569 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/_pipeline_utils/__init__.py
--rw-r--r--  2.0 unx     1485 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/_pipeline_utils/constants.py
--rw-r--r--  2.0 unx     2434 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/_pipeline_utils/models.py
--rw-r--r--  2.0 unx     5327 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/_pipeline_utils/spark.py
--rw-r--r--  2.0 unx      603 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/converters/__init__.py
--rw-r--r--  2.0 unx      697 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/converters/interfaces.py
--rw-r--r--  2.0 unx     3424 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/converters/pipeline_job_json.py
--rw-r--r--  2.0 unx      630 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/__init__.py
--rw-r--r--  2.0 unx    13189 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/databricks.py
--rw-r--r--  2.0 unx      751 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/interfaces.py
--rw-r--r--  2.0 unx      571 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/dbx/__init__.py
--rw-r--r--  2.0 unx     1114 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/dbx/setup.py
--rw-r--r--  2.0 unx      571 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/dbx/conf/__init__.py
--rw-r--r--  2.0 unx      571 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/dbx/rtdip/__init__.py
--rw-r--r--  2.0 unx      571 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/__init__.py
--rw-r--r--  2.0 unx     3310 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/common.py
--rw-r--r--  2.0 unx     1686 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/pipeline_task.py
--rw-r--r--  2.0 unx      571 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/models/__init__.py
--rw-r--r--  2.0 unx     7897 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/deploy/models/databricks.py
--rw-r--r--  2.0 unx      684 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/destinations/__init__.py
--rw-r--r--  2.0 unx      427 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/destinations/interfaces.py
--rw-r--r--  2.0 unx      569 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/destinations/spark/__init__.py
--rw-r--r--  2.0 unx     5112 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/destinations/spark/delta.py
--rw-r--r--  2.0 unx     4781 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/destinations/spark/eventhub.py
--rw-r--r--  2.0 unx     3903 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/destinations/spark/kafka.py
--rw-r--r--  2.0 unx     3659 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/destinations/spark/kinesis.py
--rw-r--r--  2.0 unx      611 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/execute/__init__.py
--rw-r--r--  2.0 unx     1448 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/execute/container.py
--rw-r--r--  2.0 unx     8378 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/execute/job.py
--rw-r--r--  2.0 unx     3037 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/execute/models.py
--rw-r--r--  2.0 unx      618 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/secrets/__init__.py
--rw-r--r--  2.0 unx     2227 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/secrets/databricks.py
--rw-r--r--  2.0 unx      824 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/secrets/interfaces.py
--rw-r--r--  2.0 unx      887 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/secrets/models.py
--rw-r--r--  2.0 unx      779 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/sources/__init__.py
--rw-r--r--  2.0 unx      993 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/sources/interfaces.py
--rw-r--r--  2.0 unx      569 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/sources/spark/__init__.py
--rw-r--r--  2.0 unx     3420 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/sources/spark/autoloader.py
--rw-r--r--  2.0 unx     4501 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/sources/spark/delta.py
--rw-r--r--  2.0 unx     4473 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/sources/spark/delta_sharing.py
--rw-r--r--  2.0 unx     5259 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/sources/spark/eventhub.py
--rw-r--r--  2.0 unx     5240 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/sources/spark/iot_hub.py
--rw-r--r--  2.0 unx     8114 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/sources/spark/kafka.py
--rw-r--r--  2.0 unx     3793 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/sources/spark/kinesis.py
--rw-r--r--  2.0 unx      692 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/transformers/__init__.py
--rw-r--r--  2.0 unx      946 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/transformers/interfaces.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/transformers/spark/__init__.py
--rw-r--r--  2.0 unx     1715 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/transformers/spark/eventhub.py
--rw-r--r--  2.0 unx     2900 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/transformers/spark/json_to_opcua.py
--rw-r--r--  2.0 unx     3560 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/transformers/spark/opcua_to_process_control_data_model.py
--rw-r--r--  2.0 unx      692 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/utilities/__init__.py
--rw-r--r--  2.0 unx      773 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/utilities/interfaces.py
--rw-r--r--  2.0 unx      569 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/utilities/spark/__init__.py
--rw-r--r--  2.0 unx     3857 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/utilities/spark/delta_table_create.py
--rw-r--r--  2.0 unx     3119 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/utilities/spark/delta_table_optimize.py
--rw-r--r--  2.0 unx     2602 b- defN 23-Apr-21 15:32 rtdip_sdk/pipelines/utilities/spark/delta_table_vacuum.py
--rw-r--r--  2.0 unx    10172 b- defN 23-Apr-21 15:32 rtdip_sdk-0.2.1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2709 b- defN 23-Apr-21 15:32 rtdip_sdk-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 15:32 rtdip_sdk-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-21 15:32 rtdip_sdk-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     7767 b- defN 23-Apr-21 15:32 rtdip_sdk-0.2.1.dist-info/RECORD
-79 files, 216300 bytes uncompressed, 79723 bytes compressed:  63.1%
+Zip file size: 99272 bytes, number of entries: 84
+-rw-r--r--  2.0 unx      571 b- defN 23-Apr-28 08:50 rtdip_sdk/__init__.py
+-rw-r--r--  2.0 unx      571 b- defN 23-Apr-28 08:50 rtdip_sdk/authentication/__init__.py
+-rw-r--r--  2.0 unx     7210 b- defN 23-Apr-28 08:50 rtdip_sdk/authentication/authenticate.py
+-rw-r--r--  2.0 unx      571 b- defN 23-Apr-28 08:50 rtdip_sdk/functions/__init__.py
+-rw-r--r--  2.0 unx     9846 b- defN 23-Apr-28 08:50 rtdip_sdk/functions/_query_builder.py
+-rw-r--r--  2.0 unx     2908 b- defN 23-Apr-28 08:50 rtdip_sdk/functions/interpolate.py
+-rw-r--r--  2.0 unx     2293 b- defN 23-Apr-28 08:50 rtdip_sdk/functions/metadata.py
+-rw-r--r--  2.0 unx     2626 b- defN 23-Apr-28 08:50 rtdip_sdk/functions/raw.py
+-rw-r--r--  2.0 unx     3052 b- defN 23-Apr-28 08:50 rtdip_sdk/functions/resample.py
+-rw-r--r--  2.0 unx     9434 b- defN 23-Apr-28 08:50 rtdip_sdk/functions/time_weighted_average.py
+-rw-r--r--  2.0 unx      571 b- defN 23-Apr-28 08:50 rtdip_sdk/odbc/__init__.py
+-rw-r--r--  2.0 unx      934 b- defN 23-Apr-28 08:50 rtdip_sdk/odbc/connection_interface.py
+-rw-r--r--  2.0 unx      952 b- defN 23-Apr-28 08:50 rtdip_sdk/odbc/cursor_interface.py
+-rw-r--r--  2.0 unx     3498 b- defN 23-Apr-28 08:50 rtdip_sdk/odbc/db_sql_connector.py
+-rw-r--r--  2.0 unx     4228 b- defN 23-Apr-28 08:50 rtdip_sdk/odbc/pyodbc_sql_connector.py
+-rw-r--r--  2.0 unx     4432 b- defN 23-Apr-28 08:50 rtdip_sdk/odbc/turbodbc_sql_connector.py
+-rw-r--r--  2.0 unx      569 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/__init__.py
+-rw-r--r--  2.0 unx     1035 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/interfaces.py
+-rw-r--r--  2.0 unx      569 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/_pipeline_utils/__init__.py
+-rw-r--r--  2.0 unx     1745 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/_pipeline_utils/constants.py
+-rw-r--r--  2.0 unx     2434 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/_pipeline_utils/models.py
+-rw-r--r--  2.0 unx     5327 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/_pipeline_utils/spark.py
+-rw-r--r--  2.0 unx      603 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/converters/__init__.py
+-rw-r--r--  2.0 unx      697 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/converters/interfaces.py
+-rw-r--r--  2.0 unx     3442 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/converters/pipeline_job_json.py
+-rw-r--r--  2.0 unx      630 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/__init__.py
+-rw-r--r--  2.0 unx    13207 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/databricks.py
+-rw-r--r--  2.0 unx      751 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/interfaces.py
+-rw-r--r--  2.0 unx      571 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/dbx/__init__.py
+-rw-r--r--  2.0 unx     1114 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/dbx/setup.py
+-rw-r--r--  2.0 unx      571 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/dbx/conf/__init__.py
+-rw-r--r--  2.0 unx      571 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/dbx/rtdip/__init__.py
+-rw-r--r--  2.0 unx      571 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/__init__.py
+-rw-r--r--  2.0 unx     3310 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/common.py
+-rw-r--r--  2.0 unx     1695 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/pipeline_task.py
+-rw-r--r--  2.0 unx      571 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/models/__init__.py
+-rw-r--r--  2.0 unx     7897 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/deploy/models/databricks.py
+-rw-r--r--  2.0 unx      684 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/destinations/__init__.py
+-rw-r--r--  2.0 unx      427 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/destinations/interfaces.py
+-rw-r--r--  2.0 unx      569 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/destinations/spark/__init__.py
+-rw-r--r--  2.0 unx     5112 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/destinations/spark/delta.py
+-rw-r--r--  2.0 unx     4781 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/destinations/spark/eventhub.py
+-rw-r--r--  2.0 unx     3903 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/destinations/spark/kafka.py
+-rw-r--r--  2.0 unx     3659 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/destinations/spark/kinesis.py
+-rw-r--r--  2.0 unx      611 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/execute/__init__.py
+-rw-r--r--  2.0 unx     1448 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/execute/container.py
+-rw-r--r--  2.0 unx     8378 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/execute/job.py
+-rw-r--r--  2.0 unx     3037 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/execute/models.py
+-rw-r--r--  2.0 unx      618 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/secrets/__init__.py
+-rw-r--r--  2.0 unx     2227 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/secrets/databricks.py
+-rw-r--r--  2.0 unx      824 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/secrets/interfaces.py
+-rw-r--r--  2.0 unx      887 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/secrets/models.py
+-rw-r--r--  2.0 unx      779 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/sources/__init__.py
+-rw-r--r--  2.0 unx      993 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/sources/interfaces.py
+-rw-r--r--  2.0 unx      569 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/sources/spark/__init__.py
+-rw-r--r--  2.0 unx     3420 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/sources/spark/autoloader.py
+-rw-r--r--  2.0 unx     4501 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/sources/spark/delta.py
+-rw-r--r--  2.0 unx     4473 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/sources/spark/delta_sharing.py
+-rw-r--r--  2.0 unx     5259 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/sources/spark/eventhub.py
+-rw-r--r--  2.0 unx     5240 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/sources/spark/iot_hub.py
+-rw-r--r--  2.0 unx     8114 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/sources/spark/kafka.py
+-rw-r--r--  2.0 unx     3793 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/sources/spark/kinesis.py
+-rw-r--r--  2.0 unx      714 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/transformers/__init__.py
+-rw-r--r--  2.0 unx      946 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/transformers/interfaces.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/transformers/spark/__init__.py
+-rw-r--r--  2.0 unx     2143 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/transformers/spark/binary_to_string.py
+-rw-r--r--  2.0 unx     2953 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/transformers/spark/opc_publisher_json_to_opcua.py
+-rw-r--r--  2.0 unx     3571 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/transformers/spark/opcua_to_process_control_data_model.py
+-rw-r--r--  2.0 unx      727 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/utilities/__init__.py
+-rw-r--r--  2.0 unx      773 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/utilities/interfaces.py
+-rw-r--r--  2.0 unx      569 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/utilities/aws/__init__.py
+-rw-r--r--  2.0 unx     4674 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/utilities/aws/s3_bucket_policy.py
+-rw-r--r--  2.0 unx      569 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/utilities/azure/__init__.py
+-rw-r--r--  2.0 unx     6556 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/utilities/azure/adls_gen2_acl.py
+-rw-r--r--  2.0 unx      569 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/utilities/spark/__init__.py
+-rw-r--r--  2.0 unx     2185 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/utilities/spark/configuration.py
+-rw-r--r--  2.0 unx     3857 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/utilities/spark/delta_table_create.py
+-rw-r--r--  2.0 unx     3119 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/utilities/spark/delta_table_optimize.py
+-rw-r--r--  2.0 unx     2602 b- defN 23-Apr-28 08:50 rtdip_sdk/pipelines/utilities/spark/delta_table_vacuum.py
+-rw-r--r--  2.0 unx    10172 b- defN 23-Apr-28 08:50 rtdip_sdk-0.2.2.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2844 b- defN 23-Apr-28 08:50 rtdip_sdk-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 08:50 rtdip_sdk-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-28 08:50 rtdip_sdk-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     8321 b- defN 23-Apr-28 08:50 rtdip_sdk-0.2.2.dist-info/RECORD
+84 files, 233849 bytes uncompressed, 85614 bytes compressed:  63.4%
```

## zipnote {}

```diff
@@ -189,50 +189,65 @@
 
 Filename: rtdip_sdk/pipelines/transformers/interfaces.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/transformers/spark/__init__.py
 Comment: 
 
-Filename: rtdip_sdk/pipelines/transformers/spark/eventhub.py
+Filename: rtdip_sdk/pipelines/transformers/spark/binary_to_string.py
 Comment: 
 
-Filename: rtdip_sdk/pipelines/transformers/spark/json_to_opcua.py
+Filename: rtdip_sdk/pipelines/transformers/spark/opc_publisher_json_to_opcua.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/transformers/spark/opcua_to_process_control_data_model.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/utilities/__init__.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/utilities/interfaces.py
 Comment: 
 
+Filename: rtdip_sdk/pipelines/utilities/aws/__init__.py
+Comment: 
+
+Filename: rtdip_sdk/pipelines/utilities/aws/s3_bucket_policy.py
+Comment: 
+
+Filename: rtdip_sdk/pipelines/utilities/azure/__init__.py
+Comment: 
+
+Filename: rtdip_sdk/pipelines/utilities/azure/adls_gen2_acl.py
+Comment: 
+
 Filename: rtdip_sdk/pipelines/utilities/spark/__init__.py
 Comment: 
 
+Filename: rtdip_sdk/pipelines/utilities/spark/configuration.py
+Comment: 
+
 Filename: rtdip_sdk/pipelines/utilities/spark/delta_table_create.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/utilities/spark/delta_table_optimize.py
 Comment: 
 
 Filename: rtdip_sdk/pipelines/utilities/spark/delta_table_vacuum.py
 Comment: 
 
-Filename: rtdip_sdk-0.2.1.dist-info/LICENSE.md
+Filename: rtdip_sdk-0.2.2.dist-info/LICENSE.md
 Comment: 
 
-Filename: rtdip_sdk-0.2.1.dist-info/METADATA
+Filename: rtdip_sdk-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: rtdip_sdk-0.2.1.dist-info/WHEEL
+Filename: rtdip_sdk-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: rtdip_sdk-0.2.1.dist-info/top_level.txt
+Filename: rtdip_sdk-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: rtdip_sdk-0.2.1.dist-info/RECORD
+Filename: rtdip_sdk-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rtdip_sdk/functions/_query_builder.py

```diff
@@ -12,21 +12,39 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from jinjasql import JinjaSql
 from six import string_types
 from copy import deepcopy
+from datetime import datetime
 
+def _is_date_format(dt, format):
+    try:
+        return datetime.strptime(dt , format)
+    except:
+        return False
+
+def _fix_date(dt, is_end_date = False):
+    if _is_date_format(dt, "%Y-%m-%d"):
+        _time = "T23:59:59" if is_end_date == True else "T00:00:00"
+        return dt + _time + "+00:00"
+    elif _is_date_format(dt, "%Y-%m-%dT%H:%M:%S"):
+        return dt + "+00:00"
+    elif _is_date_format(dt, "%Y-%m-%dT%H:%M:%S%z"):
+        return dt
+    else: 
+        raise ValueError(f"Inputted datetime: '{dt}', is not in the correct format")
+        
 def _fix_dates(parameters_dict):
-    if len(parameters_dict['start_date']) == 10:
-        parameters_dict['start_date'] = parameters_dict['start_date']+'T00:00:00'
+        
+    parameters_dict["start_date"] = _fix_date(parameters_dict["start_date"])
+    parameters_dict["end_date"] = _fix_date(parameters_dict["end_date"], True)
 
-    if len(parameters_dict['end_date']) == 10:
-        parameters_dict['end_date'] = parameters_dict['end_date']+'T23:59:59'
+    parameters_dict["time_zone"] = datetime.strptime(parameters_dict["start_date"], "%Y-%m-%dT%H:%M:%S%z").strftime("%z")
     
     return parameters_dict
 
 def _quote_sql_string(value):
     '''
     If `value` is a string type, escapes single quotes in the string
     and returns the string enclosed in single quotes.
@@ -50,47 +68,49 @@
         params[key] = _quote_sql_string(val)
     return query % params
 
 
 def _raw_query(parameters_dict: dict) -> str:
 
     raw_query = (
-        "SELECT EventTime, TagName, Status, Value FROM "
+        "SELECT from_utc_timestamp(EventTime, \"{{ time_zone | sqlsafe }}\") as EventTime, TagName, Status, Value FROM "
         "{{ business_unit | sqlsafe }}.sensors.{{ asset | sqlsafe }}_{{ data_security_level | sqlsafe }}_events_{{ data_type | sqlsafe }} "
-        "WHERE EventDate BETWEEN to_date({{ start_date }}) AND to_date({{ end_date }}) AND EventTime BETWEEN to_timestamp({{ start_date }}) AND to_timestamp({{ end_date }}) AND TagName in {{ tag_names | inclause }} "
+        "WHERE EventDate BETWEEN to_date(to_timestamp({{ start_date }})) AND to_date(to_timestamp({{ end_date }})) AND EventTime BETWEEN to_timestamp({{ start_date }}) AND to_timestamp({{ end_date }}) AND TagName in {{ tag_names | inclause }} "
         "{% if include_bad_data is defined and include_bad_data == false %}"
         "AND Status = 'Good'"
         "{% endif %}"
+        "ORDER BY EventTime"
     )
 
     raw_parameters = {
         "business_unit": parameters_dict['business_unit'].lower(),
         "region": parameters_dict['region'].lower(),
         "asset": parameters_dict['asset'].lower(),
         "data_security_level": parameters_dict['data_security_level'].lower(),
         "data_type": parameters_dict['data_type'].lower(),
         "start_date": parameters_dict['start_date'],
         "end_date": parameters_dict['end_date'],
         "tag_names": list(dict.fromkeys(parameters_dict['tag_names'])),
-        "include_bad_data": parameters_dict['include_bad_data']  
+        "include_bad_data": parameters_dict['include_bad_data'],
+        "time_zone": parameters_dict["time_zone"]
     }
 
     sql_template = JinjaSql(param_style='pyformat')
     query, bind_params = sql_template.prepare_query(raw_query, raw_parameters)
     sql_query = _get_sql_from_template(query, bind_params)
     return sql_query
 
 def _sample_query(parameters_dict: dict) -> tuple:
 
     sample_query = (
         "SELECT DISTINCT TagName, w.start AS EventTime, {{ agg_method | sqlsafe }}(Value) OVER "
-        "(PARTITION BY TagName, w.start ORDER BY EventTime ROWS BETWEEN UNBOUNDED PRECEDING AND UNBOUNDED FOLLOWING ) AS Value FROM ("
-        "SELECT EventTime, WINDOW(EventTime, {{ sample_rate + ' ' + sample_unit }}) w, TagName, Status, Value FROM "
+        "(PARTITION BY TagName, w.start ORDER BY EventTime ROWS BETWEEN UNBOUNDED PRECEDING AND UNBOUNDED FOLLOWING ) AS Value FROM (" +
+        "SELECT from_utc_timestamp(EventTime, \"{{ time_zone | sqlsafe }}\") as EventTime, WINDOW(from_utc_timestamp(EventTime, \"{{ time_zone | sqlsafe }}\"), {{ sample_rate + ' ' + sample_unit }}) w, TagName, Status, Value FROM "
         "{{ business_unit | sqlsafe }}.sensors.{{ asset | sqlsafe }}_{{ data_security_level | sqlsafe }}_events_{{ data_type | sqlsafe }} "
-        "WHERE EventDate BETWEEN to_date({{ start_date }}) AND to_date({{ end_date }}) AND EventTime BETWEEN to_timestamp({{ start_date }}) AND to_timestamp({{ end_date }}) AND TagName in {{ tag_names | inclause }} "
+        "WHERE EventDate BETWEEN to_date(to_timestamp({{ start_date }})) AND to_date(to_timestamp({{ end_date }})) AND EventTime BETWEEN to_timestamp({{ start_date }}) AND to_timestamp({{ end_date }}) AND TagName in {{ tag_names | inclause }} "
         "{% if include_bad_data is defined and include_bad_data == false %}"
         "AND Status = 'Good'"
         "{% endif %}"
         ")"      
     )
 
     sample_parameters = {
@@ -101,15 +121,16 @@
         "data_type": parameters_dict['data_type'].lower(),
         "start_date": parameters_dict['start_date'],
         "end_date": parameters_dict['end_date'],
         "tag_names": list(dict.fromkeys(parameters_dict['tag_names'])),
         "include_bad_data": parameters_dict['include_bad_data'],
         "sample_rate": parameters_dict['sample_rate'],
         "sample_unit": parameters_dict['sample_unit'],
-        "agg_method": parameters_dict['agg_method']
+        "agg_method": parameters_dict['agg_method'],
+        "time_zone": parameters_dict["time_zone"]
     }
 
     sql_template = JinjaSql(param_style='pyformat')
     query, bind_params = sql_template.prepare_query(sample_query, sample_parameters)
     sql_query = _get_sql_from_template(query, bind_params)
     return sql_query, sample_query, sample_parameters    
 
@@ -121,15 +142,16 @@
     if parameters_dict["interpolation_method"] == "backward_fill":
         interpolation_method = 'first_value/CURRENT ROW/UNBOUNDED FOLLOWING'
 
     interpolation_options = interpolation_method.split('/')
 
     interpolate_query = (
         "SELECT a.EventTime, a.TagName, {{ interpolation_options_0 | sqlsafe }}(b.Value, true) OVER (PARTITION BY a.TagName ORDER BY a.EventTime ROWS BETWEEN {{ interpolation_options_1 | sqlsafe }} AND {{ interpolation_options_2 | sqlsafe }}) AS Value FROM "
-        "(SELECT explode(sequence(to_timestamp({{ start_date }}), to_timestamp({{ end_date }}), INTERVAL {{ sample_rate + ' ' + sample_unit }})) AS EventTime, explode(array({{ tag_name_string }})) AS TagName) a "
+        "(SELECT explode(sequence(from_utc_timestamp(to_timestamp({{ start_date }}), \"{{ time_zone | sqlsafe }}\"), from_utc_timestamp(to_timestamp({{ end_date }}), \"{{ time_zone | sqlsafe }}\"), INTERVAL {{ sample_rate + ' ' + sample_unit }})) AS EventTime, "
+        f"explode(array({tag_name_string})) AS TagName) a "
         f"LEFT OUTER JOIN ({sample_query}) b "
         "ON a.EventTime = b.EventTime "
         "AND a.TagName = b.TagName"        
     )
     
     interpolate_parameters = sample_parameters.copy()
     interpolate_parameters["interpolation_options_0"] = interpolation_options[0]
```

## rtdip_sdk/functions/raw.py

```diff
@@ -48,16 +48,14 @@
     try:
         query = _query_builder(parameters_dict)
 
         try:
             cursor = connection.cursor()
             cursor.execute(query)
             df = cursor.fetch_all()
-            if df['EventTime'][0].tzinfo is None:
-                df['EventTime'] = df['EventTime'].apply(lambda x: x.replace(tzinfo=pytz.timezone("Etc/UTC")))
             cursor.close()
             return df
         except Exception as e:
             logging.exception('error returning dataframe')
             raise e
 
     except Exception as e:
```

## rtdip_sdk/functions/time_weighted_average.py

```diff
@@ -32,53 +32,71 @@
     Attributes:
         business_unit (str): Business unit 
         region (str): Region
         asset (str): Asset 
         data_security_level (str): Level of data security 
         data_type (str): Type of the data (float, integer, double, string)
         tag_names (list): List of tagname or tagnames
-        start_date (str): Start date (Either a utc date in the format YYYY-MM-DD or a utc datetime in the format YYYY-MM-DDTHH:MM:SS)
-        end_date (str): End date (Either a utc date in the format YYYY-MM-DD or a utc datetime in the format YYYY-MM-DDTHH:MM:SS)
+        start_date (str): Start date (Either a utc date in the format YYYY-MM-DD or a utc datetime in the format YYYY-MM-DDTHH:MM:SS or specify the timezone offset in the format YYYY-MM-DDTHH:MM:SS+zz:zz)
+        end_date (str): End date (Either a utc date in the format YYYY-MM-DD or a utc datetime in the format YYYY-MM-DDTHH:MM:SS or specify the timezone offset in the format YYYY-MM-DDTHH:MM:SS+zz:z)
         window_size_mins (int): Window size in minutes
         window_length (int): (Optional) add longer window time for the start or end of specified date to cater for edge cases
         include_bad_data (bool): Include "Bad" data points with True or remove "Bad" data points with False
-        step (str): data points with step "enabled" or "disabled". The options for step are "metadata" (string), True or False (bool)
+        step (bool, str): data points with step "enabled" or "disabled". The options for step are "metadata" (string), True or False (bool)
     Returns:
         DataFrame: A dataframe containing the time weighted averages.
     '''
-    try:
-        datetime_format = "%Y-%m-%dT%H:%M:%S"
-        utc="Etc/UTC"
-        if len(parameters_dict["start_date"]) == 10:
-            original_start_date = datetime.strptime(parameters_dict["start_date"] + "T00:00:00", datetime_format)
-            parameters_dict["start_date"] = parameters_dict["start_date"] + "T00:00:00"
-        else:
-            original_start_date = datetime.strptime(parameters_dict["start_date"], datetime_format)
-        if len(parameters_dict["end_date"]) == 10:
-            original_end_date = datetime.strptime(parameters_dict["end_date"] + "T23:59:59", datetime_format) 
-            parameters_dict["end_date"] = parameters_dict["end_date"] + "T23:59:59"
-        else: 
-            original_end_date = datetime.strptime(parameters_dict["end_date"], datetime_format)
+    try:  
+        dtz_format = "%Y-%m-%dT%H:%M:%S%z"
+        utc = "Etc/UTC"
+        
+        def is_date_format(dt, format):
+            try:
+                return datetime.strptime(dt , format)
+            except:
+                return False
+            
+        def set_dtz(dt, is_end_date = False):
+            if is_date_format(dt, "%Y-%m-%d"):
+                _time = "T23:59:59" if is_end_date == True else "T00:00:00"
+                return dt + _time + "+00:00"
+            elif is_date_format(dt, "%Y-%m-%dT%H:%M:%S"):
+                return dt + "+00:00"
+            elif is_date_format(dt, "%Y-%m-%dT%H:%M:%S%z"):
+                return dt
+            else: 
+                raise ValueError(f"Inputted datetime: '{dt}', is not in the correct format")
+            
+        parameters_dict["start_date"] = set_dtz(parameters_dict["start_date"])
+        parameters_dict["end_date"] = set_dtz(parameters_dict["end_date"], True)
+
+        #used to only return data between start and end date (at the end of function)
+        original_start_date = datetime.strptime(parameters_dict["start_date"], dtz_format).replace(tzinfo=pytz.timezone(utc))
+        original_end_date = datetime.strptime(parameters_dict["end_date"], dtz_format).replace(tzinfo=pytz.timezone(utc))
+
         if "window_length" in parameters_dict:       
-            parameters_dict["start_date"] = (datetime.strptime(parameters_dict["start_date"], datetime_format) - timedelta(minutes = int(parameters_dict["window_length"]))).strftime(datetime_format)
-            parameters_dict["end_date"] = (datetime.strptime(parameters_dict["end_date"], datetime_format) + timedelta(minutes = int(parameters_dict["window_length"]))).strftime(datetime_format) 
+            parameters_dict["start_date"] = (datetime.strptime(parameters_dict["start_date"], dtz_format) - timedelta(minutes = int(parameters_dict["window_length"]))).strftime(dtz_format)
+            parameters_dict["end_date"] = (datetime.strptime(parameters_dict["end_date"], dtz_format) + timedelta(minutes = int(parameters_dict["window_length"]))).strftime(dtz_format) 
         else:
-            parameters_dict["start_date"] = (datetime.strptime(parameters_dict["start_date"], datetime_format) - timedelta(minutes = int(parameters_dict["window_size_mins"]))).strftime(datetime_format)
-            parameters_dict["end_date"] = (datetime.strptime(parameters_dict["end_date"], datetime_format) + timedelta(minutes = int(parameters_dict["window_size_mins"]))).strftime(datetime_format)
+            parameters_dict["start_date"] = (datetime.strptime(parameters_dict["start_date"], dtz_format) - timedelta(minutes = int(parameters_dict["window_size_mins"]))).strftime(dtz_format)
+            parameters_dict["end_date"] = (datetime.strptime(parameters_dict["end_date"], dtz_format) + timedelta(minutes = int(parameters_dict["window_size_mins"]))).strftime(dtz_format)
+        
         pandas_df = raw_get(connection, parameters_dict)
 
         pandas_df["EventDate"] = pd.to_datetime(pandas_df["EventTime"]).dt.date  
+
         boundaries_df = pd.DataFrame(columns=["EventTime", "TagName"])
         for tag in parameters_dict["tag_names"]:
-            start_date_new_row = pd.DataFrame([[pd.to_datetime(parameters_dict["start_date"]).replace(tzinfo=pytz.timezone(utc)), tag]], columns=["EventTime", "TagName"])
-            end_date_new_row = pd.DataFrame([[pd.to_datetime(parameters_dict["end_date"]).replace(tzinfo=pytz.timezone(utc)), tag]], columns=["EventTime", "TagName"])
+            start_date_new_row = pd.DataFrame([[pd.to_datetime(parameters_dict["start_date"], utc=True).replace(tzinfo=pytz.timezone(utc)), tag]], columns=["EventTime", "TagName"])
+            end_date_new_row = pd.DataFrame([[pd.to_datetime(parameters_dict["end_date"], utc=True).replace(tzinfo=pytz.timezone(utc)), tag]], columns=["EventTime", "TagName"])
             boundaries_df = pd.concat([boundaries_df, start_date_new_row, end_date_new_row], ignore_index=True)
         boundaries_df.set_index(pd.DatetimeIndex(boundaries_df["EventTime"]), inplace=True)
         boundaries_df.drop(columns="EventTime", inplace=True)
         boundaries_df = boundaries_df.groupby(["TagName"]).resample("{}T".format(str(parameters_dict["window_size_mins"]))).ffill().drop(columns='TagName')
+        
         #preprocess - add boundaries and time interpolate missing boundary values
         preprocess_df = pandas_df.copy()
         preprocess_df["EventTime"] = preprocess_df["EventTime"].round("S")
         preprocess_df.set_index(["EventTime", "TagName", "EventDate"], inplace=True)
         preprocess_df = preprocess_df.join(boundaries_df, how="outer", rsuffix="right")
         if isinstance(parameters_dict["step"], str) and parameters_dict["step"].lower() == "metadata":
             metadata_df = metadata_get(connection, parameters_dict)
@@ -87,14 +105,15 @@
             preprocess_df = preprocess_df.merge(metadata_df, left_index=True, right_index=True)
         elif parameters_dict["step"] == True:
             preprocess_df["Step"] =  True
         elif parameters_dict["step"] == False:
             preprocess_df["Step"] = False
         else:
             raise Exception('Unexpected step value', parameters_dict["step"])
+        
         def process_time_weighted_averages_step(pandas_df):
             if pandas_df["Step"].any() == False:
                 pandas_df = pandas_df.reset_index(level=["TagName", "EventDate"]).sort_index().interpolate(method='time')
                 shift_raw_df = pandas_df.copy()
                 shift_raw_df["CalcValue"] = (shift_raw_df.index.to_series().diff().dt.seconds/86400) * shift_raw_df.Value.rolling(2).sum()
                 time_weighted_averages = shift_raw_df.resample("{}T".format(str(parameters_dict["window_size_mins"])), closed="right", label="right").CalcValue.sum() * 0.5 / parameters_dict["window_size_mins"] * 24 * 60
                 return time_weighted_averages
@@ -103,24 +122,22 @@
                 shift_raw_df = pandas_df.copy()
                 shift_raw_df["CalcValue"] = (shift_raw_df.index.to_series().diff().dt.seconds/86400) * shift_raw_df.Value.shift(1)
                 time_weighted_averages = shift_raw_df.resample("{}T".format(str(parameters_dict["window_size_mins"])), closed="right", label="right").CalcValue.sum() / parameters_dict["window_size_mins"] * 24 * 60
                 return time_weighted_averages
             
         #calculate time weighted averages
         time_weighted_averages = preprocess_df.groupby(["TagName"]).apply(process_time_weighted_averages_step).reset_index()
-
+        
         if "CalcValue" not in time_weighted_averages.columns:
             time_weighted_averages = time_weighted_averages.melt(id_vars="TagName", var_name="EventTime", value_name="Value")
         else: 
             time_weighted_averages = time_weighted_averages.rename(columns={"CalcValue": "Value"})
-            
-        time_weighted_averages = time_weighted_averages.set_index("EventTime").sort_values(by=["TagName", "EventTime"])
         
+        time_weighted_averages = time_weighted_averages.set_index("EventTime").sort_values(by=["TagName", "EventTime"])
         time_weighted_averages_datetime = time_weighted_averages.index.to_pydatetime()
-        weighted_averages_timezones = np.array([z.replace(tzinfo=pytz.timezone(utc)) for z in time_weighted_averages_datetime])
-        time_weighted_averages = time_weighted_averages[(original_start_date.replace(tzinfo=pytz.timezone(utc)) < weighted_averages_timezones) & (weighted_averages_timezones <= original_end_date.replace(tzinfo=pytz.timezone(utc)) + timedelta(seconds = 1))]
+        weighted_averages_timezones = np.array([z for z in time_weighted_averages_datetime])
+        time_weighted_averages = time_weighted_averages[(original_start_date < weighted_averages_timezones) & (weighted_averages_timezones <= original_end_date + timedelta(seconds = 1))]
         return time_weighted_averages
-    
         
     except Exception as e:
         logging.exception('error with time weighted average function', str(e))
         raise e
```

## rtdip_sdk/pipelines/_pipeline_utils/constants.py

```diff
@@ -33,10 +33,18 @@
     "spark_sql_kafka": MavenLibrary(
                 group_id="org.apache.spark", 
                 artifact_id="spark-sql-kafka-0-10_2.12",
                 version="3.4.0"
             ),
     "rtdip_sdk": PyPiLibrary(
                 name="rtdip_sdk",
-                version="0.2.0"
-            )
+                version="0.2.1"
+            ),
+    "azure_adls_gen_2": PyPiLibrary(
+                name="azure-storage-file-datalake",
+                version="12.10.1"
+            ),
+    "aws_boto3": PyPiLibrary(
+                name="boto3",
+                version="1.26.118"
+            )            
 }
```

## rtdip_sdk/pipelines/converters/pipeline_job_json.py

```diff
@@ -20,15 +20,15 @@
 from ..execute.models import PipelineJob
 from ..sources import * # NOSONAR
 from ..transformers import * # NOSONAR
 from ..destinations import * # NOSONAR
 from ..utilities import * # NOSONAR
 from ..secrets import * # NOSONAR
 
-class PipelineJobFromJson(ConverterInterface):
+class PipelineJobFromJsonConverter(ConverterInterface):
     '''
     Converts a json string into a Pipeline Job
 
     Args:
         pipeline_json (str): Json representing PipelineJob information, including tasks and related steps 
     '''
     pipeline_json: str
@@ -58,15 +58,15 @@
                     step["component_parameters"][param_key] = self._try_convert_to_pipeline_secret(param_value)
                     if not isinstance(step["component_parameters"][param_key], PipelineSecret) and isinstance(param_value, dict):
                         for key, value in param_value.items():
                             step["component_parameters"][param_key][key] = self._try_convert_to_pipeline_secret(value) 
 
         return PipelineJob(**pipeline_job_dict)
     
-class PipelineJobToJson(ConverterInterface):
+class PipelineJobToJsonConverter(ConverterInterface):
     '''
     Converts a Pipeline Job into a json string
 
     Args:
         pipeline_job (PipelineJob): A Pipeline Job consisting of tasks and steps
     '''
     pipeline_job: PipelineJob
```

## rtdip_sdk/pipelines/deploy/databricks.py

```diff
@@ -20,15 +20,15 @@
 from dbx.commands.deploy import deploy as dbx_deploy
 from dbx.commands.launch import launch as dbx_launch
 from dbx.api.auth import ProfileEnvConfigProvider
 
 from .interfaces import DeployInterface
 from .models.databricks import DatabricksJob, DatabricksJobForPipelineJob, DatabricksSparkPythonTask, DatabricksTask, DatabricksLibraries, DatabricksLibrariesMaven, DatbricksLibrariesPypi, DatabricksDBXProject
 from ..execute.job import PipelineJob
-from ..converters.pipeline_job_json import PipelineJobToJson
+from ..converters.pipeline_job_json import PipelineJobToJsonConverter
 
 __name__: str
 __version__: str
 __description__: str
 
 class DatabricksDBXDeploy(DeployInterface):
     '''
@@ -164,15 +164,15 @@
                 rtdip_version = version("rtdip-sdk")
                 databricks_job_task.libraries.append(DatabricksLibraries(pypi=DatbricksLibrariesPypi(package="rtdip-sdk[pipelines]=={}".format(rtdip_version))))
             except PackageNotFoundError as e:
                 databricks_job_task.libraries.append(DatabricksLibraries(pypi=DatbricksLibrariesPypi(package="rtdip-sdk[pipelines]")))
 
             databricks_job_task.spark_python_task = DatabricksSparkPythonTask(
                 python_file="file://{}".format("rtdip/tasks/pipeline_task.py"),
-                parameters=[PipelineJobToJson(self.pipeline_job).convert()]
+                parameters=[PipelineJobToJsonConverter(self.pipeline_job).convert()]
             )
             databricks_tasks.append(databricks_job_task)
 
         databricks_job = DatabricksJob(name=self.pipeline_job.name, tasks=databricks_tasks)
         databricks_job.__dict__.update(self.databricks_job_for_pipeline_job.__dict__)
         databricks_job.__dict__.pop("databricks_task_for_pipeline_task_list", None)
```

## rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/pipeline_task.py

```diff
@@ -21,15 +21,15 @@
 from rtdip_sdk.pipelines.utilities import * # NOSONAR
 from rtdip_sdk.pipelines.converters import * # NOSONAR
 
 class RTDIPPipelineTask(Task):
     def launch(self):
         self.logger.info("Launching RTDIP Pipeline Task")
         self.logger.info("Job to execute {}".format(sys.argv[0]))
-        pipeline_job = PipelineJobFromJson(sys.argv[0]).convert()
+        pipeline_job = PipelineJobFromJsonConverter(sys.argv[0]).convert()
         pipeline_job_execute = PipelineJobExecute(pipeline_job)
         pipeline_job_execute.run()
         self.logger.info("RTDIP Pipeline Task completed")
         
 # if you're using python_wheel_task, you'll need the entrypoint function to be used in setup.py
 def entrypoint():  # pragma: no cover
     task = RTDIPPipelineTask()
```

## rtdip_sdk/pipelines/transformers/__init__.py

```diff
@@ -8,10 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .spark.eventhub import *
-from .spark.json_to_opcua import *
+from .spark.binary_to_string import *
+from .spark.opc_publisher_json_to_opcua import *
 from .spark.opcua_to_process_control_data_model import *
```

## rtdip_sdk/pipelines/transformers/spark/opcua_to_process_control_data_model.py

```diff
@@ -14,15 +14,15 @@
 
 from pyspark.sql import DataFrame
 from pyspark.sql.functions import to_timestamp, col, regexp_replace, when, lit, coalesce
 
 from ..interfaces import TransformerInterface
 from ..._pipeline_utils.models import Libraries, SystemType
 
-class OPCUAToProcessControlDataModel(TransformerInterface):
+class OPCUAToProcessControlDataModelTransformer(TransformerInterface):
     '''
     Converts a Spark Dataframe column from a structured OPC UA schema to the RTDIP Process Control Data Model.
 
     Args:
         source_column_name (str): Spark Dataframe column containing the OPC UA data.
         status_null_value (str): If populated, will replace null values in the Status column with the specified value.
         timestamp_formats (list[str]): Specifies the timestamp formats to be used for converting the timestamp string to a Timestamp Type. For more information on formats, refer to this [documentation.](https://spark.apache.org/docs/latest/sql-ref-datetime-pattern.html)
```

## rtdip_sdk/pipelines/utilities/__init__.py

```diff
@@ -10,8 +10,9 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .spark.delta_table_create import *
 from .spark.delta_table_optimize import *
-from .spark.delta_table_vacuum import *
+from .spark.delta_table_vacuum import *
+from .azure.adls_gen2_acl import *
```

## Comparing `rtdip_sdk/pipelines/transformers/spark/eventhub.py` & `rtdip_sdk/pipelines/transformers/spark/binary_to_string.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,18 +13,30 @@
 # limitations under the License.
 
 from pyspark.sql import DataFrame
 
 from ..interfaces import TransformerInterface
 from ..._pipeline_utils.models import Libraries, SystemType
 
-class EventhubBodyBinaryToString(TransformerInterface):
+class BinaryToStringTransformer(TransformerInterface):
     '''
-    Converts the Eventhub dataframe body column from a binary to a string.
-    ''' 
+    Converts a dataframe body column from a binary to a string.
+
+    Args:
+        source_column_name (str): Spark Dataframe column containing the Binary data
+        target_column_name (str): Spark Dataframe column name to be used for the String data
+    '''
+
+    source_column_name: str
+    target_column_name: str
+
+    def __init__(self, source_column_name: str, target_column_name: str) -> None:
+        self.source_column_name = source_column_name
+        self.target_column_name = target_column_name
+
     @staticmethod
     def system_type():
         '''
         Attributes:
             SystemType (Environment): Requires PYSPARK
         '''
         return SystemType.PYSPARK
@@ -43,16 +55,16 @@
     
     def post_transform_validation(self):
         return True
 
     def transform(self, df: DataFrame) -> DataFrame:
         '''
         Args:
-            df (DataFrame): A dataframe based on the structure of the Spark Eventhub connector.
+            df (DataFrame): A dataframe containing a binary column.
 
         Returns:
             DataFrame: A dataframe with the body column converted to string.
         '''
         return (
             df
-            .withColumn("body", df["body"].cast("string"))
+            .withColumn(self.target_column_name, df[self.source_column_name].cast("string"))
         )
```

## Comparing `rtdip_sdk/pipelines/transformers/spark/json_to_opcua.py` & `rtdip_sdk/pipelines/transformers/spark/opc_publisher_json_to_opcua.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 from pyspark.sql.functions import from_json, col, explode
 from pyspark.sql.types import ArrayType, StringType
 
 from ..interfaces import TransformerInterface
 from ..._pipeline_utils.models import Libraries, SystemType
 from ..._pipeline_utils.spark import OPCUA_SCHEMA
 
-class JsonToOPCUA(TransformerInterface):
+class OPCPublisherJsonToOPCUATransformer(TransformerInterface):
     '''
-    Converts a Spark Dataframe column from a json string to OPC UA.
+    Converts a Spark Dataframe column containing a json string created by OPC Publisher to OPC UA.
 
     Args:
         source_column_name (str): Spark Dataframe column containing the Json OPC UA data
-        target_column_name (str): Column name to be used for the structyred OPC UA data.
+        target_column_name (str): Column name to be used for the structured OPC UA data
         multiple_rows_per_message (bool): Each Dataframe Row contains an array of/multiple OPC UA messages. The list of Json will be exploded into rows in the Dataframe.
     '''
 
     source_column_name: str
     target_column_name: str
     multiple_rows_per_message: bool
```

## Comparing `rtdip_sdk-0.2.1.dist-info/LICENSE.md` & `rtdip_sdk-0.2.2.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `rtdip_sdk-0.2.1.dist-info/METADATA` & `rtdip_sdk-0.2.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtdip-sdk
-Version: 0.2.1
+Version: 0.2.2
 Home-page: https://github.com/rtdip/core
 Project-URL: Issue Tracker, https://github.com/rtdip/core/issues
 Project-URL: Source, https://github.com/rtdip/core/
 Project-URL: Documentation, https://www.rtdip.io/
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -19,14 +19,16 @@
 Requires-Dist: pandas (==1.5.2)
 Requires-Dist: jinja2 (==3.0.3)
 Requires-Dist: jinjasql (==0.1.8)
 Provides-Extra: pipelines
 Requires-Dist: dependency-injector (==4.41.0) ; extra == 'pipelines'
 Requires-Dist: dbx (==0.8.10) ; extra == 'pipelines'
 Requires-Dist: pydantic (==1.10.6) ; extra == 'pipelines'
+Requires-Dist: azure-storage-file-datalake (==12.10.1) ; extra == 'pipelines'
+Requires-Dist: boto3 (==1.26.118) ; extra == 'pipelines'
 Provides-Extra: pyspark
 Requires-Dist: pyspark (==3.3.2) ; extra == 'pyspark'
 Requires-Dist: delta-spark (==2.3.0) ; extra == 'pyspark'
 
 <p align="center"><img src=https://raw.githubusercontent.com/rtdip/core/develop/docs/getting-started/images/rtdip-horizontal-color.png alt="rtdip" width=50% height=50%/></p>
 
 # What is the RTDIP SDK?
```

## Comparing `rtdip_sdk-0.2.1.dist-info/RECORD` & `rtdip_sdk-0.2.2.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 rtdip_sdk/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
 rtdip_sdk/authentication/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
 rtdip_sdk/authentication/authenticate.py,sha256=GPd7ftHVZjrGq3n9Gj7dwEjrSxpCwlSODzvQggIpfts,7210
 rtdip_sdk/functions/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
-rtdip_sdk/functions/_query_builder.py,sha256=m29X24I9U_WrgMmg9PyViEIPQ1vMWTKzdHrRG2CNLGU,8746
+rtdip_sdk/functions/_query_builder.py,sha256=6lhKs3NK0sKAWAXph2jmGhzl5mCa8qneB5kT30Q3s6g,9846
 rtdip_sdk/functions/interpolate.py,sha256=R5mAUWMU24oyC_DfbL3GoJE0nx4ddyBuYeTNCh2tdR8,2908
 rtdip_sdk/functions/metadata.py,sha256=DNy2X--PGw5ERj5sA2KuCJxChJ3uLN8TTgeIdLLWRcg,2293
-rtdip_sdk/functions/raw.py,sha256=O4Rg-DMSNx8iRxqyjfjnkzfn3Gf5l8TJOeI0ESLnOqw,2786
+rtdip_sdk/functions/raw.py,sha256=zFIsYyGdgE4GfLyidjNUH5CkgXfnNHVrLGsXV5iVeUA,2626
 rtdip_sdk/functions/resample.py,sha256=NT3bA1Ia8u834C1HC9dUQ1AaLy4PN2Yc51KN1Qee0wc,3052
-rtdip_sdk/functions/time_weighted_average.py,sha256=quQCHCpHT-zxW-SCNFV0U6vUQfV1FzJybXbXtjL1PKw,8921
+rtdip_sdk/functions/time_weighted_average.py,sha256=KvrGxZUyb1XkXg9xbzQVSzgad-F4T4LePhnsJZ-6OXY,9434
 rtdip_sdk/odbc/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
 rtdip_sdk/odbc/connection_interface.py,sha256=7FnrbBSvsCGNjutxutGvFYZfktY2hcDhyfLnCcCh-hQ,934
 rtdip_sdk/odbc/cursor_interface.py,sha256=JEWb1W72PXibztG8koTj-tOuejvoDsJh8k7mFvH-C6k,952
 rtdip_sdk/odbc/db_sql_connector.py,sha256=I6d8K3mm_ykIPh8-EjkNQDmdRGvCdFyROHsl8ErBY-g,3498
 rtdip_sdk/odbc/pyodbc_sql_connector.py,sha256=9Ap6Qh73enYXS6GnmrybN2mVH2CUCWCwUjxq7mrmtaQ,4228
 rtdip_sdk/odbc/turbodbc_sql_connector.py,sha256=Uv4DRn1y1QOiggN5nAVPB3RrS1hUuI56OsAAHspZqq0,4432
 rtdip_sdk/pipelines/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
 rtdip_sdk/pipelines/interfaces.py,sha256=RdiawOPSQ5Vxch6htM03MMKhyMBtU4RVtnTdl0jVBBU,1035
 rtdip_sdk/pipelines/_pipeline_utils/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
-rtdip_sdk/pipelines/_pipeline_utils/constants.py,sha256=insI6NqDXf80_tzyKlTnmQ_p09yp1_0X__UVuogCzd4,1485
+rtdip_sdk/pipelines/_pipeline_utils/constants.py,sha256=xFVUWjA89a-IwWy0SeeD2ZyNYpB9i5MOyglUhMMVxn4,1745
 rtdip_sdk/pipelines/_pipeline_utils/models.py,sha256=tvviN-pD1TBZQ_9t2icYGTP0LRnslore8NHlYaALlCw,2434
 rtdip_sdk/pipelines/_pipeline_utils/spark.py,sha256=SJYHa2HzZgj0VkDzYxqOC30zaYPaDC7IQ6yj25XyPDU,5327
 rtdip_sdk/pipelines/converters/__init__.py,sha256=hwO8Ac698lsn720_wfiyk7ss4cPWCFHMuNgJ7-YdMWQ,603
 rtdip_sdk/pipelines/converters/interfaces.py,sha256=wvm5Doxre6XJjc1nE9-l047MR4JjvyPCeGDIO3kUCt4,697
-rtdip_sdk/pipelines/converters/pipeline_job_json.py,sha256=8fm6NtsvN_bzDqaFiknzdfOlMjMMSMnpn9ZGDRAFd3E,3424
+rtdip_sdk/pipelines/converters/pipeline_job_json.py,sha256=8gZWk6FzsFZ3J2FjYz2Q3htpHxlXdSVHLJdqlJU6KRc,3442
 rtdip_sdk/pipelines/deploy/__init__.py,sha256=8wwgnaMDh2h_Y6kMrHKXFsXBdPASIeoLssPDgHyVSgA,630
-rtdip_sdk/pipelines/deploy/databricks.py,sha256=rv9qIxujRiMD-j6Zv2N4DQECHItfKQQOsep8znZcsME,13189
+rtdip_sdk/pipelines/deploy/databricks.py,sha256=vNc40X7ag6uj68ULgDGF-rdNx0cGo6mYNYldLkvyk7c,13207
 rtdip_sdk/pipelines/deploy/interfaces.py,sha256=s6FM0UjSFkF1LhPvBF52zOExuIIItXJql-1j9qiXvnQ,751
 rtdip_sdk/pipelines/deploy/dbx/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
 rtdip_sdk/pipelines/deploy/dbx/setup.py,sha256=7VEAGmbQ_qAd73g9T85DitK1EvObixrzoatjiufbeDU,1114
 rtdip_sdk/pipelines/deploy/dbx/conf/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
 rtdip_sdk/pipelines/deploy/dbx/rtdip/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
 rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/common.py,sha256=f7q1C5OvcHNrRNp1iAU461DKF4XnVi-dOFVs19Oj7bQ,3310
-rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/pipeline_task.py,sha256=sXMSI_gnEC3LTT-2ekEMKclZ3XXli8CbH8gIeu4xB9c,1686
+rtdip_sdk/pipelines/deploy/dbx/rtdip/tasks/pipeline_task.py,sha256=SfSnn2-D-sYWYobaRUQwFGvDg961r13oIjnEno3xWQM,1695
 rtdip_sdk/pipelines/deploy/models/__init__.py,sha256=eIke9C2leBQU1ezpJHbkoWUl7ExNw9QmxvZFbCyVomE,571
 rtdip_sdk/pipelines/deploy/models/databricks.py,sha256=BaVaRGHGoGiUiG_1ouBuAUOHc4t0nLCaLIIIj56Annc,7897
 rtdip_sdk/pipelines/destinations/__init__.py,sha256=oPnFMRb6Y1__25uf5yfR_ETeKDGfvn-hUAQupySWuV8,684
 rtdip_sdk/pipelines/destinations/interfaces.py,sha256=IjIYhBInHDAvtf52Z7zcvux9q0_ni8KkHj5kD1I6LP4,427
 rtdip_sdk/pipelines/destinations/spark/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
 rtdip_sdk/pipelines/destinations/spark/delta.py,sha256=WjMzdnEyZUVOS0DG-YoqVZ1FvKf1qVbOikl2VDXMi9g,5112
 rtdip_sdk/pipelines/destinations/spark/eventhub.py,sha256=12C5NvjzSctJytKv7iBoR5Qc1zxK0CM41JZQqQ5Ycqc,4781
@@ -56,24 +56,29 @@
 rtdip_sdk/pipelines/sources/spark/autoloader.py,sha256=rL0t5jd-RSowkpklhdSd__6adfrVD0c8LKmKvmqYBY0,3420
 rtdip_sdk/pipelines/sources/spark/delta.py,sha256=BuWtKZPDxRfe7XA6x7pJTTL8TxjJoMXEaPAomdrEdt8,4501
 rtdip_sdk/pipelines/sources/spark/delta_sharing.py,sha256=Mbb4Be4yN1X6biLDB-S6CDDos0SdKDTA97_sMY4W-1o,4473
 rtdip_sdk/pipelines/sources/spark/eventhub.py,sha256=jgUecN1ZkBKoAyVCM52SgbAPbdRl1Nknfbp-SozCRz0,5259
 rtdip_sdk/pipelines/sources/spark/iot_hub.py,sha256=LdVZkc-xOSTyq6y4sD1nmpef5zlSySJNwwtP4tXaMao,5240
 rtdip_sdk/pipelines/sources/spark/kafka.py,sha256=7OGqTZtkvNI8TaBB7hptYywclJOAzmHxOync_1jUayE,8114
 rtdip_sdk/pipelines/sources/spark/kinesis.py,sha256=uarSt6bVe-2amI8qaLd2lwabLnVcasMnrFu86KXyIDo,3793
-rtdip_sdk/pipelines/transformers/__init__.py,sha256=S_qtKJIha2LCb3oAfj_gOfgieVZCr5l1TMyvdZUc0ps,692
+rtdip_sdk/pipelines/transformers/__init__.py,sha256=kRfVwAJZ2_x58nEgV3hZj8qmwT1wS5NonF4tSJZY5bY,714
 rtdip_sdk/pipelines/transformers/interfaces.py,sha256=KZUm93QHDARxMobPg989HijfiBjSpOI8oVILSJlK30g,946
 rtdip_sdk/pipelines/transformers/spark/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rtdip_sdk/pipelines/transformers/spark/eventhub.py,sha256=Kxvb65UYOzt_bTTVs3gw9HfKG6gwvcdGMnJk6rVRWZo,1715
-rtdip_sdk/pipelines/transformers/spark/json_to_opcua.py,sha256=CWgNn91Mj3Txlq9JKdwfJSXaaLCMNC7Sbfmc0VQ9C5M,2900
-rtdip_sdk/pipelines/transformers/spark/opcua_to_process_control_data_model.py,sha256=3bw6qZgKpCJp7EyyG8w1_fzFsuhijsByTn-Pk3BcQ3Y,3560
-rtdip_sdk/pipelines/utilities/__init__.py,sha256=vGjc2wBsYJ9F6AXcZ6TC9wMnDp-vEHo8RSTH1WPjb7U,692
+rtdip_sdk/pipelines/transformers/spark/binary_to_string.py,sha256=sHIrhT4ncqIinZNSxmk5xcBsvpqH7lIpe3W_Pep8Vsw,2143
+rtdip_sdk/pipelines/transformers/spark/opc_publisher_json_to_opcua.py,sha256=Yj1ov6rxL083Pd0dHO3lTUKSs-KNVF1mGqQ3ZpcG_q4,2953
+rtdip_sdk/pipelines/transformers/spark/opcua_to_process_control_data_model.py,sha256=9EiuDH6E6reseFC-W33dnS0Yb0w7eyUKTrN6xHwPP5M,3571
+rtdip_sdk/pipelines/utilities/__init__.py,sha256=TI4telg5YtXtgyD0iLEPp_2fWDMkTHGbTwBJwWFtd_I,727
 rtdip_sdk/pipelines/utilities/interfaces.py,sha256=jHlDdFAgbUL9alAmU3Ncye_2iqywJLglFbZ04zaqNTQ,773
+rtdip_sdk/pipelines/utilities/aws/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
+rtdip_sdk/pipelines/utilities/aws/s3_bucket_policy.py,sha256=lScqjJU9fFRkgnBI1RrqG-Sswh0Ek7_waebBQrARIEY,4674
+rtdip_sdk/pipelines/utilities/azure/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
+rtdip_sdk/pipelines/utilities/azure/adls_gen2_acl.py,sha256=SXGZsO00_ZoEY9EdKs06vxAlmKLuAPcF8xX1SVbz1J4,6556
 rtdip_sdk/pipelines/utilities/spark/__init__.py,sha256=cLARnwRfLDutJ3PTR19AhwFxmrpjsYuxojv2GhlMlCU,569
+rtdip_sdk/pipelines/utilities/spark/configuration.py,sha256=hNlDyTCFr_ykTfigONZWtpAHLUHSH03Zet1LaM79pGs,2185
 rtdip_sdk/pipelines/utilities/spark/delta_table_create.py,sha256=NvPxUZapqt2_CZ3arKHkCUKcRnhdyruIBHmz3Jtok0k,3857
 rtdip_sdk/pipelines/utilities/spark/delta_table_optimize.py,sha256=8mBCct4mmhkypW41eFDbLYhWZEnlii1ANz5kwtWyNkM,3119
 rtdip_sdk/pipelines/utilities/spark/delta_table_vacuum.py,sha256=BvMUPC1NCFPXz4oN9XxsCnAsZ0vdiZTNp7bFsx7dFfg,2602
-rtdip_sdk-0.2.1.dist-info/LICENSE.md,sha256=WYmcYJG1QFgu1hfo7qrEkZ3Jhcz8NUWe6XUraZvlIFs,10172
-rtdip_sdk-0.2.1.dist-info/METADATA,sha256=aBJv_kKLezbJ33Mi_VwWHNraLKzWkl5tq79q9zR84cU,2709
-rtdip_sdk-0.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rtdip_sdk-0.2.1.dist-info/top_level.txt,sha256=DFRWw2FYwSXWlH6UsWDVt1G8Bq6QjRWN0GJ8BS4o2dg,10
-rtdip_sdk-0.2.1.dist-info/RECORD,,
+rtdip_sdk-0.2.2.dist-info/LICENSE.md,sha256=WYmcYJG1QFgu1hfo7qrEkZ3Jhcz8NUWe6XUraZvlIFs,10172
+rtdip_sdk-0.2.2.dist-info/METADATA,sha256=nD971CId17LH3wi-GcfXWYeoXTeokQ_SSXv4ezD4CWg,2844
+rtdip_sdk-0.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rtdip_sdk-0.2.2.dist-info/top_level.txt,sha256=DFRWw2FYwSXWlH6UsWDVt1G8Bq6QjRWN0GJ8BS4o2dg,10
+rtdip_sdk-0.2.2.dist-info/RECORD,,
```

