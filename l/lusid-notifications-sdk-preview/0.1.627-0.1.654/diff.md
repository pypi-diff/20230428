# Comparing `tmp/lusid-notifications-sdk-preview-0.1.627.tar.gz` & `tmp/lusid-notifications-sdk-preview-0.1.654.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-notifications-sdk-preview-0.1.627.tar", last modified: Wed Apr  5 13:20:49 2023, max compression
+gzip compressed data, was "dist/lusid-notifications-sdk-preview-0.1.654.tar", last modified: Fri Apr 28 13:59:12 2023, max compression
```

## Comparing `lusid-notifications-sdk-preview-0.1.627.tar` & `lusid-notifications-sdk-preview-0.1.654.tar`

### file list

```diff
@@ -1,65 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:20:49.000000 lusid-notifications-sdk-preview-0.1.627/
--rw-r--r--   0 root         (0) root         (0)       54 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      373 2023-04-05 13:20:49.000000 lusid-notifications-sdk-preview-0.1.627/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8970 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:20:49.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/
--rw-r--r--   0 root         (0) root         (0)     4243 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:20:49.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/api/
--rw-r--r--   0 root         (0) root         (0)      501 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6851 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    10524 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/api/deliveries_api.py
--rw-r--r--   0 root         (0) root         (0)    13990 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/api/event_types_api.py
--rw-r--r--   0 root         (0) root         (0)     6975 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/api/events_api.py
--rw-r--r--   0 root         (0) root         (0)   101406 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/api/notifications_api.py
--rw-r--r--   0 root         (0) root         (0)    47907 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/api/subscriptions_api.py
--rw-r--r--   0 root         (0) root         (0)    27436 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16635 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5099 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:20:49.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/
--rw-r--r--   0 root         (0) root         (0)     2889 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7264 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     9027 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7232 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)     6512 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/attempt.py
--rw-r--r--   0 root         (0) root         (0)     5557 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/attempt_status.py
--rw-r--r--   0 root         (0) root         (0)    16290 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/create_email_notification.py
--rw-r--r--   0 root         (0) root         (0)     8814 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/create_sms_notification.py
--rw-r--r--   0 root         (0) root         (0)    10822 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/create_subscription.py
--rw-r--r--   0 root         (0) root         (0)    16161 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/create_webhook_notification.py
--rw-r--r--   0 root         (0) root         (0)    12397 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/delivery.py
--rw-r--r--   0 root         (0) root         (0)     4091 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/event_details.py
--rw-r--r--   0 root         (0) root         (0)     8514 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     8025 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9514 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     6426 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9540 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10705 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     7344 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)    18059 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/notification.py
--rw-r--r--   0 root         (0) root         (0)     5155 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/notification_status.py
--rw-r--r--   0 root         (0) root         (0)     6099 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7775 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7327 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/resource_list_of_delivery.py
--rw-r--r--   0 root         (0) root         (0)     7523 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/resource_list_of_event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     7439 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/resource_list_of_notification.py
--rw-r--r--   0 root         (0) root         (0)     7439 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/resource_list_of_subscription.py
--rw-r--r--   0 root         (0) root         (0)    14416 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/subscription.py
--rw-r--r--   0 root         (0) root         (0)    15824 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/subscription_detail.py
--rw-r--r--   0 root         (0) root         (0)    16290 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/update_email_notification.py
--rw-r--r--   0 root         (0) root         (0)     8814 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/update_sms_notification.py
--rw-r--r--   0 root         (0) root         (0)     9939 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/update_subscription.py
--rw-r--r--   0 root         (0) root         (0)    16161 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/update_webhook_notification.py
--rw-r--r--   0 root         (0) root         (0)    13561 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:20:49.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/utilities/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:20:49.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      373 2023-04-05 13:20:49.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2626 2023-04-05 13:20:49.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 13:20:49.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-04-05 13:20:49.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-05 13:20:49.000000 lusid-notifications-sdk-preview-0.1.627/lusid_notifications_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-05 13:20:49.000000 lusid-notifications-sdk-preview-0.1.627/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2322 2023-04-05 13:20:20.000000 lusid-notifications-sdk-preview-0.1.627/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:59:12.000000 lusid-notifications-sdk-preview-0.1.654/
+-rw-r--r--   0 root         (0) root         (0)       54 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      373 2023-04-28 13:59:12.000000 lusid-notifications-sdk-preview-0.1.654/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9642 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:59:12.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/
+-rw-r--r--   0 root         (0) root         (0)     4427 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:59:12.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/api/
+-rw-r--r--   0 root         (0) root         (0)      501 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6851 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    10524 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/api/deliveries_api.py
+-rw-r--r--   0 root         (0) root         (0)    13990 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/api/event_types_api.py
+-rw-r--r--   0 root         (0) root         (0)     6975 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/api/events_api.py
+-rw-r--r--   0 root         (0) root         (0)   124757 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/api/notifications_api.py
+-rw-r--r--   0 root         (0) root         (0)    47907 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/api/subscriptions_api.py
+-rw-r--r--   0 root         (0) root         (0)    27436 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16635 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:59:12.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/
+-rw-r--r--   0 root         (0) root         (0)     3073 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7264 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     9027 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7232 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)     6512 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/attempt.py
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/attempt_status.py
+-rw-r--r--   0 root         (0) root         (0)    11703 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/create_aws_sqs_notification.py
+-rw-r--r--   0 root         (0) root         (0)    16290 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/create_email_notification.py
+-rw-r--r--   0 root         (0) root         (0)     8814 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/create_sms_notification.py
+-rw-r--r--   0 root         (0) root         (0)    10822 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/create_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    16161 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/create_webhook_notification.py
+-rw-r--r--   0 root         (0) root         (0)    12397 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/delivery.py
+-rw-r--r--   0 root         (0) root         (0)     4091 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/event_details.py
+-rw-r--r--   0 root         (0) root         (0)     8514 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     8025 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9514 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     6426 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9540 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10705 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     7344 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    18059 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/notification.py
+-rw-r--r--   0 root         (0) root         (0)     5155 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/notification_status.py
+-rw-r--r--   0 root         (0) root         (0)     6099 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7775 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7327 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/resource_list_of_delivery.py
+-rw-r--r--   0 root         (0) root         (0)     7523 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/resource_list_of_event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     7439 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/resource_list_of_notification.py
+-rw-r--r--   0 root         (0) root         (0)     7439 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/resource_list_of_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    14416 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/subscription.py
+-rw-r--r--   0 root         (0) root         (0)    15824 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/subscription_detail.py
+-rw-r--r--   0 root         (0) root         (0)    11703 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/update_aws_sqs_notification.py
+-rw-r--r--   0 root         (0) root         (0)    16290 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/update_email_notification.py
+-rw-r--r--   0 root         (0) root         (0)     8814 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/update_sms_notification.py
+-rw-r--r--   0 root         (0) root         (0)     9939 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/update_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    16161 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/update_webhook_notification.py
+-rw-r--r--   0 root         (0) root         (0)    13561 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:59:12.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/utilities/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:59:12.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      373 2023-04-28 13:59:12.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2742 2023-04-28 13:59:12.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 13:59:12.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-04-28 13:59:12.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-28 13:59:12.000000 lusid-notifications-sdk-preview-0.1.654/lusid_notifications_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 13:59:12.000000 lusid-notifications-sdk-preview-0.1.654/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2322 2023-04-28 13:57:09.000000 lusid-notifications-sdk-preview-0.1.654/setup.py
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/README.md` & `lusid-notifications-sdk-preview-0.1.654/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-notifications-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.627
-- Package version: 0.1.627
+- API version: 0.1.654
+- Package version: 0.1.654
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -92,20 +92,22 @@
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *ApplicationMetadataApi* | [**list_access_controlled_resources**](docs/ApplicationMetadataApi.md#list_access_controlled_resources) | **GET** /api/metadata/access/resources | [EARLY ACCESS] ListAccessControlledResources: Get resources available for access control
 *DeliveriesApi* | [**list_deliveries**](docs/DeliveriesApi.md#list_deliveries) | **GET** /api/deliveries | [EXPERIMENTAL] ListDeliveries: List Deliveries
 *EventTypesApi* | [**get_event_type**](docs/EventTypesApi.md#get_event_type) | **GET** /api/eventtypes/{eventType} | [EXPERIMENTAL] GetEventType: Gets the specified event type schema.
 *EventTypesApi* | [**list_event_types**](docs/EventTypesApi.md#list_event_types) | **GET** /api/eventtypes | [EXPERIMENTAL] ListEventTypes: Lists all of the available event types.
 *EventsApi* | [**create_event**](docs/EventsApi.md#create_event) | **POST** /api/events | [EXPERIMENTAL] CreateEvent: Create a new event.
+*NotificationsApi* | [**create_aws_sqs_notification**](docs/NotificationsApi.md#create_aws_sqs_notification) | **POST** /api/subscriptions/{scope}/{code}/notifications/awssqs | [EXPERIMENTAL] CreateAwsSqsNotification: Add an AWS SQS notification to a subscription.
 *NotificationsApi* | [**create_email_notification**](docs/NotificationsApi.md#create_email_notification) | **POST** /api/subscriptions/{scope}/{code}/notifications/email | [EXPERIMENTAL] CreateEmailNotification: Add an email notification to a subscription.
 *NotificationsApi* | [**create_sms_notification**](docs/NotificationsApi.md#create_sms_notification) | **POST** /api/subscriptions/{scope}/{code}/notifications/sms | [EXPERIMENTAL] CreateSmsNotification: Add an SMS notification to a subscription.
 *NotificationsApi* | [**create_webhook_notification**](docs/NotificationsApi.md#create_webhook_notification) | **POST** /api/subscriptions/{scope}/{code}/notifications/webhook | [EXPERIMENTAL] CreateWebhookNotification: Add a Webhook notification to a subscription.
 *NotificationsApi* | [**delete_notification**](docs/NotificationsApi.md#delete_notification) | **DELETE** /api/subscriptions/{scope}/{code}/notifications/{id} | [EXPERIMENTAL] DeleteNotification: Delete a notification for a given subscription.
 *NotificationsApi* | [**get_notification**](docs/NotificationsApi.md#get_notification) | **GET** /api/subscriptions/{scope}/{code}/notifications/{id} | [EXPERIMENTAL] GetNotification: Get a notification on a subscription.
 *NotificationsApi* | [**list_notifications**](docs/NotificationsApi.md#list_notifications) | **GET** /api/subscriptions/{scope}/{code}/notifications | [EXPERIMENTAL] ListNotifications: List all notifications on a subscription.
+*NotificationsApi* | [**update_aws_sqs_notification**](docs/NotificationsApi.md#update_aws_sqs_notification) | **PUT** /api/subscriptions/{scope}/{code}/notifications/awssqs/{id} | [EXPERIMENTAL] UpdateAwsSqsNotification: Update an AWS SQS notification for a given subscription.
 *NotificationsApi* | [**update_email_notification**](docs/NotificationsApi.md#update_email_notification) | **PUT** /api/subscriptions/{scope}/{code}/notifications/email/{id} | [EXPERIMENTAL] UpdateEmailNotification: Update an email notification for a given subscription.
 *NotificationsApi* | [**update_sms_notification**](docs/NotificationsApi.md#update_sms_notification) | **PUT** /api/subscriptions/{scope}/{code}/notifications/sms/{id} | [EXPERIMENTAL] UpdateSmsNotification: Update an SMS notification for a given subscription.
 *NotificationsApi* | [**update_webhook_notification**](docs/NotificationsApi.md#update_webhook_notification) | **PUT** /api/subscriptions/{scope}/{code}/notifications/webhook/{id} | [EXPERIMENTAL] UpdateWebhookNotification: Update a Webhook notification for a given subscription.
 *SubscriptionsApi* | [**create_subscription**](docs/SubscriptionsApi.md#create_subscription) | **POST** /api/subscriptions | [EXPERIMENTAL] CreateSubscription: Create a new subscription.
 *SubscriptionsApi* | [**delete_subscription**](docs/SubscriptionsApi.md#delete_subscription) | **DELETE** /api/subscriptions/{scope}/{code} | [EXPERIMENTAL] DeleteSubscription: Delete a subscription.
 *SubscriptionsApi* | [**get_subscription**](docs/SubscriptionsApi.md#get_subscription) | **GET** /api/subscriptions/{scope}/{code} | [EXPERIMENTAL] GetSubscription: Get a subscription.
 *SubscriptionsApi* | [**list_subscriptions**](docs/SubscriptionsApi.md#list_subscriptions) | **GET** /api/subscriptions | [EXPERIMENTAL] ListSubscriptions: List subscriptions.
@@ -115,14 +117,15 @@
 ## Documentation For Models
 
  - [AccessControlledAction](docs/AccessControlledAction.md)
  - [AccessControlledResource](docs/AccessControlledResource.md)
  - [ActionId](docs/ActionId.md)
  - [Attempt](docs/Attempt.md)
  - [AttemptStatus](docs/AttemptStatus.md)
+ - [CreateAwsSqsNotification](docs/CreateAwsSqsNotification.md)
  - [CreateEmailNotification](docs/CreateEmailNotification.md)
  - [CreateSmsNotification](docs/CreateSmsNotification.md)
  - [CreateSubscription](docs/CreateSubscription.md)
  - [CreateWebhookNotification](docs/CreateWebhookNotification.md)
  - [Delivery](docs/Delivery.md)
  - [EventDetails](docs/EventDetails.md)
  - [EventTypeSchema](docs/EventTypeSchema.md)
@@ -138,14 +141,15 @@
  - [ResourceListOfAccessControlledResource](docs/ResourceListOfAccessControlledResource.md)
  - [ResourceListOfDelivery](docs/ResourceListOfDelivery.md)
  - [ResourceListOfEventTypeSchema](docs/ResourceListOfEventTypeSchema.md)
  - [ResourceListOfNotification](docs/ResourceListOfNotification.md)
  - [ResourceListOfSubscription](docs/ResourceListOfSubscription.md)
  - [Subscription](docs/Subscription.md)
  - [SubscriptionDetail](docs/SubscriptionDetail.md)
+ - [UpdateAwsSqsNotification](docs/UpdateAwsSqsNotification.md)
  - [UpdateEmailNotification](docs/UpdateEmailNotification.md)
  - [UpdateSmsNotification](docs/UpdateSmsNotification.md)
  - [UpdateSubscription](docs/UpdateSubscription.md)
  - [UpdateWebhookNotification](docs/UpdateWebhookNotification.md)
 
 
 ## Documentation For Authorization
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/__init__.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.627"
+__version__ = "0.1.654"
 
 # import apis into sdk package
 from lusid_notifications.api.application_metadata_api import ApplicationMetadataApi
 from lusid_notifications.api.deliveries_api import DeliveriesApi
 from lusid_notifications.api.event_types_api import EventTypesApi
 from lusid_notifications.api.events_api import EventsApi
 from lusid_notifications.api.notifications_api import NotificationsApi
@@ -35,14 +35,15 @@
 from lusid_notifications.exceptions import ApiException
 # import models into sdk package
 from lusid_notifications.models.access_controlled_action import AccessControlledAction
 from lusid_notifications.models.access_controlled_resource import AccessControlledResource
 from lusid_notifications.models.action_id import ActionId
 from lusid_notifications.models.attempt import Attempt
 from lusid_notifications.models.attempt_status import AttemptStatus
+from lusid_notifications.models.create_aws_sqs_notification import CreateAwsSqsNotification
 from lusid_notifications.models.create_email_notification import CreateEmailNotification
 from lusid_notifications.models.create_sms_notification import CreateSmsNotification
 from lusid_notifications.models.create_subscription import CreateSubscription
 from lusid_notifications.models.create_webhook_notification import CreateWebhookNotification
 from lusid_notifications.models.delivery import Delivery
 from lusid_notifications.models.event_details import EventDetails
 from lusid_notifications.models.event_type_schema import EventTypeSchema
@@ -58,14 +59,15 @@
 from lusid_notifications.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
 from lusid_notifications.models.resource_list_of_delivery import ResourceListOfDelivery
 from lusid_notifications.models.resource_list_of_event_type_schema import ResourceListOfEventTypeSchema
 from lusid_notifications.models.resource_list_of_notification import ResourceListOfNotification
 from lusid_notifications.models.resource_list_of_subscription import ResourceListOfSubscription
 from lusid_notifications.models.subscription import Subscription
 from lusid_notifications.models.subscription_detail import SubscriptionDetail
+from lusid_notifications.models.update_aws_sqs_notification import UpdateAwsSqsNotification
 from lusid_notifications.models.update_email_notification import UpdateEmailNotification
 from lusid_notifications.models.update_sms_notification import UpdateSmsNotification
 from lusid_notifications.models.update_subscription import UpdateSubscription
 from lusid_notifications.models.update_webhook_notification import UpdateWebhookNotification
 
 # import utilities into sdk package
 from fbnsdkutilities.utilities.api_client_builder import ApiClientBuilder
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/api/application_metadata_api.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/api/application_metadata_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -141,15 +141,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.627'
+        header_params['X-LUSID-SDK-Version'] = '0.1.654'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
         }
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/api/deliveries_api.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/api/deliveries_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -179,15 +179,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.627'
+        header_params['X-LUSID-SDK-Version'] = '0.1.654'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfDelivery",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/api/event_types_api.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/api/event_types_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -160,15 +160,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.627'
+        header_params['X-LUSID-SDK-Version'] = '0.1.654'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "EventTypeSchema",
             400: "LusidValidationProblemDetails",
@@ -292,15 +292,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.627'
+        header_params['X-LUSID-SDK-Version'] = '0.1.654'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfEventTypeSchema",
             404: "str",
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/api/events_api.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/api/events_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -150,15 +150,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.627'
+        header_params['X-LUSID-SDK-Version'] = '0.1.654'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "EventDetails",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/api/notifications_api.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/api/notifications_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -19,21 +19,23 @@
 import six
 
 from lusid_notifications.api_client import ApiClient
 from lusid_notifications.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
+from lusid_notifications.models.create_aws_sqs_notification import CreateAwsSqsNotification
 from lusid_notifications.models.create_email_notification import CreateEmailNotification
 from lusid_notifications.models.create_sms_notification import CreateSmsNotification
 from lusid_notifications.models.create_webhook_notification import CreateWebhookNotification
 from lusid_notifications.models.lusid_problem_details import LusidProblemDetails
 from lusid_notifications.models.lusid_validation_problem_details import LusidValidationProblemDetails
 from lusid_notifications.models.notification import Notification
 from lusid_notifications.models.resource_list_of_notification import ResourceListOfNotification
+from lusid_notifications.models.update_aws_sqs_notification import UpdateAwsSqsNotification
 from lusid_notifications.models.update_email_notification import UpdateEmailNotification
 from lusid_notifications.models.update_sms_notification import UpdateSmsNotification
 from lusid_notifications.models.update_webhook_notification import UpdateWebhookNotification
 
 
 class NotificationsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
@@ -43,14 +45,197 @@
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
+    def create_aws_sqs_notification(self, scope, code, create_aws_sqs_notification, **kwargs):  # noqa: E501
+        """[EXPERIMENTAL] CreateAwsSqsNotification: Add an AWS SQS notification to a subscription.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.create_aws_sqs_notification(scope, code, create_aws_sqs_notification, async_req=True)
+        >>> result = thread.get()
+
+        :param scope: The scope that identifies a notification (required)
+        :type scope: str
+        :param code: The code that identifies a notification (required)
+        :type code: str
+        :param create_aws_sqs_notification: The data to create an message sent to AWS Simple Queue Service (required)
+        :type create_aws_sqs_notification: CreateAwsSqsNotification
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: Notification
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.create_aws_sqs_notification_with_http_info(scope, code, create_aws_sqs_notification, **kwargs)  # noqa: E501
+
+    def create_aws_sqs_notification_with_http_info(self, scope, code, create_aws_sqs_notification, **kwargs):  # noqa: E501
+        """[EXPERIMENTAL] CreateAwsSqsNotification: Add an AWS SQS notification to a subscription.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.create_aws_sqs_notification_with_http_info(scope, code, create_aws_sqs_notification, async_req=True)
+        >>> result = thread.get()
+
+        :param scope: The scope that identifies a notification (required)
+        :type scope: str
+        :param code: The code that identifies a notification (required)
+        :type code: str
+        :param create_aws_sqs_notification: The data to create an message sent to AWS Simple Queue Service (required)
+        :type create_aws_sqs_notification: CreateAwsSqsNotification
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :return: Returns the result object, the HTTP status code, and the headers.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: (Notification, int, HTTPHeaderDict)
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'scope',
+            'code',
+            'create_aws_sqs_notification'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_headers'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method create_aws_sqs_notification" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'scope' is set
+        if self.api_client.client_side_validation and ('scope' not in local_var_params or  # noqa: E501
+                                                        local_var_params['scope'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `scope` when calling `create_aws_sqs_notification`")  # noqa: E501
+        # verify the required parameter 'code' is set
+        if self.api_client.client_side_validation and ('code' not in local_var_params or  # noqa: E501
+                                                        local_var_params['code'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `code` when calling `create_aws_sqs_notification`")  # noqa: E501
+        # verify the required parameter 'create_aws_sqs_notification' is set
+        if self.api_client.client_side_validation and ('create_aws_sqs_notification' not in local_var_params or  # noqa: E501
+                                                        local_var_params['create_aws_sqs_notification'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `create_aws_sqs_notification` when calling `create_aws_sqs_notification`")  # noqa: E501
+
+        if self.api_client.client_side_validation and ('scope' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['scope']) > 100):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `scope` when calling `create_aws_sqs_notification`, length must be less than or equal to `100`")  # noqa: E501
+        if self.api_client.client_side_validation and ('scope' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['scope']) < 1):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `scope` when calling `create_aws_sqs_notification`, length must be greater than or equal to `1`")  # noqa: E501
+        if self.api_client.client_side_validation and 'scope' in local_var_params and not re.search(r'^[a-zA-Z0-9\-_]+$', local_var_params['scope']):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `scope` when calling `create_aws_sqs_notification`, must conform to the pattern `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
+        if self.api_client.client_side_validation and ('code' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['code']) > 100):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `code` when calling `create_aws_sqs_notification`, length must be less than or equal to `100`")  # noqa: E501
+        if self.api_client.client_side_validation and ('code' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['code']) < 1):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `code` when calling `create_aws_sqs_notification`, length must be greater than or equal to `1`")  # noqa: E501
+        if self.api_client.client_side_validation and 'code' in local_var_params and not re.search(r'^[a-zA-Z0-9\-_]+$', local_var_params['code']):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `code` when calling `create_aws_sqs_notification`, must conform to the pattern `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
+        collection_formats = {}
+
+        path_params = {}
+        if 'scope' in local_var_params:
+            path_params['scope'] = local_var_params['scope']  # noqa: E501
+        if 'code' in local_var_params:
+            path_params['code'] = local_var_params['code']  # noqa: E501
+
+        query_params = []
+
+        header_params = dict(local_var_params.get('_headers', {}))
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'create_aws_sqs_notification' in local_var_params:
+            body_params = local_var_params['create_aws_sqs_notification']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        header_params['Accept-Encoding'] = "gzip, deflate, br"
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
+
+        # set the LUSID header
+        header_params['X-LUSID-SDK-Language'] = 'Python'
+        header_params['X-LUSID-SDK-Version'] = '0.1.654'
+
+        # Authentication setting
+        auth_settings = ['oauth2']  # noqa: E501
+
+        response_types_map = {
+            201: "Notification",
+            400: "LusidValidationProblemDetails",
+        }
+
+        return self.api_client.call_api(
+            '/api/subscriptions/{scope}/{code}/notifications/awssqs', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_types_map=response_types_map,
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats,
+            _request_auth=local_var_params.get('_request_auth'))
+
     def create_email_notification(self, scope, code, create_email_notification, **kwargs):  # noqa: E501
         """[EXPERIMENTAL] CreateEmailNotification: Add an email notification to a subscription.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_email_notification(scope, code, create_email_notification, async_req=True)
@@ -199,15 +384,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.627'
+        header_params['X-LUSID-SDK-Version'] = '0.1.654'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -382,15 +567,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.627'
+        header_params['X-LUSID-SDK-Version'] = '0.1.654'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -565,15 +750,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.627'
+        header_params['X-LUSID-SDK-Version'] = '0.1.654'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -753,15 +938,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.627'
+        header_params['X-LUSID-SDK-Version'] = '0.1.654'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -938,15 +1123,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.627'
+        header_params['X-LUSID-SDK-Version'] = '0.1.654'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -1108,15 +1293,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.627'
+        header_params['X-LUSID-SDK-Version'] = '0.1.654'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfNotification",
             400: "LusidValidationProblemDetails",
@@ -1136,14 +1321,217 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
+    def update_aws_sqs_notification(self, scope, code, id, update_aws_sqs_notification, **kwargs):  # noqa: E501
+        """[EXPERIMENTAL] UpdateAwsSqsNotification: Update an AWS SQS notification for a given subscription.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.update_aws_sqs_notification(scope, code, id, update_aws_sqs_notification, async_req=True)
+        >>> result = thread.get()
+
+        :param scope: The scope that identifies a notification (required)
+        :type scope: str
+        :param code: The code that identifies a notification (required)
+        :type code: str
+        :param id: The unique identifier of the notification (required)
+        :type id: str
+        :param update_aws_sqs_notification: The data to update a notification (required)
+        :type update_aws_sqs_notification: UpdateAwsSqsNotification
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: Notification
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.update_aws_sqs_notification_with_http_info(scope, code, id, update_aws_sqs_notification, **kwargs)  # noqa: E501
+
+    def update_aws_sqs_notification_with_http_info(self, scope, code, id, update_aws_sqs_notification, **kwargs):  # noqa: E501
+        """[EXPERIMENTAL] UpdateAwsSqsNotification: Update an AWS SQS notification for a given subscription.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.update_aws_sqs_notification_with_http_info(scope, code, id, update_aws_sqs_notification, async_req=True)
+        >>> result = thread.get()
+
+        :param scope: The scope that identifies a notification (required)
+        :type scope: str
+        :param code: The code that identifies a notification (required)
+        :type code: str
+        :param id: The unique identifier of the notification (required)
+        :type id: str
+        :param update_aws_sqs_notification: The data to update a notification (required)
+        :type update_aws_sqs_notification: UpdateAwsSqsNotification
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :return: Returns the result object, the HTTP status code, and the headers.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: (Notification, int, HTTPHeaderDict)
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'scope',
+            'code',
+            'id',
+            'update_aws_sqs_notification'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_headers'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method update_aws_sqs_notification" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'scope' is set
+        if self.api_client.client_side_validation and ('scope' not in local_var_params or  # noqa: E501
+                                                        local_var_params['scope'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `scope` when calling `update_aws_sqs_notification`")  # noqa: E501
+        # verify the required parameter 'code' is set
+        if self.api_client.client_side_validation and ('code' not in local_var_params or  # noqa: E501
+                                                        local_var_params['code'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `code` when calling `update_aws_sqs_notification`")  # noqa: E501
+        # verify the required parameter 'id' is set
+        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `update_aws_sqs_notification`")  # noqa: E501
+        # verify the required parameter 'update_aws_sqs_notification' is set
+        if self.api_client.client_side_validation and ('update_aws_sqs_notification' not in local_var_params or  # noqa: E501
+                                                        local_var_params['update_aws_sqs_notification'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `update_aws_sqs_notification` when calling `update_aws_sqs_notification`")  # noqa: E501
+
+        if self.api_client.client_side_validation and ('scope' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['scope']) > 100):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `scope` when calling `update_aws_sqs_notification`, length must be less than or equal to `100`")  # noqa: E501
+        if self.api_client.client_side_validation and ('scope' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['scope']) < 1):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `scope` when calling `update_aws_sqs_notification`, length must be greater than or equal to `1`")  # noqa: E501
+        if self.api_client.client_side_validation and 'scope' in local_var_params and not re.search(r'^[a-zA-Z0-9\-_]+$', local_var_params['scope']):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `scope` when calling `update_aws_sqs_notification`, must conform to the pattern `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
+        if self.api_client.client_side_validation and ('code' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['code']) > 100):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `code` when calling `update_aws_sqs_notification`, length must be less than or equal to `100`")  # noqa: E501
+        if self.api_client.client_side_validation and ('code' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['code']) < 1):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `code` when calling `update_aws_sqs_notification`, length must be greater than or equal to `1`")  # noqa: E501
+        if self.api_client.client_side_validation and 'code' in local_var_params and not re.search(r'^[a-zA-Z0-9\-_]+$', local_var_params['code']):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `code` when calling `update_aws_sqs_notification`, must conform to the pattern `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
+        if self.api_client.client_side_validation and ('id' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['id']) > 40):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `id` when calling `update_aws_sqs_notification`, length must be less than or equal to `40`")  # noqa: E501
+        if self.api_client.client_side_validation and ('id' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['id']) < 30):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `id` when calling `update_aws_sqs_notification`, length must be greater than or equal to `30`")  # noqa: E501
+        if self.api_client.client_side_validation and 'id' in local_var_params and not re.search(r'^[a-zA-Z0-9\-]+$', local_var_params['id']):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `id` when calling `update_aws_sqs_notification`, must conform to the pattern `/^[a-zA-Z0-9\-]+$/`")  # noqa: E501
+        collection_formats = {}
+
+        path_params = {}
+        if 'scope' in local_var_params:
+            path_params['scope'] = local_var_params['scope']  # noqa: E501
+        if 'code' in local_var_params:
+            path_params['code'] = local_var_params['code']  # noqa: E501
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
+
+        query_params = []
+
+        header_params = dict(local_var_params.get('_headers', {}))
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'update_aws_sqs_notification' in local_var_params:
+            body_params = local_var_params['update_aws_sqs_notification']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        header_params['Accept-Encoding'] = "gzip, deflate, br"
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
+
+        # set the LUSID header
+        header_params['X-LUSID-SDK-Language'] = 'Python'
+        header_params['X-LUSID-SDK-Version'] = '0.1.654'
+
+        # Authentication setting
+        auth_settings = ['oauth2']  # noqa: E501
+
+        response_types_map = {
+            200: "Notification",
+            400: "LusidValidationProblemDetails",
+            404: "str",
+        }
+
+        return self.api_client.call_api(
+            '/api/subscriptions/{scope}/{code}/notifications/awssqs/{id}', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_types_map=response_types_map,
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats,
+            _request_auth=local_var_params.get('_request_auth'))
+
     def update_email_notification(self, scope, code, id, update_email_notification, **kwargs):  # noqa: E501
         """[EXPERIMENTAL] UpdateEmailNotification: Update an email notification for a given subscription.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_email_notification(scope, code, id, update_email_notification, async_req=True)
@@ -1311,15 +1699,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.627'
+        header_params['X-LUSID-SDK-Version'] = '0.1.654'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -1514,15 +1902,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.627'
+        header_params['X-LUSID-SDK-Version'] = '0.1.654'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -1717,15 +2105,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.627'
+        header_params['X-LUSID-SDK-Version'] = '0.1.654'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/api/subscriptions_api.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/api/subscriptions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -158,15 +158,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.627'
+        header_params['X-LUSID-SDK-Version'] = '0.1.654'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -327,15 +327,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.627'
+        header_params['X-LUSID-SDK-Version'] = '0.1.654'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -493,15 +493,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.627'
+        header_params['X-LUSID-SDK-Version'] = '0.1.654'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "SubscriptionDetail",
             400: "LusidValidationProblemDetails",
@@ -681,15 +681,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.627'
+        header_params['X-LUSID-SDK-Version'] = '0.1.654'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfSubscription",
             400: "LusidValidationProblemDetails",
@@ -864,15 +864,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.627'
+        header_params['X-LUSID-SDK-Version'] = '0.1.654'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/api_client.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.627/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.654/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/configuration.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.627\n"\
-               "SDK Package Version: 0.1.627".\
+               "Version of the API: 0.1.654\n"\
+               "SDK Package Version: 0.1.654".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/exceptions.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/__init__.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 
 # flake8: noqa
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
 from lusid_notifications.models.access_controlled_action import AccessControlledAction
 from lusid_notifications.models.access_controlled_resource import AccessControlledResource
 from lusid_notifications.models.action_id import ActionId
 from lusid_notifications.models.attempt import Attempt
 from lusid_notifications.models.attempt_status import AttemptStatus
+from lusid_notifications.models.create_aws_sqs_notification import CreateAwsSqsNotification
 from lusid_notifications.models.create_email_notification import CreateEmailNotification
 from lusid_notifications.models.create_sms_notification import CreateSmsNotification
 from lusid_notifications.models.create_subscription import CreateSubscription
 from lusid_notifications.models.create_webhook_notification import CreateWebhookNotification
 from lusid_notifications.models.delivery import Delivery
 from lusid_notifications.models.event_details import EventDetails
 from lusid_notifications.models.event_type_schema import EventTypeSchema
@@ -39,11 +40,12 @@
 from lusid_notifications.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
 from lusid_notifications.models.resource_list_of_delivery import ResourceListOfDelivery
 from lusid_notifications.models.resource_list_of_event_type_schema import ResourceListOfEventTypeSchema
 from lusid_notifications.models.resource_list_of_notification import ResourceListOfNotification
 from lusid_notifications.models.resource_list_of_subscription import ResourceListOfSubscription
 from lusid_notifications.models.subscription import Subscription
 from lusid_notifications.models.subscription_detail import SubscriptionDetail
+from lusid_notifications.models.update_aws_sqs_notification import UpdateAwsSqsNotification
 from lusid_notifications.models.update_email_notification import UpdateEmailNotification
 from lusid_notifications.models.update_sms_notification import UpdateSmsNotification
 from lusid_notifications.models.update_subscription import UpdateSubscription
 from lusid_notifications.models.update_webhook_notification import UpdateWebhookNotification
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/access_controlled_action.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/access_controlled_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/access_controlled_resource.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/action_id.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/action_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/attempt.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/attempt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/attempt_status.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/attempt_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/create_email_notification.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/create_email_notification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/create_sms_notification.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/create_sms_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/create_subscription.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/create_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/create_webhook_notification.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/create_webhook_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/delivery.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/delivery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/event_details.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/event_details.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/event_type_schema.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/id_selector_definition.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/id_selector_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/identifier_part_schema.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/identifier_part_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/link.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/lusid_problem_details.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/lusid_validation_problem_details.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/lusid_validation_problem_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/matching_pattern.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/matching_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/notification.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/notification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/notification_status.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/notification_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/resource_id.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/resource_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/resource_list_of_access_controlled_resource.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/resource_list_of_access_controlled_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/resource_list_of_delivery.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/resource_list_of_delivery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/resource_list_of_event_type_schema.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/resource_list_of_event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/resource_list_of_notification.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/resource_list_of_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/resource_list_of_subscription.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/resource_list_of_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/subscription.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/subscription_detail.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/subscription_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/update_email_notification.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/update_email_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/update_sms_notification.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/update_sms_notification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/update_subscription.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/update_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/models/update_webhook_notification.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/models/update_webhook_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/rest.py` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.627
+    The version of the OpenAPI document: 0.1.654
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications/utilities/config_keys.json` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-notifications-sdk-preview-0.1.627/lusid_notifications_sdk_preview.egg-info/SOURCES.txt` & `lusid-notifications-sdk-preview-0.1.654/lusid_notifications_sdk_preview.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 lusid_notifications/api/subscriptions_api.py
 lusid_notifications/models/__init__.py
 lusid_notifications/models/access_controlled_action.py
 lusid_notifications/models/access_controlled_resource.py
 lusid_notifications/models/action_id.py
 lusid_notifications/models/attempt.py
 lusid_notifications/models/attempt_status.py
+lusid_notifications/models/create_aws_sqs_notification.py
 lusid_notifications/models/create_email_notification.py
 lusid_notifications/models/create_sms_notification.py
 lusid_notifications/models/create_subscription.py
 lusid_notifications/models/create_webhook_notification.py
 lusid_notifications/models/delivery.py
 lusid_notifications/models/event_details.py
 lusid_notifications/models/event_type_schema.py
@@ -39,14 +40,15 @@
 lusid_notifications/models/resource_list_of_access_controlled_resource.py
 lusid_notifications/models/resource_list_of_delivery.py
 lusid_notifications/models/resource_list_of_event_type_schema.py
 lusid_notifications/models/resource_list_of_notification.py
 lusid_notifications/models/resource_list_of_subscription.py
 lusid_notifications/models/subscription.py
 lusid_notifications/models/subscription_detail.py
+lusid_notifications/models/update_aws_sqs_notification.py
 lusid_notifications/models/update_email_notification.py
 lusid_notifications/models/update_sms_notification.py
 lusid_notifications/models/update_subscription.py
 lusid_notifications/models/update_webhook_notification.py
 lusid_notifications/utilities/__init__.py
 lusid_notifications/utilities/config_keys.json
 lusid_notifications/utilities/config_keys.py
```

### Comparing `lusid-notifications-sdk-preview-0.1.627/setup.py` & `lusid-notifications-sdk-preview-0.1.654/setup.py`

 * *Files identical despite different names*

