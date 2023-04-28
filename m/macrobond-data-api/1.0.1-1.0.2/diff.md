# Comparing `tmp/macrobond-data-api-1.0.1.tar.gz` & `tmp/macrobond-data-api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/macrobond-data-api/macrobond-data-api/dist/.tmp-yqj0xy6g/macrobond-data-api-1.0.1.tar", last modified: Thu Apr 27 13:38:14 2023, max compression
+gzip compressed data, was "/home/runner/work/macrobond-data-api/macrobond-data-api/dist/.tmp-e8gool95/macrobond-data-api-1.0.2.tar", last modified: Fri Apr 28 15:31:06 2023, max compression
```

## Comparing `macrobond-data-api-1.0.1.tar` & `macrobond-data-api-1.0.2.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:38:14.000000 macrobond-data-api-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-27 13:38:14.000000 macrobond-data-api-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:38:14.000000 macrobond-data-api-1.0.1/macrobond_data_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-27 13:38:13.000000 macrobond-data-api-1.0.1/macrobond_data_api/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/_generated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/_get_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:38:14.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/_com_api_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    15973 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/_com_api_revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/_com_api_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/_com_api_series.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/_error_message_to_status_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/_fill_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/_fix_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/com_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/com_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:38:14.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/com_types/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/com_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/com_types/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/com_types/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/com_types/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/com_types/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/com_types/metadata_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/com_types/search_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/com_types/search_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/com_types/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/com_types/series_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/com_types/series_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/com/com_types/series_with_revisions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:38:14.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23175 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:38:14.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/enums/calendar_date_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/enums/calendar_merge_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/enums/metadata_attribute_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/enums/series_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/enums/series_missing_value_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/enums/series_partial_periods_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/enums/series_to_higher_frequency_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/enums/series_to_lower_frequency_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/enums/series_weekdays.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/enums/status_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:38:14.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/_parse_iso8601.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/_repr_html_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/format_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/get_all_vintage_series_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/get_entity_error.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/metadata_attribute_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/metadata_value_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/revision_history_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/revision_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/search_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/search_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/search_result_long.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/series_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/series_observation_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/series_with_vintages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/start_or_end_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/unified_series.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/values_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/common/types/vintage_series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:38:14.000000 macrobond-data-api-1.0.1/macrobond_data_api/util/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/util/save_credential_to_keyring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:38:14.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/_metadata_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/_split_in_to_chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)    10015 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/_subscription_list_poller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/_web_api_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/_web_api_revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/_web_api_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/_web_api_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/_web_only_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/subscription_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:38:14.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/entity_info_for_display_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/entity_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/entity_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/feed_entities_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/http_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:38:14.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/metadata/metadata_value_information_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/metadata_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/problem_details_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/response_error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/revision_history_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:38:14.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/search/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/search/item_listing_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/search/search_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/search/search_for_display_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/search/search_for_display_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/search/search_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/search/search_request_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/search/search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/search_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/series_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/series_observation_history_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/series_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:38:14.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/series_tree/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/series_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/series_tree/series_tree_location_part.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/series_tree_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/series_with_revisions_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/series_with_times_of_change_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/series_with_vintages_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/subscription_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/subscription_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/subscription_list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/subscription_list_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/unified_series_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/unified_series_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/values_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/vintage_series_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/vintage_values_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:38:14.000000 macrobond-data-api-1.0.1/macrobond_data_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-27 13:38:13.000000 macrobond-data-api-1.0.1/macrobond_data_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-04-27 13:38:14.000000 macrobond-data-api-1.0.1/macrobond_data_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:38:14.000000 macrobond-data-api-1.0.1/macrobond_data_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 13:38:14.000000 macrobond-data-api-1.0.1/macrobond_data_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-27 13:38:14.000000 macrobond-data-api-1.0.1/macrobond_data_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-27 13:38:14.000000 macrobond-data-api-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-27 13:36:45.000000 macrobond-data-api-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/_generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/_get_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/_com_api_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15973 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/_com_api_revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/_com_api_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/_com_api_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/_error_message_to_status_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/_fill_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/_fix_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/metadata_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/search_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/search_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/series_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/series_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/series_with_revisions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23175 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/calendar_date_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/calendar_merge_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/metadata_attribute_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/series_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/series_missing_value_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/series_partial_periods_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/series_to_higher_frequency_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/series_to_lower_frequency_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/series_weekdays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/enums/status_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/_parse_iso8601.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/_repr_html_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/format_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/get_all_vintage_series_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/get_entity_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/metadata_attribute_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/metadata_value_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/revision_history_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/revision_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/search_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/search_result_long.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/series_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/series_observation_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/series_with_vintages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/start_or_end_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/unified_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/values_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/common/types/vintage_series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/util/save_credential_to_keyring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/_metadata_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/_split_in_to_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/_subscription_list_poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/_web_api_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/_web_api_revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/_web_api_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/_web_api_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/_web_only_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/subscription_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/data_pacakge_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/data_package_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/data_package_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/data_package_list_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/entity_info_for_display_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/entity_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/entity_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/feed_entities_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/http_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/metadata/metadata_value_information_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/metadata_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/problem_details_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/response_error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/revision_history_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search/item_listing_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search/search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search/search_for_display_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search/search_for_display_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search/search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search/search_request_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search/search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_observation_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_tree/series_tree_location_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_tree_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_with_revisions_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_with_times_of_change_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_with_vintages_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/unified_series_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/unified_series_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/values_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/vintage_series_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/vintage_values_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/macrobond_data_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-28 15:31:06.000000 macrobond-data-api-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-28 15:29:07.000000 macrobond-data-api-1.0.2/setup.py
```

### Comparing `macrobond-data-api-1.0.1/LICENSE` & `macrobond-data-api-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/PKG-INFO` & `macrobond-data-api-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrobond-data-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: Exposes a common API in Python for the Macrobond Web and Client Data APIs
 Home-page: https://github.com/macrobond/macrobond-data-api
 Author: Macrobond Financial
 Author-email: support@macrobond.com
 Project-URL: Documentation, https://macrobond.github.io/macrobond-data-api
 Project-URL: Source, https://github.com/macrobond/macrobond-data-api
 Project-URL: Tracker, https://github.com/macrobond/macrobond-data-api/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: macrobond-data-api Version: 1.0.1 Summary: Exposes
