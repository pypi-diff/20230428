# Comparing `tmp/toucan_connectors-4.5.0.tar.gz` & `tmp/toucan_connectors-4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toucan_connectors-4.5.0.tar", max compression
+gzip compressed data, was "toucan_connectors-4.5.1.tar", max compression
```

## Comparing `toucan_connectors-4.5.0.tar` & `toucan_connectors-4.5.1.tar`

### file list

```diff
@@ -1,181 +1,181 @@
--rw-r--r--   0        0        0     1510 2023-04-24 14:57:47.480448 toucan_connectors-4.5.0/LICENSE
--rw-r--r--   0        0        0     9969 2023-04-24 14:57:47.480448 toucan_connectors-4.5.0/README.md
--rw-r--r--   0        0        0     5557 2023-04-24 14:57:47.484448 toucan_connectors-4.5.0/pyproject.toml
--rw-r--r--   0        0        0    10795 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/adobe_analytics/__init__.py
--rw-r--r--   0        0        0    13648 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/adobe_analytics/adobe-analytics.png
--rw-r--r--   0        0        0     1740 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/adobe_analytics/adobe_analytics_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/anaplan/__init__.py
--rw-r--r--   0        0        0     7277 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/anaplan/anaplan.png
--rw-r--r--   0        0        0     7006 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/anaplan/anaplan_connector.py
--rw-r--r--   0        0        0     4623 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/auth.py
--rw-r--r--   0        0        0    61900 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/aws/aws.png
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/awsathena/__init__.py
--rw-r--r--   0        0        0     2524 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/awsathena/athena.png
--rw-r--r--   0        0        0     8464 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/awsathena/awsathena_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/azure_mssql/__init__.py
--rw-r--r--   0        0        0     2404 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/azure_mssql/azure_mssql_connector.py
--rw-r--r--   0        0        0    24249 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/azure_mssql/sql-azure.png
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/clickhouse/__init__.py
--rw-r--r--   0        0        0     1780 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/clickhouse/clickhouse.png
--rw-r--r--   0        0        0     4541 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/clickhouse/clickhouse_connector.py
--rw-r--r--   0        0        0    15750 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/common.py
--rw-r--r--   0        0        0     5549 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/condition_translator.py
--rw-r--r--   0        0        0     8162 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/connection_manager.py
--rw-r--r--   0        0        0     3534 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/databricks/databricks.png
--rw-r--r--   0        0        0     5236 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/databricks/databricks_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/dataiku/__init__.py
--rw-r--r--   0        0        0    10971 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/dataiku/dataiku.png
--rw-r--r--   0        0        0     1100 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/dataiku/dataiku_connector.py
--rwxr-xr-x   0        0        0      235 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/default-logo.png
--rw-r--r--   0        0        0     3331 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/denodo/denodo.png
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/elasticsearch/__init__.py
--rw-r--r--   0        0        0    29549 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/elasticsearch/elasticsearch.png
--rw-r--r--   0        0        0     5118 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/elasticsearch/elasticsearch_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/facebook_ads/__init__.py
--rw-r--r--   0        0        0      452 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/facebook_ads/doc.md
--rw-r--r--   0        0        0      183 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/facebook_ads/enums.py
--rw-r--r--   0        0        0     5283 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/facebook_ads/facebook_ads_connector.py
--rw-r--r--   0        0        0    27755 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/facebook_ads/facebook_logo.png
--rw-r--r--   0        0        0      126 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/facebook_ads/helpers.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/facebook_insights/__init__.py
--rw-r--r--   0        0        0    38402 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/facebook_insights/facebook-insights.png
--rw-r--r--   0        0        0     3985 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/facebook_insights/facebook_insights_connector.py
--rw-r--r--   0        0        0    13001 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/github/GitHub_Logo.png
--rw-r--r--   0        0        0      412 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/github/doc.md
--rw-r--r--   0        0        0    17081 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/github/github_connector.py
--rw-r--r--   0        0        0    15903 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/github/helpers.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/google_adwords/__init__.py
--rw-r--r--   0        0        0      469 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_adwords/doc.md
--rw-r--r--   0        0        0    68711 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_adwords/google_adwords.jpg
--rw-r--r--   0        0        0     9049 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_adwords/google_adwords_connector.py
--rw-r--r--   0        0        0      834 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_adwords/helpers.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_analytics/__init__.py
--rw-r--r--   0        0        0     6243 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_analytics/google-analytics.png
--rw-r--r--   0        0        0     6799 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_analytics/google_analytics_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_big_query/__init__.py
--rw-r--r--   0        0        0    17667 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_big_query/google-bigquery.png
--rw-r--r--   0        0        0    12920 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_big_query/google_big_query_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_cloud_mysql/__init__.py
--rw-r--r--   0        0        0    24008 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png
--rw-r--r--   0        0        0     2488 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py
--rw-r--r--   0        0        0     2473 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_credentials.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_my_business/__init__.py
--rw-r--r--   0        0        0     4045 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_my_business/google-my-business.png
--rw-r--r--   0        0        0     3024 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_my_business/google_my_business_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_sheets/__init__.py
--rw-r--r--   0        0        0    14238 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_sheets/google-sheets.png
--rw-r--r--   0        0        0     9062 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_sheets/google_sheets_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_sheets_2/__init__.py
--rw-r--r--   0        0        0      361 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_sheets_2/doc.md
--rw-r--r--   0        0        0     9559 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_sheets_2/google_sheets_2_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_spreadsheet/__init__.py
--rw-r--r--   0        0        0    14238 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_spreadsheet/google-spreadsheet.png
--rw-r--r--   0        0        0     2986 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/http_api/__init__.py
--rw-r--r--   0        0        0    19694 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/http_api/http-api.png
--rw-r--r--   0        0        0     7584 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/http_api/http_api_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/hubspot/__init__.py
--rw-r--r--   0        0        0      380 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/hubspot/doc.md
--rw-r--r--   0        0        0      294 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/hubspot/enums.py
--rw-r--r--   0        0        0      173 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/hubspot/helpers.py
--rw-r--r--   0        0        0    33203 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/hubspot/hubspot.png
--rw-r--r--   0        0        0     5738 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/hubspot/hubspot_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/hubspot_private_app/__init__.py
--rw-r--r--   0        0        0     5197 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/hubspot_private_app/hubspot_connector.py
--rw-r--r--   0        0        0      140 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/install_scripts/__init__.py
--rwxr-xr-x   0        0        0      726 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/install_scripts/databricks.sh
--rwxr-xr-x   0        0        0      509 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/install_scripts/mssql.sh
--rwxr-xr-x   0        0        0      926 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/install_scripts/mssql_TLSv1_0.sh
--rwxr-xr-x   0        0        0      908 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/install_scripts/odbc.sh
--rwxr-xr-x   0        0        0      706 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/install_scripts/oracle.sh
--rw-r--r--   0        0        0     3285 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/json_wrapper.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/linkedinads/__init__.py
--rw-r--r--   0        0        0      365 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/linkedinads/doc.md
--rw-r--r--   0        0        0     9990 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/linkedinads/linkedinads.png
--rw-r--r--   0        0        0     7544 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/linkedinads/linkedinads_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/micro_strategy/__init__.py
--rw-r--r--   0        0        0     1853 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/micro_strategy/client.py
--rw-r--r--   0        0        0     4454 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/micro_strategy/data.py
--rw-r--r--   0        0        0     4664 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/micro_strategy/micro_strategy_connector.py
--rw-r--r--   0        0        0    13133 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/micro_strategy/microstrategy.png
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/mongo/__init__.py
--rw-r--r--   0        0        0    26880 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/mongo/mongo-db.png
--rw-r--r--   0        0        0    17097 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/mongo/mongo_connector.py
--rw-r--r--   0        0        0     1822 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/mongo/mongo_translator.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/mssql/__init__.py
--rw-r--r--   0        0        0    26319 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/mssql/mssql.png
--rw-r--r--   0        0        0     4673 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/mssql/mssql_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/mssql_TLSv1_0/__init__.py
--rw-r--r--   0        0        0    26319 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/mssql_TLSv1_0/mssql.png
--rw-r--r--   0        0        0     4893 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/mssql_TLSv1_0/mssql_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/mysql/__init__.py
--rw-r--r--   0        0        0     3761 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/mysql/mysql.png
--rw-r--r--   0        0        0    14657 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/mysql/mysql_connector.py
--rw-r--r--   0        0        0     2401 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/net_explorer/net_explorer.png
--rwxr-xr-x   0        0        0     3537 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/net_explorer/net_explorer_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/oauth2_connector/__init__.py
--rw-r--r--   0        0        0     6029 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/oauth2_connector/oauth2connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/odata/__init__.py
--rw-r--r--   0        0        0    31781 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/odata/odata.png
--rw-r--r--   0        0        0     2048 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/odata/odata_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/odbc/__init__.py
--rw-r--r--   0        0        0     3141 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/odbc/odbc.png
--rw-r--r--   0        0        0     1299 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/odbc/odbc_connector.py
--rw-r--r--   0        0        0    10551 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/one_drive/one_drive.png
--rwxr-xr-x   0        0        0    12312 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/one_drive/one_drive_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/oracle_sql/__init__.py
--rw-r--r--   0        0        0    12887 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/oracle_sql/oracle-sql.png
--rw-r--r--   0        0        0     3375 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/oracle_sql/oracle_sql_connector.py
--rw-r--r--   0        0        0     3948 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/pagination.py
--rw-r--r--   0        0        0     2638 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/pandas_translator.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/peakina/__init__.py
--rw-r--r--   0        0        0     1377 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/peakina/peakina.png
--rw-r--r--   0        0        0      509 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/peakina/peakina_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/postgres/__init__.py
--rw-r--r--   0        0        0    28440 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/postgres/postgres.png
--rw-r--r--   0        0        0    10400 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/postgres/postgresql_connector.py
--rw-r--r--   0        0        0    17824 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/postgres/utils.py
--rw-r--r--   0        0        0     1498 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/query_manager.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/redshift/__init__.py
--rw-r--r--   0        0        0     8867 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/redshift/redshift.png
--rw-r--r--   0        0        0    16551 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/redshift/redshift_database_connector.py
--rw-r--r--   0        0        0     1850 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/redshift/utils.py
--rw-r--r--   0        0        0      410 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/salesforce/doc.md
--rw-r--r--   0        0        0   165347 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/salesforce/salesforce-service-cloud.png
--rw-r--r--   0        0        0     8536 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/salesforce/salesforce.jpg
--rw-r--r--   0        0        0     7429 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/salesforce/salesforce_connector.py
--rw-r--r--   0        0        0      410 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/salesforce_sandbox/doc.md
--rw-r--r--   0        0        0   165347 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png
--rw-r--r--   0        0        0     8536 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/salesforce_sandbox/salesforce.jpg
--rw-r--r--   0        0        0       84 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/salesforce_sandbox/salesforce_sandbox_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/sap_hana/__init__.py
--rw-r--r--   0        0        0    20257 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/sap_hana/sap-hana.png
--rw-r--r--   0        0        0     1264 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/sap_hana/sap_hana_connector.py
--rw-r--r--   0        0        0    20013 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/share_point/share_point.png
--rw-r--r--   0        0        0      143 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/snowflake/__init__.py
--rw-r--r--   0        0        0    15417 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/snowflake/snowflake.png
--rw-r--r--   0        0        0    18251 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/snowflake/snowflake_connector.py
--rw-r--r--   0        0        0    12795 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/snowflake_common.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/snowflake_oauth2/__init__.py
--rw-r--r--   0        0        0    15417 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/snowflake_oauth2/snowflake.png
--rw-r--r--   0        0        0    12246 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/soap/__init__.py
--rw-r--r--   0        0        0      609 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/soap/helpers.py
--rw-r--r--   0        0        0    42145 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/soap/soap.png
--rw-r--r--   0        0        0     4325 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/soap/soap_connector.py
--rw-r--r--   0        0        0     3080 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/sql_query_helper.py
--rw-r--r--   0        0        0    21205 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/toucan_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/toucan_toco/__init__.py
--rwxr-xr-x   0        0        0     4372 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/toucan_toco/toucan.png
--rw-r--r--   0        0        0     1289 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/toucan_toco/toucan_toco_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/trello/__init__.py
--rw-r--r--   0        0        0     3966 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/trello/trello.png
--rw-r--r--   0        0        0     6603 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/trello/trello_connector.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/utils/__init__.py
--rw-r--r--   0        0        0      492 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/utils/datetime.py
--rw-r--r--   0        0        0      629 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/utils/pem.py
--rw-r--r--   0        0        0        0 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/wootric/__init__.py
--rw-r--r--   0        0        0     8734 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/wootric/wootric.png
--rw-r--r--   0        0        0     5228 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/wootric/wootric_connector.py
--rw-r--r--   0        0        0    14576 1970-01-01 00:00:00.000000 toucan_connectors-4.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1510 2023-04-28 07:36:04.308740 toucan_connectors-4.5.1/LICENSE
+-rw-r--r--   0        0        0     9969 2023-04-28 07:36:04.308740 toucan_connectors-4.5.1/README.md
+-rw-r--r--   0        0        0     5575 2023-04-28 07:36:04.312739 toucan_connectors-4.5.1/pyproject.toml
+-rw-r--r--   0        0        0    10795 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/adobe_analytics/__init__.py
+-rw-r--r--   0        0        0    13648 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/adobe_analytics/adobe-analytics.png
+-rw-r--r--   0        0        0     1740 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/adobe_analytics/adobe_analytics_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/anaplan/__init__.py
+-rw-r--r--   0        0        0     7277 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/anaplan/anaplan.png
+-rw-r--r--   0        0        0     7005 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/anaplan/anaplan_connector.py
+-rw-r--r--   0        0        0     4622 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/auth.py
+-rw-r--r--   0        0        0    61900 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/aws/aws.png
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/awsathena/__init__.py
+-rw-r--r--   0        0        0     2524 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/awsathena/athena.png
+-rw-r--r--   0        0        0     8464 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/awsathena/awsathena_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/azure_mssql/__init__.py
+-rw-r--r--   0        0        0     2404 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/azure_mssql/azure_mssql_connector.py
+-rw-r--r--   0        0        0    24249 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/azure_mssql/sql-azure.png
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/clickhouse/__init__.py
+-rw-r--r--   0        0        0     1780 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/clickhouse/clickhouse.png
+-rw-r--r--   0        0        0     4541 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/clickhouse/clickhouse_connector.py
+-rw-r--r--   0        0        0    15750 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/common.py
+-rw-r--r--   0        0        0     5549 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/condition_translator.py
+-rw-r--r--   0        0        0     8162 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/connection_manager.py
+-rw-r--r--   0        0        0     3534 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/databricks/databricks.png
+-rw-r--r--   0        0        0     5236 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/databricks/databricks_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/dataiku/__init__.py
+-rw-r--r--   0        0        0    10971 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/dataiku/dataiku.png
+-rw-r--r--   0        0        0     1100 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/dataiku/dataiku_connector.py
+-rwxr-xr-x   0        0        0      235 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/default-logo.png
+-rw-r--r--   0        0        0     3331 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/denodo/denodo.png
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/elasticsearch/__init__.py
+-rw-r--r--   0        0        0    29549 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/elasticsearch/elasticsearch.png
+-rw-r--r--   0        0        0     5118 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/elasticsearch/elasticsearch_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/facebook_ads/__init__.py
+-rw-r--r--   0        0        0      452 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/facebook_ads/doc.md
+-rw-r--r--   0        0        0      183 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/facebook_ads/enums.py
+-rw-r--r--   0        0        0     5283 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/facebook_ads/facebook_ads_connector.py
+-rw-r--r--   0        0        0    27755 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/facebook_ads/facebook_logo.png
+-rw-r--r--   0        0        0      126 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/facebook_ads/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/facebook_insights/__init__.py
+-rw-r--r--   0        0        0    38402 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/facebook_insights/facebook-insights.png
+-rw-r--r--   0        0        0     3985 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/facebook_insights/facebook_insights_connector.py
+-rw-r--r--   0        0        0    13001 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/github/GitHub_Logo.png
+-rw-r--r--   0        0        0      412 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/github/doc.md
+-rw-r--r--   0        0        0    17081 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/github/github_connector.py
+-rw-r--r--   0        0        0    15902 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/github/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_adwords/__init__.py
+-rw-r--r--   0        0        0      469 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_adwords/doc.md
+-rw-r--r--   0        0        0    68711 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_adwords/google_adwords.jpg
+-rw-r--r--   0        0        0     9049 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_adwords/google_adwords_connector.py
+-rw-r--r--   0        0        0      834 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_adwords/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_analytics/__init__.py
+-rw-r--r--   0        0        0     6243 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_analytics/google-analytics.png
+-rw-r--r--   0        0        0     6799 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_analytics/google_analytics_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_big_query/__init__.py
+-rw-r--r--   0        0        0    17667 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_big_query/google-bigquery.png
+-rw-r--r--   0        0        0    12920 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_big_query/google_big_query_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_cloud_mysql/__init__.py
+-rw-r--r--   0        0        0    24008 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png
+-rw-r--r--   0        0        0     2488 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py
+-rw-r--r--   0        0        0     2473 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_credentials.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_my_business/__init__.py
+-rw-r--r--   0        0        0     4045 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_my_business/google-my-business.png
+-rw-r--r--   0        0        0     3024 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_my_business/google_my_business_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_sheets/__init__.py
+-rw-r--r--   0        0        0    14238 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_sheets/google-sheets.png
+-rw-r--r--   0        0        0     9061 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_sheets/google_sheets_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_sheets_2/__init__.py
+-rw-r--r--   0        0        0      361 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_sheets_2/doc.md
+-rw-r--r--   0        0        0     9559 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_sheets_2/google_sheets_2_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_spreadsheet/__init__.py
+-rw-r--r--   0        0        0    14238 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_spreadsheet/google-spreadsheet.png
+-rw-r--r--   0        0        0     2986 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/http_api/__init__.py
+-rw-r--r--   0        0        0    19694 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/http_api/http-api.png
+-rw-r--r--   0        0        0     7584 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/http_api/http_api_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/hubspot/__init__.py
+-rw-r--r--   0        0        0      380 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/hubspot/doc.md
+-rw-r--r--   0        0        0      294 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/hubspot/enums.py
+-rw-r--r--   0        0        0      173 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/hubspot/helpers.py
+-rw-r--r--   0        0        0    33203 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/hubspot/hubspot.png
+-rw-r--r--   0        0        0     5738 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/hubspot/hubspot_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/hubspot_private_app/__init__.py
+-rw-r--r--   0        0        0     5197 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/hubspot_private_app/hubspot_connector.py
+-rw-r--r--   0        0        0      140 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/install_scripts/__init__.py
+-rwxr-xr-x   0        0        0      726 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/install_scripts/databricks.sh
+-rwxr-xr-x   0        0        0      509 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/install_scripts/mssql.sh
+-rwxr-xr-x   0        0        0      926 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/install_scripts/mssql_TLSv1_0.sh
+-rwxr-xr-x   0        0        0      908 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/install_scripts/odbc.sh
+-rwxr-xr-x   0        0        0      706 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/install_scripts/oracle.sh
+-rw-r--r--   0        0        0     3285 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/json_wrapper.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/linkedinads/__init__.py
+-rw-r--r--   0        0        0      365 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/linkedinads/doc.md
+-rw-r--r--   0        0        0     9990 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/linkedinads/linkedinads.png
+-rw-r--r--   0        0        0     7544 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/linkedinads/linkedinads_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/micro_strategy/__init__.py
+-rw-r--r--   0        0        0     1853 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/micro_strategy/client.py
+-rw-r--r--   0        0        0     4454 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/micro_strategy/data.py
+-rw-r--r--   0        0        0     4664 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/micro_strategy/micro_strategy_connector.py
+-rw-r--r--   0        0        0    13133 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/micro_strategy/microstrategy.png
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/mongo/__init__.py
+-rw-r--r--   0        0        0    26880 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/mongo/mongo-db.png
+-rw-r--r--   0        0        0    17096 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/mongo/mongo_connector.py
+-rw-r--r--   0        0        0     1822 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/mongo/mongo_translator.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/mssql/__init__.py
+-rw-r--r--   0        0        0    26319 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/mssql/mssql.png
+-rw-r--r--   0        0        0     4673 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/mssql/mssql_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/mssql_TLSv1_0/__init__.py
+-rw-r--r--   0        0        0    26319 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/mssql_TLSv1_0/mssql.png
+-rw-r--r--   0        0        0     4893 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/mssql_TLSv1_0/mssql_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/mysql/__init__.py
+-rw-r--r--   0        0        0     3761 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/mysql/mysql.png
+-rw-r--r--   0        0        0    14656 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/mysql/mysql_connector.py
+-rw-r--r--   0        0        0     2401 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/net_explorer/net_explorer.png
+-rwxr-xr-x   0        0        0     3536 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/net_explorer/net_explorer_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/oauth2_connector/__init__.py
+-rw-r--r--   0        0        0     6028 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/oauth2_connector/oauth2connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/odata/__init__.py
+-rw-r--r--   0        0        0    31781 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/odata/odata.png
+-rw-r--r--   0        0        0     2047 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/odata/odata_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/odbc/__init__.py
+-rw-r--r--   0        0        0     3141 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/odbc/odbc.png
+-rw-r--r--   0        0        0     1298 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/odbc/odbc_connector.py
+-rw-r--r--   0        0        0    10551 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/one_drive/one_drive.png
+-rwxr-xr-x   0        0        0    12312 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/one_drive/one_drive_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/oracle_sql/__init__.py
+-rw-r--r--   0        0        0    12887 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/oracle_sql/oracle-sql.png
+-rw-r--r--   0        0        0     3375 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/oracle_sql/oracle_sql_connector.py
+-rw-r--r--   0        0        0     3948 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/pagination.py
+-rw-r--r--   0        0        0     2638 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/pandas_translator.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/peakina/__init__.py
+-rw-r--r--   0        0        0     1377 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/peakina/peakina.png
+-rw-r--r--   0        0        0      509 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/peakina/peakina_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/postgres/__init__.py
+-rw-r--r--   0        0        0    28440 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/postgres/postgres.png
+-rw-r--r--   0        0        0    10400 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/postgres/postgresql_connector.py
+-rw-r--r--   0        0        0    17824 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/postgres/utils.py
+-rw-r--r--   0        0        0     1498 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/query_manager.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/redshift/__init__.py
+-rw-r--r--   0        0        0     8867 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/redshift/redshift.png
+-rw-r--r--   0        0        0    16551 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/redshift/redshift_database_connector.py
+-rw-r--r--   0        0        0     1850 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/redshift/utils.py
+-rw-r--r--   0        0        0      410 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/salesforce/doc.md
+-rw-r--r--   0        0        0   165347 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/salesforce/salesforce-service-cloud.png
+-rw-r--r--   0        0        0     8536 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/salesforce/salesforce.jpg
+-rw-r--r--   0        0        0     7429 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/salesforce/salesforce_connector.py
+-rw-r--r--   0        0        0      410 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/salesforce_sandbox/doc.md
+-rw-r--r--   0        0        0   165347 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png
+-rw-r--r--   0        0        0     8536 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/salesforce_sandbox/salesforce.jpg
+-rw-r--r--   0        0        0       84 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/salesforce_sandbox/salesforce_sandbox_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/sap_hana/__init__.py
+-rw-r--r--   0        0        0    20257 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/sap_hana/sap-hana.png
+-rw-r--r--   0        0        0     1264 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/sap_hana/sap_hana_connector.py
+-rw-r--r--   0        0        0    20013 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/share_point/share_point.png
+-rw-r--r--   0        0        0      143 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/snowflake/__init__.py
+-rw-r--r--   0        0        0    15417 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/snowflake/snowflake.png
+-rw-r--r--   0        0        0    18251 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/snowflake/snowflake_connector.py
+-rw-r--r--   0        0        0    12795 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/snowflake_common.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/snowflake_oauth2/__init__.py
+-rw-r--r--   0        0        0    15417 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/snowflake_oauth2/snowflake.png
+-rw-r--r--   0        0        0    12246 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/soap/__init__.py
+-rw-r--r--   0        0        0      609 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/soap/helpers.py
+-rw-r--r--   0        0        0    42145 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/soap/soap.png
+-rw-r--r--   0        0        0     4325 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/soap/soap_connector.py
+-rw-r--r--   0        0        0     3080 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/sql_query_helper.py
+-rw-r--r--   0        0        0    21205 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/toucan_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/toucan_toco/__init__.py
+-rwxr-xr-x   0        0        0     4372 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/toucan_toco/toucan.png
+-rw-r--r--   0        0        0     1289 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/toucan_toco/toucan_toco_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/trello/__init__.py
+-rw-r--r--   0        0        0     3966 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/trello/trello.png
+-rw-r--r--   0        0        0     6603 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/trello/trello_connector.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/utils/__init__.py
+-rw-r--r--   0        0        0      492 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/utils/datetime.py
+-rw-r--r--   0        0        0      629 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/utils/pem.py
+-rw-r--r--   0        0        0        0 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/wootric/__init__.py
+-rw-r--r--   0        0        0     8734 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/wootric/wootric.png
+-rw-r--r--   0        0        0     5228 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/wootric/wootric_connector.py
+-rw-r--r--   0        0        0    14616 1970-01-01 00:00:00.000000 toucan_connectors-4.5.1/PKG-INFO
```

### Comparing `toucan_connectors-4.5.0/LICENSE` & `toucan_connectors-4.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/README.md` & `toucan_connectors-4.5.1/README.md`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/pyproject.toml` & `toucan_connectors-4.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 profile = "black"
 include_trailing_comma = true
 line_length = 100
 multi_line_output = 3
 
 [tool.poetry]
 name = "toucan-connectors"
-version = "4.5.0"
+version = "4.5.1"
 description = "Toucan Toco Connectors"
 authors = ["Toucan Toco <dev@toucantoco.com>"]
 license = "BSD"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
@@ -59,30 +59,31 @@
 pyhdb = {version = ">=0.3.4,<1.0", optional = true}
 zeep = {version = "^4.1.0", optional = true}
 snowflake-connector-python = {version = ">=2.7.12,<4.0.0", optional = true}
 pyarrow = {version = "<12", optional = true}
 toucan-client = {version = "^1.0.1", optional = true}
 peakina = {version = "^0.11.0", optional = true}
 hubspot-api-client = {version = "^7.4.0", optional = true}
+aiohttp = "^3.8.4"
 
 [tool.poetry.dev-dependencies]
 Authlib = "^1.0.1"
 aioresponses = ">=0.7.3,<1.0"
-black = "^22.12.0"
+black = "^23.3.0"
 click = "^8.1.3"
 cryptography = ">=40.0.2"
 docker = "^6.0.1"
 flake8 = "^6.0.0"
 flake8-quotes = "^3.3.2"
 isort = "^5.12.0"
 mock = "^5.0.2"
 pytest-aiohttp = "^1.0.4"
 pytest-asyncio = ">=0.19.0,<1"
 pytest-cov = "^4.0.0"
-pytest = "^7.2.2"
+pytest = "^7.3.1"
 pytest-mock = "^3.10.0"
 pytest-rerunfailures = "^11.1"
 python-slugify = "<7"
 PyYAML = "<6"
 responses = ">=0.21.0,<1"
 psycopg2 = "^2.9.3"
 xmltodict = ">=0.13.0,<1"
```