+Metadata-Version: 2.1 Name: macrobond-data-api Version: 1.0.2 Summary: Exposes
 a common API in Python for the Macrobond Web and Client Data APIs Home-page:
 https://github.com/macrobond/macrobond-data-api Author: Macrobond Financial
 Author-email: support@macrobond.com Project-URL: Documentation, https://
 macrobond.github.io/macrobond-data-api Project-URL: Source, https://github.com/
 macrobond/macrobond-data-api Project-URL: Tracker, https://github.com/
 macrobond/macrobond-data-api/issues Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
```

### Comparing `macrobond-data-api-1.0.1/README.md` & `macrobond-data-api-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/__init__.py` & `macrobond-data-api-1.0.2/macrobond_data_api/__init__.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/_generated.py` & `macrobond-data-api-1.0.2/macrobond_data_api/_generated.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/_get_api.py` & `macrobond-data-api-1.0.2/macrobond_data_api/_get_api.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/com/_com_api_metadata.py` & `macrobond-data-api-1.0.2/macrobond_data_api/com/_com_api_metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/com/_com_api_revision.py` & `macrobond-data-api-1.0.2/macrobond_data_api/com/_com_api_revision.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/com/_com_api_search.py` & `macrobond-data-api-1.0.2/macrobond_data_api/com/_com_api_search.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/com/_com_api_series.py` & `macrobond-data-api-1.0.2/macrobond_data_api/com/_com_api_series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/com/_fill_metadata.py` & `macrobond-data-api-1.0.2/macrobond_data_api/com/_fill_metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/com/com_api.py` & `macrobond-data-api-1.0.2/macrobond_data_api/com/com_api.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/com/com_client.py` & `macrobond-data-api-1.0.2/macrobond_data_api/com/com_client.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/com/com_types/connection.py` & `macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/connection.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/com/com_types/database.py` & `macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/database.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/com/com_types/entity.py` & `macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/entity.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/com/com_types/metadata.py` & `macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/com/com_types/metadata_information.py` & `macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/metadata_information.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/com/com_types/search_query.py` & `macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/search_query.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/com/com_types/series.py` & `macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/com/com_types/series_expression.py` & `macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/series_expression.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/com/com_types/series_request.py` & `macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/series_request.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/com/com_types/series_with_revisions.py` & `macrobond-data-api-1.0.2/macrobond_data_api/com/com_types/series_with_revisions.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/api.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/api.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/client.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/client.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/enums/__init__.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/enums/metadata_attribute_type.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/enums/metadata_attribute_type.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/enums/series_frequency.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/enums/series_frequency.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/enums/series_partial_periods_method.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/enums/series_partial_periods_method.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/enums/series_to_higher_frequency_method.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/enums/series_to_higher_frequency_method.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/enums/series_to_lower_frequency_method.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/enums/series_to_lower_frequency_method.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/enums/series_weekdays.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/enums/series_weekdays.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/types/__init__.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/types/__init__.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/types/_parse_iso8601.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/types/_parse_iso8601.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/types/_repr_html_sequence.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/types/_repr_html_sequence.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/types/entity.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/types/entity.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/types/get_all_vintage_series_result.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/types/get_all_vintage_series_result.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/types/get_entity_error.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/types/get_entity_error.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/types/metadata_attribute_information.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/types/metadata_attribute_information.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/types/metadata_value_information.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/types/metadata_value_information.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/types/revision_history_request.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/types/revision_history_request.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/types/revision_info.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/types/revision_info.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/types/search_filter.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/types/search_filter.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/types/search_result.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/types/search_result.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/types/search_result_long.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/types/search_result_long.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/types/series.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/types/series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/types/series_entry.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/types/series_entry.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/types/series_observation_history.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/types/series_observation_history.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/types/series_with_vintages.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/types/series_with_vintages.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/types/start_or_end_point.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/types/start_or_end_point.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/types/unified_series.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/types/unified_series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/common/types/vintage_series.py` & `macrobond-data-api-1.0.2/macrobond_data_api/common/types/vintage_series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/util/save_credential_to_keyring.py` & `macrobond-data-api-1.0.2/macrobond_data_api/util/save_credential_to_keyring.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         old_credential = keyring.get_credential(service_name, username)
     return True
 
 
 def _test_keyring_backend() -> bool:
     try:
         keyring_backend = keyring.get_keyring()
-    except Exception:  # pylint: disable=broad-exception-caught
+    except Exception:  # pylint: disable=W0703
         print(traceback.format_exc())
         print("Error: failed to get keyring")
         return False
 
     if isinstance(keyring_backend, null_keyring_backend):
         print("Error: keyring_backend is null_keyring_backend")
         return False
@@ -137,29 +137,29 @@
     username = input("Please enter Macrobond Web Api username: ")
     password = getpass("Please enter Macrobond Web Api password: ")
 
     print("Testing username and password")
     try:
         with WebClient(username=username, password=password) as api:
             api.metadata_get_attribute_information("PrimName")
-    except Exception:  # pylint: disable=broad-exception-caught
+    except Exception:  # pylint: disable=W0703
         print(traceback.format_exc())
         print("Error: failed testing username and password")
         return False
 
     if is_darwin:
         keyring.set_password(service_name, DARWIN_USERNAME, json.dumps({"username": username, "password": password}))
     else:
         keyring.set_password(service_name, username, password)
 
     print("Testing keyring")
     try:
         with WebClient() as api:
             api.metadata_get_attribute_information("PrimName")
-    except Exception:  # pylint: disable=broad-exception-caught
+    except Exception:  # pylint: disable=W0703
         print(traceback.format_exc())
         print("Error: failed testing keyring")
         return False
 
     print(f'Successfully saved to the keyring with the service name: "{ service_name }" in {keyring_name}')
 
     return True