### Comparing `toucan_connectors-4.5.0/toucan_connectors/__init__.py` & `toucan_connectors-4.5.1/toucan_connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/adobe_analytics/adobe-analytics.png` & `toucan_connectors-4.5.1/toucan_connectors/adobe_analytics/adobe-analytics.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/adobe_analytics/adobe_analytics_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/adobe_analytics/adobe_analytics_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/anaplan/anaplan.png` & `toucan_connectors-4.5.1/toucan_connectors/anaplan/anaplan.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/anaplan/anaplan_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/anaplan/anaplan_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 
         Once the connector is configured, we can give suggestions for the `model` field.
         If `model` is set, we can give suggestions for the `view` field.
         """
 
         constraints = {}
         with contextlib.suppress(AnaplanError, KeyError):
-
             token = connector.fetch_token()
             available_workspaces = connector.get_available_workspaces(token=token)
             constraints['workspace_id'] = strlist_to_enum(
                 'workspace_id', [_format_name_and_id(w) for w in available_workspaces]
             )
 
             if 'workspace_id' in current_config:
```

### Comparing `toucan_connectors-4.5.0/toucan_connectors/auth.py` & `toucan_connectors-4.5.1/toucan_connectors/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,14 @@
             'headers': headers,
             'json': json,
         }
         self.auth = auth
         self.filter = filter
 
     def __call__(self, r):
-
         if self.auth:
             session = Auth(**self.auth).get_session()
         else:
             session = Session()
 
         res = session.request(**self.request_kwargs)
         token = jq.first(self.filter, res.json())
```

### Comparing `toucan_connectors-4.5.0/toucan_connectors/aws/aws.png` & `toucan_connectors-4.5.1/toucan_connectors/aws/aws.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/awsathena/athena.png` & `toucan_connectors-4.5.1/toucan_connectors/awsathena/athena.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/awsathena/awsathena_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/awsathena/awsathena_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/azure_mssql/azure_mssql_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/azure_mssql/azure_mssql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/azure_mssql/sql-azure.png` & `toucan_connectors-4.5.1/toucan_connectors/azure_mssql/sql-azure.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/clickhouse/clickhouse.png` & `toucan_connectors-4.5.1/toucan_connectors/clickhouse/clickhouse.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/clickhouse/clickhouse_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/clickhouse/clickhouse_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/common.py` & `toucan_connectors-4.5.1/toucan_connectors/common.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/condition_translator.py` & `toucan_connectors-4.5.1/toucan_connectors/condition_translator.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/connection_manager.py` & `toucan_connectors-4.5.1/toucan_connectors/connection_manager.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/databricks/databricks.png` & `toucan_connectors-4.5.1/toucan_connectors/databricks/databricks.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/databricks/databricks_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/databricks/databricks_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/dataiku/dataiku.png` & `toucan_connectors-4.5.1/toucan_connectors/dataiku/dataiku.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/dataiku/dataiku_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/dataiku/dataiku_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/denodo/denodo.png` & `toucan_connectors-4.5.1/toucan_connectors/denodo/denodo.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/elasticsearch/elasticsearch.png` & `toucan_connectors-4.5.1/toucan_connectors/elasticsearch/elasticsearch.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/elasticsearch/elasticsearch_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/elasticsearch/elasticsearch_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/facebook_ads/facebook_ads_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/facebook_ads/facebook_ads_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/facebook_ads/facebook_logo.png` & `toucan_connectors-4.5.1/toucan_connectors/facebook_ads/facebook_logo.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/facebook_insights/facebook-insights.png` & `toucan_connectors-4.5.1/toucan_connectors/facebook_insights/facebook-insights.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/facebook_insights/facebook_insights_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/facebook_insights/facebook_insights_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/github/GitHub_Logo.png` & `toucan_connectors-4.5.1/toucan_connectors/github/GitHub_Logo.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/github/github_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/github/github_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/github/helpers.py` & `toucan_connectors-4.5.1/toucan_connectors/github/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,14 @@
     current_record = {}
     current_record['PR Name'] = pr_row.get('title')
     current_record['PR Creation Date'] = pr_row.get('createdAt')
     current_record['PR Merging Date'] = pr_row.get('mergedAt')
     current_record['PR Additions'] = pr_row.get('additions')
     current_record['PR Deletions'] = pr_row.get('deletions')
     try:
-
         current_record['PR Type'] = [
             label['node'].get('name') for label in pr_row['labels'].get('edges')
         ]
         edges = get_edges(pr_row.get('commits'))
         # Here we choose to select the author of the last commit as the author of the PR
         # It's less wrong than choosing the author of the first commit in case of rebase
         current_record['Dev'] = edges[-1]['node']['commit']['author']['user']['login']
```

### Comparing `toucan_connectors-4.5.0/toucan_connectors/google_adwords/google_adwords.jpg` & `toucan_connectors-4.5.1/toucan_connectors/google_adwords/google_adwords.jpg`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/google_adwords/google_adwords_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/google_adwords/google_adwords_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/google_adwords/helpers.py` & `toucan_connectors-4.5.1/toucan_connectors/google_adwords/helpers.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/google_analytics/google-analytics.png` & `toucan_connectors-4.5.1/toucan_connectors/google_analytics/google-analytics.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/google_analytics/google_analytics_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/google_analytics/google_analytics_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/google_big_query/google-bigquery.png` & `toucan_connectors-4.5.1/toucan_connectors/google_big_query/google-bigquery.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/google_big_query/google_big_query_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/google_big_query/google_big_query_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png` & `toucan_connectors-4.5.1/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/google_credentials.py` & `toucan_connectors-4.5.1/toucan_connectors/google_credentials.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/google_my_business/google-my-business.png` & `toucan_connectors-4.5.1/toucan_connectors/google_my_business/google-my-business.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/google_my_business/google_my_business_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/google_my_business/google_my_business_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/google_sheets/google-sheets.png` & `toucan_connectors-4.5.1/toucan_connectors/google_sheets/google-sheets.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/google_sheets/google_sheets_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/google_sheets/google_sheets_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,14 @@
         Following the documentation, to prevent loading dates as double :
         https://developers.google.com/sheets/api/reference/rest/v4/DateTimeRenderOption
         We use FORMATTED_STRING to load as simple strings
         """
         return 'SERIAL_NUMBER' if data_source.dates_as_float else 'FORMATTED_STRING'
 
     def _retrieve_data(self, data_source: GoogleSheetsDataSource) -> pd.DataFrame:
-
         if data_source.sheet is None:
             # Select the first sheet by default
             sheet_names = self.list_sheets(data_source.spreadsheet_id)
             data_source.sheet = sheet_names[0]
 
         with self.build_sheets_api() as sheets_api:
             sheet_values = (
```

### Comparing `toucan_connectors-4.5.0/toucan_connectors/google_sheets_2/google_sheets_2_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/google_sheets_2/google_sheets_2_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/google_spreadsheet/google-spreadsheet.png` & `toucan_connectors-4.5.1/toucan_connectors/google_spreadsheet/google-spreadsheet.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/http_api/http-api.png` & `toucan_connectors-4.5.1/toucan_connectors/http_api/http-api.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/http_api/http_api_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/http_api/http_api_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/hubspot/hubspot.png` & `toucan_connectors-4.5.1/toucan_connectors/hubspot/hubspot.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/hubspot/hubspot_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/hubspot/hubspot_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/hubspot_private_app/hubspot_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/hubspot_private_app/hubspot_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/install_scripts/databricks.sh` & `toucan_connectors-4.5.1/toucan_connectors/install_scripts/databricks.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/install_scripts/mssql_TLSv1_0.sh` & `toucan_connectors-4.5.1/toucan_connectors/install_scripts/mssql_TLSv1_0.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/install_scripts/odbc.sh` & `toucan_connectors-4.5.1/toucan_connectors/install_scripts/odbc.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/install_scripts/oracle.sh` & `toucan_connectors-4.5.1/toucan_connectors/install_scripts/oracle.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/json_wrapper.py` & `toucan_connectors-4.5.1/toucan_connectors/json_wrapper.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/linkedinads/linkedinads.png` & `toucan_connectors-4.5.1/toucan_connectors/linkedinads/linkedinads.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/linkedinads/linkedinads_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/linkedinads/linkedinads_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/micro_strategy/client.py` & `toucan_connectors-4.5.1/toucan_connectors/micro_strategy/client.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/micro_strategy/data.py` & `toucan_connectors-4.5.1/toucan_connectors/micro_strategy/data.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/micro_strategy/micro_strategy_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/micro_strategy/micro_strategy_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/micro_strategy/microstrategy.png` & `toucan_connectors-4.5.1/toucan_connectors/micro_strategy/microstrategy.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/mongo/mongo-db.png` & `toucan_connectors-4.5.1/toucan_connectors/mongo/mongo-db.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/mongo/mongo_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/mongo/mongo_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,14 @@
 
 def validate_collection(client, database: str, collection: str):
     if collection not in client[database].list_collection_names():
         raise UnkwownMongoCollection(f"Collection {collection!r} doesn't exist")
 
 
 class MongoDataSource(ToucanDataSource):
-
     database: str = Field(..., description='The name of the database you want to query')
     collection: str = Field(..., description='The name of the collection you want to query')
     query: Union[dict, list] = Field(
         {},
         description='A mongo query. See more details on the Mongo '
         'Aggregation Pipeline in the MongoDB documentation',
     )
```

### Comparing `toucan_connectors-4.5.0/toucan_connectors/mongo/mongo_translator.py` & `toucan_connectors-4.5.1/toucan_connectors/mongo/mongo_translator.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/mssql/mssql.png` & `toucan_connectors-4.5.1/toucan_connectors/mssql/mssql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/mssql/mssql_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/mssql/mssql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/mssql_TLSv1_0/mssql.png` & `toucan_connectors-4.5.1/toucan_connectors/mssql_TLSv1_0/mssql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/mssql_TLSv1_0/mssql_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/mssql_TLSv1_0/mssql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/mysql/mysql.png` & `toucan_connectors-4.5.1/toucan_connectors/mysql/mysql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/mysql/mysql_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/mysql/mysql_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,14 @@
             raise ValueError('SSL option "ssl_cert" should be specified if "ssl_key" is provided !')
 
         return ssl_key
 
     def _sanitize_ssl_params(self) -> dict[str, Any]:
         params = {}
         if self.ssl_mode in (SSLMode.VERIFY_CA, SSLMode.VERIFY_IDENTITY):
-
             for ssl_opt in ('ssl_ca', 'ssl_key', 'ssl_cert'):
                 opt = getattr(self, ssl_opt)
                 if opt is None:
                     continue
                 secret = opt.get_secret_value()
                 if secret.strip() != '':
                     params[ssl_opt] = sanitize_spaces_pem(secret)
```

### Comparing `toucan_connectors-4.5.0/toucan_connectors/net_explorer/net_explorer.png` & `toucan_connectors-4.5.1/toucan_connectors/net_explorer/net_explorer.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/net_explorer/net_explorer_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/net_explorer/net_explorer_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
         headers = {'Authorization': f'Bearer {token}'}
 
         resp = requests.get(folders_url, data={}, headers=headers)
 
         return resp.json()
 
     def _retrieve_file_id(self, folders, data_source):
-
         basedir = data_source.file.split('/')[0]
         path = data_source.file.split('/')[1:]
 
         _id = None
 
         def _search(iterate_on, compare_to, for_id=False):
             for element in iterate_on:
```

### Comparing `toucan_connectors-4.5.0/toucan_connectors/oauth2_connector/oauth2connector.py` & `toucan_connectors-4.5.1/toucan_connectors/oauth2_connector/oauth2connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,14 @@
         Methods returns only access_token
         instance_url parameters are return by service, better to use it
         new method get_access_data return all information to connect (secret and instance_url)
         """
         token = self.secrets_keeper.load(self.auth_flow_id)
 
         if 'expires_at' in token:
-
             expires_at = token['expires_at']
             if isinstance(expires_at, bool):
                 is_expired = expires_at
             elif isinstance(expires_at, (int, float)):
                 is_expired = expires_at < time()
             else:
                 is_expired = expires_at.timestamp() < time()
```

### Comparing `toucan_connectors-4.5.0/toucan_connectors/odata/odata.png` & `toucan_connectors-4.5.1/toucan_connectors/odata/odata.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/odata/odata_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/odata/odata_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 class ODataConnector(ToucanConnector):
     data_source_model: ODataDataSource
 
     baseroute: HttpUrl = Field(..., title='API endpoint', description='Baseroute URL')
     auth: Auth = Field(None, title='Authentication type')
 
     def _retrieve_data(self, data_source: ODataDataSource) -> pd.DataFrame:
-
         if self.auth:
             session = self.auth.get_session()
         else:
             session = None
 
         service = ODataService(self.baseroute, reflect_entities=True, session=session)
         entities = service.entities[data_source.entity]
```

### Comparing `toucan_connectors-4.5.0/toucan_connectors/odbc/odbc.png` & `toucan_connectors-4.5.1/toucan_connectors/odbc/odbc.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/odbc/odbc_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/odbc/odbc_connector.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,13 @@
             'ansi': self.ansi,
             'timeout': self.connect_timeout,
         }
         # remove None values
         return {k: v for k, v in con_params.items() if v is not None}
 
     def _retrieve_data(self, datasource: OdbcDataSource) -> pd.DataFrame:
-
         connection = pyodbc.connect(self.connection_string, **self.get_connection_params())
         df = pandas_read_sql(
             datasource.query, con=connection, params=datasource.parameters, convert_to_qmark=True
         )
         connection.close()
         return df
```

### Comparing `toucan_connectors-4.5.0/toucan_connectors/one_drive/one_drive.png` & `toucan_connectors-4.5.1/toucan_connectors/one_drive/one_drive.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/one_drive/one_drive_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/one_drive/one_drive_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/oracle_sql/oracle-sql.png` & `toucan_connectors-4.5.1/toucan_connectors/oracle_sql/oracle-sql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/oracle_sql/oracle_sql_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/oracle_sql/oracle_sql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/pagination.py` & `toucan_connectors-4.5.1/toucan_connectors/pagination.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/pandas_translator.py` & `toucan_connectors-4.5.1/toucan_connectors/pandas_translator.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/peakina/peakina.png` & `toucan_connectors-4.5.1/toucan_connectors/peakina/peakina.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/postgres/postgres.png` & `toucan_connectors-4.5.1/toucan_connectors/postgres/postgres.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/postgres/postgresql_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/postgres/postgresql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/postgres/utils.py` & `toucan_connectors-4.5.1/toucan_connectors/postgres/utils.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/query_manager.py` & `toucan_connectors-4.5.1/toucan_connectors/query_manager.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/redshift/redshift.png` & `toucan_connectors-4.5.1/toucan_connectors/redshift/redshift.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/redshift/redshift_database_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/redshift/redshift_database_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/redshift/utils.py` & `toucan_connectors-4.5.1/toucan_connectors/redshift/utils.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/salesforce/salesforce-service-cloud.png` & `toucan_connectors-4.5.1/toucan_connectors/salesforce/salesforce-service-cloud.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/salesforce/salesforce.jpg` & `toucan_connectors-4.5.1/toucan_connectors/salesforce/salesforce.jpg`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/salesforce/salesforce_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/salesforce/salesforce_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png` & `toucan_connectors-4.5.1/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/salesforce_sandbox/salesforce.jpg` & `toucan_connectors-4.5.1/toucan_connectors/salesforce_sandbox/salesforce.jpg`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/sap_hana/sap-hana.png` & `toucan_connectors-4.5.1/toucan_connectors/sap_hana/sap-hana.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/sap_hana/sap_hana_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/sap_hana/sap_hana_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/share_point/share_point.png` & `toucan_connectors-4.5.1/toucan_connectors/share_point/share_point.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/snowflake/snowflake.png` & `toucan_connectors-4.5.1/toucan_connectors/snowflake/snowflake.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/snowflake/snowflake_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/snowflake/snowflake_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/snowflake_common.py` & `toucan_connectors-4.5.1/toucan_connectors/snowflake_common.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/snowflake_oauth2/snowflake.png` & `toucan_connectors-4.5.1/toucan_connectors/snowflake_oauth2/snowflake.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/soap/helpers.py` & `toucan_connectors-4.5.1/toucan_connectors/soap/helpers.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/soap/soap.png` & `toucan_connectors-4.5.1/toucan_connectors/soap/soap.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/soap/soap_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/soap/soap_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/sql_query_helper.py` & `toucan_connectors-4.5.1/toucan_connectors/sql_query_helper.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/toucan_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/toucan_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/toucan_toco/toucan.png` & `toucan_connectors-4.5.1/toucan_connectors/toucan_toco/toucan.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/toucan_toco/toucan_toco_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/toucan_toco/toucan_toco_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/trello/trello.png` & `toucan_connectors-4.5.1/toucan_connectors/trello/trello.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/trello/trello_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/trello/trello_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/utils/pem.py` & `toucan_connectors-4.5.1/toucan_connectors/utils/pem.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/wootric/wootric.png` & `toucan_connectors-4.5.1/toucan_connectors/wootric/wootric.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/toucan_connectors/wootric/wootric_connector.py` & `toucan_connectors-4.5.1/toucan_connectors/wootric/wootric_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.0/PKG-INFO` & `toucan_connectors-4.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toucan-connectors
-Version: 4.5.0
+Version: 4.5.1
 Summary: Toucan Toco Connectors
 License: BSD
 Author: Toucan Toco
 Author-email: dev@toucantoco.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -43,14 +43,15 @@
 Provides-Extra: soap
 Provides-Extra: toucan-toco
 Requires-Dist: Authlib (>=1.0.1,<2.0.0)
 Requires-Dist: Jinja2 (>=3.0.3,<4.0.0)
 Requires-Dist: PyJWT (>=1.5.3,<3) ; extra == "snowflake" or extra == "all"
 Requires-Dist: PyMySQL (>=1.0.2,<2.0.0) ; extra == "google-cloud-mysql" or extra == "mysql" or extra == "all"
 Requires-Dist: adobe-analytics (>=1.2.3,<2.0.0) ; extra == "adobe" or extra == "all"
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: awswrangler (>=3.0.0,<4.0.0) ; extra == "awsathena" or extra == "all"
 Requires-Dist: bearer (==3.1.0) ; extra == "all"
 Requires-Dist: cached-property (>=1.5.2,<2.0.0)
 Requires-Dist: clickhouse-driver (>=0.2.3,<1.0) ; extra == "clickhouse" or extra == "all"
 Requires-Dist: cx-Oracle (>=8.3.0,<9.0.0) ; extra == "oracle-sql" or extra == "all"
 Requires-Dist: dataiku-api-client (>=9.0.1,<10.0.0) ; extra == "dataiku" or extra == "all"
 Requires-Dist: elasticsearch (>=7.11.0,<8) ; extra == "elasticsearch" or extra == "all"
```