```

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/_metadata.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/_metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/_metadata_directory.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/_metadata_directory.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/_subscription_list_poller.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/_subscription_list_poller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from abc import ABC, abstractmethod
 from datetime import datetime, timezone
 
 import time
 from typing import List, Optional, cast, TYPE_CHECKING, Callable
 
 from macrobond_data_api.web import WebApi
-from .web_types.subscription_list_state import SubscriptionListState
+from .web_types.data_package_list_state import DataPackageListState
 
 if TYPE_CHECKING:  # pragma: no cover
-    from .web_types import SubscriptionBody, SubscriptionListItem
+    from .web_types import DataPackageBody, DataPackageListItem
 
 
 class _AbortException(Exception):
     ...
 
 
-class _SubscriptionListPoller(ABC):
+class _DataPackageListPoller(ABC):
     """
     This is work in progress and might change soon.
-    Run a loop polling for changed series in the subscription list.
+    Run a loop polling for changed series in the data package list.
     Derive from this class and override `on_full_listing_start`, `on_full_listing_items`, `on_full_listing_stop`,
     `on_incremental_start`, `on_incremental_items` and `on_incremental_stop`.
 
     Parameters
     ----------
     api : WebApi
         The API instance to use.
@@ -89,25 +89,25 @@
                     self._time_stamp_for_if_modified_since = sub.time_stamp_for_if_modified_since
 
             if self._abort:
                 return
 
             self._sleep(self.up_to_date_delay)
 
-    def _run_full_listing(self, max_attempts: int = 3) -> Optional["SubscriptionBody"]:
+    def _run_full_listing(self, max_attempts: int = 3) -> Optional["DataPackageBody"]:
         is_stated = False
 
-        def _body_callback(body: "SubscriptionBody") -> None:
+        def _body_callback(body: "DataPackageBody") -> None:
             is_stated = True  # pylint: disable=unused-variable
             self.on_full_listing_start(body)
 
         try:
             for attempt in range(1, max_attempts):
                 try:
-                    sub = self._api.get_subscription_list_iterative(
+                    sub = self._api.get_data_package_list_iterative(
                         _body_callback,
                         self.on_full_listing_items,
                         None,
                     )
                     if not sub:
                         raise ValueError("subscription is None")
 
@@ -123,25 +123,25 @@
             if is_stated:
                 self.on_full_listing_stop(True, cast(Exception, ex.__cause__))
         except Exception as ex:  # pylint: disable=broad-except
             if is_stated:
                 self.on_full_listing_stop(False, ex)
         return None
 
-    def _run_listing(self, if_modified_since: datetime, max_attempts: int = 3) -> Optional["SubscriptionBody"]:
+    def _run_listing(self, if_modified_since: datetime, max_attempts: int = 3) -> Optional["DataPackageBody"]:
         is_stated = False
 
-        def _body_callback(body: "SubscriptionBody") -> None:
+        def _body_callback(body: "DataPackageBody") -> None:
             is_stated = True  # pylint: disable=unused-variable
             self.on_incremental_start(body)
 
         try:
             for attempt in range(1, max_attempts):
                 try:
-                    sub = self._api.get_subscription_list_iterative(
+                    sub = self._api.get_data_package_list_iterative(
                         _body_callback,
                         self.on_incremental_items,
                         if_modified_since,
                     )
                     break
                 except Exception as ex:  # pylint: disable=broad-except
                     if self._abort:
@@ -149,15 +149,15 @@
                     if attempt > max_attempts:
                         raise
                     self._sleep(self.on_error_delay)
 
             if not sub:
                 raise ValueError("subscription is None")
 
-            if sub.state == SubscriptionListState.UP_TO_DATE:
+            if sub.state == DataPackageListState.UP_TO_DATE:
                 self.on_incremental_stop(False, None)
                 return sub
 
             self._sleep(self.incomplete_delay)
 
             return self._run_listing_incomplete(sub.time_stamp_for_if_modified_since, is_stated, max_attempts)
         except _AbortException as ex:
@@ -166,29 +166,29 @@
         except Exception as ex:  # pylint: disable=broad-except
             if is_stated:
                 self.on_incremental_stop(False, ex)
         return None
 
     def _run_listing_incomplete(
         self, if_modified_since: datetime, is_stated: bool, max_attempts: int = 3
-    ) -> Optional["SubscriptionBody"]:
+    ) -> Optional["DataPackageBody"]:
         try:
             while True:
                 for attempt in range(1, max_attempts):
                     try:
-                        sub = self._api.get_subscription_list_iterative(
+                        sub = self._api.get_data_package_list_iterative(
                             lambda _: None,
                             self.on_incremental_items,
                             if_modified_since,
                         )
 
                         if not sub:
                             raise ValueError("subscription is None")
 
-                        if sub.state == SubscriptionListState.UP_TO_DATE:
+                        if sub.state == DataPackageListState.UP_TO_DATE:
                             self.on_incremental_stop(False, None)
                             return sub
 
                         self._sleep(self.incomplete_delay)
 
                         if_modified_since = sub.time_stamp_for_if_modified_since
                     except Exception as ex2:  # pylint: disable=broad-except
@@ -204,19 +204,19 @@
             if is_stated:
                 self.on_incremental_stop(False, ex)
         return None
 
     # full_listing
 
     @abstractmethod
-    def on_full_listing_start(self, subscription: "SubscriptionBody") -> None:
+    def on_full_listing_start(self, subscription: "DataPackageBody") -> None:
         """This override is called when a full listing starts."""
 
     @abstractmethod
-    def on_full_listing_items(self, subscription: "SubscriptionBody", items: List["SubscriptionListItem"]) -> None:
+    def on_full_listing_items(self, subscription: "DataPackageBody", items: List["DataPackageListItem"]) -> None:
         """This override is called repeatedly with one or more items until all items are listed."""
 
     @abstractmethod
     def on_full_listing_stop(self, is_aborted: bool, exception: Optional[Exception]) -> None:
         """
         This override is called when the full listing is stopped.
         Parameters
@@ -226,19 +226,19 @@
         exception : Optional[Exception]
             If not None, there was an exception.
         """
 
     # listing
 
     @abstractmethod
-    def on_incremental_start(self, subscription: "SubscriptionBody") -> None:
+    def on_incremental_start(self, subscription: "DataPackageBody") -> None:
         """This override is called when an incremental listing starts."""
 
     @abstractmethod
-    def on_incremental_items(self, subscription: "SubscriptionBody", items: List["SubscriptionListItem"]) -> None:
+    def on_incremental_items(self, subscription: "DataPackageBody", items: List["DataPackageListItem"]) -> None:
         """This override is called repeatedly with one or more items until all updated items are listed."""
 
     @abstractmethod
     def on_incremental_stop(self, is_aborted: bool, exception: Optional[Exception]) -> None:
         """
         This override is called when the incremental listing is stopped.
         Parameters
```

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/_web_api_metadata.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/_web_api_metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/_web_api_revision.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/_web_api_revision.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         metadata = session._create_metadata(response["metadata"])
         if include_times_of_change:
             timesOfChange = response.get("timesOfChange")
             if not timesOfChange or (len(values) != 0 and _optional_str_to_datetime(timesOfChange[0]) is None):
                 values_metadata: Optional[ValuesMetadata] = [{}] * len(values)
             else:
                 values_metadata = [
-                    {"RevisionTimeStamp": _optional_str_to_datetime(x)} for x in cast(List[str], timesOfChange)
+                    {"RevisionTimeStamp": _parse_iso8601(x)} if x else {} for x in cast(List[str], timesOfChange)
                 ]
         else:
             values_metadata = None
 
         return Series(name, "", StatusCode.OK, cast(Dict[str, Any], metadata), values_metadata, values, dates)
 
     if len(series_names) == 0:
```

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/_web_api_search.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/_web_api_search.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/_web_api_series.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/_web_api_series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/_web_only_api.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/_web_only_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from typing import TYPE_CHECKING, Any, List, Optional, Callable, Tuple
 
 import ijson  # type: ignore
 
 from macrobond_data_api.common.types import SearchResultLong
 from macrobond_data_api.common.types._parse_iso8601 import _parse_iso8601
 
-from .web_types.subscription_list_state import SubscriptionListState
-from .web_types.subscription_list_item import SubscriptionListItem
-from .web_types.subscription_list import SubscriptionList as OldSubscriptionList
-from .web_types.subscription_body import SubscriptionBody
+from .web_types.data_package_list_state import DataPackageListState
+from .web_types.data_pacakge_list_item import DataPackageListItem
+from .web_types.data_package_list import DataPackageList
+from .web_types.data_package_body import DataPackageBody
 
 from .session import _raise_on_error
 from .subscription_list import SubscriptionList
 
 if TYPE_CHECKING:  # pragma: no cover
     from macrobond_data_api.common.types import SearchFilter
 
@@ -22,57 +22,57 @@
 
 
 __pdoc__ = {
     "WebApi.__init__": False,
 }
 
 
-def _get_subscription_list_iterative_pars_body(
+def _get_data_package_list_iterative_pars_body(
     ijson_parse: Any,
-) -> Tuple[Optional[datetime], Optional[datetime], Optional[SubscriptionListState]]:
+) -> Tuple[Optional[datetime], Optional[datetime], Optional[DataPackageListState]]:
     time_stamp_for_if_modified_since: Optional[datetime] = None
     download_full_list_on_or_after: Optional[datetime] = None
-    state: Optional[SubscriptionListState] = None
+    state: Optional[DataPackageListState] = None
     for prefix, event, value in ijson_parse:
         if prefix == "timeStampForIfModifiedSince":
             if event != "string":
                 raise Exception("bad format: timeStampForIfModifiedSince is not a string")
             time_stamp_for_if_modified_since = _parse_iso8601(value)
         elif prefix == "downloadFullListOnOrAfter":
             if event != "string":
                 raise Exception("bad format: downloadFullListOnOrAfter is not a string")
             download_full_list_on_or_after = _parse_iso8601(value)
         elif prefix == "state":
             if event != "number":
                 raise Exception("bad format: state is not a number")
-            state = SubscriptionListState(value)
+            state = DataPackageListState(value)
         elif event == "start_array":
             if prefix != "entities":
                 raise Exception("bad format: event start_array do not have a prefix of entities")
             break
     return time_stamp_for_if_modified_since, download_full_list_on_or_after, state
 
 
-def _get_subscription_list_iterative_pars_items(
+def _get_data_package_list_iterative_pars_items(
     ijson_parse: Any,
-    items_callback: Callable[[SubscriptionBody, List[SubscriptionListItem]], Optional[bool]],
+    items_callback: Callable[[DataPackageBody, List[DataPackageListItem]], Optional[bool]],
     buffer_size: int,
-    body: SubscriptionBody,
+    body: DataPackageBody,
 ) -> bool:
     name = ""
     modified: Optional[datetime] = None
-    items: List[SubscriptionListItem] = []
+    items: List[DataPackageListItem] = []
 
     for prefix, event, value in ijson_parse:
         if event == "end_map":
             if name == "":
                 raise Exception("bad format: name was not found")
             if modified is None:
                 raise Exception("bad format: modified was not found")
-            items.append(SubscriptionListItem(name, modified))
+            items.append(DataPackageListItem(name, modified))
             name = ""
             modified = None
             if len(items) == buffer_size:
                 if items_callback(body, items) is False:
                     return False
                 items = []
         elif event == "end_array":
@@ -87,19 +87,19 @@
             modified = _parse_iso8601(value)
 
     if len(items) != 0:
         return items_callback(body, items) is not False
     return True
 
 
-def get_subscription_list(self: "WebApi", if_modified_since: datetime = None) -> OldSubscriptionList:
+def get_data_package_list(self: "WebApi", if_modified_since: datetime = None) -> DataPackageList:
     # pylint: disable=line-too-long
     """
-    Get the items in the subscription list.
-    .. Important:: For large lists you might want to use `macrobond_data_api.web.web_api.WebApi.get_subscription_list_iterative`.
+    Get the items in the data package.
+    .. Important:: For large lists you might want to use `macrobond_data_api.web.web_api.WebApi.get_datapackage_list_iterative`.
 
     Typically you want to pass the date of time_stamp_for_if_modified_since from response of the previous call
     to get incremental updates.
 
     Parameters
     ----------
     if_modified_since : datetime
@@ -107,84 +107,84 @@
         If not specified, all items will be returned.
 
     Returns
     -------
     `macrobond_data_api.web.web_types.subscription_list.SubscriptionList`
     """
     # pylint: enable=line-too-long
-    return OldSubscriptionList(self.session.series.get_subscription_list(if_modified_since))
+    return DataPackageList(self.session.series.get_data_package_list(if_modified_since))
 
 
 # TODO: @mb-jp ree add cooment to get_subscription_list_iterative , when SubscriptionListPoller is done
 # .. Note:: For for continous polling you might
 # want to use `macrobond_data_api.web.subscription_list_poller.SubscriptionListPoller`.
 
 
-def get_subscription_list_iterative(
+def get_data_package_list_iterative(
     self: "WebApi",
-    body_callback: Callable[[SubscriptionBody], Optional[bool]],
-    items_callback: Callable[[SubscriptionBody, List[SubscriptionListItem]], Optional[bool]],
+    body_callback: Callable[[DataPackageBody], Optional[bool]],
+    items_callback: Callable[[DataPackageBody, List[DataPackageListItem]], Optional[bool]],
     if_modified_since: datetime = None,
     buffer_size: int = 200,
-) -> Optional[SubscriptionBody]:
+) -> Optional[DataPackageBody]:
     # pylint: disable=line-too-long
     """
-    Process the subscription list in batches.
+    Process the data package list in batches.
     This is more efficient since the complete list does not have to be in memory.
 
     Typically you want to pass the date of time_stamp_for_if_modified_since from response of the previous call
     to get incremental updates.
 
     Parameters
     ----------
-    body_callback : `Callable[[macrobond_data_api.web.web_types.subscription_body.SubscriptionBody], Optional[bool]]`
+    body_callback : `Callable[[macrobond_data_api.web.web_types.data_package_body.DataPackageBody], Optional[bool]]`
         The callback for the body. This call comes first. Return True to continue processing.
 
-    items_callback : Callable[[macrobond_data_api.web.web_types.subscription_body.SubscriptionBody, List[macrobond_data_api.web.web_types.subscription_list_item.SubscriptionListItem]], Optional[bool]]
+    items_callback : Callable[[macrobond_data_api.web.web_types.data_package_body.DataPackageBody, List[macrobond_data_api.web.web_types.data_package_list_item.DataPackageListItem]], Optional[bool]]
         The callback for each batch of items. Return True to continue processing.
 
     if_modified_since : datetime
         The timestamp of the property time_stamp_for_if_modified_since from the response of the previous call.
         If not specified, all items will be returned.
 
     buffer_size : int
         The maximum number of items to include in each callback
     Returns
     -------
-    `macrobond_data_api.web.web_types.subscription_body.SubscriptionBody`
+    `macrobond_data_api.web.web_types.data_package_body.DataPackageBody`
     """
     # pylint: enable=line-too-long
     params = {}
-    body: Optional[SubscriptionBody] = None
+    body: Optional[DataPackageBody] = None
 
     if if_modified_since:
         params["ifModifiedSince"] = if_modified_since.isoformat()
 
     with self._session.get("v1/series/getsubscriptionlist", params=params, stream=True) as response:
         _raise_on_error(response)
         ijson_parse = ijson.parse(response.raw)
 
         (
             time_stamp_for_if_modified_since,
             download_full_list_on_or_after,
             state,
-        ) = _get_subscription_list_iterative_pars_body(ijson_parse)
+        ) = _get_data_package_list_iterative_pars_body(ijson_parse)
 
         if state is None:
             raise Exception("bad format: state was not found")
         if time_stamp_for_if_modified_since is None:
             raise Exception("bad format: timeStampForIfModifiedSince was not found")
         if not if_modified_since and download_full_list_on_or_after is None:
             raise Exception("bad format: downloadFullListOnOrAfter was not found")
 
-        body = SubscriptionBody(time_stamp_for_if_modified_since, download_full_list_on_or_after, state)
+        body = DataPackageBody(time_stamp_for_if_modified_since, download_full_list_on_or_after, state)
         if body_callback(body) is False:
             return None
 
-        if _get_subscription_list_iterative_pars_items(ijson_parse, items_callback, buffer_size, body) is False:
+        if _get_data_package_list_iterative_pars_items(ijson_parse, items_callback, buffer_size, body) is False:
             return None
 
         return body
 
 
 # Search
```

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/session.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/session.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/subscription_list.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/subscription_list.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_api.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from macrobond_data_api.common import Api
 
 from ._web_only_api import (
     entity_search_multi_filter_long,
-    get_subscription_list,
-    get_subscription_list_iterative,
+    get_data_package_list,
+    get_data_package_list_iterative,
     subscription_list,
 )
 from ._web_api_metadata import metadata_list_values, metadata_get_attribute_information, metadata_get_value_information
 
 from ._web_api_revision import (
     get_all_vintage_series,
     get_one_nth_release,
@@ -63,16 +63,16 @@
     get_nth_release = get_nth_release
     get_all_vintage_series = get_all_vintage_series
     get_observation_history = get_observation_history
     get_many_series_with_revisions = get_many_series_with_revisions
 
     # web only
 
-    get_subscription_list = get_subscription_list
-    get_subscription_list_iterative = get_subscription_list_iterative
+    get_data_package_list = get_data_package_list
+    get_data_package_list_iterative = get_data_package_list_iterative
     entity_search_multi_filter_long = entity_search_multi_filter_long
     subscription_list = subscription_list
 
     # Search
 
     entity_search_multi_filter = entity_search_multi_filter
```

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_client.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_client.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/__init__.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,12 +43,12 @@
 
 from .revision_history_request import RevisionHistoryRequest
 
 from .series_with_vintages_response import SeriesWithVintagesResponse
 
 from .vintage_values_response import VintageValuesResponse
 
-from .subscription_list_state import SubscriptionListState
+from .data_package_list_state import DataPackageListState
 
-from .subscription_list_item import SubscriptionListItem
+from .data_pacakge_list_item import DataPackageListItem
 
-from .subscription_body import SubscriptionBody
+from .data_package_body import DataPackageBody
```

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/entity_info_for_display_response.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/entity_info_for_display_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/feed_entities_response.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/feed_entities_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/http_exception.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/http_exception.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/metadata_methods.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/metadata_methods.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/problem_details_exception.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/problem_details_exception.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/response_error_code.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/response_error_code.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/revision_history_request.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/revision_history_request.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/search/item_listing_response.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search/item_listing_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/search/search_filter.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search/search_filter.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/search_methods.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/search_methods.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/series_methods.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,15 +259,15 @@
                 "n": series_name,
                 "t": [x.isoformat() for x in date_of_the_observation],
             },
         )
         return cast(List["SeriesObservationHistoryResponse"], response.json())
 
     # Get /v1/series/getsubscriptionlist
-    def get_subscription_list(self, if_modified_since: datetime = None) -> "FeedEntitiesResponse":
+    def get_data_package_list(self, if_modified_since: datetime = None) -> "FeedEntitiesResponse":
         """
         Get a list of entities in the subscription list and timestamps when they were last changed.
         You can specify a timestamp to see what has changed since then. For this the
         timeStampForIfModifiedSince in the response from a previous call is typically used.
         This guarantees that you will not miss any updates,
         but you may see the same update more than once.
```

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/series_observation_history_response.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_observation_history_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/series_tree_methods.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_tree_methods.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/series_with_revisions_info_response.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_with_revisions_info_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/series_with_vintages_response.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/series_with_vintages_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/status_response.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/status_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/subscription_body.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/data_package_body.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from dataclasses import dataclass
 
 from typing import Optional
 
 from datetime import datetime
 
-from .subscription_list_state import SubscriptionListState
+from .data_package_list_state import DataPackageListState
 
 
 @dataclass(init=False)
-class SubscriptionBody:
+class DataPackageBody:
     __slots__ = ("time_stamp_for_if_modified_since", "download_full_list_on_or_after", "state")
 
     time_stamp_for_if_modified_since: datetime
     download_full_list_on_or_after: Optional[datetime]
-    state: SubscriptionListState
+    state: DataPackageListState
 
     def __init__(
         self,
         time_stamp_for_if_modified_since: datetime,
         download_full_list_on_or_after: Optional[datetime],
-        state: SubscriptionListState,
+        state: DataPackageListState,
     ) -> None:
         self.time_stamp_for_if_modified_since = time_stamp_for_if_modified_since
         """
         A timestamp to pass as the ifModifiedSince parameter
         in the next request to get incremental updates.
         """
         self.download_full_list_on_or_after = download_full_list_on_or_after
```

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/subscription_list_state.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/data_package_list_state.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pylint: disable=invalid-name , missing-module-docstring
 
 from enum import IntEnum
 
 
-class SubscriptionListState(IntEnum):
+class DataPackageListState(IntEnum):
     """The statate of the subscription list."""
 
     FULL_LISTING = 0
     """
     A complete listing of all series. 
     Make another request for full data at some point after timestamp in downloadFullListOnOrAfter.
     """
@@ -22,19 +22,18 @@
     """
     The list might not contain all updates.
     Wait one minute and then use the timeStampForIfModifiedSince in an a new request.
     """
 
     def __repr__(self) -> str:
         if self == self.FULL_LISTING:
-            return f"SubscriptionList State {int(self)}, A complete listing of all series."
+            return f"DataPacakgeList State {int(self)}, A complete listing of all series."
 
         if self == self.UP_TO_DATE:
             return (
-                f"SubscriptionList State {int(self)},"
-                + " The list contains all updates since the specified start date."
+                f"DataPacakgeList State {int(self)}," + " The list contains all updates since the specified start date."
             )
 
         if self == self.INCOMPLETE:
-            return f"SubscriptionList State {int(self)}, The list might not contain all updates."
+            return f"DataPacakgeList State {int(self)}, The list might not contain all updates."
 
-        return f"SubscriptionList State {int(self)}"
+        return f"DataPacakgeList State {int(self)}"
```

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api/web/web_types/unified_series_request.py` & `macrobond-data-api-1.0.2/macrobond_data_api/web/web_types/unified_series_request.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api.egg-info/PKG-INFO` & `macrobond-data-api-1.0.2/macrobond_data_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrobond-data-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: Exposes a common API in Python for the Macrobond Web and Client Data APIs
 Home-page: https://github.com/macrobond/macrobond-data-api
 Author: Macrobond Financial
 Author-email: support@macrobond.com
 Project-URL: Documentation, https://macrobond.github.io/macrobond-data-api
 Project-URL: Source, https://github.com/macrobond/macrobond-data-api
 Project-URL: Tracker, https://github.com/macrobond/macrobond-data-api/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: macrobond-data-api Version: 1.0.1 Summary: Exposes
+Metadata-Version: 2.1 Name: macrobond-data-api Version: 1.0.2 Summary: Exposes
 a common API in Python for the Macrobond Web and Client Data APIs Home-page:
 https://github.com/macrobond/macrobond-data-api Author: Macrobond Financial
 Author-email: support@macrobond.com Project-URL: Documentation, https://
 macrobond.github.io/macrobond-data-api Project-URL: Source, https://github.com/
 macrobond/macrobond-data-api Project-URL: Tracker, https://github.com/
 macrobond/macrobond-data-api/issues Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
```

### Comparing `macrobond-data-api-1.0.1/macrobond_data_api.egg-info/SOURCES.txt` & `macrobond-data-api-1.0.2/macrobond_data_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,18 @@
 macrobond_data_api/web/_web_only_api.py
 macrobond_data_api/web/scope.py
 macrobond_data_api/web/session.py
 macrobond_data_api/web/subscription_list.py
 macrobond_data_api/web/web_api.py
 macrobond_data_api/web/web_client.py
 macrobond_data_api/web/web_types/__init__.py
+macrobond_data_api/web/web_types/data_pacakge_list_item.py
+macrobond_data_api/web/web_types/data_package_body.py
+macrobond_data_api/web/web_types/data_package_list.py
+macrobond_data_api/web/web_types/data_package_list_state.py
 macrobond_data_api/web/web_types/entity_info_for_display_response.py
 macrobond_data_api/web/web_types/entity_request.py
 macrobond_data_api/web/web_types/entity_response.py
 macrobond_data_api/web/web_types/feed_entities_response.py
 macrobond_data_api/web/web_types/http_exception.py
 macrobond_data_api/web/web_types/metadata_methods.py
 macrobond_data_api/web/web_types/problem_details_exception.py
@@ -103,18 +107,14 @@
 macrobond_data_api/web/web_types/series_observation_history_response.py
 macrobond_data_api/web/web_types/series_response.py
 macrobond_data_api/web/web_types/series_tree_methods.py
 macrobond_data_api/web/web_types/series_with_revisions_info_response.py
 macrobond_data_api/web/web_types/series_with_times_of_change_response.py
 macrobond_data_api/web/web_types/series_with_vintages_response.py
 macrobond_data_api/web/web_types/status_response.py
-macrobond_data_api/web/web_types/subscription_body.py
-macrobond_data_api/web/web_types/subscription_list.py
-macrobond_data_api/web/web_types/subscription_list_item.py
-macrobond_data_api/web/web_types/subscription_list_state.py
 macrobond_data_api/web/web_types/unified_series_request.py
 macrobond_data_api/web/web_types/unified_series_response.py
 macrobond_data_api/web/web_types/values_response.py
 macrobond_data_api/web/web_types/vintage_series_response.py
 macrobond_data_api/web/web_types/vintage_values_response.py
 macrobond_data_api/web/web_types/metadata/__init__.py
 macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py
```

### Comparing `macrobond-data-api-1.0.1/setup.cfg` & `macrobond-data-api-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.1/setup.py` & `macrobond-data-api-1.0.2/setup.py`

 * *Files identical despite different names*

