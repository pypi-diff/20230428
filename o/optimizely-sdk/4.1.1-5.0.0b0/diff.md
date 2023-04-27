# Comparing `tmp/optimizely-sdk-4.1.1.tar.gz` & `tmp/optimizely-sdk-5.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimizely-sdk-4.1.1.tar", last modified: Sat Mar 11 00:34:56 2023, max compression
+gzip compressed data, was "optimizely-sdk-5.0.0b0.tar", last modified: Thu Apr 27 22:13:26 2023, max compression
```

## Comparing `optimizely-sdk-4.1.1.tar` & `optimizely-sdk-5.0.0b0.tar`

### file list

```diff
@@ -1,63 +1,89 @@
-drwxrwxrwx   0        0        0        0 2023-03-11 00:34:56.344385 optimizely-sdk-4.1.1/
--rw-rw-rw-   0        0        0    23522 2023-03-10 23:48:27.000000 optimizely-sdk-4.1.1/CHANGELOG.md
--rw-rw-rw-   0        0        0    11541 2022-10-25 17:57:39.000000 optimizely-sdk-4.1.1/LICENSE
--rw-rw-rw-   0        0        0      135 2022-05-09 19:24:29.000000 optimizely-sdk-4.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0    36447 2023-03-11 00:34:56.343386 optimizely-sdk-4.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    11540 2023-03-10 23:48:27.000000 optimizely-sdk-4.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-11 00:34:56.295220 optimizely-sdk-4.1.1/optimizely/
--rw-rw-rw-   0        0        0      581 2022-10-25 17:56:39.000000 optimizely-sdk-4.1.1/optimizely/__init__.py
--rw-rw-rw-   0        0        0     5964 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/bucketer.py
--rw-rw-rw-   0        0        0    18039 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/config_manager.py
-drwxrwxrwx   0        0        0        0 2023-03-11 00:34:56.300274 optimizely-sdk-4.1.1/optimizely/decision/
--rw-rw-rw-   0        0        0      581 2022-10-25 18:01:05.000000 optimizely-sdk-4.1.1/optimizely/decision/__init__.py
--rw-rw-rw-   0        0        0      877 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/decision/optimizely_decide_option.py
--rw-rw-rw-   0        0        0     1411 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/decision/optimizely_decision.py
--rw-rw-rw-   0        0        0      838 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/decision/optimizely_decision_message.py
--rw-rw-rw-   0        0        0    26060 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/decision_service.py
--rw-rw-rw-   0        0        0     4351 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/entities.py
--rw-rw-rw-   0        0        0     1160 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/error_handler.py
-drwxrwxrwx   0        0        0        0 2023-03-11 00:34:56.309262 optimizely-sdk-4.1.1/optimizely/event/
--rw-rw-rw-   0        0        0      581 2022-10-25 18:01:05.000000 optimizely-sdk-4.1.1/optimizely/event/__init__.py
--rw-rw-rw-   0        0        0     6294 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/event/event_factory.py
--rw-rw-rw-   0        0        0    14537 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/event/event_processor.py
--rw-rw-rw-   0        0        0      985 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/event/log_event.py
--rw-rw-rw-   0        0        0     3652 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/event/payload.py
--rw-rw-rw-   0        0        0     2606 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/event/user_event.py
--rw-rw-rw-   0        0        0     4107 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/event/user_event_factory.py
--rw-rw-rw-   0        0        0     9965 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/event_builder.py
--rw-rw-rw-   0        0        0     1579 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/event_dispatcher.py
--rw-rw-rw-   0        0        0     1714 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-03-11 00:34:56.321270 optimizely-sdk-4.1.1/optimizely/helpers/
--rw-rw-rw-   0        0        0      581 2022-10-25 18:01:05.000000 optimizely-sdk-4.1.1/optimizely/helpers/__init__.py
--rw-rw-rw-   0        0        0     3856 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/helpers/audience.py
--rw-rw-rw-   0        0        0    30577 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/helpers/condition.py
--rw-rw-rw-   0        0        0     4120 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/helpers/condition_tree_evaluator.py
--rw-rw-rw-   0        0        0     6781 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/helpers/constants.py
--rw-rw-rw-   0        0        0     7697 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/helpers/enums.py
--rw-rw-rw-   0        0        0     4927 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/helpers/event_tag_utils.py
--rw-rw-rw-   0        0        0      939 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/helpers/experiment.py
--rw-rw-rw-   0        0        0     8230 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/helpers/validator.py
-drwxrwxrwx   0        0        0        0 2023-03-11 00:34:56.323270 optimizely-sdk-4.1.1/optimizely/lib/
--rw-rw-rw-   0        0        0      581 2022-10-25 18:01:35.000000 optimizely-sdk-4.1.1/optimizely/lib/__init__.py
--rw-rw-rw-   0        0        0    14169 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/lib/pymmh3.py
--rw-rw-rw-   0        0        0     3689 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/logger.py
--rw-rw-rw-   0        0        0     5641 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/notification_center.py
--rw-rw-rw-   0        0        0    52263 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/optimizely.py
--rw-rw-rw-   0        0        0    19078 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/optimizely_config.py
--rw-rw-rw-   0        0        0     7515 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/optimizely_factory.py
--rw-rw-rw-   0        0        0     7195 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/optimizely_user_context.py
--rw-rw-rw-   0        0        0    25426 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/project_config.py
--rw-rw-rw-   0        0        0     2847 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/optimizely/user_profile.py
--rw-rw-rw-   0        0        0      679 2023-03-10 23:48:27.000000 optimizely-sdk-4.1.1/optimizely/version.py
-drwxrwxrwx   0        0        0        0 2023-03-11 00:34:56.337392 optimizely-sdk-4.1.1/optimizely_sdk.egg-info/
--rw-rw-rw-   0        0        0    36447 2023-03-11 00:34:56.000000 optimizely-sdk-4.1.1/optimizely_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1565 2023-03-11 00:34:56.000000 optimizely-sdk-4.1.1/optimizely_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-11 00:34:56.000000 optimizely-sdk-4.1.1/optimizely_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      325 2023-03-11 00:34:56.000000 optimizely-sdk-4.1.1/optimizely_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-03-11 00:34:56.000000 optimizely-sdk-4.1.1/optimizely_sdk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-11 00:34:56.341383 optimizely-sdk-4.1.1/requirements/
--rw-rw-rw-   0        0        0      120 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/requirements/core.txt
--rw-rw-rw-   0        0        0       52 2022-05-09 19:24:29.000000 optimizely-sdk-4.1.1/requirements/docs.txt
--rw-rw-rw-   0        0        0      104 2023-03-10 22:47:41.000000 optimizely-sdk-4.1.1/requirements/test.txt
--rw-rw-rw-   0        0        0       42 2023-03-11 00:34:56.344385 optimizely-sdk-4.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2440 2023-03-10 23:48:27.000000 optimizely-sdk-4.1.1/setup.py
+drwxr-xr-x   0 matjaz     (501) staff       (20)        0 2023-04-27 22:13:26.312575 optimizely-sdk-5.0.0b0/
+-rw-r--r--   0 matjaz     (501) staff       (20)    27025 2023-04-27 22:12:39.000000 optimizely-sdk-5.0.0b0/CHANGELOG.md
+-rw-r--r--   0 matjaz     (501) staff       (20)    11340 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/LICENSE
+-rw-r--r--   0 matjaz     (501) staff       (20)      129 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/MANIFEST.in
+-rw-r--r--   0 matjaz     (501) staff       (20)    39652 2023-04-27 22:13:26.312203 optimizely-sdk-5.0.0b0/PKG-INFO
+-rw-r--r--   0 matjaz     (501) staff       (20)    11362 2023-04-11 19:15:42.000000 optimizely-sdk-5.0.0b0/README.md
+drwxr-xr-x   0 matjaz     (501) staff       (20)        0 2023-04-27 22:13:26.237196 optimizely-sdk-5.0.0b0/optimizely/
+-rw-r--r--   0 matjaz     (501) staff       (20)      569 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/__init__.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     6435 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/bucketer.py
+-rw-r--r--   0 matjaz     (501) staff       (20)    20368 2023-02-07 19:07:50.000000 optimizely-sdk-5.0.0b0/optimizely/config_manager.py
+drwxr-xr-x   0 matjaz     (501) staff       (20)        0 2023-04-27 22:13:26.265372 optimizely-sdk-5.0.0b0/optimizely/decision/
+-rw-r--r--   0 matjaz     (501) staff       (20)      569 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/decision/__init__.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     1038 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/decision/optimizely_decide_option.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     1854 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/decision/optimizely_decision.py
+-rw-r--r--   0 matjaz     (501) staff       (20)      987 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/decision/optimizely_decision_message.py
+-rw-r--r--   0 matjaz     (501) staff       (20)    27066 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/decision_service.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     5985 2023-02-07 19:07:50.000000 optimizely-sdk-5.0.0b0/optimizely/entities.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     1163 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/error_handler.py
+drwxr-xr-x   0 matjaz     (501) staff       (20)        0 2023-04-27 22:13:26.272235 optimizely-sdk-5.0.0b0/optimizely/event/
+-rw-r--r--   0 matjaz     (501) staff       (20)      569 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/event/__init__.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     7195 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/event/event_factory.py
+-rw-r--r--   0 matjaz     (501) staff       (20)    15516 2022-11-17 20:53:17.000000 optimizely-sdk-5.0.0b0/optimizely/event/event_processor.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     1365 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/event/log_event.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     4190 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/event/payload.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     3401 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/event/user_event.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     4806 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/event/user_event_factory.py
+-rw-r--r--   0 matjaz     (501) staff       (20)    11074 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/event_builder.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     2032 2022-08-04 05:52:38.000000 optimizely-sdk-5.0.0b0/optimizely/event_dispatcher.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     2063 2022-09-26 17:57:06.000000 optimizely-sdk-5.0.0b0/optimizely/exceptions.py
+drwxr-xr-x   0 matjaz     (501) staff       (20)        0 2023-04-27 22:13:26.288488 optimizely-sdk-5.0.0b0/optimizely/helpers/
+-rw-r--r--   0 matjaz     (501) staff       (20)      569 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/helpers/__init__.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     4330 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/helpers/audience.py
+-rw-r--r--   0 matjaz     (501) staff       (20)    32080 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/helpers/condition.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     4396 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/helpers/condition_tree_evaluator.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     6910 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/helpers/constants.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     9162 2023-04-25 17:45:42.000000 optimizely-sdk-5.0.0b0/optimizely/helpers/enums.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     5354 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/helpers/event_tag_utils.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     1138 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/helpers/experiment.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     3377 2023-02-07 19:07:50.000000 optimizely-sdk-5.0.0b0/optimizely/helpers/sdk_settings.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     2869 2022-08-01 21:51:05.000000 optimizely-sdk-5.0.0b0/optimizely/helpers/types.py
+-rw-r--r--   0 matjaz     (501) staff       (20)    11012 2022-11-08 15:58:53.000000 optimizely-sdk-5.0.0b0/optimizely/helpers/validator.py
+drwxr-xr-x   0 matjaz     (501) staff       (20)        0 2023-04-27 22:13:26.290851 optimizely-sdk-5.0.0b0/optimizely/lib/
+-rw-r--r--   0 matjaz     (501) staff       (20)      569 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/lib/__init__.py
+-rwxr-xr-x   0 matjaz     (501) staff       (20)    13806 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/lib/pymmh3.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     4444 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/logger.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     5899 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/notification_center.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     2370 2023-02-07 19:07:50.000000 optimizely-sdk-5.0.0b0/optimizely/notification_center_registry.py
+drwxr-xr-x   0 matjaz     (501) staff       (20)        0 2023-04-27 22:13:26.299516 optimizely-sdk-5.0.0b0/optimizely/odp/
+-rw-r--r--   0 matjaz     (501) staff       (20)      569 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/odp/__init__.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     3909 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/odp/lru_cache.py
+-rw-r--r--   0 matjaz     (501) staff       (20)      626 2022-10-11 00:25:57.000000 optimizely-sdk-5.0.0b0/optimizely/odp/matjaz_playfile.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     3463 2022-09-16 20:47:34.000000 optimizely-sdk-5.0.0b0/optimizely/odp/odp_config.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     2641 2023-04-11 19:15:42.000000 optimizely-sdk-5.0.0b0/optimizely/odp/odp_event.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     3782 2023-01-23 21:14:36.000000 optimizely-sdk-5.0.0b0/optimizely/odp/odp_event_api_manager.py
+-rw-r--r--   0 matjaz     (501) staff       (20)    11104 2023-02-28 20:33:53.000000 optimizely-sdk-5.0.0b0/optimizely/odp/odp_event_manager.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     5440 2023-02-07 19:07:50.000000 optimizely-sdk-5.0.0b0/optimizely/odp/odp_manager.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     6754 2023-04-25 17:45:42.000000 optimizely-sdk-5.0.0b0/optimizely/odp/odp_segment_api_manager.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     3712 2023-01-23 21:14:36.000000 optimizely-sdk-5.0.0b0/optimizely/odp/odp_segment_manager.py
+-rw-r--r--   0 matjaz     (501) staff       (20)      871 2022-08-29 05:47:15.000000 optimizely-sdk-5.0.0b0/optimizely/odp/optimizely_odp_option.py
+-rw-r--r--   0 matjaz     (501) staff       (20)    61392 2023-04-11 19:15:42.000000 optimizely-sdk-5.0.0b0/optimizely/optimizely.py
+-rw-r--r--   0 matjaz     (501) staff       (20)    20660 2023-02-07 19:07:50.000000 optimizely-sdk-5.0.0b0/optimizely/optimizely_config.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     8127 2022-11-08 15:58:53.000000 optimizely-sdk-5.0.0b0/optimizely/optimizely_factory.py
+-rw-r--r--   0 matjaz     (501) staff       (20)    11760 2023-02-28 20:33:53.000000 optimizely-sdk-5.0.0b0/optimizely/optimizely_user_context.py
+-rw-r--r--   0 matjaz     (501) staff       (20)    27815 2023-02-07 19:07:50.000000 optimizely-sdk-5.0.0b0/optimizely/project_config.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     3196 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/optimizely/user_profile.py
+-rw-r--r--   0 matjaz     (501) staff       (20)      671 2023-04-27 22:12:39.000000 optimizely-sdk-5.0.0b0/optimizely/version.py
+drwxr-xr-x   0 matjaz     (501) staff       (20)        0 2023-04-27 22:13:26.301070 optimizely-sdk-5.0.0b0/optimizely_sdk.egg-info/
+-rw-r--r--   0 matjaz     (501) staff       (20)    39652 2023-04-27 22:13:26.000000 optimizely-sdk-5.0.0b0/optimizely_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 matjaz     (501) staff       (20)     2366 2023-04-27 22:13:26.000000 optimizely-sdk-5.0.0b0/optimizely_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 matjaz     (501) staff       (20)        1 2023-04-27 22:13:26.000000 optimizely-sdk-5.0.0b0/optimizely_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 matjaz     (501) staff       (20)      289 2023-04-27 22:13:26.000000 optimizely-sdk-5.0.0b0/optimizely_sdk.egg-info/requires.txt
+-rw-r--r--   0 matjaz     (501) staff       (20)       31 2023-04-27 22:13:26.000000 optimizely-sdk-5.0.0b0/optimizely_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 matjaz     (501) staff       (20)        0 2023-04-27 22:13:26.302421 optimizely-sdk-5.0.0b0/requirements/
+-rw-r--r--   0 matjaz     (501) staff       (20)      101 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/requirements/core.txt
+-rw-r--r--   0 matjaz     (501) staff       (20)       49 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/requirements/docs.txt
+-rw-r--r--   0 matjaz     (501) staff       (20)       84 2022-08-01 06:23:43.000000 optimizely-sdk-5.0.0b0/requirements/test.txt
+-rw-r--r--   0 matjaz     (501) staff       (20)       55 2022-11-17 20:51:38.000000 optimizely-sdk-5.0.0b0/requirements/typing.txt
+-rw-r--r--   0 matjaz     (501) staff       (20)       38 2023-04-27 22:13:26.312641 optimizely-sdk-5.0.0b0/setup.cfg
+-rw-r--r--   0 matjaz     (501) staff       (20)     2281 2023-04-11 19:15:42.000000 optimizely-sdk-5.0.0b0/setup.py
+drwxr-xr-x   0 matjaz     (501) staff       (20)        0 2023-04-27 22:13:26.311526 optimizely-sdk-5.0.0b0/z_matjaz_play/
+-rw-r--r--   0 matjaz     (501) staff       (20)        0 2022-08-01 06:35:58.000000 optimizely-sdk-5.0.0b0/z_matjaz_play/__init__.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     4553 2023-04-25 17:46:18.000000 optimizely-sdk-5.0.0b0/z_matjaz_play/agent_odp_code.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     2216 2022-08-01 06:21:00.000000 optimizely-sdk-5.0.0b0/z_matjaz_play/customer_issue_w_fetching_datafile.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     1925 2022-08-11 01:07:58.000000 optimizely-sdk-5.0.0b0/z_matjaz_play/generate_impression_events.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     6687 2023-04-25 17:46:18.000000 optimizely-sdk-5.0.0b0/z_matjaz_play/my_ats.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     6218 2022-10-18 18:09:24.000000 optimizely-sdk-5.0.0b0/z_matjaz_play/myapp.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     5876 2023-02-17 20:43:23.000000 optimizely-sdk-5.0.0b0/z_matjaz_play/myapp2.py
+-rw-r--r--   0 matjaz     (501) staff       (20)    11408 2023-02-04 04:04:51.000000 optimizely-sdk-5.0.0b0/z_matjaz_play/opti_config_v2_test.py
+-rw-r--r--   0 matjaz     (501) staff       (20)     1559 2022-08-29 05:31:08.000000 optimizely-sdk-5.0.0b0/z_matjaz_play/threading_exercises.py
```

### Comparing `optimizely-sdk-4.1.1/CHANGELOG.md` & `optimizely-sdk-5.0.0b0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,402 +1,438 @@
-# Optimizely Python SDK Changelog
-
-## 4.1.1
-March 10th, 2023
-
-We updated our README.md and other non-functional code to reflect that this SDK supports both Optimizely Feature Experimentation and Optimizely Full Stack. ([#420](https://github.com/optimizely/python-sdk/pull/420))
-
-## 4.1.0
-July 7th, 2022
-
-### Bug Fixes
-* Fix error log formatting for flag key ([#381](https://github.com/optimizely/python-sdk/pull/381))
-* Fix invalid datafile returned from `ProjectConfig.to_datafile` and `OptimizelyConfig.get_datafile` ([#321](https://github.com/optimizely/python-sdk/pull/321), [#384](https://github.com/optimizely/python-sdk/pull/384))
-
-
-## 4.0.0
-January 12th, 2022
-
-### New Features
-* Add a set of new APIs for overriding and managing user-level flag, experiment and delivery rule decisions. These methods can be used for QA and automated testing purposes. They are an extension of the OptimizelyUserContext interface ([#361](https://github.com/optimizely/python-sdk/pull/361), [#365](https://github.com/optimizely/python-sdk/pull/365), [#369](https://github.com/optimizely/python-sdk/pull/369)):
-	- setForcedDecision
-	- getForcedDecision
-	- removeForcedDecision
-	- removeAllForcedDecisions
-
-* For details, refer to our documentation pages: [OptimizelyUserContext](https://docs.developers.optimizely.com/full-stack/v4.0/docs/optimizelyusercontext-python) and [Forced Decision methods](https://docs.developers.optimizely.com/full-stack/v4.0/docs/forced-decision-methods-python).
-
-### Breaking Changes:
-
-* Support for `Python v3.4` has been dropped as of this release due to a security vulnerability with `PyYAML <v5.4`. ([#366](https://github.com/optimizely/python-sdk/pull/366))
-* We no longer support `Python v2.7, v3.5, and v3.6` including `PyPy` as of this release. ([#377](https://github.com/optimizely/python-sdk/pull/373))
-* We now support `Python v3.7 and above` including `PyPy3`.
-
-## 3.10.0
-September 16th, 2021
-
-### New Features
-* Added new public properties to OptimizelyConfig.
-  - sdk_key and environment_key [#338] (https://github.com/optimizely/python-sdk/pull/338)
-  - attributes and events [#339] (https://github.com/optimizely/python-sdk/pull/339)
-  - experiment_rules, delivery_rules, audiences and audiences in OptimizelyExperiment
-    - [#342] (https://github.com/optimizely/python-sdk/pull/342)
-    - [#351] (https://github.com/optimizely/python-sdk/pull/351/files)
-* For details please refer to our documentation page:
-  - Python-sdk: [https://docs.developers.optimizely.com/full-stack/docs/optimizelyconfig-python]
-
-* OptimizelyFeature.experiments_map of OptimizelyConfig is now deprecated. Please use OptimizelyFeature.experiment_rules and OptimizelyFeature.delivery_rules. [#360] (https://github.com/optimizely/python-sdk/pull/360)
-
-### Bug Fixes
-* Fix event processor negative timeout interval when retrieving events from queue. [#356] (https://github.com/optimizely/python-sdk/pull/356)
-
-## 3.9.1
-July 14th, 2021
-
-### Bug Fixes:
-* Fixed issue with serving incorrect variation in projects containing multiple flags with duplicate keys. [#347] (https://github.com/optimizely/python-sdk/pull/347)
-* Fixed issue with serving incorrect variation in create_impression_event in user_event_factory.py. [#350] (https://github.com/optimizely/python-sdk/pull/350)
-
-## 3.9.0
-June 1st, 2021
-
-### New Features
-* Added support for multiple concurrent prioritized experiments per flag. [#322](https://github.com/optimizely/python-sdk/pull/322)
-
-## 3.8.0
-February 12th, 2021
-
-### New Features
-* New Features
-Introducing a new primary interface for retrieving feature flag status, configuration and associated experiment decisions for users ([#309](https://github.com/optimizely/python-sdk/pull/309)). The new `OptimizelyUserContext` class is instantiated with `create_user_context` and exposes the following APIs to get `OptimizelyDecision`:
-
-    - set_attribute
-    - decide
-    - decide_all
-    - decide_for_keys
-    - track_event
-
-For details, refer to our documentation page: https://docs.developers.optimizely.com/full-stack/v4.0/docs/python-sdk.
-
-## 3.7.1
-November 19th, 2020
-
-### Bug Fixes:
-* Added "enabled" field to decision metadata structure. [#306](https://github.com/optimizely/python-sdk/pull/306)
-
-## 3.7.0
-November 2nd, 2020
-
-### New Features
-* Added support for upcoming application-controlled introduction of tracking for non-experiment Flag decisions. [#300](https://github.com/optimizely/python-sdk/pull/300)
-
-## 3.6.0
-October 1st, 2020
-
-### New Features:
-* Version targeting using semantic version syntax. [#293](https://github.com/optimizely/python-sdk/pull/293)
-* Datafile accessor API added to access current config as a JSON string. [#283](https://github.com/optimizely/python-sdk/pull/283)
-
-### Bug Fixes:
-* Fixed package installation for Python 3.4 and pypy. [#298](https://github.com/optimizely/python-sdk/pull/298)
-
-## 3.5.2
-July 14th, 2020
-
-### Bug Fixes:
-* Fixed handling of network and no status code errors when polling for datafile in `PollingConfigManager` and `AuthDatafilePollingConfigManager`. ([#287](https://github.com/optimizely/python-sdk/pull/287))
-
-## 3.5.1
-July 10th, 2020
-
-### Bug Fixes:
-* Fixed HTTP request exception handling in `PollingConfigManager`. ([#285](https://github.com/optimizely/python-sdk/pull/285))
-
-## 3.5.0
-July 9th, 2020
-
-### New Features:
-* Introduced 2 APIs to interact with feature variables:
-  * `get_feature_variable_json` allows you to get value for JSON variables related to a feature.
-  * `get_all_feature_variables` gets values for all variables under a feature.
-* Added support for fetching authenticated datafiles. `AuthDatafilePollingConfigManager` is a new config manager that allows you to poll for a datafile belonging to a secure environment. You can create a client by setting the `datafile_access_token`.
-
-### Bug Fixes:
-* Fixed log messages for targeted rollouts evaluation. ([#268](https://github.com/optimizely/python-sdk/pull/268))
-
-## 3.4.2
-June 11th, 2020
-
-### Bug Fixes:
-* Adjusted log level for audience evaluation logs. ([#267](https://github.com/optimizely/python-sdk/pull/267))
-
-## 3.4.1
-March 19th, 2020
-
-### Bug Fixes:
-* Updated `jsonschema` to address [installation issue](https://github.com/optimizely/python-sdk/issues/232).
-
-## 3.4.0
-January 27th, 2020
-
-### New Features:
-* Added a new API to get project configuration static data.
-  * Call `get_optimizely_config()` to get a snapshot of project configuration static data.
-  * It returns an `OptimizelyConfig` instance which includes a datafile revision number, all experiments, and feature flags mapped by their key values.
-  * Added caching for `get_optimizely_config()` - `OptimizelyConfig` object will be cached and reused for the lifetime of the datafile.
-  * For details, refer to our documentation page: [https://docs.developers.optimizely.com/full-stack/docs/optimizelyconfig-python](https://docs.developers.optimizely.com/full-stack/docs/optimizelyconfig-python).
-
-
-## 3.3.1
-December 16th, 2019
-
-### Bug Fixes:
-* Fixed [installation issue](https://github.com/optimizely/python-sdk/issues/220) on Windows. ([#224](https://github.com/optimizely/python-sdk/pull/224))
-* Fixed batch event processor deadline reset issue. ([#227](https://github.com/optimizely/python-sdk/pull/227))
-* Added more batch event processor debug messages. ([#227](https://github.com/optimizely/python-sdk/pull/227))
-
-## 3.3.0
-October 28th, 2019
-
-### New Features:
-* Added support for event batching via the event processor.
-  * Events generated by methods like `activate`, `track`, and `is_feature_enabled` will be held in a queue until the configured batch size is reached, or the configured flush interval has elapsed. Then, they will be batched into a single payload and sent to the event dispatcher.
-  * To configure event batching, set the `batch_size` and `flush_interval` properties when initializing instance of [BatchEventProcessor](https://github.com/optimizely/python-sdk/blob/3.3.x/optimizely/event/event_processor.py#L45).
-  * Event batching is disabled by default. You can pass in instance of `BatchEventProcessor` when creating `Optimizely` instance to enable event batching.
-  * Users can subscribe to `LogEvent` notification to be notified of whenever a payload consisting of a batch of user events is handed off to the event dispatcher to send to Optimizely's backend.
-* Introduced blocking timeout in `PollingConfigManager`. By default, calls to `get_config` will block for maximum of 10 seconds until config is available.
-
-### Bug Fixes:
-* Fixed incorrect log message when numeric metric is not used. ([#217](https://github.com/optimizely/python-sdk/pull/217))
-
-## 3.2.0
-August 27th, 2019
-
-### New Features:
-* Added support for automatic datafile management via [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151):
-  * The [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151) is an implementation of the [BaseConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L32).
-  * Users may provide one of datafile or SDK key (sdk_key) or both to `optimizely.Optimizely`. Based on that, the SDK will use the [StaticConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L73) or the [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151). Refer to the [README](README.md) for more instructions.
-  * An initial datafile can be provided to the `PollingConfigManager` to bootstrap before making HTTP requests for the hosted datafile.
-  * Requests for the datafile are made in a separate thread and are scheduled with fixed delay.
-  * Configuration updates can be subscribed to by adding the OPTIMIZELY_CONFIG_UPDATE notification listener.
-* Introduced `Optimizely.get_feature_variable` API.  ([#191](https://github.com/optimizely/python-sdk/pull/191))
-
-### Deprecated:
-
-* `NotificationCenter.clear_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
-* `NotificationCenter.clear_all_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_all_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
-
-## 3.2.0b1
-July 26th, 2019
-
-### New Features:
-* Added support for automatic datafile management via [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151):
-  * The [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151) is an implementation of the [BaseConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L32).
-  * Users may provide one of datafile or SDK key (sdk_key) or both to `optimizely.Optimizely`. Based on that, the SDK will use the [StaticConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L73) or the [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151). Refer to the [README](README.md) for more instructions.
-  * An initial datafile can be provided to the `PollingConfigManager` to bootstrap before making HTTP requests for the hosted datafile.
-  * Requests for the datafile are made in a separate thread and are scheduled with fixed delay.
-  * Configuration updates can be subscribed to by adding the OPTIMIZELY_CONFIG_UPDATE notification listener.
-* Introduced `Optimizely.get_feature_variable` API.  ([#191](https://github.com/optimizely/python-sdk/pull/191))
-
-### Deprecated:
-
-* `NotificationCenter.clear_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
-* `NotificationCenter.clear_all_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_all_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
-
-## 3.1.0
-May 3rd, 2019
-
-### New Features:
-* Introduced Decision notification listener to be able to record:
-  * Variation assignments for users activated in an experiment.
-  * Feature access for users.
-  * Feature variable value for users.
-
-### Bug Fixes:
-* Feature variable APIs now return default variable value when featureEnabled property is false.  ([#171](https://github.com/optimizely/python-sdk/pull/171))
-
-### Deprecated:
-* Activate notification listener is deprecated as of this release.  Recommendation is to use the new Decision notification listener.  Activate notification listener will be removed in the next major release.
-
-## 3.0.0
-March 1st, 2019
-
-The 3.0 release improves event tracking and supports additional audience
-targeting functionality.
-
-### New Features:
-* Event tracking:
-  * The `track` method now dispatches its conversion event *unconditionally*, without first determining whether the user is targeted by a known experiment that uses the event. This may increase outbound network traffic.
-  * In Optimizely results, conversion events sent by 3.0 SDKs don\'t explicitly name the experiments and variations that are currently targeted to the user. Instead, conversions are automatically attributed to variations that the user has previously seen, as long as those variations were served via 3.0 SDKs or by other clients capable of automatic attribution, and as long as our backend actually received the impression events for those variations.
-  * Altogether, this allows you to track conversion events and attribute them to variations even when you don't know all of a user's attribute values, and even if the user's attribute values or the experiment's configuration have changed such that the user is no longer affected by the experiment. As a result, **you may observe an increase in the conversion rate for previously-instrumented events.** If that is undesirable, you can reset the results of previously-running experiments after upgrading to the 3.0 SDK.  -   This will also allow you to attribute events to variations from other Optimizely projects in your account, even though those experiments don't appear in the same datafile.
-  * Note that for results segmentation in Optimizely results, the user attribute values from one event are automatically applied to all other events in the same session, as long as the events in question were actually received by our backend. This behavior was already in place and is not affected by the 3.0 release.
-* Support for all types of attribute values, not just strings.
-  * All values are passed through to notification listeners.
-  * Strings, booleans, and valid numbers are passed to the event dispatcher and can be used for Optimizely results segmentation.  A valid number is a finite float or numbers.Integral in the inclusive range \[-2 ^ 53, 2 ^ 53\].
-  * Strings, booleans, and valid numbers are relevant for audience conditions.
-* Support for additional matchers in audience conditions:
-  * An `exists` matcher that passes if the user has a non-null value for the targeted user attribute and fails otherwise.
-  * A `substring` matcher that resolves if the user has a string value for the targeted attribute.
-    * `gt` (greater than) and `lt` (less than) matchers that resolve if the user has a valid number value for the targeted attribute.  A valid number is a finite float or numbers.Integral in the inclusive range \[-2 ^ 53, 2 ^ 53\].
-    * The original (`exact`) matcher can now be used to target booleans and valid numbers, not just strings.
-* Support for A/B tests, feature tests, and feature rollouts whose audiences are combined using `"and"` and `"not"` operators, not just the `"or"` operator.
-* Datafile-version compatibility check: The SDK will remain uninitialized (i.e., will gracefully fail to activate experiments and features) if given a datafile version greater than 4.
-* Updated Pull Request template and commit message guidelines.
-
-### Breaking Changes:
-* Conversion events sent by 3.0 SDKs don\'t explicitly name the experiments and variations that are currently targeted to the user, so these events are unattributed in raw events data export. You must use the new *results* export to determine the variations to which events have been attributed.
-* Previously, notification listeners were only given string-valued user attributes because only strings could be passed into various method calls. That is no longer the case. You may pass non-string attribute values, and if you do, you must update your notification listeners to be able to receive whatever values you pass in.
-
-### Bug Fixes:
-* Experiments and features can no longer activate when a negatively targeted attribute has a missing, null, or malformed value.
-  * Audience conditions (except for the new `exists` matcher) no longer resolve to `false` when they fail to find an legitimate value for the targeted user attribute. The result remains `null` (unknown). Therefore, an audience that negates such a condition (using the `"not"` operator) can no longer resolve to `true` unless there is an unrelated branch in the condition tree that itself resolves to `true`.
-* Updated the default event dispatcher to log an error if the request resolves to HTTP 4xx or 5xx.  ([#140](https://github.com/optimizely/python-sdk/pull/140))
-* All methods now validate that user IDs are strings and that experiment keys, feature keys, feature variable keys, and event keys are non-empty strings.
-
-## 2.1.1
-August 21st, 2018
-
-* Fix: record conversions for all experiments using an event when using track([#136](https://github.com/optimizely/python-sdk/pull/136)).
-
-## 2.1.0
-July 2nd, 2018
-
-* Introduced support for bot filtering ([#121](https://github.com/optimizely/python-sdk/pull/121)).
-* Overhauled logging to use standard Python logging ([#123](https://github.com/optimizely/python-sdk/pull/123)).
-
-## 2.0.1
-June 19th, 2018
-
-* Fix: send impression event for Feature Test when Feature is disabled ([#128](https://github.com/optimizely/python-sdk/pull/128)).
-
-## 2.0.0
-April 12th, 2018
-
-This major release introduces APIs for Feature Management. It also
-introduces some breaking changes listed below.
-
-### New Features
-* Introduced the `is_feature_enabled` API to determine whether to show a feature to a user or not.
-
-```
-    is_enabled = optimizel_client.is_feature_enabled('my_feature_key', 'my_user', user_attributes)
-```
-
-* All enabled features for the user can be retrieved by calling:
-
-```
-    enabled_features = optimizely_client.get_enabled_features('my_user', user_attributes)
-```
-* Introduced Feature Variables to configure or parameterize a feature.  There are four variable types: `String`, `Integer`, `Double`, `Boolean`.
-
-```
-    string_variable = optimizely_client.get_feature_variable_string('my_feature_key', 'string_variable_key', 'my_user')
-    integer_variable = optimizely_client.get_feature_variable_integer('my_feature_key', 'integer_variable_key', 'my_user')
-    double_variable = optimizely_client.get_feature_variable_double('my_feature_key', 'double_variable_key', 'my_user')
-    boolean_variable = optimizely_client.get_feature_variable_boolean('my_feature_key', 'boolean_variable_key', 'my_user')
-```
-
-### Breaking changes
-* The `track` API with revenue value as a stand-alone parameter has been removed. The revenue value should be passed in as an entry in the event tags dict. The key for the revenue tag is `revenue` and the passed in value will be treated by Optimizely as the value for computing results.
-
-```
-    event_tags = {
-      'revenue': 1200
-    }
-
-    optimizely_client.track('event_key', 'my_user', user_attributes, event_tags)
-```
-
-## 2.0.0b1
-March 29th, 2018
-
-This beta release introduces APIs for Feature Management. It also
-introduces some breaking changes listed below.
-
-### New Features
-* Introduced the `is_feature_enabled` API to determine whether to show a feature to a user or not.
-```
-    is_enabled = optimizel_client.is_feature_enabled('my_feature_key', 'my_user', user_attributes)
-```
-
-* All enabled features for the user can be retrieved by calling:
-
-```
-    enabled_features = optimizely_client.get_enabled_features('my_user', user_attributes)
-```
-
-* Introduced Feature Variables to configure or parameterize a feature.  There are four variable types: `String`, `Integer`, `Double`, `Boolean`.
-
-```
-    string_variable = optimizely_client.get_feature_variable_string('my_feature_key', 'string_variable_key', 'my_user')
-    integer_variable = optimizely_client.get_feature_variable_integer('my_feature_key', 'integer_variable_key', 'my_user')
-    double_variable = optimizely_client.get_feature_variable_double('my_feature_key', 'double_variable_key', 'my_user')
-    boolean_variable = optimizely_client.get_feature_variable_boolean('my_feature_key', 'boolean_variable_key', 'my_user')
-```
-
-### Breaking changes
-* The `track` API with revenue value as a stand-alone parameter has been removed. The revenue value should be passed in as an entry in the event tags dict. The key for the revenue tag is `revenue` and the passed in value will be treated by Optimizely as the value for computing results.
-
-```
-    event_tags = {
-      'revenue': 1200
-    }
-
-    optimizely_client.track('event_key', 'my_user', user_attributes, event_tags)
-```
-
-## 1.4.0
-
-* Added support for IP anonymization.
-* Added support for notification listeners.
-* Added support for bucketing ID.
-* Updated mmh3 to handle installation failures on Windows 10.
-
-## 1.3.0
-
-* Introduced support for forced bucketing.
-* Introduced support for numeric metrics.
-* Updated event builder to support new endpoint.
-
-## 1.2.1
-
-* Removed older feature flag parsing.
-
-## 1.2.0
-
-* Added user profile service.
-
-## 1.1.1
-
-* Updated datafile parsing to be able to handle additional fields.
-* Deprecated Classic project support.
-
-## 1.1.0
-
-* Included datafile revision information in log events.
-* Added event tags to track API to allow users to pass in event metadata.
-* Deprecated the `event_value` parameter from the track method. Should use `event_tags` to pass in event value instead.
-* Updated event logging endpoint to logx.optimizely.com.
-
-## 1.0.0
-
-* Introduced support for Full Stack projects in Optimizely X. No breaking changes from previous version.
-* Introduced more graceful exception handling in instantiation and core methods.
-* Updated whitelisting to precede audience matching.
-
-## 0.1.3
-
-* Added support for v2 endpoint and datafile.
-* Updated dispatch_event to consume an Event object instead of url and params. The Event object comprises of four properties: url (string representing URL to dispatch event to), params (dict representing the params to be set for the event), http_verb (one of 'GET' or 'POST') and headers (header values to be sent along).
-* Fixed issue with tracking events for experiments in groups.
-
-## 0.1.2
-
-* Updated requirements file.
-
-## 0.1.1
-
-* Introduced option to skip JSON schema validation.
-
-## 0.1.0
-
-* Beta release of the Python SDK for server-side testing.
+# Optimizely Python SDK Changelog
+
+## 5.0.0-beta
+Apr 28th, 2023
+
+### New Features  
+
+The 5.0.0-beta release introduces a new primary feature, [Advanced Audience Targeting]( https://docs.developers.optimizely.com/feature-experimentation/docs/optimizely-data-platform-advanced-audience-targeting) enabled through integration with [Optimizely Data Platform (ODP)](https://docs.developers.optimizely.com/optimizely-data-platform/docs) ([#395](https://github.com/optimizely/python-sdk/pull/395), [#398](https://github.com/optimizely/python-sdk/pull/398), [#402](https://github.com/optimizely/python-sdk/pull/402), [#403](https://github.com/optimizely/python-sdk/pull/403), [#405](https://github.com/optimizely/python-sdk/pull/405)).  
+
+You can use ODP, a high-performance [Customer Data Platform (CDP)]( https://www.optimizely.com/optimization-glossary/customer-data-platform/), to easily create complex real-time segments (RTS) using first-party and 50+ third-party data sources out of the box. You can create custom schemas that support the user attributes important for your business, and stitch together user behavior done on different devices to better understand and target your customers for personalized user experiences. ODP can be used as a single source of truth for these segments in any Optimizely or 3rd party tool. 
+
+With ODP accounts integrated into Optimizely projects, you can build audiences using segments pre-defined in ODP. The SDK will fetch the segments for given users and make decisions using the segments. For access to ODP audience targeting in your Feature Experimentation account, please contact your Optimizely Customer Success Manager. 
+
+This version includes the following changes: 
+
+* New API added to `OptimizelyUserContext`: 
+
+  * `fetchQualifiedSegments()`: this API will retrieve user segments from the ODP server. The fetched segments will be used for audience evaluation. The fetched data will be stored in the local cache to avoid repeated network delays.
+  * When an `OptimizelyUserContext` is created, the SDK will automatically send an identify request to the ODP server to facilitate observing user activities. 
+
+* New APIs added to `OptimizelyClient`: 
+
+  * `sendOdpEvent()`: customers can build/send arbitrary ODP events that will bind user identifiers and data to user profiles in ODP.
+
+For details, refer to our documentation pages:  
+
+* [Advanced Audience Targeting](https://docs.developers.optimizely.com/feature-experimentation/docs/optimizely-data-platform-advanced-audience-targeting)  
+* [Server SDK Support](https://docs.developers.optimizely.com/feature-experimentation/v1.0/docs/advanced-audience-targeting-for-server-side-sdks) 
+* [Initialize Python SDK](https://docs.developers.optimizely.com/feature-experimentation/docs/initialize-sdk-python) 
+* [OptimizelyUserContext Python SDK](https://docs.developers.optimizely.com/feature-experimentation/docs/wip-fsodp-optimizelyusercontext-python) 
+* [Advanced Audience Targeting segment qualification methods](https://docs.developers.optimizely.com/feature-experimentation/v1.0/docs/advanced-audience-targeting-segment-qualification-methods-python) 
+* [Send Optimizely Data Platform data using Advanced Audience Targeting](https://docs.developers.optimizely.com/feature-experimentation/v1.0/docs/send-odp-data-using-advanced-audience-targeting-python) 
+
+### Breaking Changes 
+
+* `ODPManager` in the SDK is enabled by default. Unless an ODP account is integrated into the Optimizely projects, most `ODPManager` functions will be ignored. If needed, `ODPManager` can be disabled when `OptimizelyClient` is instantiated. 
+* `BaseConfigManager` abstract class now requires a get_sdk_key method. ([#413](https://github.com/optimizely/python-sdk/pull/413))
+* `PollingConfigManager` requires either the sdk_key parameter or datafile containing an sdkKey. ([#413](https://github.com/optimizely/python-sdk/pull/413))
+* Asynchronous `BatchEventProcessor` is now the default event processor. ([#378](https://github.com/optimizely/python-sdk/pull/378))
+
+## 4.1.1
+March 10th, 2023
+
+We updated our README.md and other non-functional code to reflect that this SDK supports both Optimizely Feature Experimentation and Optimizely Full Stack. ([#420](https://github.com/optimizely/python-sdk/pull/420))
+
+## 4.1.0
+July 7th, 2022
+
+### Bug Fixes
+* Fix invalid datafile returned from `ProjectConfig.to_datafile` and `OptimizelyConfig.get_datafile` ([#321](https://github.com/optimizely/python-sdk/pull/321), [#384](https://github.com/optimizely/python-sdk/pull/384))
+
+## 4.0.0
+January 12th, 2022
+
+### New Features
+* Add a set of new APIs for overriding and managing user-level flag, experiment and delivery rule decisions. These methods can be used for QA and automated testing purposes. They are an extension of the OptimizelyUserContext interface ([#361](https://github.com/optimizely/python-sdk/pull/361), [#365](https://github.com/optimizely/python-sdk/pull/365), [#369](https://github.com/optimizely/python-sdk/pull/369)):
+	- setForcedDecision
+	- getForcedDecision
+	- removeForcedDecision
+	- removeAllForcedDecisions
+
+* For details, refer to our documentation pages: [OptimizelyUserContext](https://docs.developers.optimizely.com/full-stack/v4.0/docs/optimizelyusercontext-python) and [Forced Decision methods](https://docs.developers.optimizely.com/full-stack/v4.0/docs/forced-decision-methods-python).
+
+### Breaking Changes:
+
+* Support for `Python v3.4` has been dropped as of this release due to a security vulnerability with `PyYAML <v5.4`. ([#366](https://github.com/optimizely/python-sdk/pull/366))
+* We no longer support `Python v2.7, v3.5, and v3.6` including `PyPy` as of this release. ([#377](https://github.com/optimizely/python-sdk/pull/373))
+* We now support `Python v3.7 and above` including `PyPy3`.
+
+## 3.10.0
+September 16th, 2021
+
+### New Features
+* Added new public properties to OptimizelyConfig.
+  - sdk_key and environment_key [#338] (https://github.com/optimizely/python-sdk/pull/338)
+  - attributes and events [#339] (https://github.com/optimizely/python-sdk/pull/339)
+  - experiment_rules, delivery_rules, audiences and audiences in OptimizelyExperiment
+    - [#342] (https://github.com/optimizely/python-sdk/pull/342)
+    - [#351] (https://github.com/optimizely/python-sdk/pull/351/files)
+* For details please refer to our documentation page:
+  - Python-sdk: [https://docs.developers.optimizely.com/full-stack/docs/optimizelyconfig-python]
+
+* OptimizelyFeature.experiments_map of OptimizelyConfig is now deprecated. Please use OptimizelyFeature.experiment_rules and OptimizelyFeature.delivery_rules. [#360] (https://github.com/optimizely/python-sdk/pull/360)
+
+### Bug Fixes
+* Fix event processor negative timeout interval when retrieving events from queue. [#356] (https://github.com/optimizely/python-sdk/pull/356)
+
+## 3.9.1
+July 14th, 2021
+
+### Bug Fixes:
+* Fixed issue with serving incorrect variation in projects containing multiple flags with duplicate keys. [#347] (https://github.com/optimizely/python-sdk/pull/347)
+* Fixed issue with serving incorrect variation in create_impression_event in user_event_factory.py. [#350] (https://github.com/optimizely/python-sdk/pull/350)
+
+## 3.9.0
+June 1st, 2021
+
+### New Features
+* Added support for multiple concurrent prioritized experiments per flag. [#322](https://github.com/optimizely/python-sdk/pull/322)
+
+## 3.8.0
+February 12th, 2021
+
+### New Features
+* New Features
+Introducing a new primary interface for retrieving feature flag status, configuration and associated experiment decisions for users ([#309](https://github.com/optimizely/python-sdk/pull/309)). The new `OptimizelyUserContext` class is instantiated with `create_user_context` and exposes the following APIs to get `OptimizelyDecision`:
+
+    - set_attribute
+    - decide
+    - decide_all
+    - decide_for_keys
+    - track_event
+
+For details, refer to our documentation page: https://docs.developers.optimizely.com/full-stack/v4.0/docs/python-sdk.
+
+## 3.7.1
+November 19th, 2020
+
+### Bug Fixes:
+* Added "enabled" field to decision metadata structure. [#306](https://github.com/optimizely/python-sdk/pull/306)
+
+## 3.7.0
+November 2nd, 2020
+
+### New Features
+* Added support for upcoming application-controlled introduction of tracking for non-experiment Flag decisions. [#300](https://github.com/optimizely/python-sdk/pull/300)
+
+## 3.6.0
+October 1st, 2020
+
+### New Features:
+* Version targeting using semantic version syntax. [#293](https://github.com/optimizely/python-sdk/pull/293)
+* Datafile accessor API added to access current config as a JSON string. [#283](https://github.com/optimizely/python-sdk/pull/283)
+
+### Bug Fixes:
+* Fixed package installation for Python 3.4 and pypy. [#298](https://github.com/optimizely/python-sdk/pull/298)
+
+## 3.5.2
+July 14th, 2020
+
+### Bug Fixes:
+* Fixed handling of network and no status code errors when polling for datafile in `PollingConfigManager` and `AuthDatafilePollingConfigManager`. ([#287](https://github.com/optimizely/python-sdk/pull/287))
+
+## 3.5.1
+July 10th, 2020
+
+### Bug Fixes:
+* Fixed HTTP request exception handling in `PollingConfigManager`. ([#285](https://github.com/optimizely/python-sdk/pull/285))
+
+## 3.5.0
+July 9th, 2020
+
+### New Features:
+* Introduced 2 APIs to interact with feature variables:
+  * `get_feature_variable_json` allows you to get value for JSON variables related to a feature.
+  * `get_all_feature_variables` gets values for all variables under a feature.
+* Added support for fetching authenticated datafiles. `AuthDatafilePollingConfigManager` is a new config manager that allows you to poll for a datafile belonging to a secure environment. You can create a client by setting the `datafile_access_token`.
+
+### Bug Fixes:
+* Fixed log messages for targeted rollouts evaluation. ([#268](https://github.com/optimizely/python-sdk/pull/268))
+
+## 3.4.2
+June 11th, 2020
+
+### Bug Fixes:
+* Adjusted log level for audience evaluation logs. ([#267](https://github.com/optimizely/python-sdk/pull/267))
+
+## 3.4.1
+March 19th, 2020
+
+### Bug Fixes:
+* Updated `jsonschema` to address [installation issue](https://github.com/optimizely/python-sdk/issues/232).
+
+## 3.4.0
+January 27th, 2020
+
+### New Features:
+* Added a new API to get project configuration static data.
+  * Call `get_optimizely_config()` to get a snapshot of project configuration static data.
+  * It returns an `OptimizelyConfig` instance which includes a datafile revision number, all experiments, and feature flags mapped by their key values.
+  * Added caching for `get_optimizely_config()` - `OptimizelyConfig` object will be cached and reused for the lifetime of the datafile.
+  * For details, refer to our documentation page: [https://docs.developers.optimizely.com/full-stack/docs/optimizelyconfig-python](https://docs.developers.optimizely.com/full-stack/docs/optimizelyconfig-python).
+
+
+## 3.3.1
+December 16th, 2019
+
+### Bug Fixes:
+* Fixed [installation issue](https://github.com/optimizely/python-sdk/issues/220) on Windows. ([#224](https://github.com/optimizely/python-sdk/pull/224))
+* Fixed batch event processor deadline reset issue. ([#227](https://github.com/optimizely/python-sdk/pull/227))
+* Added more batch event processor debug messages. ([#227](https://github.com/optimizely/python-sdk/pull/227))
+
+## 3.3.0
+October 28th, 2019
+
+### New Features:
+* Added support for event batching via the event processor.
+  * Events generated by methods like `activate`, `track`, and `is_feature_enabled` will be held in a queue until the configured batch size is reached, or the configured flush interval has elapsed. Then, they will be batched into a single payload and sent to the event dispatcher.
+  * To configure event batching, set the `batch_size` and `flush_interval` properties when initializing instance of [BatchEventProcessor](https://github.com/optimizely/python-sdk/blob/3.3.x/optimizely/event/event_processor.py#L45).
+  * Event batching is disabled by default. You can pass in instance of `BatchEventProcessor` when creating `Optimizely` instance to enable event batching.
+  * Users can subscribe to `LogEvent` notification to be notified of whenever a payload consisting of a batch of user events is handed off to the event dispatcher to send to Optimizely's backend.
+* Introduced blocking timeout in `PollingConfigManager`. By default, calls to `get_config` will block for maximum of 10 seconds until config is available.
+
+### Bug Fixes:
+* Fixed incorrect log message when numeric metric is not used. ([#217](https://github.com/optimizely/python-sdk/pull/217))
+
+## 3.2.0
+August 27th, 2019
+
+### New Features:
+* Added support for automatic datafile management via [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151):
+  * The [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151) is an implementation of the [BaseConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L32).
+  * Users may provide one of datafile or SDK key (sdk_key) or both to `optimizely.Optimizely`. Based on that, the SDK will use the [StaticConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L73) or the [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151). Refer to the [README](README.md) for more instructions.
+  * An initial datafile can be provided to the `PollingConfigManager` to bootstrap before making HTTP requests for the hosted datafile.
+  * Requests for the datafile are made in a separate thread and are scheduled with fixed delay.
+  * Configuration updates can be subscribed to by adding the OPTIMIZELY_CONFIG_UPDATE notification listener.
+* Introduced `Optimizely.get_feature_variable` API.  ([#191](https://github.com/optimizely/python-sdk/pull/191))
+
+### Deprecated:
+
+* `NotificationCenter.clear_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
+* `NotificationCenter.clear_all_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_all_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
+
+## 3.2.0b1
+July 26th, 2019
+
+### New Features:
+* Added support for automatic datafile management via [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151):
+  * The [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151) is an implementation of the [BaseConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L32).
+  * Users may provide one of datafile or SDK key (sdk_key) or both to `optimizely.Optimizely`. Based on that, the SDK will use the [StaticConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L73) or the [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151). Refer to the [README](README.md) for more instructions.
+  * An initial datafile can be provided to the `PollingConfigManager` to bootstrap before making HTTP requests for the hosted datafile.
+  * Requests for the datafile are made in a separate thread and are scheduled with fixed delay.
+  * Configuration updates can be subscribed to by adding the OPTIMIZELY_CONFIG_UPDATE notification listener.
+* Introduced `Optimizely.get_feature_variable` API.  ([#191](https://github.com/optimizely/python-sdk/pull/191))
+
+### Deprecated:
+
+* `NotificationCenter.clear_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
+* `NotificationCenter.clear_all_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_all_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
+
+## 3.1.0
+May 3rd, 2019
+
+### New Features:
+* Introduced Decision notification listener to be able to record:
+  * Variation assignments for users activated in an experiment.
+  * Feature access for users.
+  * Feature variable value for users.
+
+### Bug Fixes:
+* Feature variable APIs now return default variable value when featureEnabled property is false.  ([#171](https://github.com/optimizely/python-sdk/pull/171))
+
+### Deprecated:
+* Activate notification listener is deprecated as of this release.  Recommendation is to use the new Decision notification listener.  Activate notification listener will be removed in the next major release.
+
+## 3.0.0
+March 1st, 2019
+
+The 3.0 release improves event tracking and supports additional audience
+targeting functionality.
+
+### New Features:
+* Event tracking:
+  * The `track` method now dispatches its conversion event *unconditionally*, without first determining whether the user is targeted by a known experiment that uses the event. This may increase outbound network traffic.
+  * In Optimizely results, conversion events sent by 3.0 SDKs don\'t explicitly name the experiments and variations that are currently targeted to the user. Instead, conversions are automatically attributed to variations that the user has previously seen, as long as those variations were served via 3.0 SDKs or by other clients capable of automatic attribution, and as long as our backend actually received the impression events for those variations.
+  * Altogether, this allows you to track conversion events and attribute them to variations even when you don't know all of a user's attribute values, and even if the user's attribute values or the experiment's configuration have changed such that the user is no longer affected by the experiment. As a result, **you may observe an increase in the conversion rate for previously-instrumented events.** If that is undesirable, you can reset the results of previously-running experiments after upgrading to the 3.0 SDK.  -   This will also allow you to attribute events to variations from other Optimizely projects in your account, even though those experiments don't appear in the same datafile.
+  * Note that for results segmentation in Optimizely results, the user attribute values from one event are automatically applied to all other events in the same session, as long as the events in question were actually received by our backend. This behavior was already in place and is not affected by the 3.0 release.
+* Support for all types of attribute values, not just strings.
+  * All values are passed through to notification listeners.
+  * Strings, booleans, and valid numbers are passed to the event dispatcher and can be used for Optimizely results segmentation.  A valid number is a finite float or numbers.Integral in the inclusive range \[-2 ^ 53, 2 ^ 53\].
+  * Strings, booleans, and valid numbers are relevant for audience conditions.
+* Support for additional matchers in audience conditions:
+  * An `exists` matcher that passes if the user has a non-null value for the targeted user attribute and fails otherwise.
+  * A `substring` matcher that resolves if the user has a string value for the targeted attribute.
+    * `gt` (greater than) and `lt` (less than) matchers that resolve if the user has a valid number value for the targeted attribute.  A valid number is a finite float or numbers.Integral in the inclusive range \[-2 ^ 53, 2 ^ 53\].
+    * The original (`exact`) matcher can now be used to target booleans and valid numbers, not just strings.
+* Support for A/B tests, feature tests, and feature rollouts whose audiences are combined using `"and"` and `"not"` operators, not just the `"or"` operator.
+* Datafile-version compatibility check: The SDK will remain uninitialized (i.e., will gracefully fail to activate experiments and features) if given a datafile version greater than 4.
+* Updated Pull Request template and commit message guidelines.
+
+### Breaking Changes:
+* Conversion events sent by 3.0 SDKs don\'t explicitly name the experiments and variations that are currently targeted to the user, so these events are unattributed in raw events data export. You must use the new *results* export to determine the variations to which events have been attributed.
+* Previously, notification listeners were only given string-valued user attributes because only strings could be passed into various method calls. That is no longer the case. You may pass non-string attribute values, and if you do, you must update your notification listeners to be able to receive whatever values you pass in.
+
+### Bug Fixes:
+* Experiments and features can no longer activate when a negatively targeted attribute has a missing, null, or malformed value.
+  * Audience conditions (except for the new `exists` matcher) no longer resolve to `false` when they fail to find an legitimate value for the targeted user attribute. The result remains `null` (unknown). Therefore, an audience that negates such a condition (using the `"not"` operator) can no longer resolve to `true` unless there is an unrelated branch in the condition tree that itself resolves to `true`.
+* Updated the default event dispatcher to log an error if the request resolves to HTTP 4xx or 5xx.  ([#140](https://github.com/optimizely/python-sdk/pull/140))
+* All methods now validate that user IDs are strings and that experiment keys, feature keys, feature variable keys, and event keys are non-empty strings.
+
+## 2.1.1
+August 21st, 2018
+
+* Fix: record conversions for all experiments using an event when using track([#136](https://github.com/optimizely/python-sdk/pull/136)).
+
+## 2.1.0
+July 2nd, 2018
+
+* Introduced support for bot filtering ([#121](https://github.com/optimizely/python-sdk/pull/121)).
+* Overhauled logging to use standard Python logging ([#123](https://github.com/optimizely/python-sdk/pull/123)).
+
+## 2.0.1
+June 19th, 2018
+
+* Fix: send impression event for Feature Test when Feature is disabled ([#128](https://github.com/optimizely/python-sdk/pull/128)).
+
+## 2.0.0
+April 12th, 2018
+
+This major release introduces APIs for Feature Management. It also
+introduces some breaking changes listed below.
+
+### New Features
+* Introduced the `is_feature_enabled` API to determine whether to show a feature to a user or not.
+
+```
+    is_enabled = optimizel_client.is_feature_enabled('my_feature_key', 'my_user', user_attributes)
+```
+
+* All enabled features for the user can be retrieved by calling:
+
+```
+    enabled_features = optimizely_client.get_enabled_features('my_user', user_attributes)
+```
+* Introduced Feature Variables to configure or parameterize a feature.  There are four variable types: `String`, `Integer`, `Double`, `Boolean`.
+
+```
+    string_variable = optimizely_client.get_feature_variable_string('my_feature_key', 'string_variable_key', 'my_user')
+    integer_variable = optimizely_client.get_feature_variable_integer('my_feature_key', 'integer_variable_key', 'my_user')
+    double_variable = optimizely_client.get_feature_variable_double('my_feature_key', 'double_variable_key', 'my_user')
+    boolean_variable = optimizely_client.get_feature_variable_boolean('my_feature_key', 'boolean_variable_key', 'my_user')
+```
+
+### Breaking changes
+* The `track` API with revenue value as a stand-alone parameter has been removed. The revenue value should be passed in as an entry in the event tags dict. The key for the revenue tag is `revenue` and the passed in value will be treated by Optimizely as the value for computing results.
+
+```
+    event_tags = {
+      'revenue': 1200
+    }
+
+    optimizely_client.track('event_key', 'my_user', user_attributes, event_tags)
+```
+
+## 2.0.0b1
+March 29th, 2018
+
+This beta release introduces APIs for Feature Management. It also
+introduces some breaking changes listed below.
+
+### New Features
+* Introduced the `is_feature_enabled` API to determine whether to show a feature to a user or not.
+```
+    is_enabled = optimizel_client.is_feature_enabled('my_feature_key', 'my_user', user_attributes)
+```
+
+* All enabled features for the user can be retrieved by calling:
+
+```
+    enabled_features = optimizely_client.get_enabled_features('my_user', user_attributes)
+```
+
+* Introduced Feature Variables to configure or parameterize a feature.  There are four variable types: `String`, `Integer`, `Double`, `Boolean`.
+
+```
+    string_variable = optimizely_client.get_feature_variable_string('my_feature_key', 'string_variable_key', 'my_user')
+    integer_variable = optimizely_client.get_feature_variable_integer('my_feature_key', 'integer_variable_key', 'my_user')
+    double_variable = optimizely_client.get_feature_variable_double('my_feature_key', 'double_variable_key', 'my_user')
+    boolean_variable = optimizely_client.get_feature_variable_boolean('my_feature_key', 'boolean_variable_key', 'my_user')
+```
+
+### Breaking changes
+* The `track` API with revenue value as a stand-alone parameter has been removed. The revenue value should be passed in as an entry in the event tags dict. The key for the revenue tag is `revenue` and the passed in value will be treated by Optimizely as the value for computing results.
+
+```
+    event_tags = {
+      'revenue': 1200
+    }
+
+    optimizely_client.track('event_key', 'my_user', user_attributes, event_tags)
+```
+
+## 1.4.0
+
+* Added support for IP anonymization.
+* Added support for notification listeners.
+* Added support for bucketing ID.
+* Updated mmh3 to handle installation failures on Windows 10.
+
+## 1.3.0
+
+* Introduced support for forced bucketing.
+* Introduced support for numeric metrics.
+* Updated event builder to support new endpoint.
+
+## 1.2.1
+
+* Removed older feature flag parsing.
+
+## 1.2.0
+
+* Added user profile service.
+
+## 1.1.1
+
+* Updated datafile parsing to be able to handle additional fields.
+* Deprecated Classic project support.
+
+## 1.1.0
+
+* Included datafile revision information in log events.
+* Added event tags to track API to allow users to pass in event metadata.
+* Deprecated the `event_value` parameter from the track method. Should use `event_tags` to pass in event value instead.
+* Updated event logging endpoint to logx.optimizely.com.
+
+## 1.0.0
+
+* Introduced support for Full Stack projects in Optimizely X. No breaking changes from previous version.
+* Introduced more graceful exception handling in instantiation and core methods.
+* Updated whitelisting to precede audience matching.
+
+## 0.1.3
+
+* Added support for v2 endpoint and datafile.
+* Updated dispatch_event to consume an Event object instead of url and params. The Event object comprises of four properties: url (string representing URL to dispatch event to), params (dict representing the params to be set for the event), http_verb (one of 'GET' or 'POST') and headers (header values to be sent along).
+* Fixed issue with tracking events for experiments in groups.
+
+## 0.1.2
+
+* Updated requirements file.
+
+## 0.1.1
+
+* Introduced option to skip JSON schema validation.
+
+## 0.1.0
+
+* Beta release of the Python SDK for server-side testing.
```

### Comparing `optimizely-sdk-4.1.1/LICENSE` & `optimizely-sdk-5.0.0b0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2016 Optimizely
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2016 Optimizely
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `optimizely-sdk-4.1.1/PKG-INFO` & `optimizely-sdk-5.0.0b0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,683 +1,717 @@
-Metadata-Version: 2.1
-Name: optimizely-sdk
-Version: 4.1.1
-Summary: Python SDK for Optimizely Feature Experimentation, Optimizely Full Stack (legacy), and Optimizely Rollouts.
-Home-page: https://github.com/optimizely/python-sdk
-Author: Optimizely
-Author-email: developers@optimizely.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
-Optimizely Feature Experimentation is A/B testing and feature management for product development teams. Experiment in any application. Make every feature on your roadmap an opportunity to learn. Learn more at https://www.optimizely.com/products/experiment/feature-experimentation/ or see our documentation at https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/welcome. # Optimizely Python SDK
-
-[![PyPI version](https://badge.fury.io/py/optimizely-sdk.svg)](https://pypi.org/project/optimizely-sdk)
-[![Build Status](https://travis-ci.org/optimizely/python-sdk.svg?branch=master)](https://travis-ci.org/optimizely/python-sdk)
-[![Coverage Status](https://coveralls.io/repos/github/optimizely/python-sdk/badge.svg)](https://coveralls.io/github/optimizely/python-sdk)
-[![Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](http://www.apache.org/licenses/LICENSE-2.0)
-
-This repository houses the Python SDK for use with Optimizely Feature Experimentation and Optimizely Full Stack (legacy).
-
-Optimizely Feature Experimentation is an A/B testing and feature management tool for product development teams that enables you to experiment at every step. Using Optimizely Feature Experimentation allows for every feature on your roadmap to be an opportunity to discover hidden insights. Learn more at [Optimizely.com](https://www.optimizely.com/products/experiment/feature-experimentation/), or see the [developer documentation](https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/welcome).
-
-Optimizely Rollouts is [free feature flags](https://www.optimizely.com/free-feature-flagging/) for development teams. You can easily roll out and roll back features in any application without code deploys, mitigating risk for every feature on your roadmap.
-
-## Get Started
-
-Refer to the [Python SDK's developer documentation](https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/python-sdk) for detailed instructions on getting started with using the SDK.
-
-### Requirements
-
-Version `4.0+`: Python 3.7+, PyPy 3.7+
-
-Version `3.0+`: Python 2.7+, PyPy 3.4+
-
-### Install the SDK
-
-The SDK is available through [PyPi](https://pypi.python.org/pypi?name=optimizely-sdk&:action=display).
-
-To install:
-
-    pip install optimizely-sdk
-
-### Feature Management Access
-
-To access the Feature Management configuration in the Optimizely
-dashboard, please contact your Optimizely customer success manager.
-
-## Use the Python SDK
-
-### Initialization
-
-You can initialize the Optimizely instance in three ways: with a datafile, by providing an sdk_key, or by providing an implementation of
-[BaseConfigManager](https://github.com/optimizely/python-sdk/tree/master/optimizely/config_manager.py#L32).
-Each method is described below.
-
-1.  Initialize Optimizely with a datafile. This datafile will be used as
-    the source of ProjectConfig throughout the life of Optimizely instance:
-
-        optimizely.Optimizely(
-          datafile
-        )
-
-2.  Initialize Optimizely by providing an \'sdk_key\'. This will
-    initialize a PollingConfigManager that makes an HTTP GET request to
-    the URL (formed using your provided sdk key and the
-    default datafile CDN URL template) to asynchronously download the
-    project datafile at regular intervals and update ProjectConfig when
-    a new datafile is received. A hard-coded datafile can also be
-    provided along with the sdk_key that will be used
-    initially before any update:
-
-        optimizely.Optimizely(
-          sdk_key='put_your_sdk_key_here'
-        )
-
-    If providing a datafile, the initialization will look like:
-
-        optimizely.Optimizely(
-          datafile=datafile,
-          sdk_key='put_your_sdk_key_here'
-        )
-
-3.  Initialize Optimizely by providing a ConfigManager that implements
-    [BaseConfigManager](https://github.com/optimizely/python-sdk/tree/master/optimizely/config_manager.py#L34).
-    You may use our [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L150) or
-    [AuthDatafilePollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L375) as needed:
-
-        optimizely.Optimizely(
-          config_manager=custom_config_manager
-        )
-
-### PollingConfigManager
-
-The [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L150) asynchronously polls for
-datafiles from a specified URL at regular intervals by making HTTP requests.
-
-    polling_config_manager = PollingConfigManager(
-        sdk_key=None,
-        datafile=None,
-        update_interval=None,
-        url=None,
-        url_template=None,
-        logger=None,
-        error_handler=None,
-        notification_center=None,
-        skip_json_validation=False
-    )
-
-**Note**: You must provide either the sdk_key or URL. If
-you provide both, the URL takes precedence.
-
-**sdk_key** The sdk_key is used to compose the outbound
-HTTP request to the default datafile location on the Optimizely CDN.
-
-**datafile** You can provide an initial datafile to bootstrap the
-`ProjectConfigManager` so that it can be used immediately. The initial
-datafile also serves as a fallback datafile if HTTP connection cannot be
-established. The initial datafile will be discarded after the first
-successful datafile poll.
-
-**update_interval** The update_interval is used to specify a fixed
-delay in seconds between consecutive HTTP requests for the datafile.
-
-**url** The target URL from which to request the datafile.
-
-**url_template** A string with placeholder `{sdk_key}` can be provided
-so that this template along with the provided sdk key is
-used to form the target URL.
-
-You may also provide your own logger, error_handler, or
-notification_center.
-
-### AuthDatafilePollingConfigManager
-
-The [AuthDatafilePollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L375)
-implements `PollingConfigManager` and asynchronously polls for authenticated datafiles from a specified URL at regular intervals
-by making HTTP requests.
-
-    auth_datafile_polling_config_manager = AuthDatafilePollingConfigManager(
-        datafile_access_token,
-        *args,
-        **kwargs
-    )
-
-**Note**: To use [AuthDatafilePollingConfigManager](#authdatafilepollingconfigmanager), you must create a secure environment for
-your project and generate an access token for your datafile.
-
-**datafile_access_token** The datafile_access_token is attached to the outbound HTTP request header to authorize the request and fetch the datafile.
-
-### Advanced configuration
-
-The following properties can be set to override the default
-configurations for [PollingConfigManager](#pollingconfigmanager) and [AuthDatafilePollingConfigManager](#authdatafilepollingconfigmanager).
-
-| **Property Name** |                                                                                    **Default Value**                                                                                    |                        **Description**                         |
-| :---------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------: |
-|      sdk_key      |                                                                                          None                                                                                           |                   Optimizely project SDK key                   |
-|     datafile      |                                                                                          None                                                                                           | Initial datafile, typically sourced from a local cached source |
-|  update_interval  |                                                                                        5 minutes                                                                                        |          Fixed delay between fetches for the datafile          |
-|        url        |                                                                                          None                                                                                           |      Custom URL location from which to fetch the datafile      |
-|   url_template    | `PollingConfigManager:`<br/>https://cdn.optimizely.com/datafiles/{sdk_key}.json<br/>`AuthDatafilePollingConfigManager:`<br/>https://config.optimizely.com/datafiles/auth/{sdk_key}.json |             Parameterized datafile URL by SDK key              |
-
-A notification signal will be triggered whenever a _new_ datafile is
-fetched and Project Config is updated. To subscribe to these
-notifications, use:
-
-```
-notification_center.add_notification_listener(NotificationTypes.OPTIMIZELY_CONFIG_UPDATE, update_callback)
-```
-
-For Further details see the Optimizely [Feature Experimentation documentation](https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/welcome)
-to learn how to set up your first Python project and use the SDK.
-
-## SDK Development
-
-### Building the SDK
-
-Build and install the SDK with pip, using the following command:
-
-    pip install -e .
-
-### Unit Tests
-
-#### Running all tests
-
-To get test dependencies installed, use a modified version of the
-install command:
-
-    pip install -e '.[test]'
-
-You can run all unit tests with:
-
-    pytest
-
-#### Running all tests in a file
-
-To run all tests under a particular test file you can use the following
-command:
-
-    pytest tests.<file_name_without_extension>
-
-For example, to run all tests under `test_event_builder`, the command would be:
-
-    pytest tests/test_event_builder.py
-
-#### Running all tests under a class
-
-To run all tests under a particular class of tests you can use the
-following command:
-
-    pytest tests/<file_name_with_extension>::ClassName
-
-For example, to run all tests under `test_event_builder.EventTest`, the command
-would be:
-
-    pytest tests/test_event_builder.py::EventTest
-
-#### Running a single test
-
-To run a single test you can use the following command:
-
-    pytest tests/<file_name_with_extension>::ClassName::test_name
-
-For example, to run `test_event_builder.EventTest.test_init`, the command
-would be:
-
-    pytest tests/test_event_builder.py::EventTest::test_init
-
-### Contributing
-
-Please see [CONTRIBUTING](https://github.com/optimizely/python-sdk/blob/master/CONTRIBUTING.md).
-
-### Credits
-
-This software incorporates code from the following open source projects:
-
-requests (Apache-2.0 License: https://github.com/psf/requests/blob/master/LICENSE)
-
-pyOpenSSL (Apache-2.0 License https://github.com/pyca/pyopenssl/blob/main/LICENSE)
-
-cryptography (Apache-2.0 https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE)
-
-idna (BSD 3-Clause License https://github.com/kjd/idna/blob/master/LICENSE.md)
-
-### Other Optimizely SDKs
-
-- Agent - https://github.com/optimizely/agent
-
-- Android - https://github.com/optimizely/android-sdk
-
-- C# - https://github.com/optimizely/csharp-sdk
-
-- Flutter - https://github.com/optimizely/optimizely-flutter-sdk
-
-- Go - https://github.com/optimizely/go-sdk
-
-- Java - https://github.com/optimizely/java-sdk
-
-- JavaScript - https://github.com/optimizely/javascript-sdk
-
-- PHP - https://github.com/optimizely/php-sdk
-
-- Python - https://github.com/optimizely/python-sdk
-
-- React - https://github.com/optimizely/react-sdk
-
-- Ruby - https://github.com/optimizely/ruby-sdk
-
-- Swift - https://github.com/optimizely/swift-sdk
-# Optimizely Python SDK Changelog
-
-## 4.1.1
-March 10th, 2023
-
-We updated our README.md and other non-functional code to reflect that this SDK supports both Optimizely Feature Experimentation and Optimizely Full Stack. ([#420](https://github.com/optimizely/python-sdk/pull/420))
-
-## 4.1.0
-July 7th, 2022
-
-### Bug Fixes
-* Fix error log formatting for flag key ([#381](https://github.com/optimizely/python-sdk/pull/381))
-* Fix invalid datafile returned from `ProjectConfig.to_datafile` and `OptimizelyConfig.get_datafile` ([#321](https://github.com/optimizely/python-sdk/pull/321), [#384](https://github.com/optimizely/python-sdk/pull/384))
-
-
-## 4.0.0
-January 12th, 2022
-
-### New Features
-* Add a set of new APIs for overriding and managing user-level flag, experiment and delivery rule decisions. These methods can be used for QA and automated testing purposes. They are an extension of the OptimizelyUserContext interface ([#361](https://github.com/optimizely/python-sdk/pull/361), [#365](https://github.com/optimizely/python-sdk/pull/365), [#369](https://github.com/optimizely/python-sdk/pull/369)):
-	- setForcedDecision
-	- getForcedDecision
-	- removeForcedDecision
-	- removeAllForcedDecisions
-
-* For details, refer to our documentation pages: [OptimizelyUserContext](https://docs.developers.optimizely.com/full-stack/v4.0/docs/optimizelyusercontext-python) and [Forced Decision methods](https://docs.developers.optimizely.com/full-stack/v4.0/docs/forced-decision-methods-python).
-
-### Breaking Changes:
-
-* Support for `Python v3.4` has been dropped as of this release due to a security vulnerability with `PyYAML <v5.4`. ([#366](https://github.com/optimizely/python-sdk/pull/366))
-* We no longer support `Python v2.7, v3.5, and v3.6` including `PyPy` as of this release. ([#377](https://github.com/optimizely/python-sdk/pull/373))
-* We now support `Python v3.7 and above` including `PyPy3`.
-
-## 3.10.0
-September 16th, 2021
-
-### New Features
-* Added new public properties to OptimizelyConfig.
-  - sdk_key and environment_key [#338] (https://github.com/optimizely/python-sdk/pull/338)
-  - attributes and events [#339] (https://github.com/optimizely/python-sdk/pull/339)
-  - experiment_rules, delivery_rules, audiences and audiences in OptimizelyExperiment
-    - [#342] (https://github.com/optimizely/python-sdk/pull/342)
-    - [#351] (https://github.com/optimizely/python-sdk/pull/351/files)
-* For details please refer to our documentation page:
-  - Python-sdk: [https://docs.developers.optimizely.com/full-stack/docs/optimizelyconfig-python]
-
-* OptimizelyFeature.experiments_map of OptimizelyConfig is now deprecated. Please use OptimizelyFeature.experiment_rules and OptimizelyFeature.delivery_rules. [#360] (https://github.com/optimizely/python-sdk/pull/360)
-
-### Bug Fixes
-* Fix event processor negative timeout interval when retrieving events from queue. [#356] (https://github.com/optimizely/python-sdk/pull/356)
-
-## 3.9.1
-July 14th, 2021
-
-### Bug Fixes:
-* Fixed issue with serving incorrect variation in projects containing multiple flags with duplicate keys. [#347] (https://github.com/optimizely/python-sdk/pull/347)
-* Fixed issue with serving incorrect variation in create_impression_event in user_event_factory.py. [#350] (https://github.com/optimizely/python-sdk/pull/350)
-
-## 3.9.0
-June 1st, 2021
-
-### New Features
-* Added support for multiple concurrent prioritized experiments per flag. [#322](https://github.com/optimizely/python-sdk/pull/322)
-
-## 3.8.0
-February 12th, 2021
-
-### New Features
-* New Features
-Introducing a new primary interface for retrieving feature flag status, configuration and associated experiment decisions for users ([#309](https://github.com/optimizely/python-sdk/pull/309)). The new `OptimizelyUserContext` class is instantiated with `create_user_context` and exposes the following APIs to get `OptimizelyDecision`:
-
-    - set_attribute
-    - decide
-    - decide_all
-    - decide_for_keys
-    - track_event
-
-For details, refer to our documentation page: https://docs.developers.optimizely.com/full-stack/v4.0/docs/python-sdk.
-
-## 3.7.1
-November 19th, 2020
-
-### Bug Fixes:
-* Added "enabled" field to decision metadata structure. [#306](https://github.com/optimizely/python-sdk/pull/306)
-
-## 3.7.0
-November 2nd, 2020
-
-### New Features
-* Added support for upcoming application-controlled introduction of tracking for non-experiment Flag decisions. [#300](https://github.com/optimizely/python-sdk/pull/300)
-
-## 3.6.0
-October 1st, 2020
-
-### New Features:
-* Version targeting using semantic version syntax. [#293](https://github.com/optimizely/python-sdk/pull/293)
-* Datafile accessor API added to access current config as a JSON string. [#283](https://github.com/optimizely/python-sdk/pull/283)
-
-### Bug Fixes:
-* Fixed package installation for Python 3.4 and pypy. [#298](https://github.com/optimizely/python-sdk/pull/298)
-
-## 3.5.2
-July 14th, 2020
-
-### Bug Fixes:
-* Fixed handling of network and no status code errors when polling for datafile in `PollingConfigManager` and `AuthDatafilePollingConfigManager`. ([#287](https://github.com/optimizely/python-sdk/pull/287))
-
-## 3.5.1
-July 10th, 2020
-
-### Bug Fixes:
-* Fixed HTTP request exception handling in `PollingConfigManager`. ([#285](https://github.com/optimizely/python-sdk/pull/285))
-
-## 3.5.0
-July 9th, 2020
-
-### New Features:
-* Introduced 2 APIs to interact with feature variables:
-  * `get_feature_variable_json` allows you to get value for JSON variables related to a feature.
-  * `get_all_feature_variables` gets values for all variables under a feature.
-* Added support for fetching authenticated datafiles. `AuthDatafilePollingConfigManager` is a new config manager that allows you to poll for a datafile belonging to a secure environment. You can create a client by setting the `datafile_access_token`.
-
-### Bug Fixes:
-* Fixed log messages for targeted rollouts evaluation. ([#268](https://github.com/optimizely/python-sdk/pull/268))
-
-## 3.4.2
-June 11th, 2020
-
-### Bug Fixes:
-* Adjusted log level for audience evaluation logs. ([#267](https://github.com/optimizely/python-sdk/pull/267))
-
-## 3.4.1
-March 19th, 2020
-
-### Bug Fixes:
-* Updated `jsonschema` to address [installation issue](https://github.com/optimizely/python-sdk/issues/232).
-
-## 3.4.0
-January 27th, 2020
-
-### New Features:
-* Added a new API to get project configuration static data.
-  * Call `get_optimizely_config()` to get a snapshot of project configuration static data.
-  * It returns an `OptimizelyConfig` instance which includes a datafile revision number, all experiments, and feature flags mapped by their key values.
-  * Added caching for `get_optimizely_config()` - `OptimizelyConfig` object will be cached and reused for the lifetime of the datafile.
-  * For details, refer to our documentation page: [https://docs.developers.optimizely.com/full-stack/docs/optimizelyconfig-python](https://docs.developers.optimizely.com/full-stack/docs/optimizelyconfig-python).
-
-
-## 3.3.1
-December 16th, 2019
-
-### Bug Fixes:
-* Fixed [installation issue](https://github.com/optimizely/python-sdk/issues/220) on Windows. ([#224](https://github.com/optimizely/python-sdk/pull/224))
-* Fixed batch event processor deadline reset issue. ([#227](https://github.com/optimizely/python-sdk/pull/227))
-* Added more batch event processor debug messages. ([#227](https://github.com/optimizely/python-sdk/pull/227))
-
-## 3.3.0
-October 28th, 2019
-
-### New Features:
-* Added support for event batching via the event processor.
-  * Events generated by methods like `activate`, `track`, and `is_feature_enabled` will be held in a queue until the configured batch size is reached, or the configured flush interval has elapsed. Then, they will be batched into a single payload and sent to the event dispatcher.
-  * To configure event batching, set the `batch_size` and `flush_interval` properties when initializing instance of [BatchEventProcessor](https://github.com/optimizely/python-sdk/blob/3.3.x/optimizely/event/event_processor.py#L45).
-  * Event batching is disabled by default. You can pass in instance of `BatchEventProcessor` when creating `Optimizely` instance to enable event batching.
-  * Users can subscribe to `LogEvent` notification to be notified of whenever a payload consisting of a batch of user events is handed off to the event dispatcher to send to Optimizely's backend.
-* Introduced blocking timeout in `PollingConfigManager`. By default, calls to `get_config` will block for maximum of 10 seconds until config is available.
-
-### Bug Fixes:
-* Fixed incorrect log message when numeric metric is not used. ([#217](https://github.com/optimizely/python-sdk/pull/217))
-
-## 3.2.0
-August 27th, 2019
-
-### New Features:
-* Added support for automatic datafile management via [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151):
-  * The [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151) is an implementation of the [BaseConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L32).
-  * Users may provide one of datafile or SDK key (sdk_key) or both to `optimizely.Optimizely`. Based on that, the SDK will use the [StaticConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L73) or the [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151). Refer to the [README](README.md) for more instructions.
-  * An initial datafile can be provided to the `PollingConfigManager` to bootstrap before making HTTP requests for the hosted datafile.
-  * Requests for the datafile are made in a separate thread and are scheduled with fixed delay.
-  * Configuration updates can be subscribed to by adding the OPTIMIZELY_CONFIG_UPDATE notification listener.
-* Introduced `Optimizely.get_feature_variable` API.  ([#191](https://github.com/optimizely/python-sdk/pull/191))
-
-### Deprecated:
-
-* `NotificationCenter.clear_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
-* `NotificationCenter.clear_all_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_all_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
-
-## 3.2.0b1
-July 26th, 2019
-
-### New Features:
-* Added support for automatic datafile management via [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151):
-  * The [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151) is an implementation of the [BaseConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L32).
-  * Users may provide one of datafile or SDK key (sdk_key) or both to `optimizely.Optimizely`. Based on that, the SDK will use the [StaticConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L73) or the [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151). Refer to the [README](README.md) for more instructions.
-  * An initial datafile can be provided to the `PollingConfigManager` to bootstrap before making HTTP requests for the hosted datafile.
-  * Requests for the datafile are made in a separate thread and are scheduled with fixed delay.
-  * Configuration updates can be subscribed to by adding the OPTIMIZELY_CONFIG_UPDATE notification listener.
-* Introduced `Optimizely.get_feature_variable` API.  ([#191](https://github.com/optimizely/python-sdk/pull/191))
-
-### Deprecated:
-
-* `NotificationCenter.clear_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
-* `NotificationCenter.clear_all_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_all_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
-
-## 3.1.0
-May 3rd, 2019
-
-### New Features:
-* Introduced Decision notification listener to be able to record:
-  * Variation assignments for users activated in an experiment.
-  * Feature access for users.
-  * Feature variable value for users.
-
-### Bug Fixes:
-* Feature variable APIs now return default variable value when featureEnabled property is false.  ([#171](https://github.com/optimizely/python-sdk/pull/171))
-
-### Deprecated:
-* Activate notification listener is deprecated as of this release.  Recommendation is to use the new Decision notification listener.  Activate notification listener will be removed in the next major release.
-
-## 3.0.0
-March 1st, 2019
-
-The 3.0 release improves event tracking and supports additional audience
-targeting functionality.
-
-### New Features:
-* Event tracking:
-  * The `track` method now dispatches its conversion event *unconditionally*, without first determining whether the user is targeted by a known experiment that uses the event. This may increase outbound network traffic.
-  * In Optimizely results, conversion events sent by 3.0 SDKs don\'t explicitly name the experiments and variations that are currently targeted to the user. Instead, conversions are automatically attributed to variations that the user has previously seen, as long as those variations were served via 3.0 SDKs or by other clients capable of automatic attribution, and as long as our backend actually received the impression events for those variations.
-  * Altogether, this allows you to track conversion events and attribute them to variations even when you don't know all of a user's attribute values, and even if the user's attribute values or the experiment's configuration have changed such that the user is no longer affected by the experiment. As a result, **you may observe an increase in the conversion rate for previously-instrumented events.** If that is undesirable, you can reset the results of previously-running experiments after upgrading to the 3.0 SDK.  -   This will also allow you to attribute events to variations from other Optimizely projects in your account, even though those experiments don't appear in the same datafile.
-  * Note that for results segmentation in Optimizely results, the user attribute values from one event are automatically applied to all other events in the same session, as long as the events in question were actually received by our backend. This behavior was already in place and is not affected by the 3.0 release.
-* Support for all types of attribute values, not just strings.
-  * All values are passed through to notification listeners.
-  * Strings, booleans, and valid numbers are passed to the event dispatcher and can be used for Optimizely results segmentation.  A valid number is a finite float or numbers.Integral in the inclusive range \[-2 ^ 53, 2 ^ 53\].
-  * Strings, booleans, and valid numbers are relevant for audience conditions.
-* Support for additional matchers in audience conditions:
-  * An `exists` matcher that passes if the user has a non-null value for the targeted user attribute and fails otherwise.
-  * A `substring` matcher that resolves if the user has a string value for the targeted attribute.
-    * `gt` (greater than) and `lt` (less than) matchers that resolve if the user has a valid number value for the targeted attribute.  A valid number is a finite float or numbers.Integral in the inclusive range \[-2 ^ 53, 2 ^ 53\].
-    * The original (`exact`) matcher can now be used to target booleans and valid numbers, not just strings.
-* Support for A/B tests, feature tests, and feature rollouts whose audiences are combined using `"and"` and `"not"` operators, not just the `"or"` operator.
-* Datafile-version compatibility check: The SDK will remain uninitialized (i.e., will gracefully fail to activate experiments and features) if given a datafile version greater than 4.
-* Updated Pull Request template and commit message guidelines.
-
-### Breaking Changes:
-* Conversion events sent by 3.0 SDKs don\'t explicitly name the experiments and variations that are currently targeted to the user, so these events are unattributed in raw events data export. You must use the new *results* export to determine the variations to which events have been attributed.
-* Previously, notification listeners were only given string-valued user attributes because only strings could be passed into various method calls. That is no longer the case. You may pass non-string attribute values, and if you do, you must update your notification listeners to be able to receive whatever values you pass in.
-
-### Bug Fixes:
-* Experiments and features can no longer activate when a negatively targeted attribute has a missing, null, or malformed value.
-  * Audience conditions (except for the new `exists` matcher) no longer resolve to `false` when they fail to find an legitimate value for the targeted user attribute. The result remains `null` (unknown). Therefore, an audience that negates such a condition (using the `"not"` operator) can no longer resolve to `true` unless there is an unrelated branch in the condition tree that itself resolves to `true`.
-* Updated the default event dispatcher to log an error if the request resolves to HTTP 4xx or 5xx.  ([#140](https://github.com/optimizely/python-sdk/pull/140))
-* All methods now validate that user IDs are strings and that experiment keys, feature keys, feature variable keys, and event keys are non-empty strings.
-
-## 2.1.1
-August 21st, 2018
-
-* Fix: record conversions for all experiments using an event when using track([#136](https://github.com/optimizely/python-sdk/pull/136)).
-
-## 2.1.0
-July 2nd, 2018
-
-* Introduced support for bot filtering ([#121](https://github.com/optimizely/python-sdk/pull/121)).
-* Overhauled logging to use standard Python logging ([#123](https://github.com/optimizely/python-sdk/pull/123)).
-
-## 2.0.1
-June 19th, 2018
-
-* Fix: send impression event for Feature Test when Feature is disabled ([#128](https://github.com/optimizely/python-sdk/pull/128)).
-
-## 2.0.0
-April 12th, 2018
-
-This major release introduces APIs for Feature Management. It also
-introduces some breaking changes listed below.
-
-### New Features
-* Introduced the `is_feature_enabled` API to determine whether to show a feature to a user or not.
-
-```
-    is_enabled = optimizel_client.is_feature_enabled('my_feature_key', 'my_user', user_attributes)
-```
-
-* All enabled features for the user can be retrieved by calling:
-
-```
-    enabled_features = optimizely_client.get_enabled_features('my_user', user_attributes)
-```
-* Introduced Feature Variables to configure or parameterize a feature.  There are four variable types: `String`, `Integer`, `Double`, `Boolean`.
-
-```
-    string_variable = optimizely_client.get_feature_variable_string('my_feature_key', 'string_variable_key', 'my_user')
-    integer_variable = optimizely_client.get_feature_variable_integer('my_feature_key', 'integer_variable_key', 'my_user')
-    double_variable = optimizely_client.get_feature_variable_double('my_feature_key', 'double_variable_key', 'my_user')
-    boolean_variable = optimizely_client.get_feature_variable_boolean('my_feature_key', 'boolean_variable_key', 'my_user')
-```
-
-### Breaking changes
-* The `track` API with revenue value as a stand-alone parameter has been removed. The revenue value should be passed in as an entry in the event tags dict. The key for the revenue tag is `revenue` and the passed in value will be treated by Optimizely as the value for computing results.
-
-```
-    event_tags = {
-      'revenue': 1200
-    }
-
-    optimizely_client.track('event_key', 'my_user', user_attributes, event_tags)
-```
-
-## 2.0.0b1
-March 29th, 2018
-
-This beta release introduces APIs for Feature Management. It also
-introduces some breaking changes listed below.
-
-### New Features
-* Introduced the `is_feature_enabled` API to determine whether to show a feature to a user or not.
-```
-    is_enabled = optimizel_client.is_feature_enabled('my_feature_key', 'my_user', user_attributes)
-```
-
-* All enabled features for the user can be retrieved by calling:
-
-```
-    enabled_features = optimizely_client.get_enabled_features('my_user', user_attributes)
-```
-
-* Introduced Feature Variables to configure or parameterize a feature.  There are four variable types: `String`, `Integer`, `Double`, `Boolean`.
-
-```
-    string_variable = optimizely_client.get_feature_variable_string('my_feature_key', 'string_variable_key', 'my_user')
-    integer_variable = optimizely_client.get_feature_variable_integer('my_feature_key', 'integer_variable_key', 'my_user')
-    double_variable = optimizely_client.get_feature_variable_double('my_feature_key', 'double_variable_key', 'my_user')
-    boolean_variable = optimizely_client.get_feature_variable_boolean('my_feature_key', 'boolean_variable_key', 'my_user')
-```
-
-### Breaking changes
-* The `track` API with revenue value as a stand-alone parameter has been removed. The revenue value should be passed in as an entry in the event tags dict. The key for the revenue tag is `revenue` and the passed in value will be treated by Optimizely as the value for computing results.
-
-```
-    event_tags = {
-      'revenue': 1200
-    }
-
-    optimizely_client.track('event_key', 'my_user', user_attributes, event_tags)
-```
-
-## 1.4.0
-
-* Added support for IP anonymization.
-* Added support for notification listeners.
-* Added support for bucketing ID.
-* Updated mmh3 to handle installation failures on Windows 10.
-
-## 1.3.0
-
-* Introduced support for forced bucketing.
-* Introduced support for numeric metrics.
-* Updated event builder to support new endpoint.
-
-## 1.2.1
-
-* Removed older feature flag parsing.
-
-## 1.2.0
-
-* Added user profile service.
-
-## 1.1.1
-
-* Updated datafile parsing to be able to handle additional fields.
-* Deprecated Classic project support.
-
-## 1.1.0
-
-* Included datafile revision information in log events.
-* Added event tags to track API to allow users to pass in event metadata.
-* Deprecated the `event_value` parameter from the track method. Should use `event_tags` to pass in event value instead.
-* Updated event logging endpoint to logx.optimizely.com.
-
-## 1.0.0
-
-* Introduced support for Full Stack projects in Optimizely X. No breaking changes from previous version.
-* Introduced more graceful exception handling in instantiation and core methods.
-* Updated whitelisting to precede audience matching.
-
-## 0.1.3
-
-* Added support for v2 endpoint and datafile.
-* Updated dispatch_event to consume an Event object instead of url and params. The Event object comprises of four properties: url (string representing URL to dispatch event to), params (dict representing the params to be set for the event), http_verb (one of 'GET' or 'POST') and headers (header values to be sent along).
-* Fixed issue with tracking events for experiments in groups.
-
-## 0.1.2
-
-* Updated requirements file.
-
-## 0.1.1
-
-* Introduced option to skip JSON schema validation.
-
-## 0.1.0
-
-* Beta release of the Python SDK for server-side testing.
+Metadata-Version: 2.1
+Name: optimizely-sdk
+Version: 5.0.0b0
+Summary: Python SDK for Optimizely Feature Experimentation, Optimizely Full Stack (legacy), and Optimizely Rollouts.
+Home-page: https://github.com/optimizely/python-sdk
+Author: Optimizely
+Author-email: developers@optimizely.com
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
+Optimizely Feature Experimentation is A/B testing and feature management for product development teams. Experiment in any application. Make every feature on your roadmap an opportunity to learn. Learn more at https://www.optimizely.com/products/experiment/feature-experimentation/ or see our documentation at https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/welcome. # Optimizely Python SDK
+
+[![PyPI version](https://badge.fury.io/py/optimizely-sdk.svg)](https://pypi.org/project/optimizely-sdk)
+[![Build Status](https://github.com/optimizely/python-sdk/actions/workflows/python.yml/badge.svg?branch=master)](https://github.com/optimizely/python-sdk/actions/workflows/python.yml?query=branch%3Amaster)
+[![Coverage Status](https://coveralls.io/repos/github/optimizely/python-sdk/badge.svg)](https://coveralls.io/github/optimizely/python-sdk)
+[![Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](http://www.apache.org/licenses/LICENSE-2.0)
+
+This repository houses the Python SDK for use with Optimizely Feature Experimentation and Optimizely Full Stack (legacy).
+
+Optimizely Feature Experimentation is an A/B testing and feature management tool for product development teams that enables you to experiment at every step. Using Optimizely Feature Experimentation allows for every feature on your roadmap to be an opportunity to discover hidden insights. Learn more at [Optimizely.com](https://www.optimizely.com/products/experiment/feature-experimentation/), or see the [developer documentation](https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/welcome).
+
+Optimizely Rollouts is [free feature flags](https://www.optimizely.com/free-feature-flagging/) for development teams. You can easily roll out and roll back features in any application without code deploys, mitigating risk for every feature on your roadmap.
+
+## Get Started
+
+Refer to the [Python SDK's developer documentation](https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/python-sdk) for detailed instructions on getting started with using the SDK.
+
+### Requirements
+
+Version `4.0+`: Python 3.7+, PyPy 3.7+
+
+Version `3.0+`: Python 2.7+, PyPy 3.4+
+
+### Install the SDK
+
+The SDK is available through [PyPi](https://pypi.python.org/pypi?name=optimizely-sdk&:action=display).
+
+To install:
+
+    pip install optimizely-sdk
+
+### Feature Management Access
+
+To access the Feature Management configuration in the Optimizely
+dashboard, please contact your Optimizely customer success manager.
+
+## Use the Python SDK
+
+### Initialization
+
+You can initialize the Optimizely instance in three ways: with a datafile, by providing an sdk_key, or by providing an implementation of
+[BaseConfigManager](https://github.com/optimizely/python-sdk/tree/master/optimizely/config_manager.py#L32).
+Each method is described below.
+
+1.  Initialize Optimizely with a datafile. This datafile will be used as
+    the source of ProjectConfig throughout the life of Optimizely instance:
+
+        optimizely.Optimizely(
+          datafile
+        )
+
+2.  Initialize Optimizely by providing an \'sdk_key\'. This will
+    initialize a PollingConfigManager that makes an HTTP GET request to
+    the URL (formed using your provided sdk key and the
+    default datafile CDN URL template) to asynchronously download the
+    project datafile at regular intervals and update ProjectConfig when
+    a new datafile is received. A hard-coded datafile can also be
+    provided along with the sdk_key that will be used
+    initially before any update:
+
+        optimizely.Optimizely(
+          sdk_key='put_your_sdk_key_here'
+        )
+
+    If providing a datafile, the initialization will look like:
+
+        optimizely.Optimizely(
+          datafile=datafile,
+          sdk_key='put_your_sdk_key_here'
+        )
+
+3.  Initialize Optimizely by providing a ConfigManager that implements
+    [BaseConfigManager](https://github.com/optimizely/python-sdk/tree/master/optimizely/config_manager.py#L34).
+    You may use our [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L150) or
+    [AuthDatafilePollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L375) as needed:
+
+        optimizely.Optimizely(
+          config_manager=custom_config_manager
+        )
+
+### PollingConfigManager
+
+The [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L150) asynchronously polls for
+datafiles from a specified URL at regular intervals by making HTTP requests.
+
+    polling_config_manager = PollingConfigManager(
+        sdk_key=None,
+        datafile=None,
+        update_interval=None,
+        url=None,
+        url_template=None,
+        logger=None,
+        error_handler=None,
+        notification_center=None,
+        skip_json_validation=False
+    )
+
+**Note**: You must provide either the sdk_key or URL. If
+you provide both, the URL takes precedence.
+
+**sdk_key** The sdk_key is used to compose the outbound
+HTTP request to the default datafile location on the Optimizely CDN.
+
+**datafile** You can provide an initial datafile to bootstrap the
+`ProjectConfigManager` so that it can be used immediately. The initial
+datafile also serves as a fallback datafile if HTTP connection cannot be
+established. The initial datafile will be discarded after the first
+successful datafile poll.
+
+**update_interval** The update_interval is used to specify a fixed
+delay in seconds between consecutive HTTP requests for the datafile.
+
+**url** The target URL from which to request the datafile.
+
+**url_template** A string with placeholder `{sdk_key}` can be provided
+so that this template along with the provided sdk key is
+used to form the target URL.
+
+You may also provide your own logger, error_handler, or
+notification_center.
+
+### AuthDatafilePollingConfigManager
+
+The [AuthDatafilePollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L375)
+implements `PollingConfigManager` and asynchronously polls for authenticated datafiles from a specified URL at regular intervals
+by making HTTP requests.
+
+    auth_datafile_polling_config_manager = AuthDatafilePollingConfigManager(
+        datafile_access_token,
+        *args,
+        **kwargs
+    )
+
+**Note**: To use [AuthDatafilePollingConfigManager](#authdatafilepollingconfigmanager), you must create a secure environment for
+your project and generate an access token for your datafile.
+
+**datafile_access_token** The datafile_access_token is attached to the outbound HTTP request header to authorize the request and fetch the datafile.
+
+### Advanced configuration
+
+The following properties can be set to override the default
+configurations for [PollingConfigManager](#pollingconfigmanager) and [AuthDatafilePollingConfigManager](#authdatafilepollingconfigmanager).
+
+| **Property Name** |                                                                                    **Default Value**                                                                                    |                        **Description**                         |
+| :---------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------: |
+|      sdk_key      |                                                                                          None                                                                                           |                   Optimizely project SDK key                   |
+|     datafile      |                                                                                          None                                                                                           | Initial datafile, typically sourced from a local cached source |
+|  update_interval  |                                                                                        5 minutes                                                                                        |          Fixed delay between fetches for the datafile          |
+|        url        |                                                                                          None                                                                                           |      Custom URL location from which to fetch the datafile      |
+|   url_template    | `PollingConfigManager:`<br/>https://cdn.optimizely.com/datafiles/{sdk_key}.json<br/>`AuthDatafilePollingConfigManager:`<br/>https://config.optimizely.com/datafiles/auth/{sdk_key}.json |             Parameterized datafile URL by SDK key              |
+
+A notification signal will be triggered whenever a _new_ datafile is
+fetched and Project Config is updated. To subscribe to these
+notifications, use:
+
+```
+notification_center.add_notification_listener(NotificationTypes.OPTIMIZELY_CONFIG_UPDATE, update_callback)
+```
+
+For Further details see the Optimizely [Feature Experimentation documentation](https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/welcome)
+to learn how to set up your first Python project and use the SDK.
+
+## SDK Development
+
+### Building the SDK
+
+Build and install the SDK with pip, using the following command:
+
+    pip install -e .
+
+### Unit Tests
+
+#### Running all tests
+
+To get test dependencies installed, use a modified version of the
+install command:
+
+    pip install -e '.[test]'
+
+You can run all unit tests with:
+
+    pytest
+
+#### Running all tests in a file
+
+To run all tests under a particular test file you can use the following
+command:
+
+    pytest tests.<file_name_without_extension>
+
+For example, to run all tests under `test_event_builder`, the command would be:
+
+    pytest tests/test_event_builder.py
+
+#### Running all tests under a class
+
+To run all tests under a particular class of tests you can use the
+following command:
+
+    pytest tests/<file_name_with_extension>::ClassName
+
+For example, to run all tests under `test_event_builder.EventTest`, the command
+would be:
+
+    pytest tests/test_event_builder.py::EventTest
+
+#### Running a single test
+
+To run a single test you can use the following command:
+
+    pytest tests/<file_name_with_extension>::ClassName::test_name
+
+For example, to run `test_event_builder.EventTest.test_init`, the command
+would be:
+
+    pytest tests/test_event_builder.py::EventTest::test_init
+
+### Contributing
+
+Please see [CONTRIBUTING](https://github.com/optimizely/python-sdk/blob/master/CONTRIBUTING.md).
+
+### Credits
+
+This software incorporates code from the following open source projects:
+
+requests (Apache-2.0 License: https://github.com/psf/requests/blob/master/LICENSE)
+
+pyOpenSSL (Apache-2.0 License https://github.com/pyca/pyopenssl/blob/main/LICENSE)
+
+cryptography (Apache-2.0 https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE)
+
+idna (BSD 3-Clause License https://github.com/kjd/idna/blob/master/LICENSE.md)
+
+### Other Optimizely SDKs
+
+- Agent - https://github.com/optimizely/agent
+
+- Android - https://github.com/optimizely/android-sdk
+
+- C# - https://github.com/optimizely/csharp-sdk
+
+- Flutter - https://github.com/optimizely/optimizely-flutter-sdk
+
+- Go - https://github.com/optimizely/go-sdk
+
+- Java - https://github.com/optimizely/java-sdk
+
+- JavaScript - https://github.com/optimizely/javascript-sdk
+
+- PHP - https://github.com/optimizely/php-sdk
+
+- Python - https://github.com/optimizely/python-sdk
+
+- React - https://github.com/optimizely/react-sdk
+
+- Ruby - https://github.com/optimizely/ruby-sdk
+
+- Swift - https://github.com/optimizely/swift-sdk
+# Optimizely Python SDK Changelog
+
+## 5.0.0-beta
+Apr 28th, 2023
+
+### New Features  
+
+The 5.0.0-beta release introduces a new primary feature, [Advanced Audience Targeting]( https://docs.developers.optimizely.com/feature-experimentation/docs/optimizely-data-platform-advanced-audience-targeting) enabled through integration with [Optimizely Data Platform (ODP)](https://docs.developers.optimizely.com/optimizely-data-platform/docs) ([#395](https://github.com/optimizely/python-sdk/pull/395), [#398](https://github.com/optimizely/python-sdk/pull/398), [#402](https://github.com/optimizely/python-sdk/pull/402), [#403](https://github.com/optimizely/python-sdk/pull/403), [#405](https://github.com/optimizely/python-sdk/pull/405)).  
+
+You can use ODP, a high-performance [Customer Data Platform (CDP)]( https://www.optimizely.com/optimization-glossary/customer-data-platform/), to easily create complex real-time segments (RTS) using first-party and 50+ third-party data sources out of the box. You can create custom schemas that support the user attributes important for your business, and stitch together user behavior done on different devices to better understand and target your customers for personalized user experiences. ODP can be used as a single source of truth for these segments in any Optimizely or 3rd party tool. 
+
+With ODP accounts integrated into Optimizely projects, you can build audiences using segments pre-defined in ODP. The SDK will fetch the segments for given users and make decisions using the segments. For access to ODP audience targeting in your Feature Experimentation account, please contact your Optimizely Customer Success Manager. 
+
+This version includes the following changes: 
+
+* New API added to `OptimizelyUserContext`: 
+
+  * `fetchQualifiedSegments()`: this API will retrieve user segments from the ODP server. The fetched segments will be used for audience evaluation. The fetched data will be stored in the local cache to avoid repeated network delays.
+  * When an `OptimizelyUserContext` is created, the SDK will automatically send an identify request to the ODP server to facilitate observing user activities. 
+
+* New APIs added to `OptimizelyClient`: 
+
+  * `sendOdpEvent()`: customers can build/send arbitrary ODP events that will bind user identifiers and data to user profiles in ODP.
+
+For details, refer to our documentation pages:  
+
+* [Advanced Audience Targeting](https://docs.developers.optimizely.com/feature-experimentation/docs/optimizely-data-platform-advanced-audience-targeting)  
+* [Server SDK Support](https://docs.developers.optimizely.com/feature-experimentation/v1.0/docs/advanced-audience-targeting-for-server-side-sdks) 
+* [Initialize Python SDK](https://docs.developers.optimizely.com/feature-experimentation/docs/initialize-sdk-python) 
+* [OptimizelyUserContext Python SDK](https://docs.developers.optimizely.com/feature-experimentation/docs/wip-fsodp-optimizelyusercontext-python) 
+* [Advanced Audience Targeting segment qualification methods](https://docs.developers.optimizely.com/feature-experimentation/v1.0/docs/advanced-audience-targeting-segment-qualification-methods-python) 
+* [Send Optimizely Data Platform data using Advanced Audience Targeting](https://docs.developers.optimizely.com/feature-experimentation/v1.0/docs/send-odp-data-using-advanced-audience-targeting-python) 
+
+### Breaking Changes 
+
+* `ODPManager` in the SDK is enabled by default. Unless an ODP account is integrated into the Optimizely projects, most `ODPManager` functions will be ignored. If needed, `ODPManager` can be disabled when `OptimizelyClient` is instantiated. 
+* `BaseConfigManager` abstract class now requires a get_sdk_key method. ([#413](https://github.com/optimizely/python-sdk/pull/413))
+* `PollingConfigManager` requires either the sdk_key parameter or datafile containing an sdkKey. ([#413](https://github.com/optimizely/python-sdk/pull/413))
+* Asynchronous `BatchEventProcessor` is now the default event processor. ([#378](https://github.com/optimizely/python-sdk/pull/378))
+
+## 4.1.1
+March 10th, 2023
+
+We updated our README.md and other non-functional code to reflect that this SDK supports both Optimizely Feature Experimentation and Optimizely Full Stack. ([#420](https://github.com/optimizely/python-sdk/pull/420))
+
+## 4.1.0
+July 7th, 2022
+
+### Bug Fixes
+* Fix invalid datafile returned from `ProjectConfig.to_datafile` and `OptimizelyConfig.get_datafile` ([#321](https://github.com/optimizely/python-sdk/pull/321), [#384](https://github.com/optimizely/python-sdk/pull/384))
+
+## 4.0.0
+January 12th, 2022
+
+### New Features
+* Add a set of new APIs for overriding and managing user-level flag, experiment and delivery rule decisions. These methods can be used for QA and automated testing purposes. They are an extension of the OptimizelyUserContext interface ([#361](https://github.com/optimizely/python-sdk/pull/361), [#365](https://github.com/optimizely/python-sdk/pull/365), [#369](https://github.com/optimizely/python-sdk/pull/369)):
+	- setForcedDecision
+	- getForcedDecision
+	- removeForcedDecision
+	- removeAllForcedDecisions
+
+* For details, refer to our documentation pages: [OptimizelyUserContext](https://docs.developers.optimizely.com/full-stack/v4.0/docs/optimizelyusercontext-python) and [Forced Decision methods](https://docs.developers.optimizely.com/full-stack/v4.0/docs/forced-decision-methods-python).
+
+### Breaking Changes:
+
+* Support for `Python v3.4` has been dropped as of this release due to a security vulnerability with `PyYAML <v5.4`. ([#366](https://github.com/optimizely/python-sdk/pull/366))
+* We no longer support `Python v2.7, v3.5, and v3.6` including `PyPy` as of this release. ([#377](https://github.com/optimizely/python-sdk/pull/373))
+* We now support `Python v3.7 and above` including `PyPy3`.
+
+## 3.10.0
+September 16th, 2021
+
+### New Features
+* Added new public properties to OptimizelyConfig.
+  - sdk_key and environment_key [#338] (https://github.com/optimizely/python-sdk/pull/338)
+  - attributes and events [#339] (https://github.com/optimizely/python-sdk/pull/339)
+  - experiment_rules, delivery_rules, audiences and audiences in OptimizelyExperiment
+    - [#342] (https://github.com/optimizely/python-sdk/pull/342)
+    - [#351] (https://github.com/optimizely/python-sdk/pull/351/files)
+* For details please refer to our documentation page:
+  - Python-sdk: [https://docs.developers.optimizely.com/full-stack/docs/optimizelyconfig-python]
+
+* OptimizelyFeature.experiments_map of OptimizelyConfig is now deprecated. Please use OptimizelyFeature.experiment_rules and OptimizelyFeature.delivery_rules. [#360] (https://github.com/optimizely/python-sdk/pull/360)
+
+### Bug Fixes
+* Fix event processor negative timeout interval when retrieving events from queue. [#356] (https://github.com/optimizely/python-sdk/pull/356)
+
+## 3.9.1
+July 14th, 2021
+
+### Bug Fixes:
+* Fixed issue with serving incorrect variation in projects containing multiple flags with duplicate keys. [#347] (https://github.com/optimizely/python-sdk/pull/347)
+* Fixed issue with serving incorrect variation in create_impression_event in user_event_factory.py. [#350] (https://github.com/optimizely/python-sdk/pull/350)
+
+## 3.9.0
+June 1st, 2021
+
+### New Features
+* Added support for multiple concurrent prioritized experiments per flag. [#322](https://github.com/optimizely/python-sdk/pull/322)
+
+## 3.8.0
+February 12th, 2021
+
+### New Features
+* New Features
+Introducing a new primary interface for retrieving feature flag status, configuration and associated experiment decisions for users ([#309](https://github.com/optimizely/python-sdk/pull/309)). The new `OptimizelyUserContext` class is instantiated with `create_user_context` and exposes the following APIs to get `OptimizelyDecision`:
+
+    - set_attribute
+    - decide
+    - decide_all
+    - decide_for_keys
+    - track_event
+
+For details, refer to our documentation page: https://docs.developers.optimizely.com/full-stack/v4.0/docs/python-sdk.
+
+## 3.7.1
+November 19th, 2020
+
+### Bug Fixes:
+* Added "enabled" field to decision metadata structure. [#306](https://github.com/optimizely/python-sdk/pull/306)
+
+## 3.7.0
+November 2nd, 2020
+
+### New Features
+* Added support for upcoming application-controlled introduction of tracking for non-experiment Flag decisions. [#300](https://github.com/optimizely/python-sdk/pull/300)
+
+## 3.6.0
+October 1st, 2020
+
+### New Features:
+* Version targeting using semantic version syntax. [#293](https://github.com/optimizely/python-sdk/pull/293)
+* Datafile accessor API added to access current config as a JSON string. [#283](https://github.com/optimizely/python-sdk/pull/283)
+
+### Bug Fixes:
+* Fixed package installation for Python 3.4 and pypy. [#298](https://github.com/optimizely/python-sdk/pull/298)
+
+## 3.5.2
+July 14th, 2020
+
+### Bug Fixes:
+* Fixed handling of network and no status code errors when polling for datafile in `PollingConfigManager` and `AuthDatafilePollingConfigManager`. ([#287](https://github.com/optimizely/python-sdk/pull/287))
+
+## 3.5.1
+July 10th, 2020
+
+### Bug Fixes:
+* Fixed HTTP request exception handling in `PollingConfigManager`. ([#285](https://github.com/optimizely/python-sdk/pull/285))
+
+## 3.5.0
+July 9th, 2020
+
+### New Features:
+* Introduced 2 APIs to interact with feature variables:
+  * `get_feature_variable_json` allows you to get value for JSON variables related to a feature.
+  * `get_all_feature_variables` gets values for all variables under a feature.
+* Added support for fetching authenticated datafiles. `AuthDatafilePollingConfigManager` is a new config manager that allows you to poll for a datafile belonging to a secure environment. You can create a client by setting the `datafile_access_token`.
+
+### Bug Fixes:
+* Fixed log messages for targeted rollouts evaluation. ([#268](https://github.com/optimizely/python-sdk/pull/268))
+
+## 3.4.2
+June 11th, 2020
+
+### Bug Fixes:
+* Adjusted log level for audience evaluation logs. ([#267](https://github.com/optimizely/python-sdk/pull/267))
+
+## 3.4.1
+March 19th, 2020
+
+### Bug Fixes:
+* Updated `jsonschema` to address [installation issue](https://github.com/optimizely/python-sdk/issues/232).
+
+## 3.4.0
+January 27th, 2020
+
+### New Features:
+* Added a new API to get project configuration static data.
+  * Call `get_optimizely_config()` to get a snapshot of project configuration static data.
+  * It returns an `OptimizelyConfig` instance which includes a datafile revision number, all experiments, and feature flags mapped by their key values.
+  * Added caching for `get_optimizely_config()` - `OptimizelyConfig` object will be cached and reused for the lifetime of the datafile.
+  * For details, refer to our documentation page: [https://docs.developers.optimizely.com/full-stack/docs/optimizelyconfig-python](https://docs.developers.optimizely.com/full-stack/docs/optimizelyconfig-python).
+
+
+## 3.3.1
+December 16th, 2019
+
+### Bug Fixes:
+* Fixed [installation issue](https://github.com/optimizely/python-sdk/issues/220) on Windows. ([#224](https://github.com/optimizely/python-sdk/pull/224))
+* Fixed batch event processor deadline reset issue. ([#227](https://github.com/optimizely/python-sdk/pull/227))
+* Added more batch event processor debug messages. ([#227](https://github.com/optimizely/python-sdk/pull/227))
+
+## 3.3.0
+October 28th, 2019
+
+### New Features:
+* Added support for event batching via the event processor.
+  * Events generated by methods like `activate`, `track`, and `is_feature_enabled` will be held in a queue until the configured batch size is reached, or the configured flush interval has elapsed. Then, they will be batched into a single payload and sent to the event dispatcher.
+  * To configure event batching, set the `batch_size` and `flush_interval` properties when initializing instance of [BatchEventProcessor](https://github.com/optimizely/python-sdk/blob/3.3.x/optimizely/event/event_processor.py#L45).
+  * Event batching is disabled by default. You can pass in instance of `BatchEventProcessor` when creating `Optimizely` instance to enable event batching.
+  * Users can subscribe to `LogEvent` notification to be notified of whenever a payload consisting of a batch of user events is handed off to the event dispatcher to send to Optimizely's backend.
+* Introduced blocking timeout in `PollingConfigManager`. By default, calls to `get_config` will block for maximum of 10 seconds until config is available.
+
+### Bug Fixes:
+* Fixed incorrect log message when numeric metric is not used. ([#217](https://github.com/optimizely/python-sdk/pull/217))
+
+## 3.2.0
+August 27th, 2019
+
+### New Features:
+* Added support for automatic datafile management via [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151):
+  * The [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151) is an implementation of the [BaseConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L32).
+  * Users may provide one of datafile or SDK key (sdk_key) or both to `optimizely.Optimizely`. Based on that, the SDK will use the [StaticConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L73) or the [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151). Refer to the [README](README.md) for more instructions.
+  * An initial datafile can be provided to the `PollingConfigManager` to bootstrap before making HTTP requests for the hosted datafile.
+  * Requests for the datafile are made in a separate thread and are scheduled with fixed delay.
+  * Configuration updates can be subscribed to by adding the OPTIMIZELY_CONFIG_UPDATE notification listener.
+* Introduced `Optimizely.get_feature_variable` API.  ([#191](https://github.com/optimizely/python-sdk/pull/191))
+
+### Deprecated:
+
+* `NotificationCenter.clear_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
+* `NotificationCenter.clear_all_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_all_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
+
+## 3.2.0b1
+July 26th, 2019
+
+### New Features:
+* Added support for automatic datafile management via [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151):
+  * The [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151) is an implementation of the [BaseConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L32).
+  * Users may provide one of datafile or SDK key (sdk_key) or both to `optimizely.Optimizely`. Based on that, the SDK will use the [StaticConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L73) or the [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151). Refer to the [README](README.md) for more instructions.
+  * An initial datafile can be provided to the `PollingConfigManager` to bootstrap before making HTTP requests for the hosted datafile.
+  * Requests for the datafile are made in a separate thread and are scheduled with fixed delay.
+  * Configuration updates can be subscribed to by adding the OPTIMIZELY_CONFIG_UPDATE notification listener.
+* Introduced `Optimizely.get_feature_variable` API.  ([#191](https://github.com/optimizely/python-sdk/pull/191))
+
+### Deprecated:
+
+* `NotificationCenter.clear_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
+* `NotificationCenter.clear_all_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_all_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
+
+## 3.1.0
+May 3rd, 2019
+
+### New Features:
+* Introduced Decision notification listener to be able to record:
+  * Variation assignments for users activated in an experiment.
+  * Feature access for users.
+  * Feature variable value for users.
+
+### Bug Fixes:
+* Feature variable APIs now return default variable value when featureEnabled property is false.  ([#171](https://github.com/optimizely/python-sdk/pull/171))
+
+### Deprecated:
+* Activate notification listener is deprecated as of this release.  Recommendation is to use the new Decision notification listener.  Activate notification listener will be removed in the next major release.
+
+## 3.0.0
+March 1st, 2019
+
+The 3.0 release improves event tracking and supports additional audience
+targeting functionality.
+
+### New Features:
+* Event tracking:
+  * The `track` method now dispatches its conversion event *unconditionally*, without first determining whether the user is targeted by a known experiment that uses the event. This may increase outbound network traffic.
+  * In Optimizely results, conversion events sent by 3.0 SDKs don\'t explicitly name the experiments and variations that are currently targeted to the user. Instead, conversions are automatically attributed to variations that the user has previously seen, as long as those variations were served via 3.0 SDKs or by other clients capable of automatic attribution, and as long as our backend actually received the impression events for those variations.
+  * Altogether, this allows you to track conversion events and attribute them to variations even when you don't know all of a user's attribute values, and even if the user's attribute values or the experiment's configuration have changed such that the user is no longer affected by the experiment. As a result, **you may observe an increase in the conversion rate for previously-instrumented events.** If that is undesirable, you can reset the results of previously-running experiments after upgrading to the 3.0 SDK.  -   This will also allow you to attribute events to variations from other Optimizely projects in your account, even though those experiments don't appear in the same datafile.
+  * Note that for results segmentation in Optimizely results, the user attribute values from one event are automatically applied to all other events in the same session, as long as the events in question were actually received by our backend. This behavior was already in place and is not affected by the 3.0 release.
+* Support for all types of attribute values, not just strings.
+  * All values are passed through to notification listeners.
+  * Strings, booleans, and valid numbers are passed to the event dispatcher and can be used for Optimizely results segmentation.  A valid number is a finite float or numbers.Integral in the inclusive range \[-2 ^ 53, 2 ^ 53\].
+  * Strings, booleans, and valid numbers are relevant for audience conditions.
+* Support for additional matchers in audience conditions:
+  * An `exists` matcher that passes if the user has a non-null value for the targeted user attribute and fails otherwise.
+  * A `substring` matcher that resolves if the user has a string value for the targeted attribute.
+    * `gt` (greater than) and `lt` (less than) matchers that resolve if the user has a valid number value for the targeted attribute.  A valid number is a finite float or numbers.Integral in the inclusive range \[-2 ^ 53, 2 ^ 53\].
+    * The original (`exact`) matcher can now be used to target booleans and valid numbers, not just strings.
+* Support for A/B tests, feature tests, and feature rollouts whose audiences are combined using `"and"` and `"not"` operators, not just the `"or"` operator.
+* Datafile-version compatibility check: The SDK will remain uninitialized (i.e., will gracefully fail to activate experiments and features) if given a datafile version greater than 4.
+* Updated Pull Request template and commit message guidelines.
+
+### Breaking Changes:
+* Conversion events sent by 3.0 SDKs don\'t explicitly name the experiments and variations that are currently targeted to the user, so these events are unattributed in raw events data export. You must use the new *results* export to determine the variations to which events have been attributed.
+* Previously, notification listeners were only given string-valued user attributes because only strings could be passed into various method calls. That is no longer the case. You may pass non-string attribute values, and if you do, you must update your notification listeners to be able to receive whatever values you pass in.
+
+### Bug Fixes:
+* Experiments and features can no longer activate when a negatively targeted attribute has a missing, null, or malformed value.
+  * Audience conditions (except for the new `exists` matcher) no longer resolve to `false` when they fail to find an legitimate value for the targeted user attribute. The result remains `null` (unknown). Therefore, an audience that negates such a condition (using the `"not"` operator) can no longer resolve to `true` unless there is an unrelated branch in the condition tree that itself resolves to `true`.
+* Updated the default event dispatcher to log an error if the request resolves to HTTP 4xx or 5xx.  ([#140](https://github.com/optimizely/python-sdk/pull/140))
+* All methods now validate that user IDs are strings and that experiment keys, feature keys, feature variable keys, and event keys are non-empty strings.
+
+## 2.1.1
+August 21st, 2018
+
+* Fix: record conversions for all experiments using an event when using track([#136](https://github.com/optimizely/python-sdk/pull/136)).
+
+## 2.1.0
+July 2nd, 2018
+
+* Introduced support for bot filtering ([#121](https://github.com/optimizely/python-sdk/pull/121)).
+* Overhauled logging to use standard Python logging ([#123](https://github.com/optimizely/python-sdk/pull/123)).
+
+## 2.0.1
+June 19th, 2018
+
+* Fix: send impression event for Feature Test when Feature is disabled ([#128](https://github.com/optimizely/python-sdk/pull/128)).
+
+## 2.0.0
+April 12th, 2018
+
+This major release introduces APIs for Feature Management. It also
+introduces some breaking changes listed below.
+
+### New Features
+* Introduced the `is_feature_enabled` API to determine whether to show a feature to a user or not.
+
+```
+    is_enabled = optimizel_client.is_feature_enabled('my_feature_key', 'my_user', user_attributes)
+```
+
+* All enabled features for the user can be retrieved by calling:
+
+```
+    enabled_features = optimizely_client.get_enabled_features('my_user', user_attributes)
+```
+* Introduced Feature Variables to configure or parameterize a feature.  There are four variable types: `String`, `Integer`, `Double`, `Boolean`.
+
+```
+    string_variable = optimizely_client.get_feature_variable_string('my_feature_key', 'string_variable_key', 'my_user')
+    integer_variable = optimizely_client.get_feature_variable_integer('my_feature_key', 'integer_variable_key', 'my_user')
+    double_variable = optimizely_client.get_feature_variable_double('my_feature_key', 'double_variable_key', 'my_user')
+    boolean_variable = optimizely_client.get_feature_variable_boolean('my_feature_key', 'boolean_variable_key', 'my_user')
+```
+
+### Breaking changes
+* The `track` API with revenue value as a stand-alone parameter has been removed. The revenue value should be passed in as an entry in the event tags dict. The key for the revenue tag is `revenue` and the passed in value will be treated by Optimizely as the value for computing results.
+
+```
+    event_tags = {
+      'revenue': 1200
+    }
+
+    optimizely_client.track('event_key', 'my_user', user_attributes, event_tags)
+```
+
+## 2.0.0b1
+March 29th, 2018
+
+This beta release introduces APIs for Feature Management. It also
+introduces some breaking changes listed below.
+
+### New Features
+* Introduced the `is_feature_enabled` API to determine whether to show a feature to a user or not.
+```
+    is_enabled = optimizel_client.is_feature_enabled('my_feature_key', 'my_user', user_attributes)
+```
+
+* All enabled features for the user can be retrieved by calling:
+
+```
+    enabled_features = optimizely_client.get_enabled_features('my_user', user_attributes)
+```
+
+* Introduced Feature Variables to configure or parameterize a feature.  There are four variable types: `String`, `Integer`, `Double`, `Boolean`.
+
+```
+    string_variable = optimizely_client.get_feature_variable_string('my_feature_key', 'string_variable_key', 'my_user')
+    integer_variable = optimizely_client.get_feature_variable_integer('my_feature_key', 'integer_variable_key', 'my_user')
+    double_variable = optimizely_client.get_feature_variable_double('my_feature_key', 'double_variable_key', 'my_user')
+    boolean_variable = optimizely_client.get_feature_variable_boolean('my_feature_key', 'boolean_variable_key', 'my_user')
+```
+
+### Breaking changes
+* The `track` API with revenue value as a stand-alone parameter has been removed. The revenue value should be passed in as an entry in the event tags dict. The key for the revenue tag is `revenue` and the passed in value will be treated by Optimizely as the value for computing results.
+
+```
+    event_tags = {
+      'revenue': 1200
+    }
+
+    optimizely_client.track('event_key', 'my_user', user_attributes, event_tags)
+```
+
+## 1.4.0
+
+* Added support for IP anonymization.
+* Added support for notification listeners.
+* Added support for bucketing ID.
+* Updated mmh3 to handle installation failures on Windows 10.
+
+## 1.3.0
+
+* Introduced support for forced bucketing.
+* Introduced support for numeric metrics.
+* Updated event builder to support new endpoint.
+
+## 1.2.1
+
+* Removed older feature flag parsing.
+
+## 1.2.0
+
+* Added user profile service.
+
+## 1.1.1
+
+* Updated datafile parsing to be able to handle additional fields.
+* Deprecated Classic project support.
+
+## 1.1.0
+
+* Included datafile revision information in log events.
+* Added event tags to track API to allow users to pass in event metadata.
+* Deprecated the `event_value` parameter from the track method. Should use `event_tags` to pass in event value instead.
+* Updated event logging endpoint to logx.optimizely.com.
+
+## 1.0.0
+
+* Introduced support for Full Stack projects in Optimizely X. No breaking changes from previous version.
+* Introduced more graceful exception handling in instantiation and core methods.
+* Updated whitelisting to precede audience matching.
+
+## 0.1.3
+
+* Added support for v2 endpoint and datafile.
+* Updated dispatch_event to consume an Event object instead of url and params. The Event object comprises of four properties: url (string representing URL to dispatch event to), params (dict representing the params to be set for the event), http_verb (one of 'GET' or 'POST') and headers (header values to be sent along).
+* Fixed issue with tracking events for experiments in groups.
+
+## 0.1.2
+
+* Updated requirements file.
+
+## 0.1.1
+
+* Introduced option to skip JSON schema validation.
+
+## 0.1.0
+
+* Beta release of the Python SDK for server-side testing.
```

### Comparing `optimizely-sdk-4.1.1/README.md` & `optimizely-sdk-5.0.0b0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,258 +1,258 @@
-# Optimizely Python SDK
-
-[![PyPI version](https://badge.fury.io/py/optimizely-sdk.svg)](https://pypi.org/project/optimizely-sdk)
-[![Build Status](https://travis-ci.org/optimizely/python-sdk.svg?branch=master)](https://travis-ci.org/optimizely/python-sdk)
-[![Coverage Status](https://coveralls.io/repos/github/optimizely/python-sdk/badge.svg)](https://coveralls.io/github/optimizely/python-sdk)
-[![Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](http://www.apache.org/licenses/LICENSE-2.0)
-
-This repository houses the Python SDK for use with Optimizely Feature Experimentation and Optimizely Full Stack (legacy).
-
-Optimizely Feature Experimentation is an A/B testing and feature management tool for product development teams that enables you to experiment at every step. Using Optimizely Feature Experimentation allows for every feature on your roadmap to be an opportunity to discover hidden insights. Learn more at [Optimizely.com](https://www.optimizely.com/products/experiment/feature-experimentation/), or see the [developer documentation](https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/welcome).
-
-Optimizely Rollouts is [free feature flags](https://www.optimizely.com/free-feature-flagging/) for development teams. You can easily roll out and roll back features in any application without code deploys, mitigating risk for every feature on your roadmap.
-
-## Get Started
-
-Refer to the [Python SDK's developer documentation](https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/python-sdk) for detailed instructions on getting started with using the SDK.
-
-### Requirements
-
-Version `4.0+`: Python 3.7+, PyPy 3.7+
-
-Version `3.0+`: Python 2.7+, PyPy 3.4+
-
-### Install the SDK
-
-The SDK is available through [PyPi](https://pypi.python.org/pypi?name=optimizely-sdk&:action=display).
-
-To install:
-
-    pip install optimizely-sdk
-
-### Feature Management Access
-
-To access the Feature Management configuration in the Optimizely
-dashboard, please contact your Optimizely customer success manager.
-
-## Use the Python SDK
-
-### Initialization
-
-You can initialize the Optimizely instance in three ways: with a datafile, by providing an sdk_key, or by providing an implementation of
-[BaseConfigManager](https://github.com/optimizely/python-sdk/tree/master/optimizely/config_manager.py#L32).
-Each method is described below.
-
-1.  Initialize Optimizely with a datafile. This datafile will be used as
-    the source of ProjectConfig throughout the life of Optimizely instance:
-
-        optimizely.Optimizely(
-          datafile
-        )
-
-2.  Initialize Optimizely by providing an \'sdk_key\'. This will
-    initialize a PollingConfigManager that makes an HTTP GET request to
-    the URL (formed using your provided sdk key and the
-    default datafile CDN URL template) to asynchronously download the
-    project datafile at regular intervals and update ProjectConfig when
-    a new datafile is received. A hard-coded datafile can also be
-    provided along with the sdk_key that will be used
-    initially before any update:
-
-        optimizely.Optimizely(
-          sdk_key='put_your_sdk_key_here'
-        )
-
-    If providing a datafile, the initialization will look like:
-
-        optimizely.Optimizely(
-          datafile=datafile,
-          sdk_key='put_your_sdk_key_here'
-        )
-
-3.  Initialize Optimizely by providing a ConfigManager that implements
-    [BaseConfigManager](https://github.com/optimizely/python-sdk/tree/master/optimizely/config_manager.py#L34).
-    You may use our [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L150) or
-    [AuthDatafilePollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L375) as needed:
-
-        optimizely.Optimizely(
-          config_manager=custom_config_manager
-        )
-
-### PollingConfigManager
-
-The [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L150) asynchronously polls for
-datafiles from a specified URL at regular intervals by making HTTP requests.
-
-    polling_config_manager = PollingConfigManager(
-        sdk_key=None,
-        datafile=None,
-        update_interval=None,
-        url=None,
-        url_template=None,
-        logger=None,
-        error_handler=None,
-        notification_center=None,
-        skip_json_validation=False
-    )
-
-**Note**: You must provide either the sdk_key or URL. If
-you provide both, the URL takes precedence.
-
-**sdk_key** The sdk_key is used to compose the outbound
-HTTP request to the default datafile location on the Optimizely CDN.
-
-**datafile** You can provide an initial datafile to bootstrap the
-`ProjectConfigManager` so that it can be used immediately. The initial
-datafile also serves as a fallback datafile if HTTP connection cannot be
-established. The initial datafile will be discarded after the first
-successful datafile poll.
-
-**update_interval** The update_interval is used to specify a fixed
-delay in seconds between consecutive HTTP requests for the datafile.
-
-**url** The target URL from which to request the datafile.
-
-**url_template** A string with placeholder `{sdk_key}` can be provided
-so that this template along with the provided sdk key is
-used to form the target URL.
-
-You may also provide your own logger, error_handler, or
-notification_center.
-
-### AuthDatafilePollingConfigManager
-
-The [AuthDatafilePollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L375)
-implements `PollingConfigManager` and asynchronously polls for authenticated datafiles from a specified URL at regular intervals
-by making HTTP requests.
-
-    auth_datafile_polling_config_manager = AuthDatafilePollingConfigManager(
-        datafile_access_token,
-        *args,
-        **kwargs
-    )
-
-**Note**: To use [AuthDatafilePollingConfigManager](#authdatafilepollingconfigmanager), you must create a secure environment for
-your project and generate an access token for your datafile.
-
-**datafile_access_token** The datafile_access_token is attached to the outbound HTTP request header to authorize the request and fetch the datafile.
-
-### Advanced configuration
-
-The following properties can be set to override the default
-configurations for [PollingConfigManager](#pollingconfigmanager) and [AuthDatafilePollingConfigManager](#authdatafilepollingconfigmanager).
-
-| **Property Name** |                                                                                    **Default Value**                                                                                    |                        **Description**                         |
-| :---------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------: |
-|      sdk_key      |                                                                                          None                                                                                           |                   Optimizely project SDK key                   |
-|     datafile      |                                                                                          None                                                                                           | Initial datafile, typically sourced from a local cached source |
-|  update_interval  |                                                                                        5 minutes                                                                                        |          Fixed delay between fetches for the datafile          |
-|        url        |                                                                                          None                                                                                           |      Custom URL location from which to fetch the datafile      |
-|   url_template    | `PollingConfigManager:`<br/>https://cdn.optimizely.com/datafiles/{sdk_key}.json<br/>`AuthDatafilePollingConfigManager:`<br/>https://config.optimizely.com/datafiles/auth/{sdk_key}.json |             Parameterized datafile URL by SDK key              |
-
-A notification signal will be triggered whenever a _new_ datafile is
-fetched and Project Config is updated. To subscribe to these
-notifications, use:
-
-```
-notification_center.add_notification_listener(NotificationTypes.OPTIMIZELY_CONFIG_UPDATE, update_callback)
-```
-
-For Further details see the Optimizely [Feature Experimentation documentation](https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/welcome)
-to learn how to set up your first Python project and use the SDK.
-
-## SDK Development
-
-### Building the SDK
-
-Build and install the SDK with pip, using the following command:
-
-    pip install -e .
-
-### Unit Tests
-
-#### Running all tests
-
-To get test dependencies installed, use a modified version of the
-install command:
-
-    pip install -e '.[test]'
-
-You can run all unit tests with:
-
-    pytest
-
-#### Running all tests in a file
-
-To run all tests under a particular test file you can use the following
-command:
-
-    pytest tests.<file_name_without_extension>
-
-For example, to run all tests under `test_event_builder`, the command would be:
-
-    pytest tests/test_event_builder.py
-
-#### Running all tests under a class
-
-To run all tests under a particular class of tests you can use the
-following command:
-
-    pytest tests/<file_name_with_extension>::ClassName
-
-For example, to run all tests under `test_event_builder.EventTest`, the command
-would be:
-
-    pytest tests/test_event_builder.py::EventTest
-
-#### Running a single test
-
-To run a single test you can use the following command:
-
-    pytest tests/<file_name_with_extension>::ClassName::test_name
-
-For example, to run `test_event_builder.EventTest.test_init`, the command
-would be:
-
-    pytest tests/test_event_builder.py::EventTest::test_init
-
-### Contributing
-
-Please see [CONTRIBUTING](https://github.com/optimizely/python-sdk/blob/master/CONTRIBUTING.md).
-
-### Credits
-
-This software incorporates code from the following open source projects:
-
-requests (Apache-2.0 License: https://github.com/psf/requests/blob/master/LICENSE)
-
-pyOpenSSL (Apache-2.0 License https://github.com/pyca/pyopenssl/blob/main/LICENSE)
-
-cryptography (Apache-2.0 https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE)
-
-idna (BSD 3-Clause License https://github.com/kjd/idna/blob/master/LICENSE.md)
-
-### Other Optimizely SDKs
-
-- Agent - https://github.com/optimizely/agent
-
-- Android - https://github.com/optimizely/android-sdk
-
-- C# - https://github.com/optimizely/csharp-sdk
-
-- Flutter - https://github.com/optimizely/optimizely-flutter-sdk
-
-- Go - https://github.com/optimizely/go-sdk
-
-- Java - https://github.com/optimizely/java-sdk
-
-- JavaScript - https://github.com/optimizely/javascript-sdk
-
-- PHP - https://github.com/optimizely/php-sdk
-
-- Python - https://github.com/optimizely/python-sdk
-
-- React - https://github.com/optimizely/react-sdk
-
-- Ruby - https://github.com/optimizely/ruby-sdk
-
-- Swift - https://github.com/optimizely/swift-sdk
+# Optimizely Python SDK
+
+[![PyPI version](https://badge.fury.io/py/optimizely-sdk.svg)](https://pypi.org/project/optimizely-sdk)
+[![Build Status](https://github.com/optimizely/python-sdk/actions/workflows/python.yml/badge.svg?branch=master)](https://github.com/optimizely/python-sdk/actions/workflows/python.yml?query=branch%3Amaster)
+[![Coverage Status](https://coveralls.io/repos/github/optimizely/python-sdk/badge.svg)](https://coveralls.io/github/optimizely/python-sdk)
+[![Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](http://www.apache.org/licenses/LICENSE-2.0)
+
+This repository houses the Python SDK for use with Optimizely Feature Experimentation and Optimizely Full Stack (legacy).
+
+Optimizely Feature Experimentation is an A/B testing and feature management tool for product development teams that enables you to experiment at every step. Using Optimizely Feature Experimentation allows for every feature on your roadmap to be an opportunity to discover hidden insights. Learn more at [Optimizely.com](https://www.optimizely.com/products/experiment/feature-experimentation/), or see the [developer documentation](https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/welcome).
+
+Optimizely Rollouts is [free feature flags](https://www.optimizely.com/free-feature-flagging/) for development teams. You can easily roll out and roll back features in any application without code deploys, mitigating risk for every feature on your roadmap.
+
+## Get Started
+
+Refer to the [Python SDK's developer documentation](https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/python-sdk) for detailed instructions on getting started with using the SDK.
+
+### Requirements
+
+Version `4.0+`: Python 3.7+, PyPy 3.7+
+
+Version `3.0+`: Python 2.7+, PyPy 3.4+
+
+### Install the SDK
+
+The SDK is available through [PyPi](https://pypi.python.org/pypi?name=optimizely-sdk&:action=display).
+
+To install:
+
+    pip install optimizely-sdk
+
+### Feature Management Access
+
+To access the Feature Management configuration in the Optimizely
+dashboard, please contact your Optimizely customer success manager.
+
+## Use the Python SDK
+
+### Initialization
+
+You can initialize the Optimizely instance in three ways: with a datafile, by providing an sdk_key, or by providing an implementation of
+[BaseConfigManager](https://github.com/optimizely/python-sdk/tree/master/optimizely/config_manager.py#L32).
+Each method is described below.
+
+1.  Initialize Optimizely with a datafile. This datafile will be used as
+    the source of ProjectConfig throughout the life of Optimizely instance:
+
+        optimizely.Optimizely(
+          datafile
+        )
+
+2.  Initialize Optimizely by providing an \'sdk_key\'. This will
+    initialize a PollingConfigManager that makes an HTTP GET request to
+    the URL (formed using your provided sdk key and the
+    default datafile CDN URL template) to asynchronously download the
+    project datafile at regular intervals and update ProjectConfig when
+    a new datafile is received. A hard-coded datafile can also be
+    provided along with the sdk_key that will be used
+    initially before any update:
+
+        optimizely.Optimizely(
+          sdk_key='put_your_sdk_key_here'
+        )
+
+    If providing a datafile, the initialization will look like:
+
+        optimizely.Optimizely(
+          datafile=datafile,
+          sdk_key='put_your_sdk_key_here'
+        )
+
+3.  Initialize Optimizely by providing a ConfigManager that implements
+    [BaseConfigManager](https://github.com/optimizely/python-sdk/tree/master/optimizely/config_manager.py#L34).
+    You may use our [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L150) or
+    [AuthDatafilePollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L375) as needed:
+
+        optimizely.Optimizely(
+          config_manager=custom_config_manager
+        )
+
+### PollingConfigManager
+
+The [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L150) asynchronously polls for
+datafiles from a specified URL at regular intervals by making HTTP requests.
+
+    polling_config_manager = PollingConfigManager(
+        sdk_key=None,
+        datafile=None,
+        update_interval=None,
+        url=None,
+        url_template=None,
+        logger=None,
+        error_handler=None,
+        notification_center=None,
+        skip_json_validation=False
+    )
+
+**Note**: You must provide either the sdk_key or URL. If
+you provide both, the URL takes precedence.
+
+**sdk_key** The sdk_key is used to compose the outbound
+HTTP request to the default datafile location on the Optimizely CDN.
+
+**datafile** You can provide an initial datafile to bootstrap the
+`ProjectConfigManager` so that it can be used immediately. The initial
+datafile also serves as a fallback datafile if HTTP connection cannot be
+established. The initial datafile will be discarded after the first
+successful datafile poll.
+
+**update_interval** The update_interval is used to specify a fixed
+delay in seconds between consecutive HTTP requests for the datafile.
+
+**url** The target URL from which to request the datafile.
+
+**url_template** A string with placeholder `{sdk_key}` can be provided
+so that this template along with the provided sdk key is
+used to form the target URL.
+
+You may also provide your own logger, error_handler, or
+notification_center.
+
+### AuthDatafilePollingConfigManager
+
+The [AuthDatafilePollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L375)
+implements `PollingConfigManager` and asynchronously polls for authenticated datafiles from a specified URL at regular intervals
+by making HTTP requests.
+
+    auth_datafile_polling_config_manager = AuthDatafilePollingConfigManager(
+        datafile_access_token,
+        *args,
+        **kwargs
+    )
+
+**Note**: To use [AuthDatafilePollingConfigManager](#authdatafilepollingconfigmanager), you must create a secure environment for
+your project and generate an access token for your datafile.
+
+**datafile_access_token** The datafile_access_token is attached to the outbound HTTP request header to authorize the request and fetch the datafile.
+
+### Advanced configuration
+
+The following properties can be set to override the default
+configurations for [PollingConfigManager](#pollingconfigmanager) and [AuthDatafilePollingConfigManager](#authdatafilepollingconfigmanager).
+
+| **Property Name** |                                                                                    **Default Value**                                                                                    |                        **Description**                         |
+| :---------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------: |
+|      sdk_key      |                                                                                          None                                                                                           |                   Optimizely project SDK key                   |
+|     datafile      |                                                                                          None                                                                                           | Initial datafile, typically sourced from a local cached source |
+|  update_interval  |                                                                                        5 minutes                                                                                        |          Fixed delay between fetches for the datafile          |
+|        url        |                                                                                          None                                                                                           |      Custom URL location from which to fetch the datafile      |
+|   url_template    | `PollingConfigManager:`<br/>https://cdn.optimizely.com/datafiles/{sdk_key}.json<br/>`AuthDatafilePollingConfigManager:`<br/>https://config.optimizely.com/datafiles/auth/{sdk_key}.json |             Parameterized datafile URL by SDK key              |
+
+A notification signal will be triggered whenever a _new_ datafile is
+fetched and Project Config is updated. To subscribe to these
+notifications, use:
+
+```
+notification_center.add_notification_listener(NotificationTypes.OPTIMIZELY_CONFIG_UPDATE, update_callback)
+```
+
+For Further details see the Optimizely [Feature Experimentation documentation](https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/welcome)
+to learn how to set up your first Python project and use the SDK.
+
+## SDK Development
+
+### Building the SDK
+
+Build and install the SDK with pip, using the following command:
+
+    pip install -e .
+
+### Unit Tests
+
+#### Running all tests
+
+To get test dependencies installed, use a modified version of the
+install command:
+
+    pip install -e '.[test]'
+
+You can run all unit tests with:
+
+    pytest
+
+#### Running all tests in a file
+
+To run all tests under a particular test file you can use the following
+command:
+
+    pytest tests.<file_name_without_extension>
+
+For example, to run all tests under `test_event_builder`, the command would be:
+
+    pytest tests/test_event_builder.py
+
+#### Running all tests under a class
+
+To run all tests under a particular class of tests you can use the
+following command:
+
+    pytest tests/<file_name_with_extension>::ClassName
+
+For example, to run all tests under `test_event_builder.EventTest`, the command
+would be:
+
+    pytest tests/test_event_builder.py::EventTest
+
+#### Running a single test
+
+To run a single test you can use the following command:
+
+    pytest tests/<file_name_with_extension>::ClassName::test_name
+
+For example, to run `test_event_builder.EventTest.test_init`, the command
+would be:
+
+    pytest tests/test_event_builder.py::EventTest::test_init
+
+### Contributing
+
+Please see [CONTRIBUTING](https://github.com/optimizely/python-sdk/blob/master/CONTRIBUTING.md).
+
+### Credits
+
+This software incorporates code from the following open source projects:
+
+requests (Apache-2.0 License: https://github.com/psf/requests/blob/master/LICENSE)
+
+pyOpenSSL (Apache-2.0 License https://github.com/pyca/pyopenssl/blob/main/LICENSE)
+
+cryptography (Apache-2.0 https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE)
+
+idna (BSD 3-Clause License https://github.com/kjd/idna/blob/master/LICENSE.md)
+
+### Other Optimizely SDKs
+
+- Agent - https://github.com/optimizely/agent
+
+- Android - https://github.com/optimizely/android-sdk
+
+- C# - https://github.com/optimizely/csharp-sdk
+
+- Flutter - https://github.com/optimizely/optimizely-flutter-sdk
+
+- Go - https://github.com/optimizely/go-sdk
+
+- Java - https://github.com/optimizely/java-sdk
+
+- JavaScript - https://github.com/optimizely/javascript-sdk
+
+- PHP - https://github.com/optimizely/php-sdk
+
+- Python - https://github.com/optimizely/python-sdk
+
+- React - https://github.com/optimizely/react-sdk
+
+- Ruby - https://github.com/optimizely/ruby-sdk
+
+- Swift - https://github.com/optimizely/swift-sdk
```

### Comparing `optimizely-sdk-4.1.1/optimizely/__init__.py` & `optimizely-sdk-5.0.0b0/optimizely/__init__.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2016, Optimizely
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# Copyright 2016, Optimizely
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
```

### Comparing `optimizely-sdk-4.1.1/optimizely/bucketer.py` & `optimizely-sdk-5.0.0b0/optimizely/bucketer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,150 +1,166 @@
-# Copyright 2016-2017, 2019-2021 Optimizely
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import math
-
-from .lib import pymmh3 as mmh3
-
-
-MAX_TRAFFIC_VALUE = 10000
-UNSIGNED_MAX_32_BIT_VALUE = 0xFFFFFFFF
-MAX_HASH_VALUE = math.pow(2, 32)
-HASH_SEED = 1
-BUCKETING_ID_TEMPLATE = '{bucketing_id}{parent_id}'
-GROUP_POLICIES = ['random']
-
-
-class Bucketer(object):
-    """ Optimizely bucketing algorithm that evenly distributes visitors. """
-
-    def __init__(self):
-        """ Bucketer init method to set bucketing seed and logger instance. """
-
-        self.bucket_seed = HASH_SEED
-
-    def _generate_unsigned_hash_code_32_bit(self, bucketing_id):
-        """ Helper method to retrieve hash code.
-
-        Args:
-            bucketing_id: ID for bucketing.
-
-        Returns:
-            Hash code which is a 32 bit unsigned integer.
-        """
-
-        # Adjusting MurmurHash code to be unsigned
-        return mmh3.hash(bucketing_id, self.bucket_seed) & UNSIGNED_MAX_32_BIT_VALUE
-
-    def _generate_bucket_value(self, bucketing_id):
-        """ Helper function to generate bucket value in half-closed interval [0, MAX_TRAFFIC_VALUE).
-
-        Args:
-            bucketing_id: ID for bucketing.
-
-        Returns:
-            Bucket value corresponding to the provided bucketing ID.
-        """
-
-        ratio = float(self._generate_unsigned_hash_code_32_bit(bucketing_id)) / MAX_HASH_VALUE
-        return math.floor(ratio * MAX_TRAFFIC_VALUE)
-
-    def find_bucket(self, project_config, bucketing_id, parent_id, traffic_allocations):
-        """ Determine entity based on bucket value and traffic allocations.
-
-        Args:
-            project_config: Instance of ProjectConfig.
-            bucketing_id: ID to be used for bucketing the user.
-            parent_id: ID representing group or experiment.
-            traffic_allocations: Traffic allocations representing traffic allotted to experiments or variations.
-
-        Returns:
-            Entity ID which may represent experiment or variation and
-        """
-        bucketing_key = BUCKETING_ID_TEMPLATE.format(bucketing_id=bucketing_id, parent_id=parent_id)
-        bucketing_number = self._generate_bucket_value(bucketing_key)
-        message = 'Assigned bucket %s to user with bucketing ID "%s".' % (bucketing_number, bucketing_id)
-        project_config.logger.debug(
-            message
-        )
-
-        for traffic_allocation in traffic_allocations:
-            current_end_of_range = traffic_allocation.get('endOfRange')
-            if bucketing_number < current_end_of_range:
-                return traffic_allocation.get('entityId')
-
-        return None
-
-    def bucket(self, project_config, experiment, user_id, bucketing_id):
-        """ For a given experiment and bucketing ID determines variation to be shown to user.
-
-        Args:
-            project_config: Instance of ProjectConfig.
-            experiment: Object representing the experiment or rollout rule in which user is to be bucketed.
-            user_id: ID for user.
-            bucketing_id: ID to be used for bucketing the user.
-
-        Returns:
-            Variation in which user with ID user_id will be put in. None if no variation
-            and array of log messages representing decision making.
-     */.
-        """
-        decide_reasons = []
-        if not experiment:
-            return None, decide_reasons
-
-        # Determine if experiment is in a mutually exclusive group.
-        # This will not affect evaluation of rollout rules.
-        if experiment.groupPolicy in GROUP_POLICIES:
-            group = project_config.get_group(experiment.groupId)
-
-            if not group:
-                return None, decide_reasons
-
-            user_experiment_id = self.find_bucket(
-                project_config, bucketing_id, experiment.groupId, group.trafficAllocation,
-            )
-
-            if not user_experiment_id:
-                message = 'User "%s" is in no experiment.' % user_id
-                project_config.logger.info(message)
-                decide_reasons.append(message)
-                return None, decide_reasons
-
-            if user_experiment_id != experiment.id:
-                message = 'User "%s" is not in experiment "%s" of group %s.' \
-                          % (user_id, experiment.key, experiment.groupId)
-                project_config.logger.info(
-                    message
-                )
-                decide_reasons.append(message)
-                return None, decide_reasons
-
-            message = 'User "%s" is in experiment %s of group %s.' % (user_id, experiment.key, experiment.groupId)
-            project_config.logger.info(
-                message
-            )
-            decide_reasons.append(message)
-
-        # Bucket user if not in white-list and in group (if any)
-        variation_id = self.find_bucket(project_config, bucketing_id,
-                                        experiment.id, experiment.trafficAllocation)
-        if variation_id:
-            variation = project_config.get_variation_from_id_by_experiment_id(experiment.id, variation_id)
-            return variation, decide_reasons
-
-        else:
-            message = 'Bucketed into an empty traffic range. Returning nil.'
-            project_config.logger.info(message)
-            decide_reasons.append(message)
-
-        return None, decide_reasons
+# Copyright 2016-2017, 2019-2022 Optimizely
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from __future__ import annotations
+from typing import Optional, TYPE_CHECKING
+import math
+from sys import version_info
+
+from .lib import pymmh3 as mmh3
+
+
+if version_info < (3, 8):
+    from typing_extensions import Final
+else:
+    from typing import Final  # type: ignore
+
+
+if TYPE_CHECKING:
+    # prevent circular dependenacy by skipping import at runtime
+    from .project_config import ProjectConfig
+    from .entities import Experiment, Variation
+    from .helpers.types import TrafficAllocation
+
+
+MAX_TRAFFIC_VALUE: Final = 10000
+UNSIGNED_MAX_32_BIT_VALUE: Final = 0xFFFFFFFF
+MAX_HASH_VALUE: Final = math.pow(2, 32)
+HASH_SEED: Final = 1
+BUCKETING_ID_TEMPLATE: Final = '{bucketing_id}{parent_id}'
+GROUP_POLICIES: Final = ['random']
+
+
+class Bucketer:
+    """ Optimizely bucketing algorithm that evenly distributes visitors. """
+
+    def __init__(self) -> None:
+        """ Bucketer init method to set bucketing seed and logger instance. """
+
+        self.bucket_seed = HASH_SEED
+
+    def _generate_unsigned_hash_code_32_bit(self, bucketing_id: str) -> int:
+        """ Helper method to retrieve hash code.
+
+        Args:
+            bucketing_id: ID for bucketing.
+
+        Returns:
+            Hash code which is a 32 bit unsigned integer.
+        """
+
+        # Adjusting MurmurHash code to be unsigned
+        return mmh3.hash(bucketing_id, self.bucket_seed) & UNSIGNED_MAX_32_BIT_VALUE
+
+    def _generate_bucket_value(self, bucketing_id: str) -> int:
+        """ Helper function to generate bucket value in half-closed interval [0, MAX_TRAFFIC_VALUE).
+
+        Args:
+            bucketing_id: ID for bucketing.
+
+        Returns:
+            Bucket value corresponding to the provided bucketing ID.
+        """
+
+        ratio = float(self._generate_unsigned_hash_code_32_bit(bucketing_id)) / MAX_HASH_VALUE
+        return math.floor(ratio * MAX_TRAFFIC_VALUE)
+
+    def find_bucket(
+        self, project_config: ProjectConfig, bucketing_id: str,
+        parent_id: Optional[str], traffic_allocations: list[TrafficAllocation]
+    ) -> Optional[str]:
+        """ Determine entity based on bucket value and traffic allocations.
+
+        Args:
+            project_config: Instance of ProjectConfig.
+            bucketing_id: ID to be used for bucketing the user.
+            parent_id: ID representing group or experiment.
+            traffic_allocations: Traffic allocations representing traffic allotted to experiments or variations.
+
+        Returns:
+            Entity ID which may represent experiment or variation and
+        """
+        bucketing_key = BUCKETING_ID_TEMPLATE.format(bucketing_id=bucketing_id, parent_id=parent_id)
+        bucketing_number = self._generate_bucket_value(bucketing_key)
+        project_config.logger.debug(
+            f'Assigned bucket {bucketing_number} to user with bucketing ID "{bucketing_id}".'
+        )
+
+        for traffic_allocation in traffic_allocations:
+            current_end_of_range = traffic_allocation.get('endOfRange')
+            if current_end_of_range is not None and bucketing_number < current_end_of_range:
+                return traffic_allocation.get('entityId')
+
+        return None
+
+    def bucket(
+        self, project_config: ProjectConfig,
+        experiment: Experiment, user_id: str, bucketing_id: str
+    ) -> tuple[Optional[Variation], list[str]]:
+        """ For a given experiment and bucketing ID determines variation to be shown to user.
+
+        Args:
+            project_config: Instance of ProjectConfig.
+            experiment: Object representing the experiment or rollout rule in which user is to be bucketed.
+            user_id: ID for user.
+            bucketing_id: ID to be used for bucketing the user.
+
+        Returns:
+            Variation in which user with ID user_id will be put in. None if no variation
+            and array of log messages representing decision making.
+     */.
+        """
+        decide_reasons: list[str] = []
+        if not experiment:
+            return None, decide_reasons
+
+        # Determine if experiment is in a mutually exclusive group.
+        # This will not affect evaluation of rollout rules.
+        if experiment.groupPolicy in GROUP_POLICIES:
+            group = project_config.get_group(experiment.groupId)
+
+            if not group:
+                return None, decide_reasons
+
+            user_experiment_id = self.find_bucket(
+                project_config, bucketing_id, experiment.groupId, group.trafficAllocation,
+            )
+
+            if not user_experiment_id:
+                message = f'User "{user_id}" is in no experiment.'
+                project_config.logger.info(message)
+                decide_reasons.append(message)
+                return None, decide_reasons
+
+            if user_experiment_id != experiment.id:
+                message = f'User "{user_id}" is not in experiment "{experiment.key}" of group {experiment.groupId}.'
+                project_config.logger.info(message)
+                decide_reasons.append(message)
+                return None, decide_reasons
+
+            message = f'User "{user_id}" is in experiment {experiment.key} of group {experiment.groupId}.'
+            project_config.logger.info(message)
+            decide_reasons.append(message)
+
+        # Bucket user if not in white-list and in group (if any)
+        variation_id = self.find_bucket(project_config, bucketing_id,
+                                        experiment.id, experiment.trafficAllocation)
+        if variation_id:
+            variation = project_config.get_variation_from_id_by_experiment_id(experiment.id, variation_id)
+            return variation, decide_reasons
+
+        else:
+            message = 'Bucketed into an empty traffic range. Returning nil.'
+            project_config.logger.info(message)
+            decide_reasons.append(message)
+
+        return None, decide_reasons
```

### Comparing `optimizely-sdk-4.1.1/optimizely/config_manager.py` & `optimizely-sdk-5.0.0b0/optimizely/config_manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,427 +1,480 @@
-# Copyright 2019-2020, Optimizely
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import abc
-import numbers
-import requests
-import threading
-import time
-from requests import codes as http_status_codes
-from requests import exceptions as requests_exceptions
-
-from . import exceptions as optimizely_exceptions
-from . import logger as optimizely_logger
-from . import project_config
-from .error_handler import NoOpErrorHandler
-from .notification_center import NotificationCenter
-from .helpers import enums
-from .helpers import validator
-from .optimizely_config import OptimizelyConfigService
-
-ABC = abc.ABCMeta('ABC', (object,), {'__slots__': ()})
-
-
-class BaseConfigManager(ABC):
-    """ Base class for Optimizely's config manager. """
-
-    def __init__(self, logger=None, error_handler=None, notification_center=None):
-        """ Initialize config manager.
-
-        Args:
-            logger: Provides a logger instance.
-            error_handler: Provides a handle_error method to handle exceptions.
-            notification_center: Provides instance of notification_center.NotificationCenter.
-        """
-        self.logger = optimizely_logger.adapt_logger(logger or optimizely_logger.NoOpLogger())
-        self.error_handler = error_handler or NoOpErrorHandler()
-        self.notification_center = notification_center or NotificationCenter(self.logger)
-        self._validate_instantiation_options()
-
-    def _validate_instantiation_options(self):
-        """ Helper method to validate all parameters.
-
-        Raises:
-            Exception if provided options are invalid.
-        """
-        if not validator.is_logger_valid(self.logger):
-            raise optimizely_exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('logger'))
-
-        if not validator.is_error_handler_valid(self.error_handler):
-            raise optimizely_exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('error_handler'))
-
-        if not validator.is_notification_center_valid(self.notification_center):
-            raise optimizely_exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('notification_center'))
-
-    @abc.abstractmethod
-    def get_config(self):
-        """ Get config for use by optimizely.Optimizely.
-        The config should be an instance of project_config.ProjectConfig."""
-        pass
-
-
-class StaticConfigManager(BaseConfigManager):
-    """ Config manager that returns ProjectConfig based on provided datafile. """
-
-    def __init__(
-        self, datafile=None, logger=None, error_handler=None, notification_center=None, skip_json_validation=False,
-    ):
-        """ Initialize config manager. Datafile has to be provided to use.
-
-        Args:
-            datafile: JSON string representing the Optimizely project.
-            logger: Provides a logger instance.
-            error_handler: Provides a handle_error method to handle exceptions.
-            notification_center: Notification center to generate config update notification.
-            skip_json_validation: Optional boolean param which allows skipping JSON schema
-                                  validation upon object invocation. By default
-                                  JSON schema validation will be performed.
-        """
-        super(StaticConfigManager, self).__init__(
-            logger=logger, error_handler=error_handler, notification_center=notification_center,
-        )
-        self._config = None
-        self.optimizely_config = None
-        self.validate_schema = not skip_json_validation
-        self._set_config(datafile)
-
-    def _set_config(self, datafile):
-        """ Looks up and sets datafile and config based on response body.
-
-        Args:
-            datafile: JSON string representing the Optimizely project.
-        """
-
-        if self.validate_schema:
-            if not validator.is_datafile_valid(datafile):
-                self.logger.error(enums.Errors.INVALID_INPUT.format('datafile'))
-                return
-
-        error_msg = None
-        error_to_handle = None
-        config = None
-
-        try:
-            config = project_config.ProjectConfig(datafile, self.logger, self.error_handler)
-        except optimizely_exceptions.UnsupportedDatafileVersionException as error:
-            error_msg = error.args[0]
-            error_to_handle = error
-        except:
-            error_msg = enums.Errors.INVALID_INPUT.format('datafile')
-            error_to_handle = optimizely_exceptions.InvalidInputException(error_msg)
-        finally:
-            if error_msg:
-                self.logger.error(error_msg)
-                self.error_handler.handle_error(error_to_handle)
-                return
-
-        previous_revision = self._config.get_revision() if self._config else None
-
-        if previous_revision == config.get_revision():
-            return
-
-        self._config = config
-        self.optimizely_config = OptimizelyConfigService(config).get_config()
-        self.notification_center.send_notifications(enums.NotificationTypes.OPTIMIZELY_CONFIG_UPDATE)
-        self.logger.debug(
-            'Received new datafile and updated config. '
-            'Old revision number: {}. New revision number: {}.'.format(previous_revision, config.get_revision())
-        )
-
-    def get_config(self):
-        """ Returns instance of ProjectConfig.
-
-        Returns:
-            ProjectConfig. None if not set.
-        """
-
-        return self._config
-
-
-class PollingConfigManager(StaticConfigManager):
-    """ Config manager that polls for the datafile and updated ProjectConfig based on an update interval. """
-
-    DATAFILE_URL_TEMPLATE = enums.ConfigManager.DATAFILE_URL_TEMPLATE
-
-    def __init__(
-        self,
-        sdk_key=None,
-        datafile=None,
-        update_interval=None,
-        blocking_timeout=None,
-        url=None,
-        url_template=None,
-        logger=None,
-        error_handler=None,
-        notification_center=None,
-        skip_json_validation=False,
-    ):
-        """ Initialize config manager. One of sdk_key or url has to be set to be able to use.
-
-        Args:
-            sdk_key: Optional string uniquely identifying the datafile.
-            datafile: Optional JSON string representing the project.
-            update_interval: Optional floating point number representing time interval in seconds
-                             at which to request datafile and set ProjectConfig.
-            blocking_timeout: Optional Time in seconds to block the get_config call until config object
-                              has been initialized.
-            url: Optional string representing URL from where to fetch the datafile. If set it supersedes the sdk_key.
-            url_template: Optional string template which in conjunction with sdk_key
-                          determines URL from where to fetch the datafile.
-            logger: Provides a logger instance.
-            error_handler: Provides a handle_error method to handle exceptions.
-            notification_center: Notification center to generate config update notification.
-            skip_json_validation: Optional boolean param which allows skipping JSON schema
-                                  validation upon object invocation. By default
-                                  JSON schema validation will be performed.
-
-        """
-        self._config_ready_event = threading.Event()
-        super(PollingConfigManager, self).__init__(
-            datafile=datafile,
-            logger=logger,
-            error_handler=error_handler,
-            notification_center=notification_center,
-            skip_json_validation=skip_json_validation,
-        )
-        self.datafile_url = self.get_datafile_url(
-            sdk_key, url, url_template or self.DATAFILE_URL_TEMPLATE
-        )
-        self.set_update_interval(update_interval)
-        self.set_blocking_timeout(blocking_timeout)
-        self.last_modified = None
-        self._polling_thread = threading.Thread(target=self._run)
-        self._polling_thread.setDaemon(True)
-        self._polling_thread.start()
-
-    @staticmethod
-    def get_datafile_url(sdk_key, url, url_template):
-        """ Helper method to determine URL from where to fetch the datafile.
-
-        Args:
-          sdk_key: Key uniquely identifying the datafile.
-          url: String representing URL from which to fetch the datafile.
-          url_template: String representing template which is filled in with
-                        SDK key to determine URL from which to fetch the datafile.
-
-        Returns:
-          String representing URL to fetch datafile from.
-
-        Raises:
-          optimizely.exceptions.InvalidInputException if:
-          - One of sdk_key or url is not provided.
-          - url_template is invalid.
-        """
-        # Ensure that either is provided by the user.
-        if sdk_key is None and url is None:
-            raise optimizely_exceptions.InvalidInputException('Must provide at least one of sdk_key or url.')
-
-        # Return URL if one is provided or use template and SDK key to get it.
-        if url is None:
-            try:
-                return url_template.format(sdk_key=sdk_key)
-            except (AttributeError, KeyError):
-                raise optimizely_exceptions.InvalidInputException(
-                    'Invalid url_template {} provided.'.format(url_template)
-                )
-
-        return url
-
-    def _set_config(self, datafile):
-        """ Looks up and sets datafile and config based on response body.
-
-        Args:
-            datafile: JSON string representing the Optimizely project.
-        """
-        if datafile or self._config_ready_event.is_set():
-            super(PollingConfigManager, self)._set_config(datafile=datafile)
-            self._config_ready_event.set()
-
-    def get_config(self):
-        """ Returns instance of ProjectConfig. Returns immediately if project config is ready otherwise
-        blocks maximum for value of blocking_timeout in seconds.
-
-        Returns:
-            ProjectConfig. None if not set.
-        """
-
-        self._config_ready_event.wait(self.blocking_timeout)
-        return self._config
-
-    def set_update_interval(self, update_interval):
-        """ Helper method to set frequency at which datafile has to be polled and ProjectConfig updated.
-
-        Args:
-            update_interval: Time in seconds after which to update datafile.
-        """
-        if update_interval is None:
-            update_interval = enums.ConfigManager.DEFAULT_UPDATE_INTERVAL
-            self.logger.debug('Setting config update interval to default value {}.'.format(update_interval))
-
-        if not isinstance(update_interval, (int, float)):
-            raise optimizely_exceptions.InvalidInputException(
-                'Invalid update_interval "{}" provided.'.format(update_interval)
-            )
-
-        # If polling interval is less than or equal to 0 then set it to default update interval.
-        if update_interval <= 0:
-            self.logger.debug(
-                'update_interval value {} too small. Defaulting to {}'.format(
-                    update_interval, enums.ConfigManager.DEFAULT_UPDATE_INTERVAL
-                )
-            )
-            update_interval = enums.ConfigManager.DEFAULT_UPDATE_INTERVAL
-
-        self.update_interval = update_interval
-
-    def set_blocking_timeout(self, blocking_timeout):
-        """ Helper method to set time in seconds to block the config call until config has been initialized.
-
-        Args:
-            blocking_timeout: Time in seconds to block the config call.
-        """
-        if blocking_timeout is None:
-            blocking_timeout = enums.ConfigManager.DEFAULT_BLOCKING_TIMEOUT
-            self.logger.debug('Setting config blocking timeout to default value {}.'.format(blocking_timeout))
-
-        if not isinstance(blocking_timeout, (numbers.Integral, float)):
-            raise optimizely_exceptions.InvalidInputException(
-                'Invalid blocking timeout "{}" provided.'.format(blocking_timeout)
-            )
-
-        # If blocking timeout is less than 0 then set it to default blocking timeout.
-        if blocking_timeout < 0:
-            self.logger.debug(
-                'blocking timeout value {} too small. Defaulting to {}'.format(
-                    blocking_timeout, enums.ConfigManager.DEFAULT_BLOCKING_TIMEOUT
-                )
-            )
-            blocking_timeout = enums.ConfigManager.DEFAULT_BLOCKING_TIMEOUT
-
-        self.blocking_timeout = blocking_timeout
-
-    def set_last_modified(self, response_headers):
-        """ Looks up and sets last modified time based on Last-Modified header in the response.
-
-        Args:
-            response_headers: requests.Response.headers
-        """
-        self.last_modified = response_headers.get(enums.HTTPHeaders.LAST_MODIFIED)
-
-    def _handle_response(self, response):
-        """ Helper method to handle response containing datafile.
-
-        Args:
-            response: requests.Response
-        """
-        try:
-            response.raise_for_status()
-        except requests_exceptions.RequestException as err:
-            self.logger.error('Fetching datafile from {} failed. Error: {}'.format(self.datafile_url, str(err)))
-            return
-
-        # Leave datafile and config unchanged if it has not been modified.
-        if response.status_code == http_status_codes.not_modified:
-            self.logger.debug('Not updating config as datafile has not updated since {}.'.format(self.last_modified))
-            return
-
-        self.set_last_modified(response.headers)
-        self._set_config(response.content)
-
-    def fetch_datafile(self):
-        """ Fetch datafile and set ProjectConfig. """
-
-        request_headers = {}
-        if self.last_modified:
-            request_headers[enums.HTTPHeaders.IF_MODIFIED_SINCE] = self.last_modified
-
-        try:
-            response = requests.get(
-                self.datafile_url, headers=request_headers, timeout=enums.ConfigManager.REQUEST_TIMEOUT,
-            )
-        except requests_exceptions.RequestException as err:
-            self.logger.error('Fetching datafile from {} failed. Error: {}'.format(self.datafile_url, str(err)))
-            return
-
-        self._handle_response(response)
-
-    @property
-    def is_running(self):
-        """ Check if polling thread is alive or not. """
-        return self._polling_thread.is_alive()
-
-    def _run(self):
-        """ Triggered as part of the thread which fetches the datafile and sleeps until next update interval. """
-        try:
-            while self.is_running:
-                self.fetch_datafile()
-                time.sleep(self.update_interval)
-        except (OSError, OverflowError) as err:
-            self.logger.error(
-                'Error in time.sleep. ' 'Provided update_interval value may be too big. Error: {}'.format(str(err))
-            )
-            raise
-
-    def start(self):
-        """ Start the config manager and the thread to periodically fetch datafile. """
-        if not self.is_running:
-            self._polling_thread.start()
-
-
-class AuthDatafilePollingConfigManager(PollingConfigManager):
-    """ Config manager that polls for authenticated datafile using access token. """
-
-    DATAFILE_URL_TEMPLATE = enums.ConfigManager.AUTHENTICATED_DATAFILE_URL_TEMPLATE
-
-    def __init__(
-        self,
-        datafile_access_token,
-        *args,
-        **kwargs
-    ):
-        """ Initialize config manager. One of sdk_key or url has to be set to be able to use.
-
-        Args:
-            datafile_access_token: String to be attached to the request header to fetch the authenticated datafile.
-            *args: Refer to arguments descriptions in PollingConfigManager.
-            **kwargs: Refer to keyword arguments descriptions in PollingConfigManager.
-        """
-        self._set_datafile_access_token(datafile_access_token)
-        super(AuthDatafilePollingConfigManager, self).__init__(*args, **kwargs)
-
-    def _set_datafile_access_token(self, datafile_access_token):
-        """ Checks for valid access token input and sets it. """
-        if not datafile_access_token:
-            raise optimizely_exceptions.InvalidInputException(
-                'datafile_access_token cannot be empty or None.')
-        self.datafile_access_token = datafile_access_token
-
-    def fetch_datafile(self):
-        """ Fetch authenticated datafile and set ProjectConfig. """
-        request_headers = {
-            enums.HTTPHeaders.AUTHORIZATION: enums.ConfigManager.AUTHORIZATION_HEADER_DATA_TEMPLATE.format(
-                datafile_access_token=self.datafile_access_token
-            )
-        }
-
-        if self.last_modified:
-            request_headers[enums.HTTPHeaders.IF_MODIFIED_SINCE] = self.last_modified
-
-        try:
-            response = requests.get(
-                self.datafile_url, headers=request_headers, timeout=enums.ConfigManager.REQUEST_TIMEOUT,
-            )
-        except requests_exceptions.RequestException as err:
-            self.logger.error('Fetching datafile from {} failed. Error: {}'.format(self.datafile_url, str(err)))
-            return
-
-        self._handle_response(response)
+# Copyright 2019-2020, 2022-2023, Optimizely
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from __future__ import annotations
+from abc import ABC, abstractmethod
+import numbers
+from typing import TYPE_CHECKING, Any, Optional
+import requests
+import threading
+from requests import codes as http_status_codes
+from requests import exceptions as requests_exceptions
+
+from . import exceptions as optimizely_exceptions
+from . import logger as optimizely_logger
+from . import project_config
+from .error_handler import NoOpErrorHandler, BaseErrorHandler
+from .notification_center import NotificationCenter
+from .notification_center_registry import _NotificationCenterRegistry
+from .helpers import enums
+from .helpers import validator
+from .optimizely_config import OptimizelyConfig, OptimizelyConfigService
+
+
+if TYPE_CHECKING:
+    # prevent circular dependenacy by skipping import at runtime
+    from requests.models import CaseInsensitiveDict
+
+
+class BaseConfigManager(ABC):
+    """ Base class for Optimizely's config manager. """
+
+    def __init__(
+        self,
+        logger: Optional[optimizely_logger.Logger] = None,
+        error_handler: Optional[BaseErrorHandler] = None,
+        notification_center: Optional[NotificationCenter] = None
+    ):
+        """ Initialize config manager.
+
+        Args:
+            logger: Provides a logger instance.
+            error_handler: Provides a handle_error method to handle exceptions.
+            notification_center: Provides instance of notification_center.NotificationCenter.
+        """
+        self.logger = optimizely_logger.adapt_logger(logger or optimizely_logger.NoOpLogger())
+        self.error_handler = error_handler or NoOpErrorHandler()
+        self.notification_center = notification_center or NotificationCenter(self.logger)
+        self.optimizely_config: Optional[OptimizelyConfig]
+        self._validate_instantiation_options()
+
+    def _validate_instantiation_options(self) -> None:
+        """ Helper method to validate all parameters.
+
+        Raises:
+            Exception if provided options are invalid.
+        """
+        if not validator.is_logger_valid(self.logger):
+            raise optimizely_exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('logger'))
+
+        if not validator.is_error_handler_valid(self.error_handler):
+            raise optimizely_exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('error_handler'))
+
+        if not validator.is_notification_center_valid(self.notification_center):
+            raise optimizely_exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('notification_center'))
+
+    @abstractmethod
+    def get_config(self) -> Optional[project_config.ProjectConfig]:
+        """ Get config for use by optimizely.Optimizely.
+        The config should be an instance of project_config.ProjectConfig."""
+        pass
+
+    @abstractmethod
+    def get_sdk_key(self) -> Optional[str]:
+        """ Get sdk_key for use by optimizely.Optimizely.
+        The sdk_key should uniquely identify the datafile for a project and environment combination.
+        """
+        pass
+
+
+class StaticConfigManager(BaseConfigManager):
+    """ Config manager that returns ProjectConfig based on provided datafile. """
+
+    def __init__(
+        self,
+        datafile: Optional[str] = None,
+        logger: Optional[optimizely_logger.Logger] = None,
+        error_handler: Optional[BaseErrorHandler] = None,
+        notification_center: Optional[NotificationCenter] = None,
+        skip_json_validation: Optional[bool] = False,
+    ):
+        """ Initialize config manager. Datafile has to be provided to use.
+
+        Args:
+            datafile: JSON string representing the Optimizely project.
+            logger: Provides a logger instance.
+            error_handler: Provides a handle_error method to handle exceptions.
+            notification_center: Notification center to generate config update notification.
+            skip_json_validation: Optional boolean param which allows skipping JSON schema
+                                  validation upon object invocation. By default
+                                  JSON schema validation will be performed.
+        """
+        super().__init__(
+            logger=logger, error_handler=error_handler, notification_center=notification_center,
+        )
+        self._config: project_config.ProjectConfig = None  # type: ignore[assignment]
+        self.optimizely_config: Optional[OptimizelyConfig] = None
+        self._sdk_key: Optional[str] = None
+        self.validate_schema = not skip_json_validation
+        self._set_config(datafile)
+
+    def get_sdk_key(self) -> Optional[str]:
+        return self._sdk_key
+
+    def _set_config(self, datafile: Optional[str | bytes]) -> None:
+        """ Looks up and sets datafile and config based on response body.
+
+        Args:
+            datafile: JSON string representing the Optimizely project.
+        """
+
+        if self.validate_schema:
+            if not validator.is_datafile_valid(datafile):
+                self.logger.error(enums.Errors.INVALID_INPUT.format('datafile'))
+                return
+
+        error_msg = None
+        error_to_handle: Optional[Exception] = None
+        config = None
+
+        try:
+            assert datafile is not None
+            config = project_config.ProjectConfig(datafile, self.logger, self.error_handler)
+        except optimizely_exceptions.UnsupportedDatafileVersionException as error:
+            error_msg = error.args[0]
+            error_to_handle = error
+        except:
+            error_msg = enums.Errors.INVALID_INPUT.format('datafile')
+            error_to_handle = optimizely_exceptions.InvalidInputException(error_msg)
+        finally:
+            if error_msg or config is None:
+                self.logger.error(error_msg)
+                self.error_handler.handle_error(error_to_handle or Exception('Unknown Error'))
+                return
+
+        previous_revision = self._config.get_revision() if self._config else None
+
+        if previous_revision == config.get_revision():
+            return
+
+        self._config = config
+        self._sdk_key = self._sdk_key or config.sdk_key
+        self.optimizely_config = OptimizelyConfigService(config).get_config()
+        self.notification_center.send_notifications(enums.NotificationTypes.OPTIMIZELY_CONFIG_UPDATE)
+
+        internal_notification_center = _NotificationCenterRegistry.get_notification_center(
+            self._sdk_key, self.logger
+        )
+        if internal_notification_center:
+            internal_notification_center.send_notifications(enums.NotificationTypes.OPTIMIZELY_CONFIG_UPDATE)
+
+        self.logger.debug(
+            'Received new datafile and updated config. '
+            f'Old revision number: {previous_revision}. New revision number: {config.get_revision()}.'
+        )
+
+    def get_config(self) -> Optional[project_config.ProjectConfig]:
+        """ Returns instance of ProjectConfig.
+
+        Returns:
+            ProjectConfig. None if not set.
+        """
+
+        return self._config
+
+
+class PollingConfigManager(StaticConfigManager):
+    """ Config manager that polls for the datafile and updated ProjectConfig based on an update interval. """
+
+    DATAFILE_URL_TEMPLATE = enums.ConfigManager.DATAFILE_URL_TEMPLATE
+
+    def __init__(
+        self,
+        sdk_key: Optional[str] = None,
+        datafile: Optional[str] = None,
+        update_interval: Optional[float] = None,
+        blocking_timeout: Optional[int] = None,
+        url: Optional[str] = None,
+        url_template: Optional[str] = None,
+        logger: Optional[optimizely_logger.Logger] = None,
+        error_handler: Optional[BaseErrorHandler] = None,
+        notification_center: Optional[NotificationCenter] = None,
+        skip_json_validation: Optional[bool] = False,
+    ):
+        """ Initialize config manager. One of sdk_key or datafile has to be set to be able to use.
+
+        Args:
+            sdk_key: Optional string uniquely identifying the datafile. If not provided, datafile must
+                     contain a sdk_key.
+            datafile: Optional JSON string representing the project. If not provided, sdk_key is required.
+            update_interval: Optional floating point number representing time interval in seconds
+                             at which to request datafile and set ProjectConfig.
+            blocking_timeout: Optional Time in seconds to block the get_config call until config object
+                              has been initialized.
+            url: Optional string representing URL from where to fetch the datafile. If set it supersedes the sdk_key.
+            url_template: Optional string template which in conjunction with sdk_key
+                          determines URL from where to fetch the datafile.
+            logger: Provides a logger instance.
+            error_handler: Provides a handle_error method to handle exceptions.
+            notification_center: Notification center to generate config update notification.
+            skip_json_validation: Optional boolean param which allows skipping JSON schema
+                                  validation upon object invocation. By default
+                                  JSON schema validation will be performed.
+
+        """
+        self._config_ready_event = threading.Event()
+        super().__init__(
+            datafile=datafile,
+            logger=logger,
+            error_handler=error_handler,
+            notification_center=notification_center,
+            skip_json_validation=skip_json_validation,
+        )
+        self._sdk_key = sdk_key or self._sdk_key
+
+        if self._sdk_key is None:
+            raise optimizely_exceptions.InvalidInputException(enums.Errors.MISSING_SDK_KEY)
+
+        self.datafile_url = self.get_datafile_url(
+            self._sdk_key, url, url_template or self.DATAFILE_URL_TEMPLATE
+        )
+        self.set_update_interval(update_interval)
+        self.set_blocking_timeout(blocking_timeout)
+        self.last_modified: Optional[str] = None
+        self.stopped = threading.Event()
+        self._initialize_thread()
+        self._polling_thread.start()
+
+    @staticmethod
+    def get_datafile_url(sdk_key: Optional[str], url: Optional[str], url_template: Optional[str]) -> str:
+        """ Helper method to determine URL from where to fetch the datafile.
+
+        Args:
+          sdk_key: Key uniquely identifying the datafile.
+          url: String representing URL from which to fetch the datafile.
+          url_template: String representing template which is filled in with
+                        SDK key to determine URL from which to fetch the datafile.
+
+        Returns:
+          String representing URL to fetch datafile from.
+
+        Raises:
+          optimizely.exceptions.InvalidInputException if:
+          - One of sdk_key or url is not provided.
+          - url_template is invalid.
+        """
+        # Ensure that either is provided by the user.
+        if sdk_key is None and url is None:
+            raise optimizely_exceptions.InvalidInputException('Must provide at least one of sdk_key or url.')
+
+        # Return URL if one is provided or use template and SDK key to get it.
+        if url is None:
+            try:
+                assert url_template is not None
+                return url_template.format(sdk_key=sdk_key)
+            except (AssertionError, AttributeError, KeyError):
+                raise optimizely_exceptions.InvalidInputException(
+                    f'Invalid url_template {url_template} provided.'
+                )
+
+        return url
+
+    def _set_config(self, datafile: Optional[str | bytes]) -> None:
+        """ Looks up and sets datafile and config based on response body.
+
+        Args:
+            datafile: JSON string representing the Optimizely project.
+        """
+        if datafile or self._config_ready_event.is_set():
+            super()._set_config(datafile=datafile)
+            self._config_ready_event.set()
+
+    def get_config(self) -> Optional[project_config.ProjectConfig]:
+        """ Returns instance of ProjectConfig. Returns immediately if project config is ready otherwise
+        blocks maximum for value of blocking_timeout in seconds.
+
+        Returns:
+            ProjectConfig. None if not set.
+        """
+
+        self._config_ready_event.wait(self.blocking_timeout)
+        return self._config
+
+    def set_update_interval(self, update_interval: Optional[int | float]) -> None:
+        """ Helper method to set frequency at which datafile has to be polled and ProjectConfig updated.
+
+        Args:
+            update_interval: Time in seconds after which to update datafile.
+        """
+        if update_interval is None:
+            update_interval = enums.ConfigManager.DEFAULT_UPDATE_INTERVAL
+            self.logger.debug(f'Setting config update interval to default value {update_interval}.')
+
+        if not isinstance(update_interval, (int, float)):
+            raise optimizely_exceptions.InvalidInputException(
+                f'Invalid update_interval "{update_interval}" provided.'
+            )
+
+        # If polling interval is less than or equal to 0 then set it to default update interval.
+        if update_interval <= 0:
+            self.logger.debug(
+                f'update_interval value {update_interval} too small. '
+                f'Defaulting to {enums.ConfigManager.DEFAULT_UPDATE_INTERVAL}'
+            )
+            update_interval = enums.ConfigManager.DEFAULT_UPDATE_INTERVAL
+
+        self.update_interval = update_interval
+
+    def set_blocking_timeout(self, blocking_timeout: Optional[int | float]) -> None:
+        """ Helper method to set time in seconds to block the config call until config has been initialized.
+
+        Args:
+            blocking_timeout: Time in seconds to block the config call.
+        """
+        if blocking_timeout is None:
+            blocking_timeout = enums.ConfigManager.DEFAULT_BLOCKING_TIMEOUT
+            self.logger.debug(f'Setting config blocking timeout to default value {blocking_timeout}.')
+
+        if not isinstance(blocking_timeout, (numbers.Integral, float)):
+            raise optimizely_exceptions.InvalidInputException(
+                f'Invalid blocking timeout "{blocking_timeout}" provided.'
+            )
+
+        # If blocking timeout is less than 0 then set it to default blocking timeout.
+        if blocking_timeout < 0:
+            self.logger.debug(
+                f'blocking timeout value {blocking_timeout} too small. '
+                f'Defaulting to {enums.ConfigManager.DEFAULT_BLOCKING_TIMEOUT}'
+            )
+            blocking_timeout = enums.ConfigManager.DEFAULT_BLOCKING_TIMEOUT
+
+        self.blocking_timeout = blocking_timeout
+
+    def set_last_modified(self, response_headers: CaseInsensitiveDict[str]) -> None:
+        """ Looks up and sets last modified time based on Last-Modified header in the response.
+
+        Args:
+            response_headers: requests.Response.headers
+        """
+        self.last_modified = response_headers.get(enums.HTTPHeaders.LAST_MODIFIED)
+
+    def _handle_response(self, response: requests.Response) -> None:
+        """ Helper method to handle response containing datafile.
+
+        Args:
+            response: requests.Response
+        """
+        try:
+            response.raise_for_status()
+        except requests_exceptions.RequestException as err:
+            self.logger.error(f'Fetching datafile from {self.datafile_url} failed. Error: {err}')
+            return
+
+        # Leave datafile and config unchanged if it has not been modified.
+        if response.status_code == http_status_codes.not_modified:
+            self.logger.debug(f'Not updating config as datafile has not updated since {self.last_modified}.')
+            return
+
+        self.set_last_modified(response.headers)
+        self._set_config(response.content)
+
+    def fetch_datafile(self) -> None:
+        """ Fetch datafile and set ProjectConfig. """
+
+        request_headers = {}
+        if self.last_modified:
+            request_headers[enums.HTTPHeaders.IF_MODIFIED_SINCE] = self.last_modified
+
+        try:
+            response = requests.get(
+                self.datafile_url, headers=request_headers, timeout=enums.ConfigManager.REQUEST_TIMEOUT,
+            )
+        except requests_exceptions.RequestException as err:
+            self.logger.error(f'Fetching datafile from {self.datafile_url} failed. Error: {err}')
+            return
+
+        self._handle_response(response)
+
+    @property
+    def is_running(self) -> bool:
+        """ Check if polling thread is alive or not. """
+        return self._polling_thread.is_alive()
+
+    def stop(self) -> None:
+        """ Stop the polling thread and briefly wait for it to exit. """
+        if self.is_running:
+            self.stopped.set()
+            # no need to wait too long as this exists to avoid interfering with tests
+            self._polling_thread.join(timeout=0.2)
+
+    def _run(self) -> None:
+        """ Triggered as part of the thread which fetches the datafile and sleeps until next update interval. """
+        try:
+            while True:
+                self.fetch_datafile()
+                if self.stopped.wait(self.update_interval):
+                    self.stopped.clear()
+                    break
+        except (OSError, OverflowError) as err:
+            self.logger.error(
+                f'Provided update_interval value may be too big. Error: {err}'
+            )
+            raise
+
+    def start(self) -> None:
+        """ Start the config manager and the thread to periodically fetch datafile. """
+        if not self.is_running:
+            self._polling_thread.start()
+
+    def _initialize_thread(self) -> None:
+        self._polling_thread = threading.Thread(target=self._run, daemon=True)
+
+
+class AuthDatafilePollingConfigManager(PollingConfigManager):
+    """ Config manager that polls for authenticated datafile using access token. """
+
+    DATAFILE_URL_TEMPLATE = enums.ConfigManager.AUTHENTICATED_DATAFILE_URL_TEMPLATE
+
+    def __init__(
+        self,
+        datafile_access_token: str,
+        *args: Any,
+        **kwargs: Any
+    ):
+        """ Initialize config manager. One of sdk_key or datafile has to be set to be able to use.
+
+        Args:
+            datafile_access_token: String to be attached to the request header to fetch the authenticated datafile.
+            *args: Refer to arguments descriptions in PollingConfigManager.
+            **kwargs: Refer to keyword arguments descriptions in PollingConfigManager.
+        """
+        self._set_datafile_access_token(datafile_access_token)
+        super().__init__(*args, **kwargs)
+
+    def _set_datafile_access_token(self, datafile_access_token: str) -> None:
+        """ Checks for valid access token input and sets it. """
+        if not datafile_access_token:
+            raise optimizely_exceptions.InvalidInputException(
+                'datafile_access_token cannot be empty or None.')
+        self.datafile_access_token = datafile_access_token
+
+    def fetch_datafile(self) -> None:
+        """ Fetch authenticated datafile and set ProjectConfig. """
+        request_headers = {
+            enums.HTTPHeaders.AUTHORIZATION: enums.ConfigManager.AUTHORIZATION_HEADER_DATA_TEMPLATE.format(
+                datafile_access_token=self.datafile_access_token
+            )
+        }
+
+        if self.last_modified:
+            request_headers[enums.HTTPHeaders.IF_MODIFIED_SINCE] = self.last_modified
+
+        try:
+            response = requests.get(
+                self.datafile_url, headers=request_headers, timeout=enums.ConfigManager.REQUEST_TIMEOUT,
+            )
+        except requests_exceptions.RequestException as err:
+            self.logger.error(f'Fetching datafile from {self.datafile_url} failed. Error: {err}')
+            return
+
+        self._handle_response(response)
```

### Comparing `optimizely-sdk-4.1.1/optimizely/decision/__init__.py` & `optimizely-sdk-5.0.0b0/optimizely/event/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2021, Optimizely
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# Copyright 2019, Optimizely
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
```

### Comparing `optimizely-sdk-4.1.1/optimizely/decision/optimizely_decide_option.py` & `optimizely-sdk-5.0.0b0/optimizely/decision/optimizely_decide_option.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,27 @@
-# Copyright 2021, Optimizely
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-
-class OptimizelyDecideOption(object):
-    DISABLE_DECISION_EVENT = 'DISABLE_DECISION_EVENT'
-    ENABLED_FLAGS_ONLY = 'ENABLED_FLAGS_ONLY'
-    IGNORE_USER_PROFILE_SERVICE = 'IGNORE_USER_PROFILE_SERVICE'
-    INCLUDE_REASONS = 'INCLUDE_REASONS'
-    EXCLUDE_VARIABLES = 'EXCLUDE_VARIABLES'
+# Copyright 2021, 2022, Optimizely
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from sys import version_info
+
+if version_info < (3, 8):
+    from typing_extensions import Final
+else:
+    from typing import Final  # type: ignore
+
+
+class OptimizelyDecideOption:
+    DISABLE_DECISION_EVENT: Final = 'DISABLE_DECISION_EVENT'
+    ENABLED_FLAGS_ONLY: Final = 'ENABLED_FLAGS_ONLY'
+    IGNORE_USER_PROFILE_SERVICE: Final = 'IGNORE_USER_PROFILE_SERVICE'
+    INCLUDE_REASONS: Final = 'INCLUDE_REASONS'
+    EXCLUDE_VARIABLES: Final = 'EXCLUDE_VARIABLES'
```

### Comparing `optimizely-sdk-4.1.1/optimizely/decision/optimizely_decision_message.py` & `optimizely-sdk-5.0.0b0/optimizely/version.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-# Copyright 2021, Optimizely
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-
-class OptimizelyDecisionMessage(object):
-    SDK_NOT_READY = 'Optimizely SDK not configured properly yet.'
-    FLAG_KEY_INVALID = 'No flag was found for key "{}".'
-    VARIABLE_VALUE_INVALID = 'Variable value for key "{}" is invalid or wrong type.'
+# Copyright 2016-2020, 2022-2023, Optimizely
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+version_info = (5, 0, '0-beta')
+__version__ = '.'.join(str(v) for v in version_info)
```

### Comparing `optimizely-sdk-4.1.1/optimizely/decision_service.py` & `optimizely-sdk-5.0.0b0/optimizely/decision_service.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,549 +1,582 @@
-# Copyright 2017-2022, Optimizely
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from collections import namedtuple
-
-from six import string_types
-
-from . import bucketer
-from .decision.optimizely_decide_option import OptimizelyDecideOption
-from .helpers import audience as audience_helper
-from .helpers import enums
-from .helpers import experiment as experiment_helper
-from .helpers import validator
-from .optimizely_user_context import OptimizelyUserContext
-from .user_profile import UserProfile
-
-Decision = namedtuple('Decision', 'experiment variation source')
-
-
-class DecisionService(object):
-    """ Class encapsulating all decision related capabilities. """
-
-    def __init__(self, logger, user_profile_service):
-        self.bucketer = bucketer.Bucketer()
-        self.logger = logger
-        self.user_profile_service = user_profile_service
-
-        # Map of user IDs to another map of experiments to variations.
-        # This contains all the forced variations set by the user
-        # by calling set_forced_variation (it is not the same as the
-        # whitelisting forcedVariations data structure).
-        self.forced_variation_map = {}
-
-    def _get_bucketing_id(self, user_id, attributes):
-        """ Helper method to determine bucketing ID for the user.
-
-        Args:
-          user_id: ID for user.
-          attributes: Dict representing user attributes. May consist of bucketing ID to be used.
-
-        Returns:
-          String representing bucketing ID if it is a String type in attributes else return user ID
-          array of log messages representing decision making.
-        """
-        decide_reasons = []
-        attributes = attributes or {}
-        bucketing_id = attributes.get(enums.ControlAttributes.BUCKETING_ID)
-
-        if bucketing_id is not None:
-            if isinstance(bucketing_id, string_types):
-                return bucketing_id, decide_reasons
-            message = 'Bucketing ID attribute is not a string. Defaulted to user_id.'
-            self.logger.warning(message)
-            decide_reasons.append(message)
-
-        return user_id, decide_reasons
-
-    def set_forced_variation(self, project_config, experiment_key, user_id, variation_key):
-        """ Sets users to a map of experiments to forced variations.
-
-          Args:
-            project_config: Instance of ProjectConfig.
-            experiment_key: Key for experiment.
-            user_id: The user ID.
-            variation_key: Key for variation. If None, then clear the existing experiment-to-variation mapping.
-
-          Returns:
-            A boolean value that indicates if the set completed successfully.
-        """
-        experiment = project_config.get_experiment_from_key(experiment_key)
-        if not experiment:
-            # The invalid experiment key will be logged inside this call.
-            return False
-
-        experiment_id = experiment.id
-        if variation_key is None:
-            if user_id in self.forced_variation_map:
-                experiment_to_variation_map = self.forced_variation_map.get(user_id)
-                if experiment_id in experiment_to_variation_map:
-                    del self.forced_variation_map[user_id][experiment_id]
-                    self.logger.debug(
-                        'Variation mapped to experiment "%s" has been removed for user "%s".'
-                        % (experiment_key, user_id)
-                    )
-                else:
-                    self.logger.debug(
-                        'Nothing to remove. Variation mapped to experiment "%s" for user "%s" does not exist.'
-                        % (experiment_key, user_id)
-                    )
-            else:
-                self.logger.debug('Nothing to remove. User "%s" does not exist in the forced variation map.' % user_id)
-            return True
-
-        if not validator.is_non_empty_string(variation_key):
-            self.logger.debug('Variation key is invalid.')
-            return False
-
-        forced_variation = project_config.get_variation_from_key(experiment_key, variation_key)
-        if not forced_variation:
-            # The invalid variation key will be logged inside this call.
-            return False
-
-        variation_id = forced_variation.id
-
-        if user_id not in self.forced_variation_map:
-            self.forced_variation_map[user_id] = {experiment_id: variation_id}
-        else:
-            self.forced_variation_map[user_id][experiment_id] = variation_id
-
-        self.logger.debug(
-            'Set variation "%s" for experiment "%s" and user "%s" in the forced variation map.'
-            % (variation_id, experiment_id, user_id)
-        )
-        return True
-
-    def get_forced_variation(self, project_config, experiment_key, user_id):
-        """ Gets the forced variation key for the given user and experiment.
-
-          Args:
-            project_config: Instance of ProjectConfig.
-            experiment_key: Key for experiment.
-            user_id: The user ID.
-
-          Returns:
-            The variation which the given user and experiment should be forced into and
-             array of log messages representing decision making.
-        """
-        decide_reasons = []
-        if user_id not in self.forced_variation_map:
-            message = 'User "%s" is not in the forced variation map.' % user_id
-            self.logger.debug(message)
-            return None, decide_reasons
-
-        experiment = project_config.get_experiment_from_key(experiment_key)
-        if not experiment:
-            # The invalid experiment key will be logged inside this call.
-            return None, decide_reasons
-
-        experiment_to_variation_map = self.forced_variation_map.get(user_id)
-
-        if not experiment_to_variation_map:
-            message = 'No experiment "%s" mapped to user "%s" in the forced variation map.' % (experiment_key, user_id)
-            self.logger.debug(
-                message
-            )
-            return None, decide_reasons
-
-        variation_id = experiment_to_variation_map.get(experiment.id)
-        if variation_id is None:
-            message = 'No variation mapped to experiment "%s" in the forced variation map.' % experiment_key
-            self.logger.debug(message)
-            return None, decide_reasons
-
-        variation = project_config.get_variation_from_id(experiment_key, variation_id)
-        message = 'Variation "%s" is mapped to experiment "%s" and user "%s" in the forced variation map' \
-                  % (variation.key, experiment_key, user_id)
-        self.logger.debug(
-            message
-        )
-        decide_reasons.append(message)
-        return variation, decide_reasons
-
-    def get_whitelisted_variation(self, project_config, experiment, user_id):
-        """ Determine if a user is forced into a variation (through whitelisting)
-        for the given experiment and return that variation.
-
-        Args:
-          project_config: Instance of ProjectConfig.
-          experiment: Object representing the experiment for which user is to be bucketed.
-          user_id: ID for the user.
-
-        Returns:
-          Variation in which the user with ID user_id is forced into. None if no variation and
-           array of log messages representing decision making.
-        """
-        decide_reasons = []
-        forced_variations = experiment.forcedVariations
-
-        if forced_variations and user_id in forced_variations:
-            forced_variation_key = forced_variations.get(user_id)
-            forced_variation = project_config.get_variation_from_key(experiment.key, forced_variation_key)
-
-            if forced_variation:
-                message = 'User "%s" is forced in variation "%s".' % (user_id, forced_variation_key)
-                self.logger.info(message)
-                decide_reasons.append(message)
-
-            return forced_variation, decide_reasons
-
-        return None, decide_reasons
-
-    def get_stored_variation(self, project_config, experiment, user_profile):
-        """ Determine if the user has a stored variation available for the given experiment and return that.
-
-        Args:
-          project_config: Instance of ProjectConfig.
-          experiment: Object representing the experiment for which user is to be bucketed.
-          user_profile: UserProfile object representing the user's profile.
-
-        Returns:
-          Variation if available. None otherwise.
-        """
-        user_id = user_profile.user_id
-        variation_id = user_profile.get_variation_for_experiment(experiment.id)
-
-        if variation_id:
-            variation = project_config.get_variation_from_id(experiment.key, variation_id)
-            if variation:
-                message = 'Found a stored decision. User "%s" is in variation "%s" of experiment "%s".' \
-                          % (user_id, variation.key, experiment.key)
-                self.logger.info(
-                    message
-                )
-                return variation
-
-        return None
-
-    def get_variation(self, project_config, experiment, user_context, options=None):
-        """ Top-level function to help determine variation user should be put in.
-
-        First, check if experiment is running.
-        Second, check if user is forced in a variation.
-        Third, check if there is a stored decision for the user and return the corresponding variation.
-        Fourth, figure out if user is in the experiment by evaluating audience conditions if any.
-        Fifth, bucket the user and return the variation.
-
-        Args:
-          project_config: Instance of ProjectConfig.
-          experiment: Experiment for which user variation needs to be determined.
-          user_context: contains user id and attributes
-          options: Decide options.
-
-        Returns:
-          Variation user should see. None if user is not in experiment or experiment is not running
-          And an array of log messages representing decision making.
-        """
-        user_id = user_context.user_id
-        attributes = user_context.get_user_attributes()
-
-        if options:
-            ignore_user_profile = OptimizelyDecideOption.IGNORE_USER_PROFILE_SERVICE in options
-        else:
-            ignore_user_profile = False
-
-        decide_reasons = []
-        # Check if experiment is running
-        if not experiment_helper.is_experiment_running(experiment):
-            message = 'Experiment "%s" is not running.' % experiment.key
-            self.logger.info(message)
-            decide_reasons.append(message)
-            return None, decide_reasons
-
-        # Check if the user is forced into a variation
-        variation, reasons_received = self.get_forced_variation(project_config, experiment.key, user_id)
-        decide_reasons += reasons_received
-        if variation:
-            return variation, decide_reasons
-
-        # Check to see if user is white-listed for a certain variation
-        variation, reasons_received = self.get_whitelisted_variation(project_config, experiment, user_id)
-        decide_reasons += reasons_received
-        if variation:
-            return variation, decide_reasons
-
-        # Check to see if user has a decision available for the given experiment
-        user_profile = UserProfile(user_id)
-        if not ignore_user_profile and self.user_profile_service:
-            try:
-                retrieved_profile = self.user_profile_service.lookup(user_id)
-            except:
-                self.logger.exception('Unable to retrieve user profile for user "{}" as lookup failed.'.format(user_id))
-                retrieved_profile = None
-
-            if validator.is_user_profile_valid(retrieved_profile):
-                user_profile = UserProfile(**retrieved_profile)
-                variation = self.get_stored_variation(project_config, experiment, user_profile)
-                if variation:
-                    message = 'Returning previously activated variation ID "{}" of experiment ' \
-                              '"{}" for user "{}" from user profile.'.format(variation, experiment, user_id)
-                    self.logger.info(message)
-                    decide_reasons.append(message)
-                    return variation, decide_reasons
-            else:
-                self.logger.warning('User profile has invalid format.')
-
-        # Bucket user and store the new decision
-        audience_conditions = experiment.get_audience_conditions_or_ids()
-        user_meets_audience_conditions, reasons_received = audience_helper.does_user_meet_audience_conditions(
-            project_config, audience_conditions,
-            enums.ExperimentAudienceEvaluationLogs,
-            experiment.key,
-            attributes, self.logger)
-        decide_reasons += reasons_received
-        if not user_meets_audience_conditions:
-            message = 'User "{}" does not meet conditions to be in experiment "{}".'.format(user_id, experiment.key)
-            self.logger.info(
-                message
-            )
-            decide_reasons.append(message)
-            return None, decide_reasons
-
-        # Determine bucketing ID to be used
-        bucketing_id, bucketing_id_reasons = self._get_bucketing_id(user_id, attributes)
-        decide_reasons += bucketing_id_reasons
-        variation, bucket_reasons = self.bucketer.bucket(project_config, experiment, user_id, bucketing_id)
-        decide_reasons += bucket_reasons
-        if variation:
-            message = 'User "%s" is in variation "%s" of experiment %s.' % (user_id, variation.key, experiment.key)
-            self.logger.info(
-                message
-            )
-            decide_reasons.append(message)
-            # Store this new decision and return the variation for the user
-            if not ignore_user_profile and self.user_profile_service:
-                try:
-                    user_profile.save_variation_for_experiment(experiment.id, variation.id)
-                    self.user_profile_service.save(user_profile.__dict__)
-                except:
-                    self.logger.exception('Unable to save user profile for user "{}".'.format(user_id))
-            return variation, decide_reasons
-        message = 'User "%s" is in no variation.' % user_id
-        self.logger.info(message)
-        decide_reasons.append(message)
-        return None, decide_reasons
-
-    def get_variation_for_rollout(self, project_config, feature, user):
-        """ Determine which experiment/variation the user is in for a given rollout.
-            Returns the variation of the first experiment the user qualifies for.
-
-        Args:
-          project_config: Instance of ProjectConfig.
-          flagKey: Feature key.
-          rollout: Rollout for which we are getting the variation.
-          user: ID and attributes for user.
-          options: Decide options.
-
-        Returns:
-          Decision namedtuple consisting of experiment and variation for the user and
-          array of log messages representing decision making.
-        """
-        decide_reasons = []
-        user_id = user.user_id
-        attributes = user.get_user_attributes()
-
-        if not feature or not feature.rolloutId:
-            return Decision(None, None, enums.DecisionSources.ROLLOUT), decide_reasons
-
-        rollout = project_config.get_rollout_from_id(feature.rolloutId)
-
-        if not rollout:
-            message = 'There is no rollout of feature {}.'.format(feature.key)
-            self.logger.debug(message)
-            decide_reasons.append(message)
-            return Decision(None, None, enums.DecisionSources.ROLLOUT), decide_reasons
-
-        rollout_rules = project_config.get_rollout_experiments(rollout)
-
-        if not rollout_rules:
-            message = 'Rollout {} has no experiments.'.format(rollout.id)
-            self.logger.debug(message)
-            decide_reasons.append(message)
-            return Decision(None, None, enums.DecisionSources.ROLLOUT), decide_reasons
-
-        index = 0
-        while index < len(rollout_rules):
-            skip_to_everyone_else = False
-
-            # check forced decision first
-            rule = rollout_rules[index]
-            optimizely_decision_context = OptimizelyUserContext.OptimizelyDecisionContext(feature.key, rule.key)
-            forced_decision_variation, reasons_received = self.validated_forced_decision(
-                project_config, optimizely_decision_context, user)
-            decide_reasons += reasons_received
-
-            if forced_decision_variation:
-                return Decision(experiment=rule, variation=forced_decision_variation,
-                                source=enums.DecisionSources.ROLLOUT), decide_reasons
-
-            bucketing_id, bucket_reasons = self._get_bucketing_id(user_id, attributes)
-            decide_reasons += bucket_reasons
-
-            everyone_else = (index == len(rollout_rules) - 1)
-            logging_key = "Everyone Else" if everyone_else else str(index + 1)
-
-            rollout_rule = project_config.get_experiment_from_id(rule.id)
-            audience_conditions = rollout_rule.get_audience_conditions_or_ids()
-
-            audience_decision_response, reasons_received_audience = audience_helper.does_user_meet_audience_conditions(
-                project_config, audience_conditions, enums.RolloutRuleAudienceEvaluationLogs,
-                logging_key, attributes, self.logger)
-
-            decide_reasons += reasons_received_audience
-
-            if audience_decision_response:
-                message = 'User "{}" meets audience conditions for targeting rule {}.'.format(user_id, logging_key)
-                self.logger.debug(message)
-                decide_reasons.append(message)
-
-                bucketed_variation, bucket_reasons = self.bucketer.bucket(project_config, rollout_rule, user_id,
-                                                                          bucketing_id)
-                decide_reasons.extend(bucket_reasons)
-
-                if bucketed_variation:
-                    message = 'User "{}" bucketed into a targeting rule {}.'.format(user_id, logging_key)
-                    self.logger.debug(message)
-                    decide_reasons.append(message)
-                    return Decision(experiment=rule, variation=bucketed_variation,
-                                    source=enums.DecisionSources.ROLLOUT), decide_reasons
-
-                elif not everyone_else:
-                    # skip this logging for EveryoneElse since this has a message not for everyone_else
-                    message = 'User "{}" not bucketed into a targeting rule {}. ' \
-                              'Checking "Everyone Else" rule now.'.format(user_id, logging_key)
-                    self.logger.debug(message)
-                    decide_reasons.append(message)
-
-                    # skip the rest of rollout rules to the everyone-else rule if audience matches but not bucketed.
-                    skip_to_everyone_else = True
-
-            else:
-                message = 'User "{}" does not meet audience conditions for targeting rule {}.'.format(
-                    user_id, logging_key)
-                self.logger.debug(message)
-                decide_reasons.append(message)
-
-            # the last rule is special for "Everyone Else"
-            index = len(rollout_rules) - 1 if skip_to_everyone_else else index + 1
-
-        return Decision(None, None, enums.DecisionSources.ROLLOUT), decide_reasons
-
-    def get_variation_for_feature(self, project_config, feature, user_context, options=None):
-        """ Returns the experiment/variation the user is bucketed in for the given feature.
-
-        Args:
-          project_config: Instance of ProjectConfig.
-          feature: Feature for which we are determining if it is enabled or not for the given user.
-          user: user context for user.
-          attributes: Dict representing user attributes.
-          options: Decide options.
-
-        Returns:
-          Decision namedtuple consisting of experiment and variation for the user.
-    """
-        decide_reasons = []
-
-        # Check if the feature flag is under an experiment and the the user is bucketed into one of these experiments
-        if feature.experimentIds:
-            # Evaluate each experiment ID and return the first bucketed experiment variation
-            for experiment in feature.experimentIds:
-                experiment = project_config.get_experiment_from_id(experiment)
-                decision_variation = None
-
-                if experiment:
-                    optimizely_decision_context = OptimizelyUserContext.OptimizelyDecisionContext(feature.key,
-                                                                                                  experiment.key)
-
-                    forced_decision_variation, reasons_received = self.validated_forced_decision(
-                        project_config, optimizely_decision_context, user_context)
-                    decide_reasons += reasons_received
-
-                    if forced_decision_variation:
-                        decision_variation = forced_decision_variation
-                    else:
-                        decision_variation, variation_reasons = self.get_variation(project_config,
-                                                                                   experiment, user_context, options)
-                        decide_reasons += variation_reasons
-
-                    if decision_variation:
-                        message = 'User "{}" bucketed into a experiment "{}" of feature "{}".'.format(
-                            user_context.user_id, experiment.key, feature.key)
-                        self.logger.debug(message)
-                        return Decision(experiment, decision_variation,
-                                        enums.DecisionSources.FEATURE_TEST), decide_reasons
-
-        message = 'User "{}" is not bucketed into any of the experiments on the feature "{}".'.format(
-            user_context.user_id, feature.key)
-        self.logger.debug(message)
-        variation, rollout_variation_reasons = self.get_variation_for_rollout(project_config, feature, user_context)
-        if rollout_variation_reasons:
-            decide_reasons += rollout_variation_reasons
-        return variation, decide_reasons
-
-    def validated_forced_decision(self, project_config, decision_context, user_context):
-        """
-        Gets forced decisions based on flag key, rule key and variation.
-
-        Args:
-            project_config: a project config
-            decision context: a decision context
-            user_context context: a user context
-
-        Returns:
-            Variation of the forced decision.
-        """
-        reasons = []
-
-        forced_decision = user_context.get_forced_decision(decision_context)
-
-        flag_key = decision_context.flag_key
-        rule_key = decision_context.rule_key
-
-        if forced_decision:
-            if not project_config:
-                return None, reasons
-            variation = project_config.get_flag_variation(flag_key, 'key', forced_decision.variation_key)
-            if variation:
-                if rule_key:
-                    user_has_forced_decision = enums.ForcedDecisionLogs \
-                        .USER_HAS_FORCED_DECISION_WITH_RULE_SPECIFIED.format(forced_decision.variation_key,
-                                                                             flag_key,
-                                                                             rule_key,
-                                                                             user_context.user_id)
-
-                else:
-                    user_has_forced_decision = enums.ForcedDecisionLogs \
-                        .USER_HAS_FORCED_DECISION_WITHOUT_RULE_SPECIFIED.format(forced_decision.variation_key,
-                                                                                flag_key,
-                                                                                user_context.user_id)
-
-                reasons.append(user_has_forced_decision)
-                user_context.logger.info(user_has_forced_decision)
-
-                return variation, reasons
-
-            else:
-                if rule_key:
-                    user_has_forced_decision_but_invalid = enums.ForcedDecisionLogs \
-                        .USER_HAS_FORCED_DECISION_WITH_RULE_SPECIFIED_BUT_INVALID.format(flag_key,
-                                                                                         rule_key,
-                                                                                         user_context.user_id)
-                else:
-                    user_has_forced_decision_but_invalid = enums.ForcedDecisionLogs \
-                        .USER_HAS_FORCED_DECISION_WITHOUT_RULE_SPECIFIED_BUT_INVALID.format(flag_key,
-                                                                                            user_context.user_id)
-
-                reasons.append(user_has_forced_decision_but_invalid)
-                user_context.logger.info(user_has_forced_decision_but_invalid)
-
-        return None, reasons
+# Copyright 2017-2022, Optimizely
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from __future__ import annotations
+from typing import TYPE_CHECKING, NamedTuple, Optional, Sequence
+
+from . import bucketer
+from . import entities
+from .decision.optimizely_decide_option import OptimizelyDecideOption
+from .helpers import audience as audience_helper
+from .helpers import enums
+from .helpers import experiment as experiment_helper
+from .helpers import validator
+from .optimizely_user_context import OptimizelyUserContext, UserAttributes
+from .user_profile import UserProfile, UserProfileService
+
+if TYPE_CHECKING:
+    # prevent circular dependenacy by skipping import at runtime
+    from .project_config import ProjectConfig
+    from .logger import Logger
+
+
+class Decision(NamedTuple):
+    """Named tuple containing selected experiment, variation and source.
+    None if no experiment/variation was selected."""
+    experiment: Optional[entities.Experiment]
+    variation: Optional[entities.Variation]
+    source: str
+
+
+class DecisionService:
+    """ Class encapsulating all decision related capabilities. """
+
+    def __init__(self, logger: Logger, user_profile_service: Optional[UserProfileService]):
+        self.bucketer = bucketer.Bucketer()
+        self.logger = logger
+        self.user_profile_service = user_profile_service
+
+        # Map of user IDs to another map of experiments to variations.
+        # This contains all the forced variations set by the user
+        # by calling set_forced_variation (it is not the same as the
+        # whitelisting forcedVariations data structure).
+        self.forced_variation_map: dict[str, dict[str, str]] = {}
+
+    def _get_bucketing_id(self, user_id: str, attributes: Optional[UserAttributes]) -> tuple[str, list[str]]:
+        """ Helper method to determine bucketing ID for the user.
+
+        Args:
+          user_id: ID for user.
+          attributes: Dict representing user attributes. May consist of bucketing ID to be used.
+
+        Returns:
+          String representing bucketing ID if it is a String type in attributes else return user ID
+          array of log messages representing decision making.
+        """
+        decide_reasons: list[str] = []
+        attributes = attributes or UserAttributes({})
+        bucketing_id = attributes.get(enums.ControlAttributes.BUCKETING_ID)
+
+        if bucketing_id is not None:
+            if isinstance(bucketing_id, str):
+                return bucketing_id, decide_reasons
+            message = 'Bucketing ID attribute is not a string. Defaulted to user_id.'
+            self.logger.warning(message)
+            decide_reasons.append(message)
+
+        return user_id, decide_reasons
+
+    def set_forced_variation(
+        self, project_config: ProjectConfig, experiment_key: str,
+        user_id: str, variation_key: Optional[str]
+    ) -> bool:
+        """ Sets users to a map of experiments to forced variations.
+
+          Args:
+            project_config: Instance of ProjectConfig.
+            experiment_key: Key for experiment.
+            user_id: The user ID.
+            variation_key: Key for variation. If None, then clear the existing experiment-to-variation mapping.
+
+          Returns:
+            A boolean value that indicates if the set completed successfully.
+        """
+        experiment = project_config.get_experiment_from_key(experiment_key)
+        if not experiment:
+            # The invalid experiment key will be logged inside this call.
+            return False
+
+        experiment_id = experiment.id
+        if variation_key is None:
+            if user_id in self.forced_variation_map:
+                experiment_to_variation_map = self.forced_variation_map[user_id]
+                if experiment_id in experiment_to_variation_map:
+                    del self.forced_variation_map[user_id][experiment_id]
+                    self.logger.debug(
+                        f'Variation mapped to experiment "{experiment_key}" has been removed for user "{user_id}".'
+                    )
+                else:
+                    self.logger.debug(
+                        f'Nothing to remove. Variation mapped to experiment "{experiment_key}" for '
+                        f'user "{user_id}" does not exist.'
+                    )
+            else:
+                self.logger.debug(f'Nothing to remove. User "{user_id}" does not exist in the forced variation map.')
+            return True
+
+        if not validator.is_non_empty_string(variation_key):
+            self.logger.debug('Variation key is invalid.')
+            return False
+
+        forced_variation = project_config.get_variation_from_key(experiment_key, variation_key)
+        if not forced_variation:
+            # The invalid variation key will be logged inside this call.
+            return False
+
+        variation_id = forced_variation.id
+
+        if user_id not in self.forced_variation_map:
+            self.forced_variation_map[user_id] = {experiment_id: variation_id}
+        else:
+            self.forced_variation_map[user_id][experiment_id] = variation_id
+
+        self.logger.debug(
+            f'Set variation "{variation_id}" for experiment "{experiment_id}" and '
+            f'user "{user_id}" in the forced variation map.'
+        )
+        return True
+
+    def get_forced_variation(
+        self, project_config: ProjectConfig, experiment_key: str, user_id: str
+    ) -> tuple[Optional[entities.Variation], list[str]]:
+        """ Gets the forced variation key for the given user and experiment.
+
+          Args:
+            project_config: Instance of ProjectConfig.
+            experiment_key: Key for experiment.
+            user_id: The user ID.
+
+          Returns:
+            The variation which the given user and experiment should be forced into and
+             array of log messages representing decision making.
+        """
+        decide_reasons: list[str] = []
+        if user_id not in self.forced_variation_map:
+            message = f'User "{user_id}" is not in the forced variation map.'
+            self.logger.debug(message)
+            return None, decide_reasons
+
+        experiment = project_config.get_experiment_from_key(experiment_key)
+        if not experiment:
+            # The invalid experiment key will be logged inside this call.
+            return None, decide_reasons
+
+        experiment_to_variation_map = self.forced_variation_map.get(user_id)
+
+        if not experiment_to_variation_map:
+            message = f'No experiment "{experiment_key}" mapped to user "{user_id}" in the forced variation map.'
+            self.logger.debug(message)
+            return None, decide_reasons
+
+        variation_id = experiment_to_variation_map.get(experiment.id)
+        if variation_id is None:
+            message = f'No variation mapped to experiment "{experiment_key}" in the forced variation map.'
+            self.logger.debug(message)
+            return None, decide_reasons
+
+        variation = project_config.get_variation_from_id(experiment_key, variation_id)
+        # this case is logged in get_variation_from_id
+        if variation is None:
+            return None, decide_reasons
+
+        message = f'Variation "{variation.key}" is mapped to experiment "{experiment_key}" and ' \
+                  f'user "{user_id}" in the forced variation map'
+        self.logger.debug(message)
+        decide_reasons.append(message)
+        return variation, decide_reasons
+
+    def get_whitelisted_variation(
+        self, project_config: ProjectConfig, experiment: entities.Experiment, user_id: str
+    ) -> tuple[Optional[entities.Variation], list[str]]:
+        """ Determine if a user is forced into a variation (through whitelisting)
+        for the given experiment and return that variation.
+
+        Args:
+          project_config: Instance of ProjectConfig.
+          experiment: Object representing the experiment for which user is to be bucketed.
+          user_id: ID for the user.
+
+        Returns:
+          Variation in which the user with ID user_id is forced into. None if no variation and
+           array of log messages representing decision making.
+        """
+        decide_reasons = []
+        forced_variations = experiment.forcedVariations
+
+        if forced_variations and user_id in forced_variations:
+            forced_variation_key = forced_variations[user_id]
+            forced_variation = project_config.get_variation_from_key(experiment.key, forced_variation_key)
+
+            if forced_variation:
+                message = f'User "{user_id}" is forced in variation "{forced_variation_key}".'
+                self.logger.info(message)
+                decide_reasons.append(message)
+
+            return forced_variation, decide_reasons
+
+        return None, decide_reasons
+
+    def get_stored_variation(
+        self, project_config: ProjectConfig, experiment: entities.Experiment, user_profile: UserProfile
+    ) -> Optional[entities.Variation]:
+        """ Determine if the user has a stored variation available for the given experiment and return that.
+
+        Args:
+          project_config: Instance of ProjectConfig.
+          experiment: Object representing the experiment for which user is to be bucketed.
+          user_profile: UserProfile object representing the user's profile.
+
+        Returns:
+          Variation if available. None otherwise.
+        """
+        user_id = user_profile.user_id
+        variation_id = user_profile.get_variation_for_experiment(experiment.id)
+
+        if variation_id:
+            variation = project_config.get_variation_from_id(experiment.key, variation_id)
+            if variation:
+                message = f'Found a stored decision. User "{user_id}" is in ' \
+                          f'variation "{variation.key}" of experiment "{experiment.key}".'
+                self.logger.info(message)
+                return variation
+
+        return None
+
+    def get_variation(
+        self,
+        project_config: ProjectConfig,
+        experiment: entities.Experiment,
+        user_context: OptimizelyUserContext,
+        options: Optional[Sequence[str]] = None
+    ) -> tuple[Optional[entities.Variation], list[str]]:
+        """ Top-level function to help determine variation user should be put in.
+
+        First, check if experiment is running.
+        Second, check if user is forced in a variation.
+        Third, check if there is a stored decision for the user and return the corresponding variation.
+        Fourth, figure out if user is in the experiment by evaluating audience conditions if any.
+        Fifth, bucket the user and return the variation.
+
+        Args:
+          project_config: Instance of ProjectConfig.
+          experiment: Experiment for which user variation needs to be determined.
+          user_context: contains user id and attributes
+          options: Decide options.
+
+        Returns:
+          Variation user should see. None if user is not in experiment or experiment is not running
+          And an array of log messages representing decision making.
+        """
+        user_id = user_context.user_id
+
+        if options:
+            ignore_user_profile = OptimizelyDecideOption.IGNORE_USER_PROFILE_SERVICE in options
+        else:
+            ignore_user_profile = False
+
+        decide_reasons = []
+        # Check if experiment is running
+        if not experiment_helper.is_experiment_running(experiment):
+            message = f'Experiment "{experiment.key}" is not running.'
+            self.logger.info(message)
+            decide_reasons.append(message)
+            return None, decide_reasons
+
+        # Check if the user is forced into a variation
+        variation: Optional[entities.Variation]
+        variation, reasons_received = self.get_forced_variation(project_config, experiment.key, user_id)
+        decide_reasons += reasons_received
+        if variation:
+            return variation, decide_reasons
+
+        # Check to see if user is white-listed for a certain variation
+        variation, reasons_received = self.get_whitelisted_variation(project_config, experiment, user_id)
+        decide_reasons += reasons_received
+        if variation:
+            return variation, decide_reasons
+
+        # Check to see if user has a decision available for the given experiment
+        user_profile = UserProfile(user_id)
+        if not ignore_user_profile and self.user_profile_service:
+            try:
+                retrieved_profile = self.user_profile_service.lookup(user_id)
+            except:
+                self.logger.exception(f'Unable to retrieve user profile for user "{user_id}" as lookup failed.')
+                retrieved_profile = None
+
+            if retrieved_profile and validator.is_user_profile_valid(retrieved_profile):
+                user_profile = UserProfile(**retrieved_profile)
+                variation = self.get_stored_variation(project_config, experiment, user_profile)
+                if variation:
+                    message = f'Returning previously activated variation ID "{variation}" of experiment ' \
+                              f'"{experiment}" for user "{user_id}" from user profile.'
+                    self.logger.info(message)
+                    decide_reasons.append(message)
+                    return variation, decide_reasons
+            else:
+                self.logger.warning('User profile has invalid format.')
+
+        # Bucket user and store the new decision
+        audience_conditions = experiment.get_audience_conditions_or_ids()
+        user_meets_audience_conditions, reasons_received = audience_helper.does_user_meet_audience_conditions(
+            project_config, audience_conditions,
+            enums.ExperimentAudienceEvaluationLogs,
+            experiment.key,
+            user_context, self.logger)
+        decide_reasons += reasons_received
+        if not user_meets_audience_conditions:
+            message = f'User "{user_id}" does not meet conditions to be in experiment "{experiment.key}".'
+            self.logger.info(message)
+            decide_reasons.append(message)
+            return None, decide_reasons
+
+        # Determine bucketing ID to be used
+        bucketing_id, bucketing_id_reasons = self._get_bucketing_id(user_id, user_context.get_user_attributes())
+        decide_reasons += bucketing_id_reasons
+        variation, bucket_reasons = self.bucketer.bucket(project_config, experiment, user_id, bucketing_id)
+        decide_reasons += bucket_reasons
+        if isinstance(variation, entities.Variation):
+            message = f'User "{user_id}" is in variation "{variation.key}" of experiment {experiment.key}.'
+            self.logger.info(message)
+            decide_reasons.append(message)
+            # Store this new decision and return the variation for the user
+            if not ignore_user_profile and self.user_profile_service:
+                try:
+                    user_profile.save_variation_for_experiment(experiment.id, variation.id)
+                    self.user_profile_service.save(user_profile.__dict__)
+                except:
+                    self.logger.exception(f'Unable to save user profile for user "{user_id}".')
+            return variation, decide_reasons
+        message = f'User "{user_id}" is in no variation.'
+        self.logger.info(message)
+        decide_reasons.append(message)
+        return None, decide_reasons
+
+    def get_variation_for_rollout(
+        self, project_config: ProjectConfig, feature: entities.FeatureFlag, user_context: OptimizelyUserContext
+    ) -> tuple[Decision, list[str]]:
+        """ Determine which experiment/variation the user is in for a given rollout.
+            Returns the variation of the first experiment the user qualifies for.
+
+        Args:
+          project_config: Instance of ProjectConfig.
+          flagKey: Feature key.
+          rollout: Rollout for which we are getting the variation.
+          user: ID and attributes for user.
+          options: Decide options.
+
+        Returns:
+          Decision namedtuple consisting of experiment and variation for the user and
+          array of log messages representing decision making.
+        """
+        decide_reasons: list[str] = []
+        user_id = user_context.user_id
+        attributes = user_context.get_user_attributes()
+
+        if not feature or not feature.rolloutId:
+            return Decision(None, None, enums.DecisionSources.ROLLOUT), decide_reasons
+
+        rollout = project_config.get_rollout_from_id(feature.rolloutId)
+
+        if not rollout:
+            message = f'There is no rollout of feature {feature.key}.'
+            self.logger.debug(message)
+            decide_reasons.append(message)
+            return Decision(None, None, enums.DecisionSources.ROLLOUT), decide_reasons
+
+        rollout_rules = project_config.get_rollout_experiments(rollout)
+
+        if not rollout_rules:
+            message = f'Rollout {rollout.id} has no experiments.'
+            self.logger.debug(message)
+            decide_reasons.append(message)
+            return Decision(None, None, enums.DecisionSources.ROLLOUT), decide_reasons
+
+        index = 0
+        while index < len(rollout_rules):
+            skip_to_everyone_else = False
+
+            # check forced decision first
+            rule = rollout_rules[index]
+            optimizely_decision_context = OptimizelyUserContext.OptimizelyDecisionContext(feature.key, rule.key)
+            forced_decision_variation, reasons_received = self.validated_forced_decision(
+                project_config, optimizely_decision_context, user_context)
+            decide_reasons += reasons_received
+
+            if forced_decision_variation:
+                return Decision(experiment=rule, variation=forced_decision_variation,
+                                source=enums.DecisionSources.ROLLOUT), decide_reasons
+
+            bucketing_id, bucket_reasons = self._get_bucketing_id(user_id, attributes)
+            decide_reasons += bucket_reasons
+
+            everyone_else = (index == len(rollout_rules) - 1)
+            logging_key = "Everyone Else" if everyone_else else str(index + 1)
+
+            rollout_rule = project_config.get_experiment_from_id(rule.id)
+            # error is logged in get_experiment_from_id
+            if rollout_rule is None:
+                continue
+            audience_conditions = rollout_rule.get_audience_conditions_or_ids()
+
+            audience_decision_response, reasons_received_audience = audience_helper.does_user_meet_audience_conditions(
+                project_config, audience_conditions, enums.RolloutRuleAudienceEvaluationLogs,
+                logging_key, user_context, self.logger)
+
+            decide_reasons += reasons_received_audience
+
+            if audience_decision_response:
+                message = f'User "{user_id}" meets audience conditions for targeting rule {logging_key}.'
+                self.logger.debug(message)
+                decide_reasons.append(message)
+
+                bucketed_variation, bucket_reasons = self.bucketer.bucket(project_config, rollout_rule, user_id,
+                                                                          bucketing_id)
+                decide_reasons.extend(bucket_reasons)
+
+                if bucketed_variation:
+                    message = f'User "{user_id}" bucketed into a targeting rule {logging_key}.'
+                    self.logger.debug(message)
+                    decide_reasons.append(message)
+                    return Decision(experiment=rule, variation=bucketed_variation,
+                                    source=enums.DecisionSources.ROLLOUT), decide_reasons
+
+                elif not everyone_else:
+                    # skip this logging for EveryoneElse since this has a message not for everyone_else
+                    message = f'User "{user_id}" not bucketed into a targeting rule {logging_key}. ' \
+                              'Checking "Everyone Else" rule now.'
+                    self.logger.debug(message)
+                    decide_reasons.append(message)
+
+                    # skip the rest of rollout rules to the everyone-else rule if audience matches but not bucketed.
+                    skip_to_everyone_else = True
+
+            else:
+                message = f'User "{user_id}" does not meet audience conditions for targeting rule {logging_key}.'
+                self.logger.debug(message)
+                decide_reasons.append(message)
+
+            # the last rule is special for "Everyone Else"
+            index = len(rollout_rules) - 1 if skip_to_everyone_else else index + 1
+
+        return Decision(None, None, enums.DecisionSources.ROLLOUT), decide_reasons
+
+    def get_variation_for_feature(
+        self,
+        project_config: ProjectConfig,
+        feature: entities.FeatureFlag,
+        user_context: OptimizelyUserContext,
+        options: Optional[list[str]] = None
+    ) -> tuple[Decision, list[str]]:
+        """ Returns the experiment/variation the user is bucketed in for the given feature.
+
+        Args:
+          project_config: Instance of ProjectConfig.
+          feature: Feature for which we are determining if it is enabled or not for the given user.
+          user_context: user context for user.
+          options: Decide options.
+
+        Returns:
+          Decision namedtuple consisting of experiment and variation for the user.
+    """
+        decide_reasons = []
+
+        # Check if the feature flag is under an experiment and the the user is bucketed into one of these experiments
+        if feature.experimentIds:
+            # Evaluate each experiment ID and return the first bucketed experiment variation
+            for experiment_id in feature.experimentIds:
+                experiment = project_config.get_experiment_from_id(experiment_id)
+                decision_variation = None
+
+                if experiment:
+                    optimizely_decision_context = OptimizelyUserContext.OptimizelyDecisionContext(feature.key,
+                                                                                                  experiment.key)
+
+                    forced_decision_variation, reasons_received = self.validated_forced_decision(
+                        project_config, optimizely_decision_context, user_context)
+                    decide_reasons += reasons_received
+
+                    if forced_decision_variation:
+                        decision_variation = forced_decision_variation
+                    else:
+                        decision_variation, variation_reasons = self.get_variation(project_config,
+                                                                                   experiment, user_context, options)
+                        decide_reasons += variation_reasons
+
+                    if decision_variation:
+                        message = f'User "{user_context.user_id}" bucketed into a ' \
+                                  f'experiment "{experiment.key}" of feature "{feature.key}".'
+                        self.logger.debug(message)
+                        return Decision(experiment, decision_variation,
+                                        enums.DecisionSources.FEATURE_TEST), decide_reasons
+
+        message = f'User "{user_context.user_id}" is not bucketed into any of the ' \
+                  f'experiments on the feature "{feature.key}".'
+        self.logger.debug(message)
+        variation, rollout_variation_reasons = self.get_variation_for_rollout(project_config, feature, user_context)
+        if rollout_variation_reasons:
+            decide_reasons += rollout_variation_reasons
+        return variation, decide_reasons
+
+    def validated_forced_decision(
+        self,
+        project_config: ProjectConfig,
+        decision_context: OptimizelyUserContext.OptimizelyDecisionContext,
+        user_context: OptimizelyUserContext
+    ) -> tuple[Optional[entities.Variation], list[str]]:
+        """
+        Gets forced decisions based on flag key, rule key and variation.
+
+        Args:
+            project_config: a project config
+            decision context: a decision context
+            user_context context: a user context
+
+        Returns:
+            Variation of the forced decision.
+        """
+        reasons: list[str] = []
+
+        forced_decision = user_context.get_forced_decision(decision_context)
+
+        flag_key = decision_context.flag_key
+        rule_key = decision_context.rule_key
+
+        if forced_decision:
+            if not project_config:
+                return None, reasons
+            variation = project_config.get_flag_variation(flag_key, 'key', forced_decision.variation_key)
+            if variation:
+                if rule_key:
+                    user_has_forced_decision = enums.ForcedDecisionLogs \
+                        .USER_HAS_FORCED_DECISION_WITH_RULE_SPECIFIED.format(forced_decision.variation_key,
+                                                                             flag_key,
+                                                                             rule_key,
+                                                                             user_context.user_id)
+
+                else:
+                    user_has_forced_decision = enums.ForcedDecisionLogs \
+                        .USER_HAS_FORCED_DECISION_WITHOUT_RULE_SPECIFIED.format(forced_decision.variation_key,
+                                                                                flag_key,
+                                                                                user_context.user_id)
+
+                reasons.append(user_has_forced_decision)
+                user_context.logger.info(user_has_forced_decision)
+
+                return variation, reasons
+
+            else:
+                if rule_key:
+                    user_has_forced_decision_but_invalid = enums.ForcedDecisionLogs \
+                        .USER_HAS_FORCED_DECISION_WITH_RULE_SPECIFIED_BUT_INVALID.format(flag_key,
+                                                                                         rule_key,
+                                                                                         user_context.user_id)
+                else:
+                    user_has_forced_decision_but_invalid = enums.ForcedDecisionLogs \
+                        .USER_HAS_FORCED_DECISION_WITHOUT_RULE_SPECIFIED_BUT_INVALID.format(flag_key,
+                                                                                            user_context.user_id)
+
+                reasons.append(user_has_forced_decision_but_invalid)
+                user_context.logger.info(user_has_forced_decision_but_invalid)
+
+        return None, reasons
```

### Comparing `optimizely-sdk-4.1.1/optimizely/event/__init__.py` & `optimizely-sdk-5.0.0b0/optimizely/helpers/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2019, Optimizely
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# Copyright 2016, Optimizely
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
```

### Comparing `optimizely-sdk-4.1.1/optimizely/event/event_processor.py` & `optimizely-sdk-5.0.0b0/optimizely/event/event_processor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,369 +1,398 @@
-# Copyright 2019-2021 Optimizely
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import abc
-import numbers
-import threading
-import time
-
-from datetime import timedelta
-from six.moves import queue
-
-from optimizely import logger as _logging
-from optimizely import notification_center as _notification_center
-from optimizely.event_dispatcher import EventDispatcher as default_event_dispatcher
-from optimizely.helpers import enums
-from optimizely.helpers import validator
-from .event_factory import EventFactory
-from .user_event import UserEvent
-
-ABC = abc.ABCMeta('ABC', (object,), {'__slots__': ()})
-
-
-class BaseEventProcessor(ABC):
-    """ Class encapsulating event processing. Override with your own implementation. """
-
-    @abc.abstractmethod
-    def process(self, user_event):
-        """ Method to provide intermediary processing stage within event production.
-    Args:
-      user_event: UserEvent instance that needs to be processed and dispatched.
-    """
-        pass
-
-
-class BatchEventProcessor(BaseEventProcessor):
-    """
-  BatchEventProcessor is an implementation of the BaseEventProcessor that batches events.
-
-  The BatchEventProcessor maintains a single consumer thread that pulls events off of
-  the blocking queue and buffers them for either a configured batch size or for a
-  maximum duration before the resulting LogEvent is sent to the EventDispatcher.
-  """
-
-    _DEFAULT_QUEUE_CAPACITY = 1000
-    _DEFAULT_BATCH_SIZE = 10
-    _DEFAULT_FLUSH_INTERVAL = 30
-    _DEFAULT_TIMEOUT_INTERVAL = 5
-    _SHUTDOWN_SIGNAL = object()
-    _FLUSH_SIGNAL = object()
-    LOCK = threading.Lock()
-
-    def __init__(
-        self,
-        event_dispatcher,
-        logger=None,
-        start_on_init=False,
-        event_queue=None,
-        batch_size=None,
-        flush_interval=None,
-        timeout_interval=None,
-        notification_center=None,
-    ):
-        """ BatchEventProcessor init method to configure event batching.
-
-    Args:
-      event_dispatcher: Provides a dispatch_event method which if given a URL and params sends a request to it.
-      logger: Optional component which provides a log method to log messages. By default nothing would be logged.
-      start_on_init: Optional boolean param which starts the consumer thread if set to True.
-                     Default value is False.
-      event_queue: Optional component which accumulates the events until dispacthed.
-      batch_size: Optional param which defines the upper limit on the number of events in event_queue after which
-                  the event_queue will be flushed.
-      flush_interval: Optional floating point number representing time interval in seconds after which event_queue will
-                      be flushed.
-      timeout_interval: Optional floating point number representing time interval in seconds before joining the consumer
-                        thread.
-      notification_center: Optional instance of notification_center.NotificationCenter.
-    """
-        self.event_dispatcher = event_dispatcher or default_event_dispatcher
-        self.logger = _logging.adapt_logger(logger or _logging.NoOpLogger())
-        self.event_queue = event_queue or queue.Queue(maxsize=self._DEFAULT_QUEUE_CAPACITY)
-        self.batch_size = (
-            batch_size
-            if self._validate_instantiation_props(batch_size, 'batch_size', self._DEFAULT_BATCH_SIZE)
-            else self._DEFAULT_BATCH_SIZE
-        )
-        self.flush_interval = (
-            timedelta(seconds=flush_interval)
-            if self._validate_instantiation_props(flush_interval, 'flush_interval', self._DEFAULT_FLUSH_INTERVAL)
-            else timedelta(seconds=self._DEFAULT_FLUSH_INTERVAL)
-        )
-        self.timeout_interval = (
-            timedelta(seconds=timeout_interval)
-            if self._validate_instantiation_props(timeout_interval, 'timeout_interval', self._DEFAULT_TIMEOUT_INTERVAL)
-            else timedelta(seconds=self._DEFAULT_TIMEOUT_INTERVAL)
-        )
-
-        self.notification_center = notification_center or _notification_center.NotificationCenter(self.logger)
-        self._current_batch = list()
-
-        if not validator.is_notification_center_valid(self.notification_center):
-            self.logger.error(enums.Errors.INVALID_INPUT.format('notification_center'))
-            self.logger.debug('Creating notification center for use.')
-            self.notification_center = _notification_center.NotificationCenter(self.logger)
-
-        self.executor = None
-        if start_on_init is True:
-            self.start()
-
-    @property
-    def is_running(self):
-        """ Property to check if consumer thread is alive or not. """
-        return self.executor.is_alive() if self.executor else False
-
-    def _validate_instantiation_props(self, prop, prop_name, default_value):
-        """ Method to determine if instantiation properties like batch_size, flush_interval
-    and timeout_interval are valid.
-
-    Args:
-      prop: Property value that needs to be validated.
-      prop_name: Property name.
-      default_value: Default value for property.
-
-    Returns:
-      False if property value is None or less than or equal to 0 or not a finite number.
-      False if property name is batch_size and value is a floating point number.
-      True otherwise.
-    """
-        is_valid = True
-
-        if prop is None or not validator.is_finite_number(prop) or prop <= 0:
-            is_valid = False
-
-        if prop_name == 'batch_size' and not isinstance(prop, numbers.Integral):
-            is_valid = False
-
-        if is_valid is False:
-            self.logger.info('Using default value {} for {}.'.format(default_value, prop_name))
-
-        return is_valid
-
-    def _get_time(self, _time=None):
-        """ Method to return time as float in seconds. If _time is None, uses current time.
-
-    Args:
-      _time: time in seconds.
-
-    Returns:
-      Float time in seconds.
-    """
-        if _time is None:
-            return time.time()
-
-        return _time
-
-    def start(self):
-        """ Starts the batch processing thread to batch events. """
-        if hasattr(self, 'executor') and self.is_running:
-            self.logger.warning('BatchEventProcessor already started.')
-            return
-
-        self.flushing_interval_deadline = self._get_time() + self._get_time(self.flush_interval.total_seconds())
-        self.executor = threading.Thread(target=self._run)
-        self.executor.setDaemon(True)
-        self.executor.start()
-
-    def _run(self):
-        """ Triggered as part of the thread which batches events or flushes event_queue and hangs on get
-    for flush interval if queue is empty.
-    """
-        try:
-            while True:
-                loop_time = self._get_time()
-                loop_time_flush_interval = self._get_time(self.flush_interval.total_seconds())
-
-                if loop_time >= self.flushing_interval_deadline:
-                    self._flush_batch()
-                    self.flushing_interval_deadline = loop_time + loop_time_flush_interval
-                    self.logger.debug('Flush interval deadline. Flushed batch.')
-
-                try:
-                    interval = self.flushing_interval_deadline - loop_time
-                    item = self.event_queue.get(True, interval)
-
-                    if item is None:
-                        continue
-
-                except queue.Empty:
-                    continue
-
-                if item == self._SHUTDOWN_SIGNAL:
-                    self.logger.debug('Received shutdown signal.')
-                    break
-
-                if item == self._FLUSH_SIGNAL:
-                    self.logger.debug('Received flush signal.')
-                    self._flush_batch()
-                    continue
-
-                if isinstance(item, UserEvent):
-                    self._add_to_batch(item)
-
-        except Exception as exception:
-            self.logger.error('Uncaught exception processing buffer. Error: ' + str(exception))
-
-        finally:
-            self.logger.info('Exiting processing loop. Attempting to flush pending events.')
-            self._flush_batch()
-
-    def flush(self):
-        """ Adds flush signal to event_queue. """
-
-        self.event_queue.put(self._FLUSH_SIGNAL)
-
-    def _flush_batch(self):
-        """ Flushes current batch by dispatching event. """
-        batch_len = len(self._current_batch)
-        if batch_len == 0:
-            self.logger.debug('Nothing to flush.')
-            return
-
-        self.logger.debug('Flushing batch size ' + str(batch_len))
-
-        with self.LOCK:
-            to_process_batch = list(self._current_batch)
-            self._current_batch = list()
-
-        log_event = EventFactory.create_log_event(to_process_batch, self.logger)
-
-        self.notification_center.send_notifications(enums.NotificationTypes.LOG_EVENT, log_event)
-
-        try:
-            self.event_dispatcher.dispatch_event(log_event)
-        except Exception as e:
-            self.logger.error('Error dispatching event: ' + str(log_event) + ' ' + str(e))
-
-    def process(self, user_event):
-        """ Method to process the user_event by putting it in event_queue.
-
-    Args:
-      user_event: UserEvent Instance.
-    """
-        if not isinstance(user_event, UserEvent):
-            self.logger.error('Provided event is in an invalid format.')
-            return
-
-        self.logger.debug(
-            'Received event of type {} for user {}.'.format(type(user_event).__name__, user_event.user_id)
-        )
-
-        try:
-            self.event_queue.put_nowait(user_event)
-        except queue.Full:
-            self.logger.warning(
-                'Payload not accepted by the queue. Current size: {}'.format(str(self.event_queue.qsize()))
-            )
-
-    def _add_to_batch(self, user_event):
-        """ Method to append received user event to current batch.
-
-    Args:
-      user_event: UserEvent Instance.
-    """
-        if self._should_split(user_event):
-            self.logger.debug('Flushing batch on split.')
-            self._flush_batch()
-
-        # Reset the deadline if starting a new batch.
-        if len(self._current_batch) == 0:
-            self.flushing_interval_deadline = self._get_time() + self._get_time(self.flush_interval.total_seconds())
-
-        with self.LOCK:
-            self._current_batch.append(user_event)
-        if len(self._current_batch) >= self.batch_size:
-            self.logger.debug('Flushing on batch size.')
-            self._flush_batch()
-
-    def _should_split(self, user_event):
-        """ Method to check if current event batch should split into two.
-
-    Args:
-      user_event: UserEvent Instance.
-
-    Returns:
-      - True, if revision number and project_id of last event in current batch do not match received event's
-      revision number and project id respectively.
-      - False, otherwise.
-    """
-        if len(self._current_batch) == 0:
-            return False
-
-        current_context = self._current_batch[-1].event_context
-        new_context = user_event.event_context
-
-        if current_context.revision != new_context.revision:
-            return True
-
-        if current_context.project_id != new_context.project_id:
-            return True
-
-        return False
-
-    def stop(self):
-        """ Stops and disposes batch event processor. """
-        self.event_queue.put(self._SHUTDOWN_SIGNAL)
-        self.logger.warning('Stopping Scheduler.')
-
-        if self.executor:
-            self.executor.join(self.timeout_interval.total_seconds())
-
-        if self.is_running:
-            self.logger.error('Timeout exceeded while attempting to close for ' + str(self.timeout_interval) + ' ms.')
-
-
-class ForwardingEventProcessor(BaseEventProcessor):
-    """
-  ForwardingEventProcessor serves as the default EventProcessor.
-
-  The ForwardingEventProcessor sends the LogEvent to EventDispatcher as soon as it is received.
-  """
-
-    def __init__(self, event_dispatcher, logger=None, notification_center=None):
-        """ ForwardingEventProcessor init method to configure event dispatching.
-
-    Args:
-      event_dispatcher: Provides a dispatch_event method which if given a URL and params sends a request to it.
-      logger: Optional component which provides a log method to log messages. By default nothing would be logged.
-      notification_center: Optional instance of notification_center.NotificationCenter.
-    """
-        self.event_dispatcher = event_dispatcher or default_event_dispatcher
-        self.logger = _logging.adapt_logger(logger or _logging.NoOpLogger())
-        self.notification_center = notification_center or _notification_center.NotificationCenter(self.logger)
-
-        if not validator.is_notification_center_valid(self.notification_center):
-            self.logger.error(enums.Errors.INVALID_INPUT.format('notification_center'))
-            self.notification_center = _notification_center.NotificationCenter()
-
-    def process(self, user_event):
-        """ Method to process the user_event by dispatching it.
-
-    Args:
-      user_event: UserEvent Instance.
-    """
-        if not isinstance(user_event, UserEvent):
-            self.logger.error('Provided event is in an invalid format.')
-            return
-
-        self.logger.debug(
-            'Received event of type {} for user {}.'.format(type(user_event).__name__, user_event.user_id)
-        )
-
-        log_event = EventFactory.create_log_event(user_event, self.logger)
-
-        self.notification_center.send_notifications(enums.NotificationTypes.LOG_EVENT, log_event)
-
-        try:
-            self.event_dispatcher.dispatch_event(log_event)
-        except Exception as e:
-            self.logger.exception('Error dispatching event: ' + str(log_event) + ' ' + str(e))
+# Copyright 2019-2022, Optimizely
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from __future__ import annotations
+from abc import ABC, abstractmethod
+import numbers
+import threading
+import time
+
+from typing import Optional
+from datetime import timedelta
+import queue
+from sys import version_info
+
+from optimizely import logger as _logging
+from optimizely import notification_center as _notification_center
+from optimizely.event_dispatcher import EventDispatcher, CustomEventDispatcher
+from optimizely.helpers import enums
+from optimizely.helpers import validator
+from .event_factory import EventFactory
+from .user_event import UserEvent
+
+
+if version_info < (3, 8):
+    from typing_extensions import Final
+else:
+    from typing import Final  # type: ignore
+
+
+class BaseEventProcessor(ABC):
+    """ Class encapsulating event processing. Override with your own implementation. """
+
+    @abstractmethod
+    def process(self, user_event: UserEvent) -> None:
+        """ Method to provide intermediary processing stage within event production.
+    Args:
+      user_event: UserEvent instance that needs to be processed and dispatched.
+    """
+        pass
+
+
+class BatchEventProcessor(BaseEventProcessor):
+    """
+  BatchEventProcessor is an implementation of the BaseEventProcessor that batches events.
+
+  The BatchEventProcessor maintains a single consumer thread that pulls events off of
+  the blocking queue and buffers them for either a configured batch size or for a
+  maximum duration before the resulting LogEvent is sent to the EventDispatcher.
+  """
+
+    class Signal:
+        '''Used to create unique objects for sending signals to event queue.'''
+        pass
+
+    _DEFAULT_QUEUE_CAPACITY: Final = 1000
+    _DEFAULT_BATCH_SIZE: Final = 10
+    _DEFAULT_FLUSH_INTERVAL: Final = 30
+    _DEFAULT_TIMEOUT_INTERVAL: Final = 5
+    _SHUTDOWN_SIGNAL: Final = Signal()
+    _FLUSH_SIGNAL: Final = Signal()
+    LOCK: Final = threading.Lock()
+
+    def __init__(
+        self,
+        event_dispatcher: Optional[type[EventDispatcher] | CustomEventDispatcher] = None,
+        logger: Optional[_logging.Logger] = None,
+        start_on_init: bool = False,
+        event_queue: Optional[queue.Queue[UserEvent | Signal]] = None,
+        batch_size: Optional[int] = None,
+        flush_interval: Optional[float] = None,
+        timeout_interval: Optional[float] = None,
+        notification_center: Optional[_notification_center.NotificationCenter] = None,
+    ):
+        """ BatchEventProcessor init method to configure event batching.
+
+    Args:
+      event_dispatcher: Provides a dispatch_event method which if given a URL and params sends a request to it.
+      logger: Optional component which provides a log method to log messages. By default nothing would be logged.
+      start_on_init: Optional boolean param which starts the consumer thread if set to True.
+                     Default value is False.
+      event_queue: Optional component which accumulates the events until dispacthed.
+      batch_size: Optional param which defines the upper limit on the number of events in event_queue after which
+                  the event_queue will be flushed.
+      flush_interval: Optional floating point number representing time interval in seconds after which event_queue will
+                      be flushed.
+      timeout_interval: Optional floating point number representing time interval in seconds before joining the consumer
+                        thread.
+      notification_center: Optional instance of notification_center.NotificationCenter.
+    """
+        self.event_dispatcher = event_dispatcher or EventDispatcher
+        self.logger = _logging.adapt_logger(logger or _logging.NoOpLogger())
+        self.event_queue = event_queue or queue.Queue(maxsize=self._DEFAULT_QUEUE_CAPACITY)
+        self.batch_size: int = (
+            batch_size  # type: ignore[assignment]
+            if self._validate_instantiation_props(batch_size, 'batch_size', self._DEFAULT_BATCH_SIZE)
+            else self._DEFAULT_BATCH_SIZE
+        )
+        self.flush_interval: timedelta = (
+            timedelta(seconds=flush_interval)  # type: ignore[arg-type]
+            if self._validate_instantiation_props(flush_interval, 'flush_interval', self._DEFAULT_FLUSH_INTERVAL)
+            else timedelta(seconds=self._DEFAULT_FLUSH_INTERVAL)
+        )
+        self.timeout_interval: timedelta = (
+            timedelta(seconds=timeout_interval)  # type: ignore[arg-type]
+            if self._validate_instantiation_props(timeout_interval, 'timeout_interval', self._DEFAULT_TIMEOUT_INTERVAL)
+            else timedelta(seconds=self._DEFAULT_TIMEOUT_INTERVAL)
+        )
+
+        self.notification_center = notification_center or _notification_center.NotificationCenter(self.logger)
+        self._current_batch: list[UserEvent] = []
+
+        if not validator.is_notification_center_valid(self.notification_center):
+            self.logger.error(enums.Errors.INVALID_INPUT.format('notification_center'))
+            self.logger.debug('Creating notification center for use.')
+            self.notification_center = _notification_center.NotificationCenter(self.logger)
+
+        self.executor: Optional[threading.Thread] = None
+        if start_on_init is True:
+            self.start()
+
+    @property
+    def is_running(self) -> bool:
+        """ Property to check if consumer thread is alive or not. """
+        return self.executor.is_alive() if self.executor else False
+
+    def _validate_instantiation_props(
+        self,
+        prop: Optional[numbers.Integral | int | float],
+        prop_name: str,
+        default_value: numbers.Integral | int | float
+    ) -> bool:
+        """ Method to determine if instantiation properties like batch_size, flush_interval
+    and timeout_interval are valid.
+
+    Args:
+      prop: Property value that needs to be validated.
+      prop_name: Property name.
+      default_value: Default value for property.
+
+    Returns:
+      False if property value is None or less than or equal to 0 or not a finite number.
+      False if property name is batch_size and value is a floating point number.
+      True otherwise.
+    """
+        is_valid = True
+
+        if prop is None or not validator.is_finite_number(prop) or prop <= 0:
+            is_valid = False
+
+        if prop_name == 'batch_size' and not isinstance(prop, numbers.Integral):
+            is_valid = False
+
+        if is_valid is False:
+            self.logger.info(f'Using default value {default_value} for {prop_name}.')
+
+        return is_valid
+
+    def _get_time(self, _time: Optional[float] = None) -> float:
+        """ Method to return time as float in seconds. If _time is None, uses current time.
+
+    Args:
+      _time: time in seconds.
+
+    Returns:
+      Float time in seconds.
+    """
+        if _time is None:
+            return time.time()
+
+        return _time
+
+    def start(self) -> None:
+        """ Starts the batch processing thread to batch events. """
+        if hasattr(self, 'executor') and self.is_running:
+            self.logger.warning('BatchEventProcessor already started.')
+            return
+
+        self.flushing_interval_deadline = self._get_time() + self._get_time(self.flush_interval.total_seconds())
+        self.executor = threading.Thread(target=self._run)
+        self.executor.daemon = True
+        self.executor.start()
+
+    def _run(self) -> None:
+        """ Triggered as part of the thread which batches events or flushes event_queue and hangs on get
+    for flush interval if queue is empty.
+    """
+        try:
+            while True:
+                loop_time = self._get_time()
+                loop_time_flush_interval = self._get_time(self.flush_interval.total_seconds())
+
+                if loop_time >= self.flushing_interval_deadline:
+                    self._flush_batch()
+                    self.flushing_interval_deadline = loop_time + loop_time_flush_interval
+                    self.logger.debug('Flush interval deadline. Flushed batch.')
+
+                try:
+                    interval = self.flushing_interval_deadline - loop_time
+                    item = self.event_queue.get(True, interval)
+
+                    if item is None:
+                        continue
+
+                except queue.Empty:
+                    continue
+
+                if item == self._SHUTDOWN_SIGNAL:
+                    self.logger.debug('Received shutdown signal.')
+                    break
+
+                if item == self._FLUSH_SIGNAL:
+                    self.logger.debug('Received flush signal.')
+                    self._flush_batch()
+                    continue
+
+                if isinstance(item, UserEvent):
+                    self._add_to_batch(item)
+
+        except Exception as exception:
+            self.logger.error(f'Uncaught exception processing buffer. Error: {exception}')
+
+        finally:
+            self.logger.info('Exiting processing loop. Attempting to flush pending events.')
+            self._flush_batch()
+
+    def flush(self) -> None:
+        """ Adds flush signal to event_queue. """
+
+        self.event_queue.put(self._FLUSH_SIGNAL)
+
+    def _flush_batch(self) -> None:
+        """ Flushes current batch by dispatching event. """
+        batch_len = len(self._current_batch)
+        if batch_len == 0:
+            self.logger.debug('Nothing to flush.')
+            return
+
+        self.logger.debug(f'Flushing batch size {batch_len}')
+
+        with self.LOCK:
+            to_process_batch = list(self._current_batch)
+            self._current_batch = list()
+
+        log_event = EventFactory.create_log_event(to_process_batch, self.logger)
+
+        self.notification_center.send_notifications(enums.NotificationTypes.LOG_EVENT, log_event)
+
+        if log_event is None:
+            self.logger.exception('Error dispatching event: Cannot dispatch None event.')
+            return
+
+        try:
+            self.event_dispatcher.dispatch_event(log_event)
+        except Exception as e:
+            self.logger.error(f'Error dispatching event: {log_event} {e}')
+
+    def process(self, user_event: UserEvent) -> None:
+        """ Method to process the user_event by putting it in event_queue.
+
+    Args:
+      user_event: UserEvent Instance.
+    """
+        if not isinstance(user_event, UserEvent):
+            self.logger.error('Provided event is in an invalid format.')
+            return
+
+        self.logger.debug(
+            f'Received event of type {type(user_event).__name__} for user {user_event.user_id}.'
+        )
+
+        try:
+            self.event_queue.put_nowait(user_event)
+        except queue.Full:
+            self.logger.warning(
+                f'Payload not accepted by the queue. Current size: {self.event_queue.qsize()}'
+            )
+
+    def _add_to_batch(self, user_event: UserEvent) -> None:
+        """ Method to append received user event to current batch.
+
+    Args:
+      user_event: UserEvent Instance.
+    """
+        if self._should_split(user_event):
+            self.logger.debug('Flushing batch on split.')
+            self._flush_batch()
+
+        # Reset the deadline if starting a new batch.
+        if len(self._current_batch) == 0:
+            self.flushing_interval_deadline = self._get_time() + self._get_time(self.flush_interval.total_seconds())
+
+        with self.LOCK:
+            self._current_batch.append(user_event)
+        if len(self._current_batch) >= self.batch_size:
+            self.logger.debug('Flushing on batch size.')
+            self._flush_batch()
+
+    def _should_split(self, user_event: UserEvent) -> bool:
+        """ Method to check if current event batch should split into two.
+
+    Args:
+      user_event: UserEvent Instance.
+
+    Returns:
+      - True, if revision number and project_id of last event in current batch do not match received event's
+      revision number and project id respectively.
+      - False, otherwise.
+    """
+        if len(self._current_batch) == 0:
+            return False
+
+        current_context = self._current_batch[-1].event_context
+        new_context = user_event.event_context
+
+        if current_context.revision != new_context.revision:
+            return True
+
+        if current_context.project_id != new_context.project_id:
+            return True
+
+        return False
+
+    def stop(self) -> None:
+        """ Stops and disposes batch event processor. """
+        self.event_queue.put(self._SHUTDOWN_SIGNAL)
+        self.logger.warning('Stopping Scheduler.')
+
+        if self.executor:
+            self.executor.join(self.timeout_interval.total_seconds())
+
+        if self.is_running:
+            self.logger.error(f'Timeout exceeded while attempting to close for {self.timeout_interval} ms.')
+
+
+class ForwardingEventProcessor(BaseEventProcessor):
+    """
+  ForwardingEventProcessor serves as the default EventProcessor.
+
+  The ForwardingEventProcessor sends the LogEvent to EventDispatcher as soon as it is received.
+  """
+
+    def __init__(
+        self,
+        event_dispatcher: type[EventDispatcher] | CustomEventDispatcher,
+        logger: Optional[_logging.Logger] = None,
+        notification_center: Optional[_notification_center.NotificationCenter] = None
+    ):
+        """ ForwardingEventProcessor init method to configure event dispatching.
+
+    Args:
+      event_dispatcher: Provides a dispatch_event method which if given a URL and params sends a request to it.
+      logger: Optional component which provides a log method to log messages. By default nothing would be logged.
+      notification_center: Optional instance of notification_center.NotificationCenter.
+    """
+        self.event_dispatcher = event_dispatcher or EventDispatcher
+        self.logger = _logging.adapt_logger(logger or _logging.NoOpLogger())
+        self.notification_center = notification_center or _notification_center.NotificationCenter(self.logger)
+
+        if not validator.is_notification_center_valid(self.notification_center):
+            self.logger.error(enums.Errors.INVALID_INPUT.format('notification_center'))
+            self.notification_center = _notification_center.NotificationCenter()
+
+    def process(self, user_event: UserEvent) -> None:
+        """ Method to process the user_event by dispatching it.
+
+    Args:
+      user_event: UserEvent Instance.
+    """
+        if not isinstance(user_event, UserEvent):
+            self.logger.error('Provided event is in an invalid format.')
+            return
+
+        self.logger.debug(
+            f'Received event of type {type(user_event).__name__} for user {user_event.user_id}.'
+        )
+
+        log_event = EventFactory.create_log_event(user_event, self.logger)
+
+        self.notification_center.send_notifications(enums.NotificationTypes.LOG_EVENT, log_event)
+
+        if log_event is None:
+            self.logger.exception('Error dispatching event: Cannot dispatch None event.')
+            return
+
+        try:
+            self.event_dispatcher.dispatch_event(log_event)
+        except Exception as e:
+            self.logger.exception(f'Error dispatching event: {log_event} {e}')
```

### Comparing `optimizely-sdk-4.1.1/optimizely/event/payload.py` & `optimizely-sdk-5.0.0b0/optimizely/event/payload.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,119 +1,138 @@
-# Copyright 2019 Optimizely
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import json
-
-
-class EventBatch(object):
-    """ Class respresenting Event Batch. """
-
-    def __init__(
-        self,
-        account_id,
-        project_id,
-        revision,
-        client_name,
-        client_version,
-        anonymize_ip,
-        enrich_decisions=True,
-        visitors=None,
-    ):
-        self.account_id = account_id
-        self.project_id = project_id
-        self.revision = revision
-        self.client_name = client_name
-        self.client_version = client_version
-        self.anonymize_ip = anonymize_ip
-        self.enrich_decisions = enrich_decisions
-        self.visitors = visitors or []
-
-    def __eq__(self, other):
-        batch_obj = self.get_event_params()
-        return batch_obj == other
-
-    def _dict_clean(self, obj):
-        """ Helper method to remove keys from dictionary with None values. """
-
-        result = {}
-        for k, v in obj:
-            if v is None and k in ['revenue', 'value', 'tags', 'decisions']:
-                continue
-            else:
-                result[k] = v
-        return result
-
-    def get_event_params(self):
-        """ Method to return valid params for LogEvent payload. """
-
-        return json.loads(json.dumps(self.__dict__, default=lambda o: o.__dict__), object_pairs_hook=self._dict_clean,)
-
-
-class Decision(object):
-    """ Class respresenting Decision. """
-
-    def __init__(self, campaign_id, experiment_id, variation_id, metadata):
-        self.campaign_id = campaign_id
-        self.experiment_id = experiment_id
-        self.variation_id = variation_id
-        self.metadata = metadata
-
-
-class Metadata(object):
-    """ Class respresenting Metadata. """
-
-    def __init__(self, flag_key, rule_key, rule_type, variation_key, enabled):
-        self.flag_key = flag_key
-        self.rule_key = rule_key
-        self.rule_type = rule_type
-        self.variation_key = variation_key
-        self.enabled = enabled
-
-
-class Snapshot(object):
-    """ Class representing Snapshot. """
-
-    def __init__(self, events, decisions=None):
-        self.events = events
-        self.decisions = decisions
-
-
-class SnapshotEvent(object):
-    """ Class representing Snapshot Event. """
-
-    def __init__(self, entity_id, uuid, key, timestamp, revenue=None, value=None, tags=None):
-        self.entity_id = entity_id
-        self.uuid = uuid
-        self.key = key
-        self.timestamp = timestamp
-        self.revenue = revenue
-        self.value = value
-        self.tags = tags
-
-
-class Visitor(object):
-    """ Class representing Visitor. """
-
-    def __init__(self, snapshots, attributes, visitor_id):
-        self.snapshots = snapshots
-        self.attributes = attributes
-        self.visitor_id = visitor_id
-
-
-class VisitorAttribute(object):
-    """ Class representing Visitor Attribute. """
-
-    def __init__(self, entity_id, key, attribute_type, value):
-        self.entity_id = entity_id
-        self.key = key
-        self.type = attribute_type
-        self.value = value
+# Copyright 2019, 2022, Optimizely
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from __future__ import annotations
+import json
+from numbers import Integral
+from typing import TYPE_CHECKING, Any, Optional
+
+
+if TYPE_CHECKING:
+    from optimizely.helpers.event_tag_utils import EventTags
+
+
+class EventBatch:
+    """ Class respresenting Event Batch. """
+
+    def __init__(
+        self,
+        account_id: str,
+        project_id: str,
+        revision: str,
+        client_name: str,
+        client_version: str,
+        anonymize_ip: bool,
+        enrich_decisions: bool = True,
+        visitors: Optional[list[Visitor]] = None,
+    ):
+        self.account_id = account_id
+        self.project_id = project_id
+        self.revision = revision
+        self.client_name = client_name
+        self.client_version = client_version
+        self.anonymize_ip = anonymize_ip
+        self.enrich_decisions = enrich_decisions
+        self.visitors = visitors or []
+
+    def __eq__(self, other: object) -> bool:
+        batch_obj = self.get_event_params()
+        return batch_obj == other
+
+    def _dict_clean(self, obj: list[tuple[str, Any]]) -> dict[str, Any]:
+        """ Helper method to remove keys from dictionary with None values. """
+
+        result = {}
+        for k, v in obj:
+            if v is None and k in ['revenue', 'value', 'tags', 'decisions']:
+                continue
+            else:
+                result[k] = v
+        return result
+
+    def get_event_params(self) -> dict[str, Any]:
+        """ Method to return valid params for LogEvent payload. """
+
+        return json.loads(  # type: ignore[no-any-return]
+            json.dumps(self.__dict__, default=lambda o: o.__dict__),
+            object_pairs_hook=self._dict_clean,
+        )
+
+
+class Decision:
+    """ Class respresenting Decision. """
+
+    def __init__(self, campaign_id: str, experiment_id: str, variation_id: str, metadata: Metadata):
+        self.campaign_id = campaign_id
+        self.experiment_id = experiment_id
+        self.variation_id = variation_id
+        self.metadata = metadata
+
+
+class Metadata:
+    """ Class respresenting Metadata. """
+
+    def __init__(self, flag_key: str, rule_key: str, rule_type: str, variation_key: str, enabled: bool):
+        self.flag_key = flag_key
+        self.rule_key = rule_key
+        self.rule_type = rule_type
+        self.variation_key = variation_key
+        self.enabled = enabled
+
+
+class Snapshot:
+    """ Class representing Snapshot. """
+
+    def __init__(self, events: list[SnapshotEvent], decisions: Optional[list[Decision]] = None):
+        self.events = events
+        self.decisions = decisions
+
+
+class SnapshotEvent:
+    """ Class representing Snapshot Event. """
+
+    def __init__(
+        self,
+        entity_id: str,
+        uuid: str,
+        key: str,
+        timestamp: int,
+        revenue: Optional[Integral] = None,
+        value: Any = None,
+        tags: Optional[EventTags] = None
+    ):
+        self.entity_id = entity_id
+        self.uuid = uuid
+        self.key = key
+        self.timestamp = timestamp
+        self.revenue = revenue
+        self.value = value
+        self.tags = tags
+
+
+class Visitor:
+    """ Class representing Visitor. """
+
+    def __init__(self, snapshots: list[Snapshot], attributes: list[VisitorAttribute], visitor_id: str):
+        self.snapshots = snapshots
+        self.attributes = attributes
+        self.visitor_id = visitor_id
+
+
+class VisitorAttribute:
+    """ Class representing Visitor Attribute. """
+
+    def __init__(self, entity_id: str, key: str, attribute_type: str, value: Any):
+        self.entity_id = entity_id
+        self.key = key
+        self.type = attribute_type
+        self.value = value
```

### Comparing `optimizely-sdk-4.1.1/optimizely/event_builder.py` & `optimizely-sdk-5.0.0b0/optimizely/event_builder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,257 +1,292 @@
-# Copyright 2016-2019, Optimizely
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import time
-import uuid
-
-from . import version
-from .helpers import enums
-from .helpers import event_tag_utils
-from .helpers import validator
-
-
-class Event(object):
-    """ Representation of an event which can be sent to the Optimizely logging endpoint. """
-
-    def __init__(self, url, params, http_verb=None, headers=None):
-        self.url = url
-        self.params = params
-        self.http_verb = http_verb or 'GET'
-        self.headers = headers
-
-
-class EventBuilder(object):
-    """ Class which encapsulates methods to build events for tracking
-  impressions and conversions using the new V3 event API (batch). """
-
-    EVENTS_URL = 'https://logx.optimizely.com/v1/events'
-    HTTP_VERB = 'POST'
-    HTTP_HEADERS = {'Content-Type': 'application/json'}
-
-    class EventParams(object):
-        ACCOUNT_ID = 'account_id'
-        PROJECT_ID = 'project_id'
-        EXPERIMENT_ID = 'experiment_id'
-        CAMPAIGN_ID = 'campaign_id'
-        VARIATION_ID = 'variation_id'
-        END_USER_ID = 'visitor_id'
-        ENRICH_DECISIONS = 'enrich_decisions'
-        EVENTS = 'events'
-        EVENT_ID = 'entity_id'
-        ATTRIBUTES = 'attributes'
-        DECISIONS = 'decisions'
-        TIME = 'timestamp'
-        KEY = 'key'
-        TAGS = 'tags'
-        UUID = 'uuid'
-        USERS = 'visitors'
-        SNAPSHOTS = 'snapshots'
-        SOURCE_SDK_TYPE = 'client_name'
-        SOURCE_SDK_VERSION = 'client_version'
-        CUSTOM = 'custom'
-        ANONYMIZE_IP = 'anonymize_ip'
-        REVISION = 'revision'
-
-    def _get_attributes_data(self, project_config, attributes):
-        """ Get attribute(s) information.
-
-    Args:
-      project_config: Instance of ProjectConfig.
-      attributes: Dict representing user attributes and values which need to be recorded.
-
-    Returns:
-      List consisting of valid attributes for the user. Empty otherwise.
-    """
-
-        params = []
-
-        if isinstance(attributes, dict):
-            for attribute_key in attributes.keys():
-                attribute_value = attributes.get(attribute_key)
-                # Omit attribute values that are not supported by the log endpoint.
-                if validator.is_attribute_valid(attribute_key, attribute_value):
-                    attribute_id = project_config.get_attribute_id(attribute_key)
-                    if attribute_id:
-                        params.append(
-                            {
-                                'entity_id': attribute_id,
-                                'key': attribute_key,
-                                'type': self.EventParams.CUSTOM,
-                                'value': attribute_value,
-                            }
-                        )
-
-        # Append Bot Filtering Attribute
-        bot_filtering_value = project_config.get_bot_filtering_value()
-        if isinstance(bot_filtering_value, bool):
-            params.append(
-                {
-                    'entity_id': enums.ControlAttributes.BOT_FILTERING,
-                    'key': enums.ControlAttributes.BOT_FILTERING,
-                    'type': self.EventParams.CUSTOM,
-                    'value': bot_filtering_value,
-                }
-            )
-
-        return params
-
-    def _get_time(self):
-        """ Get time in milliseconds to be added.
-
-    Returns:
-      int Current time in milliseconds.
-    """
-
-        return int(round(time.time() * 1000))
-
-    def _get_common_params(self, project_config, user_id, attributes):
-        """ Get params which are used same in both conversion and impression events.
-
-    Args:
-      project_config: Instance of ProjectConfig.
-      user_id: ID for user.
-      attributes: Dict representing user attributes and values which need to be recorded.
-
-    Returns:
-     Dict consisting of parameters common to both impression and conversion events.
-    """
-        common_params = {
-            self.EventParams.PROJECT_ID: project_config.get_project_id(),
-            self.EventParams.ACCOUNT_ID: project_config.get_account_id(),
-        }
-
-        visitor = {
-            self.EventParams.END_USER_ID: user_id,
-            self.EventParams.SNAPSHOTS: [],
-        }
-
-        common_params[self.EventParams.USERS] = []
-        common_params[self.EventParams.USERS].append(visitor)
-        common_params[self.EventParams.USERS][0][self.EventParams.ATTRIBUTES] = self._get_attributes_data(
-            project_config, attributes
-        )
-
-        common_params[self.EventParams.SOURCE_SDK_TYPE] = 'python-sdk'
-        common_params[self.EventParams.ENRICH_DECISIONS] = True
-        common_params[self.EventParams.SOURCE_SDK_VERSION] = version.__version__
-        common_params[self.EventParams.ANONYMIZE_IP] = project_config.get_anonymize_ip_value()
-        common_params[self.EventParams.REVISION] = project_config.get_revision()
-
-        return common_params
-
-    def _get_required_params_for_impression(self, experiment, variation_id):
-        """ Get parameters that are required for the impression event to register.
-
-    Args:
-      experiment: Experiment for which impression needs to be recorded.
-      variation_id: ID for variation which would be presented to user.
-
-    Returns:
-      Dict consisting of decisions and events info for impression event.
-    """
-        snapshot = {}
-
-        snapshot[self.EventParams.DECISIONS] = [
-            {
-                self.EventParams.EXPERIMENT_ID: experiment.id,
-                self.EventParams.VARIATION_ID: variation_id,
-                self.EventParams.CAMPAIGN_ID: experiment.layerId,
-            }
-        ]
-
-        snapshot[self.EventParams.EVENTS] = [
-            {
-                self.EventParams.EVENT_ID: experiment.layerId,
-                self.EventParams.TIME: self._get_time(),
-                self.EventParams.KEY: 'campaign_activated',
-                self.EventParams.UUID: str(uuid.uuid4()),
-            }
-        ]
-
-        return snapshot
-
-    def _get_required_params_for_conversion(self, project_config, event_key, event_tags):
-        """ Get parameters that are required for the conversion event to register.
-
-    Args:
-      project_config: Instance of ProjectConfig.
-      event_key: Key representing the event which needs to be recorded.
-      event_tags: Dict representing metadata associated with the event.
-
-    Returns:
-      Dict consisting of the decisions and events info for conversion event.
-    """
-        snapshot = {}
-
-        event_dict = {
-            self.EventParams.EVENT_ID: project_config.get_event(event_key).id,
-            self.EventParams.TIME: self._get_time(),
-            self.EventParams.KEY: event_key,
-            self.EventParams.UUID: str(uuid.uuid4()),
-        }
-
-        if event_tags:
-            revenue_value = event_tag_utils.get_revenue_value(event_tags)
-            if revenue_value is not None:
-                event_dict[event_tag_utils.REVENUE_METRIC_TYPE] = revenue_value
-
-            numeric_value = event_tag_utils.get_numeric_value(event_tags, project_config.logger)
-            if numeric_value is not None:
-                event_dict[event_tag_utils.NUMERIC_METRIC_TYPE] = numeric_value
-
-            if len(event_tags) > 0:
-                event_dict[self.EventParams.TAGS] = event_tags
-
-        snapshot[self.EventParams.EVENTS] = [event_dict]
-        return snapshot
-
-    def create_impression_event(self, project_config, experiment, variation_id, user_id, attributes):
-        """ Create impression Event to be sent to the logging endpoint.
-
-    Args:
-      project_config: Instance of ProjectConfig.
-      experiment: Experiment for which impression needs to be recorded.
-      variation_id: ID for variation which would be presented to user.
-      user_id: ID for user.
-      attributes: Dict representing user attributes and values which need to be recorded.
-
-    Returns:
-      Event object encapsulating the impression event.
-    """
-
-        params = self._get_common_params(project_config, user_id, attributes)
-        impression_params = self._get_required_params_for_impression(experiment, variation_id)
-
-        params[self.EventParams.USERS][0][self.EventParams.SNAPSHOTS].append(impression_params)
-
-        return Event(self.EVENTS_URL, params, http_verb=self.HTTP_VERB, headers=self.HTTP_HEADERS)
-
-    def create_conversion_event(self, project_config, event_key, user_id, attributes, event_tags):
-        """ Create conversion Event to be sent to the logging endpoint.
-
-    Args:
-      project_config: Instance of ProjectConfig.
-      event_key: Key representing the event which needs to be recorded.
-      user_id: ID for user.
-      attributes: Dict representing user attributes and values.
-      event_tags: Dict representing metadata associated with the event.
-
-    Returns:
-      Event object encapsulating the conversion event.
-    """
-
-        params = self._get_common_params(project_config, user_id, attributes)
-        conversion_params = self._get_required_params_for_conversion(project_config, event_key, event_tags)
-
-        params[self.EventParams.USERS][0][self.EventParams.SNAPSHOTS].append(conversion_params)
-        return Event(self.EVENTS_URL, params, http_verb=self.HTTP_VERB, headers=self.HTTP_HEADERS)
+# Copyright 2016-2019, 2022, Optimizely
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from __future__ import annotations
+import time
+from typing import TYPE_CHECKING, Any, Optional
+import uuid
+from sys import version_info
+
+from . import version
+from .helpers import enums
+from .helpers import event_tag_utils
+from .helpers import validator
+
+if version_info < (3, 8):
+    from typing_extensions import Final, Literal
+else:
+    from typing import Final, Literal  # type: ignore
+
+if TYPE_CHECKING:
+    # prevent circular dependenacy by skipping import at runtime
+    from .entities import Experiment
+    from .optimizely_user_context import UserAttributes
+    from .project_config import ProjectConfig
+
+
+class Event:
+    """ Representation of an event which can be sent to the Optimizely logging endpoint. """
+
+    def __init__(
+        self,
+        url: str,
+        params: dict[str, Any],
+        http_verb: Optional[Literal['POST', 'GET']] = None,
+        headers: Optional[dict[str, str]] = None
+    ):
+        self.url = url
+        self.params = params
+        self.http_verb = http_verb or 'GET'
+        self.headers = headers
+
+
+class EventBuilder:
+    """ Class which encapsulates methods to build events for tracking
+  impressions and conversions using the new V3 event API (batch). """
+
+    EVENTS_URL: Final = 'https://logx.optimizely.com/v1/events'
+    HTTP_VERB: Final = 'POST'
+    HTTP_HEADERS: Final = {'Content-Type': 'application/json'}
+
+    class EventParams:
+        ACCOUNT_ID: Final = 'account_id'
+        PROJECT_ID: Final = 'project_id'
+        EXPERIMENT_ID: Final = 'experiment_id'
+        CAMPAIGN_ID: Final = 'campaign_id'
+        VARIATION_ID: Final = 'variation_id'
+        END_USER_ID: Final = 'visitor_id'
+        ENRICH_DECISIONS: Final = 'enrich_decisions'
+        EVENTS: Final = 'events'
+        EVENT_ID: Final = 'entity_id'
+        ATTRIBUTES: Final = 'attributes'
+        DECISIONS: Final = 'decisions'
+        TIME: Final = 'timestamp'
+        KEY: Final = 'key'
+        TAGS: Final = 'tags'
+        UUID: Final = 'uuid'
+        USERS: Final = 'visitors'
+        SNAPSHOTS: Final = 'snapshots'
+        SOURCE_SDK_TYPE: Final = 'client_name'
+        SOURCE_SDK_VERSION: Final = 'client_version'
+        CUSTOM: Final = 'custom'
+        ANONYMIZE_IP: Final = 'anonymize_ip'
+        REVISION: Final = 'revision'
+
+    def _get_attributes_data(
+        self, project_config: ProjectConfig, attributes: UserAttributes
+    ) -> list[dict[str, Any]]:
+        """ Get attribute(s) information.
+
+    Args:
+      project_config: Instance of ProjectConfig.
+      attributes: Dict representing user attributes and values which need to be recorded.
+
+    Returns:
+      List consisting of valid attributes for the user. Empty otherwise.
+    """
+
+        params = []
+
+        if isinstance(attributes, dict):
+            for attribute_key in attributes.keys():
+                attribute_value = attributes.get(attribute_key)
+                # Omit attribute values that are not supported by the log endpoint.
+                if validator.is_attribute_valid(attribute_key, attribute_value):
+                    attribute_id = project_config.get_attribute_id(attribute_key)
+                    if attribute_id:
+                        params.append(
+                            {
+                                'entity_id': attribute_id,
+                                'key': attribute_key,
+                                'type': self.EventParams.CUSTOM,
+                                'value': attribute_value,
+                            }
+                        )
+
+        # Append Bot Filtering Attribute
+        bot_filtering_value = project_config.get_bot_filtering_value()
+        if isinstance(bot_filtering_value, bool):
+            params.append(
+                {
+                    'entity_id': enums.ControlAttributes.BOT_FILTERING,
+                    'key': enums.ControlAttributes.BOT_FILTERING,
+                    'type': self.EventParams.CUSTOM,
+                    'value': bot_filtering_value,
+                }
+            )
+
+        return params
+
+    def _get_time(self) -> int:
+        """ Get time in milliseconds to be added.
+
+    Returns:
+      int Current time in milliseconds.
+    """
+
+        return int(round(time.time() * 1000))
+
+    def _get_common_params(
+        self, project_config: ProjectConfig, user_id: str, attributes: UserAttributes
+    ) -> dict[str, Any]:
+        """ Get params which are used same in both conversion and impression events.
+
+    Args:
+      project_config: Instance of ProjectConfig.
+      user_id: ID for user.
+      attributes: Dict representing user attributes and values which need to be recorded.
+
+    Returns:
+     Dict consisting of parameters common to both impression and conversion events.
+    """
+        common_params: dict[str, Any] = {
+            self.EventParams.PROJECT_ID: project_config.get_project_id(),
+            self.EventParams.ACCOUNT_ID: project_config.get_account_id(),
+        }
+
+        visitor = {
+            self.EventParams.END_USER_ID: user_id,
+            self.EventParams.SNAPSHOTS: [],
+        }
+
+        common_params[self.EventParams.USERS] = []
+        common_params[self.EventParams.USERS].append(visitor)
+        common_params[self.EventParams.USERS][0][self.EventParams.ATTRIBUTES] = self._get_attributes_data(
+            project_config, attributes
+        )
+
+        common_params[self.EventParams.SOURCE_SDK_TYPE] = 'python-sdk'
+        common_params[self.EventParams.ENRICH_DECISIONS] = True
+        common_params[self.EventParams.SOURCE_SDK_VERSION] = version.__version__
+        common_params[self.EventParams.ANONYMIZE_IP] = project_config.get_anonymize_ip_value()
+        common_params[self.EventParams.REVISION] = project_config.get_revision()
+
+        return common_params
+
+    def _get_required_params_for_impression(
+        self, experiment: Experiment, variation_id: str
+    ) -> dict[str, list[dict[str, str | int]]]:
+        """ Get parameters that are required for the impression event to register.
+
+    Args:
+      experiment: Experiment for which impression needs to be recorded.
+      variation_id: ID for variation which would be presented to user.
+
+    Returns:
+      Dict consisting of decisions and events info for impression event.
+    """
+        snapshot: dict[str, list[dict[str, str | int]]] = {}
+
+        snapshot[self.EventParams.DECISIONS] = [
+            {
+                self.EventParams.EXPERIMENT_ID: experiment.id,
+                self.EventParams.VARIATION_ID: variation_id,
+                self.EventParams.CAMPAIGN_ID: experiment.layerId,
+            }
+        ]
+
+        snapshot[self.EventParams.EVENTS] = [
+            {
+                self.EventParams.EVENT_ID: experiment.layerId,
+                self.EventParams.TIME: self._get_time(),
+                self.EventParams.KEY: 'campaign_activated',
+                self.EventParams.UUID: str(uuid.uuid4()),
+            }
+        ]
+
+        return snapshot
+
+    def _get_required_params_for_conversion(
+        self, project_config: ProjectConfig, event_key: str, event_tags: event_tag_utils.EventTags
+    ) -> dict[str, list[dict[str, Any]]]:
+        """ Get parameters that are required for the conversion event to register.
+
+    Args:
+      project_config: Instance of ProjectConfig.
+      event_key: Key representing the event which needs to be recorded.
+      event_tags: Dict representing metadata associated with the event.
+
+    Returns:
+      Dict consisting of the decisions and events info for conversion event.
+    """
+        snapshot = {}
+        event = project_config.get_event(event_key)
+
+        event_dict: dict[str, Any] = {
+            self.EventParams.EVENT_ID: event.id if event else None,
+            self.EventParams.TIME: self._get_time(),
+            self.EventParams.KEY: event_key,
+            self.EventParams.UUID: str(uuid.uuid4()),
+        }
+
+        if event_tags:
+            revenue_value = event_tag_utils.get_revenue_value(event_tags)
+            if revenue_value is not None:
+                event_dict[event_tag_utils.REVENUE_METRIC_TYPE] = revenue_value
+
+            numeric_value = event_tag_utils.get_numeric_value(event_tags, project_config.logger)
+            if numeric_value is not None:
+                event_dict[event_tag_utils.NUMERIC_METRIC_TYPE] = numeric_value
+
+            if len(event_tags) > 0:
+                event_dict[self.EventParams.TAGS] = event_tags
+
+        snapshot[self.EventParams.EVENTS] = [event_dict]
+        return snapshot
+
+    def create_impression_event(
+        self, project_config: ProjectConfig, experiment: Experiment,
+        variation_id: str, user_id: str, attributes: UserAttributes
+    ) -> Event:
+        """ Create impression Event to be sent to the logging endpoint.
+
+    Args:
+      project_config: Instance of ProjectConfig.
+      experiment: Experiment for which impression needs to be recorded.
+      variation_id: ID for variation which would be presented to user.
+      user_id: ID for user.
+      attributes: Dict representing user attributes and values which need to be recorded.
+
+    Returns:
+      Event object encapsulating the impression event.
+    """
+
+        params = self._get_common_params(project_config, user_id, attributes)
+        impression_params = self._get_required_params_for_impression(experiment, variation_id)
+
+        params[self.EventParams.USERS][0][self.EventParams.SNAPSHOTS].append(impression_params)
+
+        return Event(self.EVENTS_URL, params, http_verb=self.HTTP_VERB, headers=self.HTTP_HEADERS)
+
+    def create_conversion_event(
+        self, project_config: ProjectConfig, event_key: str,
+        user_id: str, attributes: UserAttributes, event_tags: event_tag_utils.EventTags
+    ) -> Event:
+        """ Create conversion Event to be sent to the logging endpoint.
+
+    Args:
+      project_config: Instance of ProjectConfig.
+      event_key: Key representing the event which needs to be recorded.
+      user_id: ID for user.
+      attributes: Dict representing user attributes and values.
+      event_tags: Dict representing metadata associated with the event.
+
+    Returns:
+      Event object encapsulating the conversion event.
+    """
+
+        params = self._get_common_params(project_config, user_id, attributes)
+        conversion_params = self._get_required_params_for_conversion(project_config, event_key, event_tags)
+
+        params[self.EventParams.USERS][0][self.EventParams.SNAPSHOTS].append(conversion_params)
+        return Event(self.EVENTS_URL, params, http_verb=self.HTTP_VERB, headers=self.HTTP_HEADERS)
```

### Comparing `optimizely-sdk-4.1.1/optimizely/exceptions.py` & `optimizely-sdk-5.0.0b0/optimizely/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,7 +60,25 @@
     pass
 
 
 class UnsupportedDatafileVersionException(Exception):
     """ Raised when provided version in datafile is not supported. """
 
     pass
+
+
+class OdpNotEnabled(Exception):
+    """ Raised when Optimizely Data Platform (ODP) is not enabled. """
+
+    pass
+
+
+class OdpNotIntegrated(Exception):
+    """ Raised when Optimizely Data Platform (ODP) is not integrated. """
+
+    pass
+
+
+class OdpInvalidData(Exception):
+    """ Raised when passing invalid ODP data. """
+
+    pass
```

### Comparing `optimizely-sdk-4.1.1/optimizely/helpers/__init__.py` & `optimizely-sdk-5.0.0b0/optimizely/lib/__init__.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2016, Optimizely
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# Copyright 2016, Optimizely
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
```

### Comparing `optimizely-sdk-4.1.1/optimizely/helpers/audience.py` & `optimizely-sdk-5.0.0b0/optimizely/helpers/audience.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,88 +1,98 @@
-# Copyright 2016, 2018-2021, Optimizely
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import json
-
-from . import condition as condition_helper
-from . import condition_tree_evaluator
-
-
-def does_user_meet_audience_conditions(config,
-                                       audience_conditions,
-                                       audience_logs,
-                                       logging_key,
-                                       attributes,
-                                       logger):
-    """ Determine for given experiment if user satisfies the audiences for the experiment.
-
-    Args:
-        config: project_config.ProjectConfig object representing the project.
-        audience_conditions: Audience conditions corresponding to the experiment or rollout rule.
-        audience_logs: Log class capturing the messages to be logged .
-        logging_key: String representing experiment key or rollout rule. To be used in log messages only.
-        attributes: Dict representing user attributes which will be used in determining
-                    if the audience conditions are met. If not provided, default to an empty dict.
-        logger: Provides a logger to send log messages to.
-
-    Returns:
-        Boolean representing if user satisfies audience conditions for any of the audiences or not
-        And an array of log messages representing decision making.
-    """
-    decide_reasons = []
-    message = audience_logs.EVALUATING_AUDIENCES_COMBINED.format(logging_key, json.dumps(audience_conditions))
-    logger.debug(message)
-    decide_reasons.append(message)
-
-    # Return True in case there are no audiences
-    if audience_conditions is None or audience_conditions == []:
-        message = audience_logs.AUDIENCE_EVALUATION_RESULT_COMBINED.format(logging_key, 'TRUE')
-        logger.info(message)
-        decide_reasons.append(message)
-
-        return True, decide_reasons
-
-    if attributes is None:
-        attributes = {}
-
-    def evaluate_custom_attr(audience_id, index):
-        audience = config.get_audience(audience_id)
-        custom_attr_condition_evaluator = condition_helper.CustomAttributeConditionEvaluator(
-            audience.conditionList, attributes, logger
-        )
-
-        return custom_attr_condition_evaluator.evaluate(index)
-
-    def evaluate_audience(audience_id):
-        audience = config.get_audience(audience_id)
-
-        if audience is None:
-            return None
-        _message = audience_logs.EVALUATING_AUDIENCE.format(audience_id, audience.conditions)
-        logger.debug(_message)
-
-        result = condition_tree_evaluator.evaluate(
-            audience.conditionStructure, lambda index: evaluate_custom_attr(audience_id, index),
-        )
-
-        result_str = str(result).upper() if result is not None else 'UNKNOWN'
-        _message = audience_logs.AUDIENCE_EVALUATION_RESULT.format(audience_id, result_str)
-        logger.debug(_message)
-
-        return result
-
-    eval_result = condition_tree_evaluator.evaluate(audience_conditions, evaluate_audience)
-    eval_result = eval_result or False
-    message = audience_logs.AUDIENCE_EVALUATION_RESULT_COMBINED.format(logging_key, str(eval_result).upper())
-    logger.info(message)
-    decide_reasons.append(message)
-    return eval_result, decide_reasons
+# Copyright 2016, 2018-2022, Optimizely
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from __future__ import annotations
+import json
+from typing import TYPE_CHECKING, Optional, Sequence, Type
+
+from . import condition as condition_helper
+from . import condition_tree_evaluator
+from optimizely import optimizely_user_context
+
+if TYPE_CHECKING:
+    # prevent circular dependenacy by skipping import at runtime
+    from optimizely.project_config import ProjectConfig
+    from optimizely.logger import Logger
+    from optimizely.helpers.enums import ExperimentAudienceEvaluationLogs, RolloutRuleAudienceEvaluationLogs
+
+
+def does_user_meet_audience_conditions(
+    config: ProjectConfig,
+    audience_conditions: Optional[Sequence[str | list[str]]],
+    audience_logs: Type[ExperimentAudienceEvaluationLogs | RolloutRuleAudienceEvaluationLogs],
+    logging_key: str,
+    user_context: optimizely_user_context.OptimizelyUserContext,
+    logger: Logger
+) -> tuple[bool, list[str]]:
+    """ Determine for given experiment if user satisfies the audiences for the experiment.
+
+    Args:
+        config: project_config.ProjectConfig object representing the project.
+        audience_conditions: Audience conditions corresponding to the experiment or rollout rule.
+        audience_logs: Log class capturing the messages to be logged .
+        logging_key: String representing experiment key or rollout rule. To be used in log messages only.
+        attributes: Dict representing user attributes which will be used in determining
+                    if the audience conditions are met. If not provided, default to an empty dict.
+        logger: Provides a logger to send log messages to.
+
+    Returns:
+        Boolean representing if user satisfies audience conditions for any of the audiences or not
+        And an array of log messages representing decision making.
+    """
+    decide_reasons = []
+    message = audience_logs.EVALUATING_AUDIENCES_COMBINED.format(logging_key, json.dumps(audience_conditions))
+    logger.debug(message)
+    decide_reasons.append(message)
+
+    # Return True in case there are no audiences
+    if audience_conditions is None or audience_conditions == []:
+        message = audience_logs.AUDIENCE_EVALUATION_RESULT_COMBINED.format(logging_key, 'TRUE')
+        logger.info(message)
+        decide_reasons.append(message)
+
+        return True, decide_reasons
+
+    def evaluate_custom_attr(audience_id: str, index: int) -> Optional[bool]:
+        audience = config.get_audience(audience_id)
+        if not audience or audience.conditionList is None:
+            return None
+        custom_attr_condition_evaluator = condition_helper.CustomAttributeConditionEvaluator(
+            audience.conditionList, user_context, logger
+        )
+
+        return custom_attr_condition_evaluator.evaluate(index)
+
+    def evaluate_audience(audience_id: str) -> Optional[bool]:
+        audience = config.get_audience(audience_id)
+
+        if audience is None:
+            return None
+        _message = audience_logs.EVALUATING_AUDIENCE.format(audience_id, audience.conditions)
+        logger.debug(_message)
+
+        result = condition_tree_evaluator.evaluate(
+            audience.conditionStructure, lambda index: evaluate_custom_attr(audience_id, index),
+        )
+
+        result_str = str(result).upper() if result is not None else 'UNKNOWN'
+        _message = audience_logs.AUDIENCE_EVALUATION_RESULT.format(audience_id, result_str)
+        logger.debug(_message)
+
+        return result
+
+    eval_result = condition_tree_evaluator.evaluate(audience_conditions, evaluate_audience)
+    eval_result = eval_result or False
+    message = audience_logs.AUDIENCE_EVALUATION_RESULT_COMBINED.format(logging_key, str(eval_result).upper())
+    logger.info(message)
+    decide_reasons.append(message)
+    return eval_result, decide_reasons
```

### Comparing `optimizely-sdk-4.1.1/optimizely/helpers/condition_tree_evaluator.py` & `optimizely-sdk-5.0.0b0/optimizely/helpers/condition_tree_evaluator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,119 +1,125 @@
-# Copyright 2018-2019, Optimizely
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from .condition import ConditionOperatorTypes
-
-
-def and_evaluator(conditions, leaf_evaluator):
-    """ Evaluates a list of conditions as if the evaluator had been applied
-  to each entry and the results AND-ed together.
-
-  Args:
-    conditions: List of conditions ex: [operand_1, operand_2].
-    leaf_evaluator: Function which will be called to evaluate leaf condition values.
-
-  Returns:
-    Boolean:
-      - True if all operands evaluate to True.
-      - False if a single operand evaluates to False.
-    None: if conditions couldn't be evaluated.
-  """
-    saw_null_result = False
-
-    for condition in conditions:
-        result = evaluate(condition, leaf_evaluator)
-        if result is False:
-            return False
-        if result is None:
-            saw_null_result = True
-
-    return None if saw_null_result else True
-
-
-def or_evaluator(conditions, leaf_evaluator):
-    """ Evaluates a list of conditions as if the evaluator had been applied
-  to each entry and the results OR-ed together.
-
-  Args:
-    conditions: List of conditions ex: [operand_1, operand_2].
-    leaf_evaluator: Function which will be called to evaluate leaf condition values.
-
-  Returns:
-    Boolean:
-      - True if any operand evaluates to True.
-      - False if all operands evaluate to False.
-    None: if conditions couldn't be evaluated.
-  """
-    saw_null_result = False
-
-    for condition in conditions:
-        result = evaluate(condition, leaf_evaluator)
-        if result is True:
-            return True
-        if result is None:
-            saw_null_result = True
-
-    return None if saw_null_result else False
-
-
-def not_evaluator(conditions, leaf_evaluator):
-    """ Evaluates a list of conditions as if the evaluator had been applied
-  to a single entry and NOT was applied to the result.
-
-  Args:
-    conditions: List of conditions ex: [operand_1, operand_2].
-    leaf_evaluator: Function which will be called to evaluate leaf condition values.
-
-  Returns:
-    Boolean:
-      - True if the operand evaluates to False.
-      - False if the operand evaluates to True.
-    None: if conditions is empty or condition couldn't be evaluated.
-  """
-    if not len(conditions) > 0:
-        return None
-
-    result = evaluate(conditions[0], leaf_evaluator)
-    return None if result is None else not result
-
-
-EVALUATORS_BY_OPERATOR_TYPE = {
-    ConditionOperatorTypes.AND: and_evaluator,
-    ConditionOperatorTypes.OR: or_evaluator,
-    ConditionOperatorTypes.NOT: not_evaluator,
-}
-
-
-def evaluate(conditions, leaf_evaluator):
-    """ Top level method to evaluate conditions.
-
-  Args:
-    conditions: Nested array of and/or conditions, or a single leaf condition value of any type.
-                Example: ['and', '0', ['or', '1', '2']]
-    leaf_evaluator: Function which will be called to evaluate leaf condition values.
-
-  Returns:
-    Boolean: Result of evaluating the conditions using the operator rules and the leaf evaluator.
-    None: if conditions couldn't be evaluated.
-
-  """
-
-    if isinstance(conditions, list):
-        if conditions[0] in list(EVALUATORS_BY_OPERATOR_TYPE.keys()):
-            return EVALUATORS_BY_OPERATOR_TYPE[conditions[0]](conditions[1:], leaf_evaluator)
-        else:
-            # assume OR when operator is not explicit.
-            return EVALUATORS_BY_OPERATOR_TYPE[ConditionOperatorTypes.OR](conditions, leaf_evaluator)
-
-    leaf_condition = conditions
-    return leaf_evaluator(leaf_condition)
+# Copyright 2018-2019, 2022, Optimizely
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from __future__ import annotations
+from typing import Any, Callable, Optional, Sequence
+
+from .condition import ConditionOperatorTypes
+
+
+LeafEvaluator = Callable[[Any], Optional[bool]]
+
+
+def and_evaluator(conditions: Sequence[str | list[str]], leaf_evaluator: LeafEvaluator) -> Optional[bool]:
+    """ Evaluates a list of conditions as if the evaluator had been applied
+  to each entry and the results AND-ed together.
+
+  Args:
+    conditions: List of conditions ex: [operand_1, operand_2].
+    leaf_evaluator: Function which will be called to evaluate leaf condition values.
+
+  Returns:
+    Boolean:
+      - True if all operands evaluate to True.
+      - False if a single operand evaluates to False.
+    None: if conditions couldn't be evaluated.
+  """
+    saw_null_result = False
+
+    for condition in conditions:
+        result = evaluate(condition, leaf_evaluator)
+        if result is False:
+            return False
+        if result is None:
+            saw_null_result = True
+
+    return None if saw_null_result else True
+
+
+def or_evaluator(conditions: Sequence[str | list[str]], leaf_evaluator: LeafEvaluator) -> Optional[bool]:
+    """ Evaluates a list of conditions as if the evaluator had been applied
+  to each entry and the results OR-ed together.
+
+  Args:
+    conditions: List of conditions ex: [operand_1, operand_2].
+    leaf_evaluator: Function which will be called to evaluate leaf condition values.
+
+  Returns:
+    Boolean:
+      - True if any operand evaluates to True.
+      - False if all operands evaluate to False.
+    None: if conditions couldn't be evaluated.
+  """
+    saw_null_result = False
+
+    for condition in conditions:
+        result = evaluate(condition, leaf_evaluator)
+        if result is True:
+            return True
+        if result is None:
+            saw_null_result = True
+
+    return None if saw_null_result else False
+
+
+def not_evaluator(conditions: Sequence[str | list[str]], leaf_evaluator: LeafEvaluator) -> Optional[bool]:
+    """ Evaluates a list of conditions as if the evaluator had been applied
+  to a single entry and NOT was applied to the result.
+
+  Args:
+    conditions: List of conditions ex: [operand_1, operand_2].
+    leaf_evaluator: Function which will be called to evaluate leaf condition values.
+
+  Returns:
+    Boolean:
+      - True if the operand evaluates to False.
+      - False if the operand evaluates to True.
+    None: if conditions is empty or condition couldn't be evaluated.
+  """
+    if not len(conditions) > 0:
+        return None
+
+    result = evaluate(conditions[0], leaf_evaluator)
+    return None if result is None else not result
+
+
+EVALUATORS_BY_OPERATOR_TYPE = {
+    ConditionOperatorTypes.AND: and_evaluator,
+    ConditionOperatorTypes.OR: or_evaluator,
+    ConditionOperatorTypes.NOT: not_evaluator,
+}
+
+
+def evaluate(conditions: Optional[Sequence[str | list[str]]], leaf_evaluator: LeafEvaluator) -> Optional[bool]:
+    """ Top level method to evaluate conditions.
+
+  Args:
+    conditions: Nested array of and/or conditions, or a single leaf condition value of any type.
+                Example: ['and', '0', ['or', '1', '2']]
+    leaf_evaluator: Function which will be called to evaluate leaf condition values.
+
+  Returns:
+    Boolean: Result of evaluating the conditions using the operator rules and the leaf evaluator.
+    None: if conditions couldn't be evaluated.
+
+  """
+
+    if isinstance(conditions, list):
+        if conditions[0] in list(EVALUATORS_BY_OPERATOR_TYPE.keys()):
+            return EVALUATORS_BY_OPERATOR_TYPE[conditions[0]](conditions[1:], leaf_evaluator)
+        else:
+            # assume OR when operator is not explicit.
+            return EVALUATORS_BY_OPERATOR_TYPE[ConditionOperatorTypes.OR](conditions, leaf_evaluator)
+
+    leaf_condition = conditions
+    return leaf_evaluator(leaf_condition)
```

### Comparing `optimizely-sdk-4.1.1/optimizely/helpers/constants.py` & `optimizely-sdk-5.0.0b0/optimizely/helpers/constants.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,164 +1,172 @@
-# Copyright 2016-2017, Optimizely
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-JSON_SCHEMA = {
-    "$schema": "http://json-schema.org/draft-04/schema#",
-    "type": "object",
-    "properties": {
-        "projectId": {"type": "string"},
-        "accountId": {"type": "string"},
-        "groups": {
-            "type": "array",
-            "items": {
-                "type": "object",
-                "properties": {
-                    "id": {"type": "string"},
-                    "policy": {"type": "string"},
-                    "trafficAllocation": {
-                        "type": "array",
-                        "items": {
-                            "type": "object",
-                            "properties": {"entityId": {"type": "string"}, "endOfRange": {"type": "integer"}},
-                            "required": ["entityId", "endOfRange"],
-                        },
-                    },
-                    "experiments": {
-                        "type": "array",
-                        "items": {
-                            "type": "object",
-                            "properties": {
-                                "id": {"type": "string"},
-                                "layerId": {"type": "string"},
-                                "key": {"type": "string"},
-                                "status": {"type": "string"},
-                                "variations": {
-                                    "type": "array",
-                                    "items": {
-                                        "type": "object",
-                                        "properties": {"id": {"type": "string"}, "key": {"type": "string"}},
-                                        "required": ["id", "key"],
-                                    },
-                                },
-                                "trafficAllocation": {
-                                    "type": "array",
-                                    "items": {
-                                        "type": "object",
-                                        "properties": {
-                                            "entityId": {"type": "string"},
-                                            "endOfRange": {"type": "integer"},
-                                        },
-                                        "required": ["entityId", "endOfRange"],
-                                    },
-                                },
-                                "audienceIds": {"type": "array", "items": {"type": "string"}},
-                                "forcedVariations": {"type": "object"},
-                            },
-                            "required": [
-                                "id",
-                                "layerId",
-                                "key",
-                                "status",
-                                "variations",
-                                "trafficAllocation",
-                                "audienceIds",
-                                "forcedVariations",
-                            ],
-                        },
-                    },
-                },
-                "required": ["id", "policy", "trafficAllocation", "experiments"],
-            },
-        },
-        "experiments": {
-            "type": "array",
-            "items": {
-                "type": "object",
-                "properties": {
-                    "id": {"type": "string"},
-                    "layerId": {"type": "string"},
-                    "key": {"type": "string"},
-                    "status": {"type": "string"},
-                    "variations": {
-                        "type": "array",
-                        "items": {
-                            "type": "object",
-                            "properties": {"id": {"type": "string"}, "key": {"type": "string"}},
-                            "required": ["id", "key"],
-                        },
-                    },
-                    "trafficAllocation": {
-                        "type": "array",
-                        "items": {
-                            "type": "object",
-                            "properties": {"entityId": {"type": "string"}, "endOfRange": {"type": "integer"}},
-                            "required": ["entityId", "endOfRange"],
-                        },
-                    },
-                    "audienceIds": {"type": "array", "items": {"type": "string"}},
-                    "forcedVariations": {"type": "object"},
-                },
-                "required": [
-                    "id",
-                    "layerId",
-                    "key",
-                    "status",
-                    "variations",
-                    "trafficAllocation",
-                    "audienceIds",
-                    "forcedVariations",
-                ],
-            },
-        },
-        "events": {
-            "type": "array",
-            "items": {
-                "type": "object",
-                "properties": {
-                    "key": {"type": "string"},
-                    "experimentIds": {"type": "array", "items": {"type": "string"}},
-                    "id": {"type": "string"},
-                },
-                "required": ["key", "experimentIds", "id"],
-            },
-        },
-        "audiences": {
-            "type": "array",
-            "items": {
-                "type": "object",
-                "properties": {"id": {"type": "string"}, "name": {"type": "string"}, "conditions": {"type": "string"}},
-                "required": ["id", "name", "conditions"],
-            },
-        },
-        "attributes": {
-            "type": "array",
-            "items": {
-                "type": "object",
-                "properties": {"id": {"type": "string"}, "key": {"type": "string"}},
-                "required": ["id", "key"],
-            },
-        },
-        "version": {"type": "string"},
-        "revision": {"type": "string"},
-    },
-    "required": [
-        "projectId",
-        "accountId",
-        "groups",
-        "experiments",
-        "events",
-        "audiences",
-        "attributes",
-        "version",
-        "revision",
-    ],
-}
+# Copyright 2016-2017, Optimizely
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+JSON_SCHEMA = {
+    "$schema": "http://json-schema.org/draft-04/schema#",
+    "type": "object",
+    "properties": {
+        "projectId": {"type": "string"},
+        "accountId": {"type": "string"},
+        "groups": {
+            "type": "array",
+            "items": {
+                "type": "object",
+                "properties": {
+                    "id": {"type": "string"},
+                    "policy": {"type": "string"},
+                    "trafficAllocation": {
+                        "type": "array",
+                        "items": {
+                            "type": "object",
+                            "properties": {"entityId": {"type": "string"}, "endOfRange": {"type": "integer"}},
+                            "required": ["entityId", "endOfRange"],
+                        },
+                    },
+                    "experiments": {
+                        "type": "array",
+                        "items": {
+                            "type": "object",
+                            "properties": {
+                                "id": {"type": "string"},
+                                "layerId": {"type": "string"},
+                                "key": {"type": "string"},
+                                "status": {"type": "string"},
+                                "variations": {
+                                    "type": "array",
+                                    "items": {
+                                        "type": "object",
+                                        "properties": {"id": {"type": "string"}, "key": {"type": "string"}},
+                                        "required": ["id", "key"],
+                                    },
+                                },
+                                "trafficAllocation": {
+                                    "type": "array",
+                                    "items": {
+                                        "type": "object",
+                                        "properties": {
+                                            "entityId": {"type": "string"},
+                                            "endOfRange": {"type": "integer"},
+                                        },
+                                        "required": ["entityId", "endOfRange"],
+                                    },
+                                },
+                                "audienceIds": {"type": "array", "items": {"type": "string"}},
+                                "forcedVariations": {"type": "object"},
+                            },
+                            "required": [
+                                "id",
+                                "layerId",
+                                "key",
+                                "status",
+                                "variations",
+                                "trafficAllocation",
+                                "audienceIds",
+                                "forcedVariations",
+                            ],
+                        },
+                    },
+                },
+                "required": ["id", "policy", "trafficAllocation", "experiments"],
+            },
+        },
+        "experiments": {
+            "type": "array",
+            "items": {
+                "type": "object",
+                "properties": {
+                    "id": {"type": "string"},
+                    "layerId": {"type": "string"},
+                    "key": {"type": "string"},
+                    "status": {"type": "string"},
+                    "variations": {
+                        "type": "array",
+                        "items": {
+                            "type": "object",
+                            "properties": {"id": {"type": "string"}, "key": {"type": "string"}},
+                            "required": ["id", "key"],
+                        },
+                    },
+                    "trafficAllocation": {
+                        "type": "array",
+                        "items": {
+                            "type": "object",
+                            "properties": {"entityId": {"type": "string"}, "endOfRange": {"type": "integer"}},
+                            "required": ["entityId", "endOfRange"],
+                        },
+                    },
+                    "audienceIds": {"type": "array", "items": {"type": "string"}},
+                    "forcedVariations": {"type": "object"},
+                },
+                "required": [
+                    "id",
+                    "layerId",
+                    "key",
+                    "status",
+                    "variations",
+                    "trafficAllocation",
+                    "audienceIds",
+                    "forcedVariations",
+                ],
+            },
+        },
+        "events": {
+            "type": "array",
+            "items": {
+                "type": "object",
+                "properties": {
+                    "key": {"type": "string"},
+                    "experimentIds": {"type": "array", "items": {"type": "string"}},
+                    "id": {"type": "string"},
+                },
+                "required": ["key", "experimentIds", "id"],
+            },
+        },
+        "audiences": {
+            "type": "array",
+            "items": {
+                "type": "object",
+                "properties": {"id": {"type": "string"}, "name": {"type": "string"}, "conditions": {"type": "string"}},
+                "required": ["id", "name", "conditions"],
+            },
+        },
+        "attributes": {
+            "type": "array",
+            "items": {
+                "type": "object",
+                "properties": {"id": {"type": "string"}, "key": {"type": "string"}},
+                "required": ["id", "key"],
+            },
+        },
+        "version": {"type": "string"},
+        "revision": {"type": "string"},
+        "integrations": {
+            "type": "array",
+            "items": {
+                "type": "object",
+                "properties": {"key": {"type": "string"}, "host": {"type": "string"}, "publicKey": {"type": "string"}},
+                "required": ["key"],
+            }
+        }
+    },
+    "required": [
+        "projectId",
+        "accountId",
+        "groups",
+        "experiments",
+        "events",
+        "audiences",
+        "attributes",
+        "version",
+        "revision",
+    ],
+}
```

### Comparing `optimizely-sdk-4.1.1/optimizely/helpers/event_tag_utils.py` & `optimizely-sdk-5.0.0b0/optimizely/helpers/event_tag_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,130 +1,144 @@
-# Copyright 2017, Optimizely
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from . import enums
-import math
-import numbers
-
-REVENUE_METRIC_TYPE = 'revenue'
-NUMERIC_METRIC_TYPE = 'value'
-
-
-def get_revenue_value(event_tags):
-    if event_tags is None:
-        return None
-
-    if not isinstance(event_tags, dict):
-        return None
-
-    if REVENUE_METRIC_TYPE not in event_tags:
-        return None
-
-    raw_value = event_tags[REVENUE_METRIC_TYPE]
-
-    if isinstance(raw_value, bool):
-        return None
-
-    if not isinstance(raw_value, numbers.Integral):
-        return None
-
-    return raw_value
-
-
-def get_numeric_value(event_tags, logger=None):
-    """
-  A smart getter of the numeric value from the event tags.
-
-  Args:
-      event_tags: A dictionary of event tags.
-      logger: Optional logger.
-
-  Returns:
-      A float numeric metric value is returned when the provided numeric
-      metric value is in the following format:
-          - A string (properly formatted, e.g., no commas)
-          - An integer
-          - A float or double
-      None is returned when the provided numeric metric values is in
-      the following format:
-          - None
-          - A boolean
-          - inf, -inf, nan
-          - A string not properly formatted (e.g., '1,234')
-          - Any values that cannot be cast to a float (e.g., an array or dictionary)
-  """
-
-    logger_message_debug = None
-    numeric_metric_value = None
-
-    if event_tags is None:
-        return numeric_metric_value
-    elif not isinstance(event_tags, dict):
-        if logger:
-            logger.log(enums.LogLevels.ERROR, 'Event tags is not a dictionary.')
-        return numeric_metric_value
-    elif NUMERIC_METRIC_TYPE not in event_tags:
-        return numeric_metric_value
-    else:
-        numeric_metric_value = event_tags[NUMERIC_METRIC_TYPE]
-        try:
-            if isinstance(numeric_metric_value, (numbers.Integral, float, str)):
-                # Attempt to convert the numeric metric value to a float
-                # (if it isn't already a float).
-                cast_numeric_metric_value = float(numeric_metric_value)
-
-                # If not a float after casting, then make everything else a None.
-                # Other potential values are nan, inf, and -inf.
-                if not isinstance(cast_numeric_metric_value, float) or \
-                   math.isnan(cast_numeric_metric_value) or \
-                   math.isinf(cast_numeric_metric_value):
-                    logger_message_debug = 'Provided numeric value {} is in an invalid format.'.format(
-                        numeric_metric_value
-                    )
-                    numeric_metric_value = None
-                else:
-                    # Handle booleans as a special case.
-                    # They are treated like an integer in the cast, but we do not want to cast this.
-                    if isinstance(numeric_metric_value, bool):
-                        logger_message_debug = 'Provided numeric value is a boolean, which is an invalid format.'
-                        numeric_metric_value = None
-                    else:
-                        numeric_metric_value = cast_numeric_metric_value
-            else:
-                logger_message_debug = 'Numeric metric value is not in integer, float, or string form.'
-                numeric_metric_value = None
-
-        except ValueError:
-            logger_message_debug = 'Value error while casting numeric metric value to a float.'
-            numeric_metric_value = None
-
-    # Log all potential debug messages while converting the numeric value to a float.
-    if logger and logger_message_debug:
-        logger.log(enums.LogLevels.DEBUG, logger_message_debug)
-
-    # Log the final numeric metric value
-    if numeric_metric_value is not None:
-        if logger:
-            logger.log(
-                enums.LogLevels.INFO,
-                'The numeric metric value {} will be sent to results.'.format(numeric_metric_value),
-            )
-    else:
-        if logger:
-            logger.log(
-                enums.LogLevels.WARNING,
-                'The provided numeric metric value {} is in an invalid format and will not be sent to results.'.format(
-                    numeric_metric_value
-                ),
-            )
-
-    return numeric_metric_value
+# Copyright 2017, 2022, Optimizely
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from __future__ import annotations
+from typing import TYPE_CHECKING, Any, Optional, NewType, Dict
+from . import enums
+import math
+import numbers
+from sys import version_info
+
+if version_info < (3, 8):
+    from typing_extensions import Final
+else:
+    from typing import Final  # type: ignore
+
+
+if TYPE_CHECKING:
+    # prevent circular dependenacy by skipping import at runtime
+    from optimizely.logger import Logger
+
+
+REVENUE_METRIC_TYPE: Final = 'revenue'
+NUMERIC_METRIC_TYPE: Final = 'value'
+
+# type for tracking event tags (essentially a sub-type of dict)
+EventTags = NewType('EventTags', Dict[str, Any])
+
+
+def get_revenue_value(event_tags: Optional[EventTags]) -> Optional[numbers.Integral]:
+    if event_tags is None:
+        return None
+
+    if not isinstance(event_tags, dict):
+        return None
+
+    if REVENUE_METRIC_TYPE not in event_tags:
+        return None
+
+    raw_value = event_tags[REVENUE_METRIC_TYPE]
+
+    if isinstance(raw_value, bool):
+        return None
+
+    if not isinstance(raw_value, numbers.Integral):
+        return None
+
+    return raw_value
+
+
+def get_numeric_value(event_tags: Optional[EventTags], logger: Optional[Logger] = None) -> Optional[float]:
+    """
+  A smart getter of the numeric value from the event tags.
+
+  Args:
+      event_tags: A dictionary of event tags.
+      logger: Optional logger.
+
+  Returns:
+      A float numeric metric value is returned when the provided numeric
+      metric value is in the following format:
+          - A string (properly formatted, e.g., no commas)
+          - An integer
+          - A float or double
+      None is returned when the provided numeric metric values is in
+      the following format:
+          - None
+          - A boolean
+          - inf, -inf, nan
+          - A string not properly formatted (e.g., '1,234')
+          - Any values that cannot be cast to a float (e.g., an array or dictionary)
+  """
+
+    logger_message_debug = None
+    numeric_metric_value = None
+
+    if event_tags is None:
+        return numeric_metric_value
+    elif not isinstance(event_tags, dict):
+        if logger:
+            logger.log(enums.LogLevels.ERROR, 'Event tags is not a dictionary.')
+        return numeric_metric_value
+    elif NUMERIC_METRIC_TYPE not in event_tags:
+        return numeric_metric_value
+    else:
+        numeric_metric_value = event_tags[NUMERIC_METRIC_TYPE]
+        try:
+            if isinstance(numeric_metric_value, (numbers.Integral, float, str)):
+                # Attempt to convert the numeric metric value to a float
+                # (if it isn't already a float).
+                cast_numeric_metric_value = float(numeric_metric_value)
+
+                # If not a float after casting, then make everything else a None.
+                # Other potential values are nan, inf, and -inf.
+                if not isinstance(cast_numeric_metric_value, float) or \
+                   math.isnan(cast_numeric_metric_value) or \
+                   math.isinf(cast_numeric_metric_value):
+                    logger_message_debug = f'Provided numeric value {numeric_metric_value} is in an invalid format.'
+                    numeric_metric_value = None
+                else:
+                    # Handle booleans as a special case.
+                    # They are treated like an integer in the cast, but we do not want to cast this.
+                    if isinstance(numeric_metric_value, bool):
+                        logger_message_debug = 'Provided numeric value is a boolean, which is an invalid format.'
+                        numeric_metric_value = None
+                    else:
+                        numeric_metric_value = cast_numeric_metric_value
+            else:
+                logger_message_debug = 'Numeric metric value is not in integer, float, or string form.'
+                numeric_metric_value = None
+
+        except ValueError:
+            logger_message_debug = 'Value error while casting numeric metric value to a float.'
+            numeric_metric_value = None
+
+    # Log all potential debug messages while converting the numeric value to a float.
+    if logger and logger_message_debug:
+        logger.log(enums.LogLevels.DEBUG, logger_message_debug)
+
+    # Log the final numeric metric value
+    if numeric_metric_value is not None:
+        if logger:
+            logger.log(
+                enums.LogLevels.INFO,
+                f'The numeric metric value {numeric_metric_value} will be sent to results.'
+            )
+    else:
+        if logger:
+            logger.log(
+                enums.LogLevels.WARNING,
+                f'The provided numeric metric value {numeric_metric_value}'
+                ' is in an invalid format and will not be sent to results.'
+            )
+
+    return numeric_metric_value  # type: ignore[no-any-return]
```

### Comparing `optimizely-sdk-4.1.1/optimizely/helpers/experiment.py` & `optimizely-sdk-5.0.0b0/optimizely/helpers/experiment.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,34 @@
-# Copyright 2016, Optimizely
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-ALLOWED_EXPERIMENT_STATUS = ['Running']
-
-
-def is_experiment_running(experiment):
-    """ Determine for given experiment if experiment is running.
-
-  Args:
-    experiment: Object representing the experiment.
-
-  Returns:
-    Boolean representing if experiment is running or not.
-  """
-
-    return experiment.status in ALLOWED_EXPERIMENT_STATUS
+# Copyright 2016, 2022, Optimizely
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+from __future__ import annotations
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    # prevent circular dependenacy by skipping import at runtime
+    from optimizely.entities import Experiment
+
+
+ALLOWED_EXPERIMENT_STATUS = ['Running']
+
+
+def is_experiment_running(experiment: Experiment) -> bool:
+    """ Determine for given experiment if experiment is running.
+
+  Args:
+    experiment: Object representing the experiment.
+
+  Returns:
+    Boolean representing if experiment is running or not.
+  """
+
+    return experiment.status in ALLOWED_EXPERIMENT_STATUS
```

### Comparing `optimizely-sdk-4.1.1/optimizely/lib/__init__.py` & `optimizely-sdk-5.0.0b0/optimizely/odp/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2016, Optimizely
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# Copyright 2022, Optimizely
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
```

### Comparing `optimizely-sdk-4.1.1/optimizely/lib/pymmh3.py` & `optimizely-sdk-5.0.0b0/optimizely/lib/pymmh3.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,470 +1,456 @@
-'''
-pymmh3 was written by Fredrik Kihlander and enhanced by Swapnil Gusani, and is placed in the public
-domain. The authors hereby disclaim copyright to this source code.
-
-pure python implementation of the murmur3 hash algorithm
-
-https://code.google.com/p/smhasher/wiki/MurmurHash3
-
-This was written for the times when you do not want to compile c-code and install modules,
-and you only want a drop-in murmur3 implementation.
-
-As this is purely python it is FAR from performant and if performance is anything that is needed
-a proper c-module is suggested!
-
-This module is written to have the same format as mmh3 python package found here for simple conversions:
-
-https://pypi.python.org/pypi/mmh3/2.3.1
-'''
-
-import sys as _sys
-
-if _sys.version_info > (3, 0):
-
-    def xrange(a, b, c):
-        return range(a, b, c)
-
-    def xencode(x):
-        if isinstance(x, bytes) or isinstance(x, bytearray):
-            return x
-        else:
-            return x.encode()
-
-
-else:
-
-    def xencode(x):
-        return x
-
-
-del _sys
-
-
-def hash(key, seed=0x0):
-    ''' Implements 32bit murmur3 hash. '''
-
-    key = bytearray(xencode(key))
-
-    def fmix(h):
-        h ^= h >> 16
-        h = (h * 0x85EBCA6B) & 0xFFFFFFFF
-        h ^= h >> 13
-        h = (h * 0xC2B2AE35) & 0xFFFFFFFF
-        h ^= h >> 16
-        return h
-
-    length = len(key)
-    nblocks = int(length / 4)
-
-    h1 = seed
-
-    c1 = 0xCC9E2D51
-    c2 = 0x1B873593
-
-    # body
-    for block_start in xrange(0, nblocks * 4, 4):
-        # ??? big endian?
-        k1 = key[block_start + 3] << 24 | key[block_start + 2] << 16 | key[block_start + 1] << 8 | key[block_start + 0]
-
-        k1 = (c1 * k1) & 0xFFFFFFFF
-        k1 = (k1 << 15 | k1 >> 17) & 0xFFFFFFFF  # inlined ROTL32
-        k1 = (c2 * k1) & 0xFFFFFFFF
-
-        h1 ^= k1
-        h1 = (h1 << 13 | h1 >> 19) & 0xFFFFFFFF  # inlined ROTL32
-        h1 = (h1 * 5 + 0xE6546B64) & 0xFFFFFFFF
-
-    # tail
-    tail_index = nblocks * 4
-    k1 = 0
-    tail_size = length & 3
-
-    if tail_size >= 3:
-        k1 ^= key[tail_index + 2] << 16
-    if tail_size >= 2:
-        k1 ^= key[tail_index + 1] << 8
-    if tail_size >= 1:
-        k1 ^= key[tail_index + 0]
-
-    if tail_size > 0:
-        k1 = (k1 * c1) & 0xFFFFFFFF
-        k1 = (k1 << 15 | k1 >> 17) & 0xFFFFFFFF  # inlined ROTL32
-        k1 = (k1 * c2) & 0xFFFFFFFF
-        h1 ^= k1
-
-    # finalization
-    unsigned_val = fmix(h1 ^ length)
-    if unsigned_val & 0x80000000 == 0:
-        return unsigned_val
-    else:
-        return -((unsigned_val ^ 0xFFFFFFFF) + 1)
-
-
-def hash128(key, seed=0x0, x64arch=True):
-    ''' Implements 128bit murmur3 hash. '''
-
-    def hash128_x64(key, seed):
-        ''' Implements 128bit murmur3 hash for x64. '''
-
-        def fmix(k):
-            k ^= k >> 33
-            k = (k * 0xFF51AFD7ED558CCD) & 0xFFFFFFFFFFFFFFFF
-            k ^= k >> 33
-            k = (k * 0xC4CEB9FE1A85EC53) & 0xFFFFFFFFFFFFFFFF
-            k ^= k >> 33
-            return k
-
-        length = len(key)
-        nblocks = int(length / 16)
-
-        h1 = seed
-        h2 = seed
-
-        c1 = 0x87C37B91114253D5
-        c2 = 0x4CF5AD432745937F
-
-        # body
-        for block_start in xrange(0, nblocks * 8, 8):
-            # ??? big endian?
-            k1 = (
-                key[2 * block_start + 7] << 56 |
-                key[2 * block_start + 6] << 48 |
-                key[2 * block_start + 5] << 40 |
-                key[2 * block_start + 4] << 32 |
-                key[2 * block_start + 3] << 24 |
-                key[2 * block_start + 2] << 16 |
-                key[2 * block_start + 1] << 8 |
-                key[2 * block_start + 0]
-            )
-
-            k2 = (
-                key[2 * block_start + 15] << 56 |
-                key[2 * block_start + 14] << 48 |
-                key[2 * block_start + 13] << 40 |
-                key[2 * block_start + 12] << 32 |
-                key[2 * block_start + 11] << 24 |
-                key[2 * block_start + 10] << 16 |
-                key[2 * block_start + 9] << 8 |
-                key[2 * block_start + 8]
-            )
-
-            k1 = (c1 * k1) & 0xFFFFFFFFFFFFFFFF
-            k1 = (k1 << 31 | k1 >> 33) & 0xFFFFFFFFFFFFFFFF  # inlined ROTL64
-            k1 = (c2 * k1) & 0xFFFFFFFFFFFFFFFF
-            h1 ^= k1
-
-            h1 = (h1 << 27 | h1 >> 37) & 0xFFFFFFFFFFFFFFFF  # inlined ROTL64
-            h1 = (h1 + h2) & 0xFFFFFFFFFFFFFFFF
-            h1 = (h1 * 5 + 0x52DCE729) & 0xFFFFFFFFFFFFFFFF
-
-            k2 = (c2 * k2) & 0xFFFFFFFFFFFFFFFF
-            k2 = (k2 << 33 | k2 >> 31) & 0xFFFFFFFFFFFFFFFF  # inlined ROTL64
-            k2 = (c1 * k2) & 0xFFFFFFFFFFFFFFFF
-            h2 ^= k2
-
-            h2 = (h2 << 31 | h2 >> 33) & 0xFFFFFFFFFFFFFFFF  # inlined ROTL64
-            h2 = (h1 + h2) & 0xFFFFFFFFFFFFFFFF
-            h2 = (h2 * 5 + 0x38495AB5) & 0xFFFFFFFFFFFFFFFF
-
-        # tail
-        tail_index = nblocks * 16
-        k1 = 0
-        k2 = 0
-        tail_size = length & 15
-
-        if tail_size >= 15:
-            k2 ^= key[tail_index + 14] << 48
-        if tail_size >= 14:
-            k2 ^= key[tail_index + 13] << 40
-        if tail_size >= 13:
-            k2 ^= key[tail_index + 12] << 32
-        if tail_size >= 12:
-            k2 ^= key[tail_index + 11] << 24
-        if tail_size >= 11:
-            k2 ^= key[tail_index + 10] << 16
-        if tail_size >= 10:
-            k2 ^= key[tail_index + 9] << 8
-        if tail_size >= 9:
-            k2 ^= key[tail_index + 8]
-
-        if tail_size > 8:
-            k2 = (k2 * c2) & 0xFFFFFFFFFFFFFFFF
-            k2 = (k2 << 33 | k2 >> 31) & 0xFFFFFFFFFFFFFFFF  # inlined ROTL64
-            k2 = (k2 * c1) & 0xFFFFFFFFFFFFFFFF
-            h2 ^= k2
-
-        if tail_size >= 8:
-            k1 ^= key[tail_index + 7] << 56
-        if tail_size >= 7:
-            k1 ^= key[tail_index + 6] << 48
-        if tail_size >= 6:
-            k1 ^= key[tail_index + 5] << 40
-        if tail_size >= 5:
-            k1 ^= key[tail_index + 4] << 32
-        if tail_size >= 4:
-            k1 ^= key[tail_index + 3] << 24
-        if tail_size >= 3:
-            k1 ^= key[tail_index + 2] << 16
-        if tail_size >= 2:
-            k1 ^= key[tail_index + 1] << 8
-        if tail_size >= 1:
-            k1 ^= key[tail_index + 0]
-
-        if tail_size > 0:
-            k1 = (k1 * c1) & 0xFFFFFFFFFFFFFFFF
-            k1 = (k1 << 31 | k1 >> 33) & 0xFFFFFFFFFFFFFFFF  # inlined ROTL64
-            k1 = (k1 * c2) & 0xFFFFFFFFFFFFFFFF
-            h1 ^= k1
-
-        # finalization
-        h1 ^= length
-        h2 ^= length
-
-        h1 = (h1 + h2) & 0xFFFFFFFFFFFFFFFF
-        h2 = (h1 + h2) & 0xFFFFFFFFFFFFFFFF
-
-        h1 = fmix(h1)
-        h2 = fmix(h2)
-
-        h1 = (h1 + h2) & 0xFFFFFFFFFFFFFFFF
-        h2 = (h1 + h2) & 0xFFFFFFFFFFFFFFFF
-
-        return h2 << 64 | h1
-
-    def hash128_x86(key, seed):
-        ''' Implements 128bit murmur3 hash for x86. '''
-
-        def fmix(h):
-            h ^= h >> 16
-            h = (h * 0x85EBCA6B) & 0xFFFFFFFF
-            h ^= h >> 13
-            h = (h * 0xC2B2AE35) & 0xFFFFFFFF
-            h ^= h >> 16
-            return h
-
-        length = len(key)
-        nblocks = int(length / 16)
-
-        h1 = seed
-        h2 = seed
-        h3 = seed
-        h4 = seed
-
-        c1 = 0x239B961B
-        c2 = 0xAB0E9789
-        c3 = 0x38B34AE5
-        c4 = 0xA1E38B93
-
-        # body
-        for block_start in xrange(0, nblocks * 16, 16):
-            k1 = (
-                key[block_start + 3] << 24 |
-                key[block_start + 2] << 16 |
-                key[block_start + 1] << 8 |
-                key[block_start + 0]
-            )
-
-            k2 = (
-                key[block_start + 7] << 24 |
-                key[block_start + 6] << 16 |
-                key[block_start + 5] << 8 |
-                key[block_start + 4]
-            )
-
-            k3 = (
-                key[block_start + 11] << 24 |
-                key[block_start + 10] << 16 |
-                key[block_start + 9] << 8 |
-                key[block_start + 8]
-            )
-
-            k4 = (
-                key[block_start + 15] << 24 |
-                key[block_start + 14] << 16 |
-                key[block_start + 13] << 8 |
-                key[block_start + 12]
-            )
-
-            k1 = (c1 * k1) & 0xFFFFFFFF
-            k1 = (k1 << 15 | k1 >> 17) & 0xFFFFFFFF  # inlined ROTL32
-            k1 = (c2 * k1) & 0xFFFFFFFF
-            h1 ^= k1
-
-            h1 = (h1 << 19 | h1 >> 13) & 0xFFFFFFFF  # inlined ROTL32
-            h1 = (h1 + h2) & 0xFFFFFFFF
-            h1 = (h1 * 5 + 0x561CCD1B) & 0xFFFFFFFF
-
-            k2 = (c2 * k2) & 0xFFFFFFFF
-            k2 = (k2 << 16 | k2 >> 16) & 0xFFFFFFFF  # inlined ROTL32
-            k2 = (c3 * k2) & 0xFFFFFFFF
-            h2 ^= k2
-
-            h2 = (h2 << 17 | h2 >> 15) & 0xFFFFFFFF  # inlined ROTL32
-            h2 = (h2 + h3) & 0xFFFFFFFF
-            h2 = (h2 * 5 + 0x0BCAA747) & 0xFFFFFFFF
-
-            k3 = (c3 * k3) & 0xFFFFFFFF
-            k3 = (k3 << 17 | k3 >> 15) & 0xFFFFFFFF  # inlined ROTL32
-            k3 = (c4 * k3) & 0xFFFFFFFF
-            h3 ^= k3
-
-            h3 = (h3 << 15 | h3 >> 17) & 0xFFFFFFFF  # inlined ROTL32
-            h3 = (h3 + h4) & 0xFFFFFFFF
-            h3 = (h3 * 5 + 0x96CD1C35) & 0xFFFFFFFF
-
-            k4 = (c4 * k4) & 0xFFFFFFFF
-            k4 = (k4 << 18 | k4 >> 14) & 0xFFFFFFFF  # inlined ROTL32
-            k4 = (c1 * k4) & 0xFFFFFFFF
-            h4 ^= k4
-
-            h4 = (h4 << 13 | h4 >> 19) & 0xFFFFFFFF  # inlined ROTL32
-            h4 = (h1 + h4) & 0xFFFFFFFF
-            h4 = (h4 * 5 + 0x32AC3B17) & 0xFFFFFFFF
-
-        # tail
-        tail_index = nblocks * 16
-        k1 = 0
-        k2 = 0
-        k3 = 0
-        k4 = 0
-        tail_size = length & 15
-
-        if tail_size >= 15:
-            k4 ^= key[tail_index + 14] << 16
-        if tail_size >= 14:
-            k4 ^= key[tail_index + 13] << 8
-        if tail_size >= 13:
-            k4 ^= key[tail_index + 12]
-
-        if tail_size > 12:
-            k4 = (k4 * c4) & 0xFFFFFFFF
-            k4 = (k4 << 18 | k4 >> 14) & 0xFFFFFFFF  # inlined ROTL32
-            k4 = (k4 * c1) & 0xFFFFFFFF
-            h4 ^= k4
-
-        if tail_size >= 12:
-            k3 ^= key[tail_index + 11] << 24
-        if tail_size >= 11:
-            k3 ^= key[tail_index + 10] << 16
-        if tail_size >= 10:
-            k3 ^= key[tail_index + 9] << 8
-        if tail_size >= 9:
-            k3 ^= key[tail_index + 8]
-
-        if tail_size > 8:
-            k3 = (k3 * c3) & 0xFFFFFFFF
-            k3 = (k3 << 17 | k3 >> 15) & 0xFFFFFFFF  # inlined ROTL32
-            k3 = (k3 * c4) & 0xFFFFFFFF
-            h3 ^= k3
-
-        if tail_size >= 8:
-            k2 ^= key[tail_index + 7] << 24
-        if tail_size >= 7:
-            k2 ^= key[tail_index + 6] << 16
-        if tail_size >= 6:
-            k2 ^= key[tail_index + 5] << 8
-        if tail_size >= 5:
-            k2 ^= key[tail_index + 4]
-
-        if tail_size > 4:
-            k2 = (k2 * c2) & 0xFFFFFFFF
-            k2 = (k2 << 16 | k2 >> 16) & 0xFFFFFFFF  # inlined ROTL32
-            k2 = (k2 * c3) & 0xFFFFFFFF
-            h2 ^= k2
-
-        if tail_size >= 4:
-            k1 ^= key[tail_index + 3] << 24
-        if tail_size >= 3:
-            k1 ^= key[tail_index + 2] << 16
-        if tail_size >= 2:
-            k1 ^= key[tail_index + 1] << 8
-        if tail_size >= 1:
-            k1 ^= key[tail_index + 0]
-
-        if tail_size > 0:
-            k1 = (k1 * c1) & 0xFFFFFFFF
-            k1 = (k1 << 15 | k1 >> 17) & 0xFFFFFFFF  # inlined ROTL32
-            k1 = (k1 * c2) & 0xFFFFFFFF
-            h1 ^= k1
-
-        # finalization
-        h1 ^= length
-        h2 ^= length
-        h3 ^= length
-        h4 ^= length
-
-        h1 = (h1 + h2) & 0xFFFFFFFF
-        h1 = (h1 + h3) & 0xFFFFFFFF
-        h1 = (h1 + h4) & 0xFFFFFFFF
-        h2 = (h1 + h2) & 0xFFFFFFFF
-        h3 = (h1 + h3) & 0xFFFFFFFF
-        h4 = (h1 + h4) & 0xFFFFFFFF
-
-        h1 = fmix(h1)
-        h2 = fmix(h2)
-        h3 = fmix(h3)
-        h4 = fmix(h4)
-
-        h1 = (h1 + h2) & 0xFFFFFFFF
-        h1 = (h1 + h3) & 0xFFFFFFFF
-        h1 = (h1 + h4) & 0xFFFFFFFF
-        h2 = (h1 + h2) & 0xFFFFFFFF
-        h3 = (h1 + h3) & 0xFFFFFFFF
-        h4 = (h1 + h4) & 0xFFFFFFFF
-
-        return h4 << 96 | h3 << 64 | h2 << 32 | h1
-
-    key = bytearray(xencode(key))
-
-    if x64arch:
-        return hash128_x64(key, seed)
-    else:
-        return hash128_x86(key, seed)
-
-
-def hash64(key, seed=0x0, x64arch=True):
-    ''' Implements 64bit murmur3 hash. Returns a tuple. '''
-
-    hash_128 = hash128(key, seed, x64arch)
-
-    unsigned_val1 = hash_128 & 0xFFFFFFFFFFFFFFFF
-    if unsigned_val1 & 0x8000000000000000 == 0:
-        signed_val1 = unsigned_val1
-    else:
-        signed_val1 = -((unsigned_val1 ^ 0xFFFFFFFFFFFFFFFF) + 1)
-
-    unsigned_val2 = (hash_128 >> 64) & 0xFFFFFFFFFFFFFFFF
-    if unsigned_val2 & 0x8000000000000000 == 0:
-        signed_val2 = unsigned_val2
-    else:
-        signed_val2 = -((unsigned_val2 ^ 0xFFFFFFFFFFFFFFFF) + 1)
-
-    return (int(signed_val1), int(signed_val2))
-
-
-def hash_bytes(key, seed=0x0, x64arch=True):
-    ''' Implements 128bit murmur3 hash. Returns a byte string. '''
-
-    hash_128 = hash128(key, seed, x64arch)
-
-    bytestring = ''
-
-    for i in xrange(0, 16, 1):
-        lsbyte = hash_128 & 0xFF
-        bytestring = bytestring + str(chr(lsbyte))
-        hash_128 = hash_128 >> 8
-
-    return bytestring
-
-
-if __name__ == "__main__":
-    import argparse
-
-    parser = argparse.ArgumentParser('pymurmur3', 'pymurmur [options] "string to hash"')
-    parser.add_argument('--seed', type=int, default=0)
-    parser.add_argument('strings', default=[], nargs='+')
-
-    opts = parser.parse_args()
-
-    for str_to_hash in opts.strings:
-        sys.stdout.write('"%s" = 0x%08X\n' % (str_to_hash, hash(str_to_hash)))
+'''
+pymmh3 was written by Fredrik Kihlander and enhanced by Swapnil Gusani, and is placed in the public
+domain. The authors hereby disclaim copyright to this source code.
+
+pure python implementation of the murmur3 hash algorithm
+
+https://code.google.com/p/smhasher/wiki/MurmurHash3
+
+This was written for the times when you do not want to compile c-code and install modules,
+and you only want a drop-in murmur3 implementation.
+
+As this is purely python it is FAR from performant and if performance is anything that is needed
+a proper c-module is suggested!
+
+This module is written to have the same format as mmh3 python package found here for simple conversions:
+
+https://pypi.python.org/pypi/mmh3/2.3.1
+'''
+from __future__ import annotations
+
+def xencode(x: bytes | bytearray | str) -> bytes | bytearray:
+    if isinstance(x, bytes) or isinstance(x, bytearray):
+        return x
+    else:
+        return x.encode()
+
+
+def hash(key: str | bytearray, seed: int = 0x0) -> int:
+    ''' Implements 32bit murmur3 hash. '''
+
+    key = bytearray(xencode(key))
+
+    def fmix(h: int) -> int:
+        h ^= h >> 16
+        h = (h * 0x85EBCA6B) & 0xFFFFFFFF
+        h ^= h >> 13
+        h = (h * 0xC2B2AE35) & 0xFFFFFFFF
+        h ^= h >> 16
+        return h
+
+    length = len(key)
+    nblocks = int(length / 4)
+
+    h1 = seed
+
+    c1 = 0xCC9E2D51
+    c2 = 0x1B873593
+
+    # body
+    for block_start in range(0, nblocks * 4, 4):
+        # ??? big endian?
+        k1 = key[block_start + 3] << 24 | key[block_start + 2] << 16 | key[block_start + 1] << 8 | key[block_start + 0]
+
+        k1 = (c1 * k1) & 0xFFFFFFFF
+        k1 = (k1 << 15 | k1 >> 17) & 0xFFFFFFFF  # inlined ROTL32
+        k1 = (c2 * k1) & 0xFFFFFFFF
+
+        h1 ^= k1
+        h1 = (h1 << 13 | h1 >> 19) & 0xFFFFFFFF  # inlined ROTL32
+        h1 = (h1 * 5 + 0xE6546B64) & 0xFFFFFFFF
+
+    # tail
+    tail_index = nblocks * 4
+    k1 = 0
+    tail_size = length & 3
+
+    if tail_size >= 3:
+        k1 ^= key[tail_index + 2] << 16
+    if tail_size >= 2:
+        k1 ^= key[tail_index + 1] << 8
+    if tail_size >= 1:
+        k1 ^= key[tail_index + 0]
+
+    if tail_size > 0:
+        k1 = (k1 * c1) & 0xFFFFFFFF
+        k1 = (k1 << 15 | k1 >> 17) & 0xFFFFFFFF  # inlined ROTL32
+        k1 = (k1 * c2) & 0xFFFFFFFF
+        h1 ^= k1
+
+    # finalization
+    unsigned_val = fmix(h1 ^ length)
+    if unsigned_val & 0x80000000 == 0:
+        return unsigned_val
+    else:
+        return -((unsigned_val ^ 0xFFFFFFFF) + 1)
+
+
+def hash128(key: bytes, seed: int = 0x0, x64arch: bool = True) -> int:
+    ''' Implements 128bit murmur3 hash. '''
+
+    def hash128_x64(key: bytes, seed: int) -> int:
+        ''' Implements 128bit murmur3 hash for x64. '''
+
+        def fmix(k: int) -> int:
+            k ^= k >> 33
+            k = (k * 0xFF51AFD7ED558CCD) & 0xFFFFFFFFFFFFFFFF
+            k ^= k >> 33
+            k = (k * 0xC4CEB9FE1A85EC53) & 0xFFFFFFFFFFFFFFFF
+            k ^= k >> 33
+            return k
+
+        length = len(key)
+        nblocks = int(length / 16)
+
+        h1 = seed
+        h2 = seed
+
+        c1 = 0x87C37B91114253D5
+        c2 = 0x4CF5AD432745937F
+
+        # body
+        for block_start in range(0, nblocks * 8, 8):
+            # ??? big endian?
+            k1 = (
+                key[2 * block_start + 7] << 56 |
+                key[2 * block_start + 6] << 48 |
+                key[2 * block_start + 5] << 40 |
+                key[2 * block_start + 4] << 32 |
+                key[2 * block_start + 3] << 24 |
+                key[2 * block_start + 2] << 16 |
+                key[2 * block_start + 1] << 8 |
+                key[2 * block_start + 0]
+            )
+
+            k2 = (
+                key[2 * block_start + 15] << 56 |
+                key[2 * block_start + 14] << 48 |
+                key[2 * block_start + 13] << 40 |
+                key[2 * block_start + 12] << 32 |
+                key[2 * block_start + 11] << 24 |
+                key[2 * block_start + 10] << 16 |
+                key[2 * block_start + 9] << 8 |
+                key[2 * block_start + 8]
+            )
+
+            k1 = (c1 * k1) & 0xFFFFFFFFFFFFFFFF
+            k1 = (k1 << 31 | k1 >> 33) & 0xFFFFFFFFFFFFFFFF  # inlined ROTL64
+            k1 = (c2 * k1) & 0xFFFFFFFFFFFFFFFF
+            h1 ^= k1
+
+            h1 = (h1 << 27 | h1 >> 37) & 0xFFFFFFFFFFFFFFFF  # inlined ROTL64
+            h1 = (h1 + h2) & 0xFFFFFFFFFFFFFFFF
+            h1 = (h1 * 5 + 0x52DCE729) & 0xFFFFFFFFFFFFFFFF
+
+            k2 = (c2 * k2) & 0xFFFFFFFFFFFFFFFF
+            k2 = (k2 << 33 | k2 >> 31) & 0xFFFFFFFFFFFFFFFF  # inlined ROTL64
+            k2 = (c1 * k2) & 0xFFFFFFFFFFFFFFFF
+            h2 ^= k2
+
+            h2 = (h2 << 31 | h2 >> 33) & 0xFFFFFFFFFFFFFFFF  # inlined ROTL64
+            h2 = (h1 + h2) & 0xFFFFFFFFFFFFFFFF
+            h2 = (h2 * 5 + 0x38495AB5) & 0xFFFFFFFFFFFFFFFF
+
+        # tail
+        tail_index = nblocks * 16
+        k1 = 0
+        k2 = 0
+        tail_size = length & 15
+
+        if tail_size >= 15:
+            k2 ^= key[tail_index + 14] << 48
+        if tail_size >= 14:
+            k2 ^= key[tail_index + 13] << 40
+        if tail_size >= 13:
+            k2 ^= key[tail_index + 12] << 32
+        if tail_size >= 12:
+            k2 ^= key[tail_index + 11] << 24
+        if tail_size >= 11:
+            k2 ^= key[tail_index + 10] << 16
+        if tail_size >= 10:
+            k2 ^= key[tail_index + 9] << 8
+        if tail_size >= 9:
+            k2 ^= key[tail_index + 8]
+
+        if tail_size > 8:
+            k2 = (k2 * c2) & 0xFFFFFFFFFFFFFFFF
+            k2 = (k2 << 33 | k2 >> 31) & 0xFFFFFFFFFFFFFFFF  # inlined ROTL64
+            k2 = (k2 * c1) & 0xFFFFFFFFFFFFFFFF
+            h2 ^= k2
+
+        if tail_size >= 8:
+            k1 ^= key[tail_index + 7] << 56
+        if tail_size >= 7:
+            k1 ^= key[tail_index + 6] << 48
+        if tail_size >= 6:
+            k1 ^= key[tail_index + 5] << 40
+        if tail_size >= 5:
+            k1 ^= key[tail_index + 4] << 32
+        if tail_size >= 4:
+            k1 ^= key[tail_index + 3] << 24
+        if tail_size >= 3:
+            k1 ^= key[tail_index + 2] << 16
+        if tail_size >= 2:
+            k1 ^= key[tail_index + 1] << 8
+        if tail_size >= 1:
+            k1 ^= key[tail_index + 0]
+
+        if tail_size > 0:
+            k1 = (k1 * c1) & 0xFFFFFFFFFFFFFFFF
+            k1 = (k1 << 31 | k1 >> 33) & 0xFFFFFFFFFFFFFFFF  # inlined ROTL64
+            k1 = (k1 * c2) & 0xFFFFFFFFFFFFFFFF
+            h1 ^= k1
+
+        # finalization
+        h1 ^= length
+        h2 ^= length
+
+        h1 = (h1 + h2) & 0xFFFFFFFFFFFFFFFF
+        h2 = (h1 + h2) & 0xFFFFFFFFFFFFFFFF
+
+        h1 = fmix(h1)
+        h2 = fmix(h2)
+
+        h1 = (h1 + h2) & 0xFFFFFFFFFFFFFFFF
+        h2 = (h1 + h2) & 0xFFFFFFFFFFFFFFFF
+
+        return h2 << 64 | h1
+
+    def hash128_x86(key: bytes, seed: int) -> int:
+        ''' Implements 128bit murmur3 hash for x86. '''
+
+        def fmix(h: int) -> int:
+            h ^= h >> 16
+            h = (h * 0x85EBCA6B) & 0xFFFFFFFF
+            h ^= h >> 13
+            h = (h * 0xC2B2AE35) & 0xFFFFFFFF
+            h ^= h >> 16
+            return h
+
+        length = len(key)
+        nblocks = int(length / 16)
+
+        h1 = seed
+        h2 = seed
+        h3 = seed
+        h4 = seed
+
+        c1 = 0x239B961B
+        c2 = 0xAB0E9789
+        c3 = 0x38B34AE5
+        c4 = 0xA1E38B93
+
+        # body
+        for block_start in range(0, nblocks * 16, 16):
+            k1 = (
+                key[block_start + 3] << 24 |
+                key[block_start + 2] << 16 |
+                key[block_start + 1] << 8 |
+                key[block_start + 0]
+            )
+
+            k2 = (
+                key[block_start + 7] << 24 |
+                key[block_start + 6] << 16 |
+                key[block_start + 5] << 8 |
+                key[block_start + 4]
+            )
+
+            k3 = (
+                key[block_start + 11] << 24 |
+                key[block_start + 10] << 16 |
+                key[block_start + 9] << 8 |
+                key[block_start + 8]
+            )
+
+            k4 = (
+                key[block_start + 15] << 24 |
+                key[block_start + 14] << 16 |
+                key[block_start + 13] << 8 |
+                key[block_start + 12]
+            )
+
+            k1 = (c1 * k1) & 0xFFFFFFFF
+            k1 = (k1 << 15 | k1 >> 17) & 0xFFFFFFFF  # inlined ROTL32
+            k1 = (c2 * k1) & 0xFFFFFFFF
+            h1 ^= k1
+
+            h1 = (h1 << 19 | h1 >> 13) & 0xFFFFFFFF  # inlined ROTL32
+            h1 = (h1 + h2) & 0xFFFFFFFF
+            h1 = (h1 * 5 + 0x561CCD1B) & 0xFFFFFFFF
+
+            k2 = (c2 * k2) & 0xFFFFFFFF
+            k2 = (k2 << 16 | k2 >> 16) & 0xFFFFFFFF  # inlined ROTL32
+            k2 = (c3 * k2) & 0xFFFFFFFF
+            h2 ^= k2
+
+            h2 = (h2 << 17 | h2 >> 15) & 0xFFFFFFFF  # inlined ROTL32
+            h2 = (h2 + h3) & 0xFFFFFFFF
+            h2 = (h2 * 5 + 0x0BCAA747) & 0xFFFFFFFF
+
+            k3 = (c3 * k3) & 0xFFFFFFFF
+            k3 = (k3 << 17 | k3 >> 15) & 0xFFFFFFFF  # inlined ROTL32
+            k3 = (c4 * k3) & 0xFFFFFFFF
+            h3 ^= k3
+
+            h3 = (h3 << 15 | h3 >> 17) & 0xFFFFFFFF  # inlined ROTL32
+            h3 = (h3 + h4) & 0xFFFFFFFF
+            h3 = (h3 * 5 + 0x96CD1C35) & 0xFFFFFFFF
+
+            k4 = (c4 * k4) & 0xFFFFFFFF
+            k4 = (k4 << 18 | k4 >> 14) & 0xFFFFFFFF  # inlined ROTL32
+            k4 = (c1 * k4) & 0xFFFFFFFF
+            h4 ^= k4
+
+            h4 = (h4 << 13 | h4 >> 19) & 0xFFFFFFFF  # inlined ROTL32
+            h4 = (h1 + h4) & 0xFFFFFFFF
+            h4 = (h4 * 5 + 0x32AC3B17) & 0xFFFFFFFF
+
+        # tail
+        tail_index = nblocks * 16
+        k1 = 0
+        k2 = 0
+        k3 = 0
+        k4 = 0
+        tail_size = length & 15
+
+        if tail_size >= 15:
+            k4 ^= key[tail_index + 14] << 16
+        if tail_size >= 14:
+            k4 ^= key[tail_index + 13] << 8
+        if tail_size >= 13:
+            k4 ^= key[tail_index + 12]
+
+        if tail_size > 12:
+            k4 = (k4 * c4) & 0xFFFFFFFF
+            k4 = (k4 << 18 | k4 >> 14) & 0xFFFFFFFF  # inlined ROTL32
+            k4 = (k4 * c1) & 0xFFFFFFFF
+            h4 ^= k4
+
+        if tail_size >= 12:
+            k3 ^= key[tail_index + 11] << 24
+        if tail_size >= 11:
+            k3 ^= key[tail_index + 10] << 16
+        if tail_size >= 10:
+            k3 ^= key[tail_index + 9] << 8
+        if tail_size >= 9:
+            k3 ^= key[tail_index + 8]
+
+        if tail_size > 8:
+            k3 = (k3 * c3) & 0xFFFFFFFF
+            k3 = (k3 << 17 | k3 >> 15) & 0xFFFFFFFF  # inlined ROTL32
+            k3 = (k3 * c4) & 0xFFFFFFFF
+            h3 ^= k3
+
+        if tail_size >= 8:
+            k2 ^= key[tail_index + 7] << 24
+        if tail_size >= 7:
+            k2 ^= key[tail_index + 6] << 16
+        if tail_size >= 6:
+            k2 ^= key[tail_index + 5] << 8
+        if tail_size >= 5:
+            k2 ^= key[tail_index + 4]
+
+        if tail_size > 4:
+            k2 = (k2 * c2) & 0xFFFFFFFF
+            k2 = (k2 << 16 | k2 >> 16) & 0xFFFFFFFF  # inlined ROTL32
+            k2 = (k2 * c3) & 0xFFFFFFFF
+            h2 ^= k2
+
+        if tail_size >= 4:
+            k1 ^= key[tail_index + 3] << 24
+        if tail_size >= 3:
+            k1 ^= key[tail_index + 2] << 16
+        if tail_size >= 2:
+            k1 ^= key[tail_index + 1] << 8
+        if tail_size >= 1:
+            k1 ^= key[tail_index + 0]
+
+        if tail_size > 0:
+            k1 = (k1 * c1) & 0xFFFFFFFF
+            k1 = (k1 << 15 | k1 >> 17) & 0xFFFFFFFF  # inlined ROTL32
+            k1 = (k1 * c2) & 0xFFFFFFFF
+            h1 ^= k1
+
+        # finalization
+        h1 ^= length
+        h2 ^= length
+        h3 ^= length
+        h4 ^= length
+
+        h1 = (h1 + h2) & 0xFFFFFFFF
+        h1 = (h1 + h3) & 0xFFFFFFFF
+        h1 = (h1 + h4) & 0xFFFFFFFF
+        h2 = (h1 + h2) & 0xFFFFFFFF
+        h3 = (h1 + h3) & 0xFFFFFFFF
+        h4 = (h1 + h4) & 0xFFFFFFFF
+
+        h1 = fmix(h1)
+        h2 = fmix(h2)
+        h3 = fmix(h3)
+        h4 = fmix(h4)
+
+        h1 = (h1 + h2) & 0xFFFFFFFF
+        h1 = (h1 + h3) & 0xFFFFFFFF
+        h1 = (h1 + h4) & 0xFFFFFFFF
+        h2 = (h1 + h2) & 0xFFFFFFFF
+        h3 = (h1 + h3) & 0xFFFFFFFF
+        h4 = (h1 + h4) & 0xFFFFFFFF
+
+        return h4 << 96 | h3 << 64 | h2 << 32 | h1
+
+    key = bytearray(xencode(key))
+
+    if x64arch:
+        return hash128_x64(key, seed)
+    else:
+        return hash128_x86(key, seed)
+
+
+def hash64(key: bytes, seed: int = 0x0, x64arch: bool = True) -> tuple[int, int]:
+    ''' Implements 64bit murmur3 hash. Returns a tuple. '''
+
+    hash_128 = hash128(key, seed, x64arch)
+
+    unsigned_val1 = hash_128 & 0xFFFFFFFFFFFFFFFF
+    if unsigned_val1 & 0x8000000000000000 == 0:
+        signed_val1 = unsigned_val1
+    else:
+        signed_val1 = -((unsigned_val1 ^ 0xFFFFFFFFFFFFFFFF) + 1)
+
+    unsigned_val2 = (hash_128 >> 64) & 0xFFFFFFFFFFFFFFFF
+    if unsigned_val2 & 0x8000000000000000 == 0:
+        signed_val2 = unsigned_val2
+    else:
+        signed_val2 = -((unsigned_val2 ^ 0xFFFFFFFFFFFFFFFF) + 1)
+
+    return (int(signed_val1), int(signed_val2))
+
+
+def hash_bytes(key: bytes, seed: int = 0x0, x64arch: bool = True) -> str:
+    ''' Implements 128bit murmur3 hash. Returns a byte string. '''
+
+    hash_128 = hash128(key, seed, x64arch)
+
+    bytestring = ''
+
+    for i in range(0, 16, 1):
+        lsbyte = hash_128 & 0xFF
+        bytestring = bytestring + str(chr(lsbyte))
+        hash_128 = hash_128 >> 8
+
+    return bytestring
+
+
+if __name__ == "__main__":
+    import argparse
+    import sys
+
+    parser = argparse.ArgumentParser('pymurmur3', 'pymurmur [options] "string to hash"')
+    parser.add_argument('--seed', type=int, default=0)
+    parser.add_argument('strings', default=[], nargs='+')
+
+    opts = parser.parse_args()
+
+    for str_to_hash in opts.strings:
+        sys.stdout.write(f'"{str_to_hash}" = 0x{hash(str_to_hash):08X}\n')
```

### Comparing `optimizely-sdk-4.1.1/optimizely/notification_center.py` & `optimizely-sdk-5.0.0b0/optimizely/notification_center.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,134 +1,142 @@
-# Copyright 2017-2019, Optimizely
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from .helpers import enums
-from . import logger as optimizely_logger
-
-
-NOTIFICATION_TYPES = tuple(
-    getattr(enums.NotificationTypes, attr) for attr in dir(enums.NotificationTypes) if not attr.startswith('__')
-)
-
-
-class NotificationCenter(object):
-    """ Class encapsulating methods to manage notifications and their listeners.
-  The enums.NotificationTypes includes predefined notifications."""
-
-    def __init__(self, logger=None):
-        self.listener_id = 1
-        self.notification_listeners = {}
-        for notification_type in NOTIFICATION_TYPES:
-            self.notification_listeners[notification_type] = []
-        self.logger = optimizely_logger.adapt_logger(logger or optimizely_logger.NoOpLogger())
-
-    def add_notification_listener(self, notification_type, notification_callback):
-        """ Add a notification callback to the notification center for a given notification type.
-
-    Args:
-      notification_type: A string representing the notification type from helpers.enums.NotificationTypes
-      notification_callback: Closure of function to call when event is triggered.
-
-    Returns:
-      Integer notification ID used to remove the notification or
-      -1 if the notification listener has already been added or
-      if the notification type is invalid.
-    """
-
-        if notification_type not in NOTIFICATION_TYPES:
-            self.logger.error('Invalid notification_type: {} provided. Not adding listener.'.format(notification_type))
-            return -1
-
-        for _, listener in self.notification_listeners[notification_type]:
-            if listener == notification_callback:
-                self.logger.error('Listener has already been added. Not adding it again.')
-                return -1
-
-        self.notification_listeners[notification_type].append((self.listener_id, notification_callback))
-        current_listener_id = self.listener_id
-        self.listener_id += 1
-
-        return current_listener_id
-
-    def remove_notification_listener(self, notification_id):
-        """ Remove a previously added notification callback.
-
-    Args:
-      notification_id: The numeric id passed back from add_notification_listener
-
-    Returns:
-      The function returns boolean true if found and removed, false otherwise.
-    """
-
-        for listener in self.notification_listeners.values():
-            listener_to_remove = list(filter(lambda tup: tup[0] == notification_id, listener))
-            if len(listener_to_remove) > 0:
-                listener.remove(listener_to_remove[0])
-                return True
-
-        return False
-
-    def clear_notification_listeners(self, notification_type):
-        """ Remove notification listeners for a certain notification type.
-
-    Args:
-      notification_type: String denoting notification type.
-    """
-
-        if notification_type not in NOTIFICATION_TYPES:
-            self.logger.error(
-                'Invalid notification_type: {} provided. Not removing any listener.'.format(notification_type)
-            )
-        self.notification_listeners[notification_type] = []
-
-    def clear_notifications(self, notification_type):
-        """ (DEPRECATED since 3.2.0, use clear_notification_listeners)
-    Remove notification listeners for a certain notification type.
-
-    Args:
-      notification_type: key to the list of notifications .helpers.enums.NotificationTypes
-    """
-        self.clear_notification_listeners(notification_type)
-
-    def clear_all_notification_listeners(self):
-        """ Remove all notification listeners. """
-        for notification_type in self.notification_listeners.keys():
-            self.clear_notification_listeners(notification_type)
-
-    def clear_all_notifications(self):
-        """ (DEPRECATED since 3.2.0, use clear_all_notification_listeners)
-    Remove all notification listeners. """
-        self.clear_all_notification_listeners()
-
-    def send_notifications(self, notification_type, *args):
-        """ Fires off the notification for the specific event.  Uses var args to pass in a
-        arbitrary list of parameter according to which notification type was fired.
-
-    Args:
-      notification_type: Type of notification to fire (String from .helpers.enums.NotificationTypes)
-      args: Variable list of arguments to the callback.
-    """
-
-        if notification_type not in NOTIFICATION_TYPES:
-            self.logger.error(
-                'Invalid notification_type: {} provided. ' 'Not triggering any notification.'.format(notification_type)
-            )
-            return
-
-        if notification_type in self.notification_listeners:
-            for notification_id, callback in self.notification_listeners[notification_type]:
-                try:
-                    callback(*args)
-                except:
-                    self.logger.exception(
-                        'Unknown problem when sending "{}" type notification.'.format(notification_type)
-                    )
+# Copyright 2017-2019, 2022, Optimizely
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from __future__ import annotations
+from typing import Any, Callable, Optional
+from .helpers import enums
+from . import logger as optimizely_logger
+from sys import version_info
+
+if version_info < (3, 8):
+    from typing_extensions import Final
+else:
+    from typing import Final  # type: ignore
+
+
+NOTIFICATION_TYPES: Final = tuple(
+    getattr(enums.NotificationTypes, attr) for attr in dir(enums.NotificationTypes) if not attr.startswith('__')
+)
+
+
+class NotificationCenter:
+    """ Class encapsulating methods to manage notifications and their listeners.
+  The enums.NotificationTypes includes predefined notifications."""
+
+    def __init__(self, logger: Optional[optimizely_logger.Logger] = None):
+        self.listener_id = 1
+        self.notification_listeners: dict[str, list[tuple[int, Callable[..., None]]]] = {}
+        for notification_type in NOTIFICATION_TYPES:
+            self.notification_listeners[notification_type] = []
+        self.logger = optimizely_logger.adapt_logger(logger or optimizely_logger.NoOpLogger())
+
+    def add_notification_listener(self, notification_type: str, notification_callback: Callable[..., None]) -> int:
+        """ Add a notification callback to the notification center for a given notification type.
+
+    Args:
+      notification_type: A string representing the notification type from helpers.enums.NotificationTypes
+      notification_callback: Closure of function to call when event is triggered.
+
+    Returns:
+      Integer notification ID used to remove the notification or
+      -1 if the notification listener has already been added or
+      if the notification type is invalid.
+    """
+
+        if notification_type not in NOTIFICATION_TYPES:
+            self.logger.error(f'Invalid notification_type: {notification_type} provided. Not adding listener.')
+            return -1
+
+        for _, listener in self.notification_listeners[notification_type]:
+            if listener == notification_callback:
+                self.logger.error('Listener has already been added. Not adding it again.')
+                return -1
+
+        self.notification_listeners[notification_type].append((self.listener_id, notification_callback))
+        current_listener_id = self.listener_id
+        self.listener_id += 1
+
+        return current_listener_id
+
+    def remove_notification_listener(self, notification_id: int) -> bool:
+        """ Remove a previously added notification callback.
+
+    Args:
+      notification_id: The numeric id passed back from add_notification_listener
+
+    Returns:
+      The function returns boolean true if found and removed, false otherwise.
+    """
+
+        for listener in self.notification_listeners.values():
+            listener_to_remove = list(filter(lambda tup: tup[0] == notification_id, listener))
+            if len(listener_to_remove) > 0:
+                listener.remove(listener_to_remove[0])
+                return True
+
+        return False
+
+    def clear_notification_listeners(self, notification_type: str) -> None:
+        """ Remove notification listeners for a certain notification type.
+
+    Args:
+      notification_type: String denoting notification type.
+    """
+
+        if notification_type not in NOTIFICATION_TYPES:
+            self.logger.error(
+                f'Invalid notification_type: {notification_type} provided. Not removing any listener.'
+            )
+        self.notification_listeners[notification_type] = []
+
+    def clear_notifications(self, notification_type: str) -> None:
+        """ (DEPRECATED since 3.2.0, use clear_notification_listeners)
+    Remove notification listeners for a certain notification type.
+
+    Args:
+      notification_type: key to the list of notifications .helpers.enums.NotificationTypes
+    """
+        self.clear_notification_listeners(notification_type)
+
+    def clear_all_notification_listeners(self) -> None:
+        """ Remove all notification listeners. """
+        for notification_type in self.notification_listeners.keys():
+            self.clear_notification_listeners(notification_type)
+
+    def clear_all_notifications(self) -> None:
+        """ (DEPRECATED since 3.2.0, use clear_all_notification_listeners)
+    Remove all notification listeners. """
+        self.clear_all_notification_listeners()
+
+    def send_notifications(self, notification_type: str, *args: Any) -> None:
+        """ Fires off the notification for the specific event.  Uses var args to pass in a
+        arbitrary list of parameter according to which notification type was fired.
+
+    Args:
+      notification_type: Type of notification to fire (String from .helpers.enums.NotificationTypes)
+      args: Variable list of arguments to the callback.
+    """
+
+        if notification_type not in NOTIFICATION_TYPES:
+            self.logger.error(
+                f'Invalid notification_type: {notification_type} provided. ' 'Not triggering any notification.'
+            )
+            return
+
+        if notification_type in self.notification_listeners:
+            for notification_id, callback in self.notification_listeners[notification_type]:
+                try:
+                    callback(*args)
+                except:
+                    self.logger.exception(
+                        f'Unknown problem when sending "{notification_type}" type notification.'
+                    )
```

### Comparing `optimizely-sdk-4.1.1/optimizely/optimizely.py` & `optimizely-sdk-5.0.0b0/optimizely/optimizely.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,1187 +1,1424 @@
-# Copyright 2016-2022, Optimizely
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from six import string_types
-
-from . import decision_service
-from . import entities
-from . import event_builder
-from . import exceptions
-from . import logger as _logging
-from .config_manager import AuthDatafilePollingConfigManager
-from .config_manager import PollingConfigManager
-from .config_manager import StaticConfigManager
-from .decision.optimizely_decide_option import OptimizelyDecideOption
-from .decision.optimizely_decision import OptimizelyDecision
-from .decision.optimizely_decision_message import OptimizelyDecisionMessage
-from .decision_service import Decision
-from .error_handler import NoOpErrorHandler as noop_error_handler
-from .event import event_factory, user_event_factory
-from .event.event_processor import ForwardingEventProcessor
-from .event_dispatcher import EventDispatcher as default_event_dispatcher
-from .helpers import enums, validator
-from .helpers.enums import DecisionSources
-from .notification_center import NotificationCenter
-from .optimizely_config import OptimizelyConfigService
-from .optimizely_user_context import OptimizelyUserContext
-
-
-class Optimizely(object):
-    """ Class encapsulating all SDK functionality. """
-
-    def __init__(
-            self,
-            datafile=None,
-            event_dispatcher=None,
-            logger=None,
-            error_handler=None,
-            skip_json_validation=False,
-            user_profile_service=None,
-            sdk_key=None,
-            config_manager=None,
-            notification_center=None,
-            event_processor=None,
-            datafile_access_token=None,
-            default_decide_options=None
-    ):
-        """ Optimizely init method for managing Custom projects.
-
-        Args:
-          datafile: Optional JSON string representing the project. Must provide at least one of datafile or sdk_key.
-          event_dispatcher: Provides a dispatch_event method which if given a URL and params sends a request to it.
-          logger: Optional component which provides a log method to log messages. By default nothing would be logged.
-          error_handler: Optional component which provides a handle_error method to handle exceptions.
-                         By default all exceptions will be suppressed.
-          skip_json_validation: Optional boolean param which allows skipping JSON schema validation upon object
-          invocation.
-                                By default JSON schema validation will be performed.
-          user_profile_service: Optional component which provides methods to store and manage user profiles.
-          sdk_key: Optional string uniquely identifying the datafile corresponding to project and environment
-          combination.
-                   Must provide at least one of datafile or sdk_key.
-          config_manager: Optional component which implements optimizely.config_manager.BaseConfigManager.
-          notification_center: Optional instance of notification_center.NotificationCenter. Useful when providing own
-                               config_manager.BaseConfigManager implementation which can be using the
-                               same NotificationCenter instance.
-          event_processor: Optional component which processes the given event(s).
-                           By default optimizely.event.event_processor.ForwardingEventProcessor is used
-                           which simply forwards events to the event dispatcher.
-                           To enable event batching configure and use
-                           optimizely.event.event_processor.BatchEventProcessor.
-          datafile_access_token: Optional string used to fetch authenticated datafile for a secure project environment.
-          default_decide_options: Optional list of decide options used with the decide APIs.
-        """
-        self.logger_name = '.'.join([__name__, self.__class__.__name__])
-        self.is_valid = True
-        self.event_dispatcher = event_dispatcher or default_event_dispatcher
-        self.logger = _logging.adapt_logger(logger or _logging.NoOpLogger())
-        self.error_handler = error_handler or noop_error_handler
-        self.config_manager = config_manager
-        self.notification_center = notification_center or NotificationCenter(self.logger)
-        self.event_processor = event_processor or ForwardingEventProcessor(
-            self.event_dispatcher, logger=self.logger, notification_center=self.notification_center,
-        )
-
-        if default_decide_options is None:
-            self.default_decide_options = []
-        else:
-            self.default_decide_options = default_decide_options
-
-        if isinstance(self.default_decide_options, list):
-            self.default_decide_options = self.default_decide_options[:]
-        else:
-            self.logger.debug('Provided default decide options is not a list.')
-            self.default_decide_options = []
-
-        try:
-            self._validate_instantiation_options()
-        except exceptions.InvalidInputException as error:
-            self.is_valid = False
-            # We actually want to log this error to stderr, so make sure the logger
-            # has a handler capable of doing that.
-            self.logger = _logging.reset_logger(self.logger_name)
-            self.logger.exception(str(error))
-            return
-
-        config_manager_options = {
-            'datafile': datafile,
-            'logger': self.logger,
-            'error_handler': self.error_handler,
-            'notification_center': self.notification_center,
-            'skip_json_validation': skip_json_validation,
-        }
-
-        if not self.config_manager:
-            if sdk_key:
-                config_manager_options['sdk_key'] = sdk_key
-                if datafile_access_token:
-                    config_manager_options['datafile_access_token'] = datafile_access_token
-                    self.config_manager = AuthDatafilePollingConfigManager(**config_manager_options)
-                else:
-                    self.config_manager = PollingConfigManager(**config_manager_options)
-            else:
-                self.config_manager = StaticConfigManager(**config_manager_options)
-
-        self.event_builder = event_builder.EventBuilder()
-        self.decision_service = decision_service.DecisionService(self.logger, user_profile_service)
-
-    def _validate_instantiation_options(self):
-        """ Helper method to validate all instantiation parameters.
-
-        Raises:
-          Exception if provided instantiation options are valid.
-        """
-        if self.config_manager and not validator.is_config_manager_valid(self.config_manager):
-            raise exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('config_manager'))
-
-        if not validator.is_event_dispatcher_valid(self.event_dispatcher):
-            raise exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('event_dispatcher'))
-
-        if not validator.is_logger_valid(self.logger):
-            raise exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('logger'))
-
-        if not validator.is_error_handler_valid(self.error_handler):
-            raise exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('error_handler'))
-
-        if not validator.is_notification_center_valid(self.notification_center):
-            raise exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('notification_center'))
-
-        if not validator.is_event_processor_valid(self.event_processor):
-            raise exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('event_processor'))
-
-    def _validate_user_inputs(self, attributes=None, event_tags=None):
-        """ Helper method to validate user inputs.
-
-        Args:
-          attributes: Dict representing user attributes.
-          event_tags: Dict representing metadata associated with an event.
-
-        Returns:
-          Boolean True if inputs are valid. False otherwise.
-
-        """
-
-        if attributes and not validator.are_attributes_valid(attributes):
-            self.logger.error('Provided attributes are in an invalid format.')
-            self.error_handler.handle_error(exceptions.InvalidAttributeException(enums.Errors.INVALID_ATTRIBUTE_FORMAT))
-            return False
-
-        if event_tags and not validator.are_event_tags_valid(event_tags):
-            self.logger.error('Provided event tags are in an invalid format.')
-            self.error_handler.handle_error(exceptions.InvalidEventTagException(enums.Errors.INVALID_EVENT_TAG_FORMAT))
-            return False
-
-        return True
-
-    def _send_impression_event(self, project_config, experiment, variation, flag_key, rule_key, rule_type, enabled,
-                               user_id, attributes):
-        """ Helper method to send impression event.
-
-        Args:
-          project_config: Instance of ProjectConfig.
-          experiment: Experiment for which impression event is being sent.
-          variation: Variation picked for user for the given experiment.
-          flag_key: key for a feature flag.
-          rule_key: key for an experiment.
-          rule_type: type for the source.
-          enabled: boolean representing if feature is enabled
-          user_id: ID for user.
-          attributes: Dict representing user attributes and values which need to be recorded.
-        """
-        if not experiment:
-            experiment = entities.Experiment.get_default()
-
-        variation_id = variation.id if variation is not None else None
-        user_event = user_event_factory.UserEventFactory.create_impression_event(
-            project_config, experiment, variation_id, flag_key, rule_key, rule_type, enabled, user_id, attributes
-        )
-
-        self.event_processor.process(user_event)
-
-        # Kept for backward compatibility.
-        # This notification is deprecated and new Decision notifications
-        # are sent via their respective method calls.
-        if len(self.notification_center.notification_listeners[enums.NotificationTypes.ACTIVATE]) > 0:
-            log_event = event_factory.EventFactory.create_log_event(user_event, self.logger)
-            self.notification_center.send_notifications(
-                enums.NotificationTypes.ACTIVATE, experiment, user_id, attributes, variation, log_event.__dict__,
-            )
-
-    def _get_feature_variable_for_type(
-            self, project_config, feature_key, variable_key, variable_type, user_id, attributes
-    ):
-        """ Helper method to determine value for a certain variable attached to a feature flag based on type of variable.
-
-        Args:
-          project_config: Instance of ProjectConfig.
-          feature_key: Key of the feature whose variable's value is being accessed.
-          variable_key: Key of the variable whose value is to be accessed.
-          variable_type: Type of variable which could be one of boolean/double/integer/string.
-          user_id: ID for user.
-          attributes: Dict representing user attributes.
-
-        Returns:
-          Value of the variable. None if:
-          - Feature key is invalid.
-          - Variable key is invalid.
-          - Mismatch with type of variable.
-        """
-        if not validator.is_non_empty_string(feature_key):
-            self.logger.error(enums.Errors.INVALID_INPUT.format('feature_key'))
-            return None
-
-        if not validator.is_non_empty_string(variable_key):
-            self.logger.error(enums.Errors.INVALID_INPUT.format('variable_key'))
-            return None
-
-        if not isinstance(user_id, string_types):
-            self.logger.error(enums.Errors.INVALID_INPUT.format('user_id'))
-            return None
-
-        if not self._validate_user_inputs(attributes):
-            return None
-
-        feature_flag = project_config.get_feature_from_key(feature_key)
-        if not feature_flag:
-            return None
-
-        variable = project_config.get_variable_for_feature(feature_key, variable_key)
-        if not variable:
-            return None
-
-        # For non-typed method, use type of variable; else, return None if type differs
-        variable_type = variable_type or variable.type
-        if variable.type != variable_type:
-            self.logger.warning(
-                'Requested variable type "%s", but variable is of type "%s". '
-                'Use correct API to retrieve value. Returning None.' % (variable_type, variable.type)
-            )
-            return None
-
-        feature_enabled = False
-        source_info = {}
-        variable_value = variable.defaultValue
-
-        user_context = self.create_user_context(user_id, attributes)
-        decision, _ = self.decision_service.get_variation_for_feature(project_config, feature_flag, user_context)
-
-        if decision.variation:
-
-            feature_enabled = decision.variation.featureEnabled
-            if feature_enabled:
-                variable_value = project_config.get_variable_value_for_variation(variable, decision.variation)
-                self.logger.info(
-                    'Got variable value "%s" for variable "%s" of feature flag "%s".'
-                    % (variable_value, variable_key, feature_key)
-                )
-            else:
-                self.logger.info(
-                    'Feature "%s" is not enabled for user "%s". '
-                    'Returning the default variable value "%s".' % (feature_key, user_id, variable_value)
-                )
-        else:
-            self.logger.info(
-                'User "%s" is not in any variation or rollout rule. '
-                'Returning default value for variable "%s" of feature flag "%s".' % (user_id, variable_key, feature_key)
-            )
-
-        if decision.source == enums.DecisionSources.FEATURE_TEST:
-            source_info = {
-                'experiment_key': decision.experiment.key,
-                'variation_key': decision.variation.key,
-            }
-
-        try:
-            actual_value = project_config.get_typecast_value(variable_value, variable_type)
-        except:
-            self.logger.error('Unable to cast value. Returning None.')
-            actual_value = None
-
-        self.notification_center.send_notifications(
-            enums.NotificationTypes.DECISION,
-            enums.DecisionNotificationTypes.FEATURE_VARIABLE,
-            user_id,
-            attributes or {},
-            {
-                'feature_key': feature_key,
-                'feature_enabled': feature_enabled,
-                'source': decision.source,
-                'variable_key': variable_key,
-                'variable_value': actual_value,
-                'variable_type': variable_type,
-                'source_info': source_info,
-            },
-        )
-        return actual_value
-
-    def _get_all_feature_variables_for_type(
-            self, project_config, feature_key, user_id, attributes,
-    ):
-        """ Helper method to determine value for all variables attached to a feature flag.
-
-        Args:
-          project_config: Instance of ProjectConfig.
-          feature_key: Key of the feature whose variable's value is being accessed.
-          user_id: ID for user.
-          attributes: Dict representing user attributes.
-
-        Returns:
-          Dictionary of all variables. None if:
-          - Feature key is invalid.
-        """
-        if not validator.is_non_empty_string(feature_key):
-            self.logger.error(enums.Errors.INVALID_INPUT.format('feature_key'))
-            return None
-
-        if not isinstance(user_id, string_types):
-            self.logger.error(enums.Errors.INVALID_INPUT.format('user_id'))
-            return None
-
-        if not self._validate_user_inputs(attributes):
-            return None
-
-        feature_flag = project_config.get_feature_from_key(feature_key)
-        if not feature_flag:
-            return None
-
-        feature_enabled = False
-        source_info = {}
-
-        user_context = self.create_user_context(user_id, attributes)
-        decision, _ = self.decision_service.get_variation_for_feature(project_config, feature_flag, user_context)
-
-        if decision.variation:
-
-            feature_enabled = decision.variation.featureEnabled
-            if feature_enabled:
-                self.logger.info(
-                    'Feature "%s" is enabled for user "%s".' % (feature_key, user_id)
-                )
-            else:
-                self.logger.info(
-                    'Feature "%s" is not enabled for user "%s".' % (feature_key, user_id)
-                )
-        else:
-            self.logger.info(
-                'User "%s" is not in any variation or rollout rule. '
-                'Returning default value for all variables of feature flag "%s".' % (user_id, feature_key)
-            )
-
-        all_variables = {}
-        for variable_key in feature_flag.variables:
-            variable = project_config.get_variable_for_feature(feature_key, variable_key)
-            variable_value = variable.defaultValue
-            if feature_enabled:
-                variable_value = project_config.get_variable_value_for_variation(variable, decision.variation)
-                self.logger.debug(
-                    'Got variable value "%s" for variable "%s" of feature flag "%s".'
-                    % (variable_value, variable_key, feature_key)
-                )
-
-            try:
-                actual_value = project_config.get_typecast_value(variable_value, variable.type)
-            except:
-                self.logger.error('Unable to cast value. Returning None.')
-                actual_value = None
-
-            all_variables[variable_key] = actual_value
-
-        if decision.source == enums.DecisionSources.FEATURE_TEST:
-            source_info = {
-                'experiment_key': decision.experiment.key,
-                'variation_key': decision.variation.key,
-            }
-
-        self.notification_center.send_notifications(
-            enums.NotificationTypes.DECISION,
-            enums.DecisionNotificationTypes.ALL_FEATURE_VARIABLES,
-            user_id,
-            attributes or {},
-            {
-                'feature_key': feature_key,
-                'feature_enabled': feature_enabled,
-                'variable_values': all_variables,
-                'source': decision.source,
-                'source_info': source_info,
-            },
-        )
-        return all_variables
-
-    def activate(self, experiment_key, user_id, attributes=None):
-        """ Buckets visitor and sends impression event to Optimizely.
-
-        Args:
-          experiment_key: Experiment which needs to be activated.
-          user_id: ID for user.
-          attributes: Dict representing user attributes and values which need to be recorded.
-
-        Returns:
-          Variation key representing the variation the user will be bucketed in.
-          None if user is not in experiment or if experiment is not Running.
-        """
-
-        if not self.is_valid:
-            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('activate'))
-            return None
-
-        if not validator.is_non_empty_string(experiment_key):
-            self.logger.error(enums.Errors.INVALID_INPUT.format('experiment_key'))
-            return None
-
-        if not isinstance(user_id, string_types):
-            self.logger.error(enums.Errors.INVALID_INPUT.format('user_id'))
-            return None
-
-        project_config = self.config_manager.get_config()
-        if not project_config:
-            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('activate'))
-            return None
-
-        variation_key = self.get_variation(experiment_key, user_id, attributes)
-
-        if not variation_key:
-            self.logger.info('Not activating user "%s".' % user_id)
-            return None
-
-        experiment = project_config.get_experiment_from_key(experiment_key)
-        variation = project_config.get_variation_from_key(experiment_key, variation_key)
-
-        # Create and dispatch impression event
-        self.logger.info('Activating user "%s" in experiment "%s".' % (user_id, experiment.key))
-        self._send_impression_event(project_config, experiment, variation, '', experiment.key,
-                                    enums.DecisionSources.EXPERIMENT, True, user_id, attributes)
-
-        return variation.key
-
-    def track(self, event_key, user_id, attributes=None, event_tags=None):
-        """ Send conversion event to Optimizely.
-
-        Args:
-          event_key: Event key representing the event which needs to be recorded.
-          user_id: ID for user.
-          attributes: Dict representing visitor attributes and values which need to be recorded.
-          event_tags: Dict representing metadata associated with the event.
-        """
-
-        if not self.is_valid:
-            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('track'))
-            return
-
-        if not validator.is_non_empty_string(event_key):
-            self.logger.error(enums.Errors.INVALID_INPUT.format('event_key'))
-            return
-
-        if not isinstance(user_id, string_types):
-            self.logger.error(enums.Errors.INVALID_INPUT.format('user_id'))
-            return
-
-        if not self._validate_user_inputs(attributes, event_tags):
-            return
-
-        project_config = self.config_manager.get_config()
-        if not project_config:
-            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('track'))
-            return
-
-        event = project_config.get_event(event_key)
-        if not event:
-            self.logger.info('Not tracking user "%s" for event "%s".' % (user_id, event_key))
-            return
-
-        user_event = user_event_factory.UserEventFactory.create_conversion_event(
-            project_config, event_key, user_id, attributes, event_tags
-        )
-
-        self.event_processor.process(user_event)
-        self.logger.info('Tracking event "%s" for user "%s".' % (event_key, user_id))
-
-        if len(self.notification_center.notification_listeners[enums.NotificationTypes.TRACK]) > 0:
-            log_event = event_factory.EventFactory.create_log_event(user_event, self.logger)
-            self.notification_center.send_notifications(
-                enums.NotificationTypes.TRACK, event_key, user_id, attributes, event_tags, log_event.__dict__,
-            )
-
-    def get_variation(self, experiment_key, user_id, attributes=None):
-        """ Gets variation where user will be bucketed.
-
-        Args:
-          experiment_key: Experiment for which user variation needs to be determined.
-          user_id: ID for user.
-          attributes: Dict representing user attributes.
-
-        Returns:
-          Variation key representing the variation the user will be bucketed in.
-          None if user is not in experiment or if experiment is not Running.
-        """
-
-        if not self.is_valid:
-            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('get_variation'))
-            return None
-
-        if not validator.is_non_empty_string(experiment_key):
-            self.logger.error(enums.Errors.INVALID_INPUT.format('experiment_key'))
-            return None
-
-        if not isinstance(user_id, string_types):
-            self.logger.error(enums.Errors.INVALID_INPUT.format('user_id'))
-            return None
-
-        project_config = self.config_manager.get_config()
-        if not project_config:
-            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('get_variation'))
-            return None
-
-        experiment = project_config.get_experiment_from_key(experiment_key)
-        variation_key = None
-
-        if not experiment:
-            self.logger.info('Experiment key "%s" is invalid. Not activating user "%s".' % (experiment_key, user_id))
-            return None
-
-        if not self._validate_user_inputs(attributes):
-            return None
-
-        user_context = self.create_user_context(user_id, attributes)
-
-        variation, _ = self.decision_service.get_variation(project_config, experiment, user_context)
-        if variation:
-            variation_key = variation.key
-
-        if project_config.is_feature_experiment(experiment.id):
-            decision_notification_type = enums.DecisionNotificationTypes.FEATURE_TEST
-        else:
-            decision_notification_type = enums.DecisionNotificationTypes.AB_TEST
-
-        self.notification_center.send_notifications(
-            enums.NotificationTypes.DECISION,
-            decision_notification_type,
-            user_id,
-            attributes or {},
-            {'experiment_key': experiment_key, 'variation_key': variation_key},
-        )
-
-        return variation_key
-
-    def is_feature_enabled(self, feature_key, user_id, attributes=None):
-        """ Returns true if the feature is enabled for the given user.
-
-        Args:
-          feature_key: The key of the feature for which we are determining if it is enabled or not for the given user.
-          user_id: ID for user.
-          attributes: Dict representing user attributes.
-
-        Returns:
-          True if the feature is enabled for the user. False otherwise.
-        """
-
-        if not self.is_valid:
-            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('is_feature_enabled'))
-            return False
-
-        if not validator.is_non_empty_string(feature_key):
-            self.logger.error(enums.Errors.INVALID_INPUT.format('feature_key'))
-            return False
-
-        if not isinstance(user_id, string_types):
-            self.logger.error(enums.Errors.INVALID_INPUT.format('user_id'))
-            return False
-
-        if not self._validate_user_inputs(attributes):
-            return False
-
-        project_config = self.config_manager.get_config()
-        if not project_config:
-            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('is_feature_enabled'))
-            return False
-
-        feature = project_config.get_feature_from_key(feature_key)
-        if not feature:
-            return False
-
-        feature_enabled = False
-        source_info = {}
-        user_context = self.create_user_context(user_id, attributes)
-        decision, _ = self.decision_service.get_variation_for_feature(project_config, feature, user_context)
-        is_source_experiment = decision.source == enums.DecisionSources.FEATURE_TEST
-        is_source_rollout = decision.source == enums.DecisionSources.ROLLOUT
-
-        if decision.variation:
-            if decision.variation.featureEnabled is True:
-                feature_enabled = True
-
-        if (is_source_rollout or not decision.variation) and project_config.get_send_flag_decisions_value():
-            self._send_impression_event(
-                project_config, decision.experiment, decision.variation, feature.key, decision.experiment.key if
-                decision.experiment else '', decision.source, feature_enabled, user_id, attributes
-            )
-
-        # Send event if Decision came from an experiment.
-        if is_source_experiment and decision.variation:
-            source_info = {
-                'experiment_key': decision.experiment.key,
-                'variation_key': decision.variation.key,
-            }
-            self._send_impression_event(
-                project_config, decision.experiment, decision.variation, feature.key, decision.experiment.key,
-                decision.source, feature_enabled, user_id, attributes
-            )
-
-        if feature_enabled:
-            self.logger.info('Feature "%s" is enabled for user "%s".' % (feature_key, user_id))
-        else:
-            self.logger.info('Feature "%s" is not enabled for user "%s".' % (feature_key, user_id))
-
-        self.notification_center.send_notifications(
-            enums.NotificationTypes.DECISION,
-            enums.DecisionNotificationTypes.FEATURE,
-            user_id,
-            attributes or {},
-            {
-                'feature_key': feature_key,
-                'feature_enabled': feature_enabled,
-                'source': decision.source,
-                'source_info': source_info,
-            },
-        )
-
-        return feature_enabled
-
-    def get_enabled_features(self, user_id, attributes=None):
-        """ Returns the list of features that are enabled for the user.
-
-        Args:
-          user_id: ID for user.
-          attributes: Dict representing user attributes.
-
-        Returns:
-          A list of the keys of the features that are enabled for the user.
-        """
-
-        enabled_features = []
-        if not self.is_valid:
-            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('get_enabled_features'))
-            return enabled_features
-
-        if not isinstance(user_id, string_types):
-            self.logger.error(enums.Errors.INVALID_INPUT.format('user_id'))
-            return enabled_features
-
-        if not self._validate_user_inputs(attributes):
-            return enabled_features
-
-        project_config = self.config_manager.get_config()
-        if not project_config:
-            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('get_enabled_features'))
-            return enabled_features
-
-        for feature in project_config.feature_key_map.values():
-            if self.is_feature_enabled(feature.key, user_id, attributes):
-                enabled_features.append(feature.key)
-
-        return enabled_features
-
-    def get_feature_variable(self, feature_key, variable_key, user_id, attributes=None):
-        """ Returns value for a variable attached to a feature flag.
-
-        Args:
-          feature_key: Key of the feature whose variable's value is being accessed.
-          variable_key: Key of the variable whose value is to be accessed.
-          user_id: ID for user.
-          attributes: Dict representing user attributes.
-
-        Returns:
-          Value of the variable. None if:
-          - Feature key is invalid.
-          - Variable key is invalid.
-        """
-        project_config = self.config_manager.get_config()
-        if not project_config:
-            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('get_feature_variable'))
-            return None
-
-        return self._get_feature_variable_for_type(project_config, feature_key, variable_key, None, user_id, attributes)
-
-    def get_feature_variable_boolean(self, feature_key, variable_key, user_id, attributes=None):
-        """ Returns value for a certain boolean variable attached to a feature flag.
-
-        Args:
-          feature_key: Key of the feature whose variable's value is being accessed.
-          variable_key: Key of the variable whose value is to be accessed.
-          user_id: ID for user.
-          attributes: Dict representing user attributes.
-
-        Returns:
-          Boolean value of the variable. None if:
-          - Feature key is invalid.
-          - Variable key is invalid.
-          - Mismatch with type of variable.
-        """
-
-        variable_type = entities.Variable.Type.BOOLEAN
-        project_config = self.config_manager.get_config()
-        if not project_config:
-            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('get_feature_variable_boolean'))
-            return None
-
-        return self._get_feature_variable_for_type(
-            project_config, feature_key, variable_key, variable_type, user_id, attributes,
-        )
-
-    def get_feature_variable_double(self, feature_key, variable_key, user_id, attributes=None):
-        """ Returns value for a certain double variable attached to a feature flag.
-
-        Args:
-          feature_key: Key of the feature whose variable's value is being accessed.
-          variable_key: Key of the variable whose value is to be accessed.
-          user_id: ID for user.
-          attributes: Dict representing user attributes.
-
-        Returns:
-          Double value of the variable. None if:
-          - Feature key is invalid.
-          - Variable key is invalid.
-          - Mismatch with type of variable.
-        """
-
-        variable_type = entities.Variable.Type.DOUBLE
-        project_config = self.config_manager.get_config()
-        if not project_config:
-            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('get_feature_variable_double'))
-            return None
-
-        return self._get_feature_variable_for_type(
-            project_config, feature_key, variable_key, variable_type, user_id, attributes,
-        )
-
-    def get_feature_variable_integer(self, feature_key, variable_key, user_id, attributes=None):
-        """ Returns value for a certain integer variable attached to a feature flag.
-
-        Args:
-          feature_key: Key of the feature whose variable's value is being accessed.
-          variable_key: Key of the variable whose value is to be accessed.
-          user_id: ID for user.
-          attributes: Dict representing user attributes.
-
-        Returns:
-          Integer value of the variable. None if:
-          - Feature key is invalid.
-          - Variable key is invalid.
-          - Mismatch with type of variable.
-        """
-
-        variable_type = entities.Variable.Type.INTEGER
-        project_config = self.config_manager.get_config()
-        if not project_config:
-            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('get_feature_variable_integer'))
-            return None
-
-        return self._get_feature_variable_for_type(
-            project_config, feature_key, variable_key, variable_type, user_id, attributes,
-        )
-
-    def get_feature_variable_string(self, feature_key, variable_key, user_id, attributes=None):
-        """ Returns value for a certain string variable attached to a feature.
-
-        Args:
-          feature_key: Key of the feature whose variable's value is being accessed.
-          variable_key: Key of the variable whose value is to be accessed.
-          user_id: ID for user.
-          attributes: Dict representing user attributes.
-
-        Returns:
-          String value of the variable. None if:
-          - Feature key is invalid.
-          - Variable key is invalid.
-          - Mismatch with type of variable.
-        """
-
-        variable_type = entities.Variable.Type.STRING
-        project_config = self.config_manager.get_config()
-        if not project_config:
-            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('get_feature_variable_string'))
-            return None
-
-        return self._get_feature_variable_for_type(
-            project_config, feature_key, variable_key, variable_type, user_id, attributes,
-        )
-
-    def get_feature_variable_json(self, feature_key, variable_key, user_id, attributes=None):
-        """ Returns value for a certain JSON variable attached to a feature.
-
-        Args:
-          feature_key: Key of the feature whose variable's value is being accessed.
-          variable_key: Key of the variable whose value is to be accessed.
-          user_id: ID for user.
-          attributes: Dict representing user attributes.
-
-        Returns:
-          Dictionary object of the variable. None if:
-          - Feature key is invalid.
-          - Variable key is invalid.
-          - Mismatch with type of variable.
-        """
-
-        variable_type = entities.Variable.Type.JSON
-        project_config = self.config_manager.get_config()
-        if not project_config:
-            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('get_feature_variable_json'))
-            return None
-
-        return self._get_feature_variable_for_type(
-            project_config, feature_key, variable_key, variable_type, user_id, attributes,
-        )
-
-    def get_all_feature_variables(self, feature_key, user_id, attributes=None):
-        """ Returns dictionary of all variables and their corresponding values in the context of a feature.
-
-        Args:
-          feature_key: Key of the feature whose variable's value is being accessed.
-          user_id: ID for user.
-          attributes: Dict representing user attributes.
-
-        Returns:
-          Dictionary mapping variable key to variable value. None if:
-          - Feature key is invalid.
-        """
-
-        project_config = self.config_manager.get_config()
-        if not project_config:
-            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('get_all_feature_variables'))
-            return None
-
-        return self._get_all_feature_variables_for_type(
-            project_config, feature_key, user_id, attributes,
-        )
-
-    def set_forced_variation(self, experiment_key, user_id, variation_key):
-        """ Force a user into a variation for a given experiment.
-
-        Args:
-         experiment_key: A string key identifying the experiment.
-         user_id: The user ID.
-         variation_key: A string variation key that specifies the variation which the user.
-         will be forced into. If null, then clear the existing experiment-to-variation mapping.
-
-        Returns:
-          A boolean value that indicates if the set completed successfully.
-        """
-
-        if not self.is_valid:
-            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('set_forced_variation'))
-            return False
-
-        if not validator.is_non_empty_string(experiment_key):
-            self.logger.error(enums.Errors.INVALID_INPUT.format('experiment_key'))
-            return False
-
-        if not isinstance(user_id, string_types):
-            self.logger.error(enums.Errors.INVALID_INPUT.format('user_id'))
-            return False
-
-        project_config = self.config_manager.get_config()
-        if not project_config:
-            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('set_forced_variation'))
-            return False
-
-        return self.decision_service.set_forced_variation(project_config, experiment_key, user_id, variation_key)
-
-    def get_forced_variation(self, experiment_key, user_id):
-        """ Gets the forced variation for a given user and experiment.
-
-        Args:
-          experiment_key: A string key identifying the experiment.
-          user_id: The user ID.
-
-        Returns:
-          The forced variation key. None if no forced variation key.
-        """
-
-        if not self.is_valid:
-            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('get_forced_variation'))
-            return None
-
-        if not validator.is_non_empty_string(experiment_key):
-            self.logger.error(enums.Errors.INVALID_INPUT.format('experiment_key'))
-            return None
-
-        if not isinstance(user_id, string_types):
-            self.logger.error(enums.Errors.INVALID_INPUT.format('user_id'))
-            return None
-
-        project_config = self.config_manager.get_config()
-        if not project_config:
-            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('get_forced_variation'))
-            return None
-
-        forced_variation, _ = self.decision_service.get_forced_variation(project_config, experiment_key, user_id)
-        return forced_variation.key if forced_variation else None
-
-    def get_optimizely_config(self):
-        """ Gets OptimizelyConfig instance for the current project config.
-
-        Returns:
-            OptimizelyConfig instance. None if the optimizely instance is invalid or
-            project config isn't available.
-        """
-        if not self.is_valid:
-            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('get_optimizely_config'))
-            return None
-
-        project_config = self.config_manager.get_config()
-        if not project_config:
-            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('get_optimizely_config'))
-            return None
-
-        # Customized Config Manager may not have optimizely_config defined.
-        if hasattr(self.config_manager, 'optimizely_config'):
-            return self.config_manager.optimizely_config
-
-        return OptimizelyConfigService(project_config).get_config()
-
-    def create_user_context(self, user_id, attributes=None):
-        """
-        We do not check for is_valid here as a user context can be created successfully
-        even when the SDK is not fully configured.
-
-        Args:
-            user_id: string to use as user id for user context
-            attributes: dictionary of attributes or None
-
-        Returns:
-            UserContext instance or None if the user id or attributes are invalid.
-        """
-        if not isinstance(user_id, string_types):
-            self.logger.error(enums.Errors.INVALID_INPUT.format('user_id'))
-            return None
-
-        if attributes is not None and type(attributes) is not dict:
-            self.logger.error(enums.Errors.INVALID_INPUT.format('attributes'))
-            return None
-
-        return OptimizelyUserContext(self, self.logger, user_id, attributes)
-
-    def _decide(self, user_context, key, decide_options=None):
-        """
-        decide calls optimizely decide with feature key provided
-        Args:
-            user_context: UserContent with userid and attributes
-            key: feature key
-            decide_options: list of OptimizelyDecideOption
-
-        Returns:
-            Decision object
-        """
-
-        # raising on user context as it is internal and not provided directly by the user.
-        if not isinstance(user_context, OptimizelyUserContext):
-            raise exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('user_context'))
-
-        reasons = []
-
-        # check if SDK is ready
-        if not self.is_valid:
-            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('decide'))
-            reasons.append(OptimizelyDecisionMessage.SDK_NOT_READY)
-            return OptimizelyDecision(flag_key=key, user_context=user_context, reasons=reasons)
-
-        # validate that key is a string
-        if not isinstance(key, string_types):
-            self.logger.error('Key parameter is invalid')
-            reasons.append(OptimizelyDecisionMessage.FLAG_KEY_INVALID.format(key))
-            return OptimizelyDecision(flag_key=key, user_context=user_context, reasons=reasons)
-
-        # validate that key maps to a feature flag
-        config = self.config_manager.get_config()
-        if not config:
-            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('decide'))
-            reasons.append(OptimizelyDecisionMessage.SDK_NOT_READY)
-            return OptimizelyDecision(flag_key=key, user_context=user_context, reasons=reasons)
-
-        feature_flag = config.get_feature_from_key(key)
-        if feature_flag is None:
-            self.logger.error(f"No feature flag was found for key '{key}'.")
-            reasons.append(OptimizelyDecisionMessage.FLAG_KEY_INVALID.format(key))
-            return OptimizelyDecision(flag_key=key, user_context=user_context, reasons=reasons)
-
-        # merge decide_options and default_decide_options
-        if isinstance(decide_options, list):
-            decide_options += self.default_decide_options
-        else:
-            self.logger.debug('Provided decide options is not an array. Using default decide options.')
-            decide_options = self.default_decide_options
-
-        # Create Optimizely Decision Result.
-        user_id = user_context.user_id
-        attributes = user_context.get_user_attributes()
-        variation_key = None
-        variation = None
-        feature_enabled = False
-        rule_key = None
-        flag_key = key
-        all_variables = {}
-        experiment = None
-        decision_source = DecisionSources.ROLLOUT
-        source_info = {}
-        decision_event_dispatched = False
-
-        # Check forced decisions first
-        optimizely_decision_context = OptimizelyUserContext.OptimizelyDecisionContext(flag_key=key, rule_key=rule_key)
-        forced_decision_response = self.decision_service.validated_forced_decision(config,
-                                                                                   optimizely_decision_context,
-                                                                                   user_context)
-        variation, decision_reasons = forced_decision_response
-        reasons += decision_reasons
-
-        if variation:
-            decision = Decision(None, variation, enums.DecisionSources.FEATURE_TEST)
-        else:
-            # Regular decision
-            decision, decision_reasons = self.decision_service.get_variation_for_feature(config,
-                                                                                         feature_flag,
-                                                                                         user_context, decide_options)
-
-            reasons += decision_reasons
-
-        # Fill in experiment and variation if returned (rollouts can have featureEnabled variables as well.)
-        if decision.experiment is not None:
-            experiment = decision.experiment
-            source_info["experiment"] = experiment
-            rule_key = experiment.key if experiment else None
-        if decision.variation is not None:
-            variation = decision.variation
-            variation_key = variation.key
-            feature_enabled = variation.featureEnabled
-            decision_source = decision.source
-            source_info["variation"] = variation
-
-        # Send impression event if Decision came from a feature
-        # test and decide options doesn't include disableDecisionEvent
-        if OptimizelyDecideOption.DISABLE_DECISION_EVENT not in decide_options:
-            if decision_source == DecisionSources.FEATURE_TEST or config.send_flag_decisions:
-                self._send_impression_event(config, experiment, variation, flag_key, rule_key or '',
-                                            decision_source, feature_enabled,
-                                            user_id, attributes)
-
-                decision_event_dispatched = True
-
-        # Generate all variables map if decide options doesn't include excludeVariables
-        if OptimizelyDecideOption.EXCLUDE_VARIABLES not in decide_options:
-            for variable_key in feature_flag.variables:
-                variable = config.get_variable_for_feature(flag_key, variable_key)
-                variable_value = variable.defaultValue
-                if feature_enabled:
-                    variable_value = config.get_variable_value_for_variation(variable, decision.variation)
-                    self.logger.debug(
-                        'Got variable value "%s" for variable "%s" of feature flag "%s".'
-                        % (variable_value, variable_key, flag_key)
-                    )
-
-                try:
-                    actual_value = config.get_typecast_value(variable_value, variable.type)
-                except:
-                    self.logger.error('Unable to cast value. Returning None.')
-                    actual_value = None
-
-                all_variables[variable_key] = actual_value
-
-        should_include_reasons = OptimizelyDecideOption.INCLUDE_REASONS in decide_options
-
-        # Send notification
-        self.notification_center.send_notifications(
-            enums.NotificationTypes.DECISION,
-            enums.DecisionNotificationTypes.FLAG,
-            user_id,
-            attributes or {},
-            {
-                'flag_key': flag_key,
-                'enabled': feature_enabled,
-                'variables': all_variables,
-                'variation_key': variation_key,
-                'rule_key': rule_key,
-                'reasons': reasons if should_include_reasons else [],
-                'decision_event_dispatched': decision_event_dispatched
-
-            },
-        )
-
-        return OptimizelyDecision(variation_key=variation_key, enabled=feature_enabled, variables=all_variables,
-                                  rule_key=rule_key, flag_key=flag_key,
-                                  user_context=user_context, reasons=reasons if should_include_reasons else []
-                                  )
-
-    def _decide_all(self, user_context, decide_options=None):
-        """
-        decide_all will return a decision for every feature key in the current config
-        Args:
-            user_context: UserContent object
-            decide_options: Array of DecisionOption
-
-        Returns:
-            A dictionary of feature key to Decision
-        """
-        # raising on user context as it is internal and not provided directly by the user.
-        if not isinstance(user_context, OptimizelyUserContext):
-            raise exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('user_context'))
-
-        # check if SDK is ready
-        if not self.is_valid:
-            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('decide_all'))
-            return {}
-
-        config = self.config_manager.get_config()
-        if not config:
-            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('decide'))
-            return {}
-
-        keys = []
-        for f in config.feature_flags:
-            keys.append(f['key'])
-        return self._decide_for_keys(user_context, keys, decide_options)
-
-    def _decide_for_keys(self, user_context, keys, decide_options=None):
-        """
-        Args:
-            user_context: UserContent
-            keys: list of feature keys to run decide on.
-            decide_options: an array of DecisionOption objects
-
-        Returns:
-            An dictionary of feature key to Decision
-        """
-        # raising on user context as it is internal and not provided directly by the user.
-        if not isinstance(user_context, OptimizelyUserContext):
-            raise exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('user_context'))
-
-        # check if SDK is ready
-        if not self.is_valid:
-            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('decide_for_keys'))
-            return {}
-
-        # merge decide_options and default_decide_options
-        merged_decide_options = []
-        if isinstance(decide_options, list):
-            merged_decide_options = decide_options[:]
-            merged_decide_options += self.default_decide_options
-        else:
-            self.logger.debug('Provided decide options is not an array. Using default decide options.')
-            merged_decide_options = self.default_decide_options
-
-        enabled_flags_only = OptimizelyDecideOption.ENABLED_FLAGS_ONLY in merged_decide_options
-
-        decisions = {}
-        for key in keys:
-            decision = self._decide(user_context, key, decide_options)
-            if enabled_flags_only and not decision.enabled:
-                continue
-            decisions[key] = decision
-        return decisions
+# Copyright 2016-2023, Optimizely
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Any, Optional
+
+from . import decision_service
+from . import entities
+from . import event_builder
+from . import exceptions
+from . import logger as _logging
+from . import project_config
+from .config_manager import AuthDatafilePollingConfigManager
+from .config_manager import BaseConfigManager
+from .config_manager import PollingConfigManager
+from .config_manager import StaticConfigManager
+from .decision.optimizely_decide_option import OptimizelyDecideOption
+from .decision.optimizely_decision import OptimizelyDecision
+from .decision.optimizely_decision_message import OptimizelyDecisionMessage
+from .decision_service import Decision
+from .error_handler import NoOpErrorHandler, BaseErrorHandler
+from .event import event_factory, user_event_factory
+from .event.event_processor import BatchEventProcessor, BaseEventProcessor
+from .event_dispatcher import EventDispatcher, CustomEventDispatcher
+from .helpers import enums, validator
+from .helpers.sdk_settings import OptimizelySdkSettings
+from .helpers.enums import DecisionSources
+from .notification_center import NotificationCenter
+from .notification_center_registry import _NotificationCenterRegistry
+from .odp.lru_cache import LRUCache
+from .odp.odp_manager import OdpManager
+from .optimizely_config import OptimizelyConfig, OptimizelyConfigService
+from .optimizely_user_context import OptimizelyUserContext, UserAttributes
+
+if TYPE_CHECKING:
+    # prevent circular dependency by skipping import at runtime
+    from .user_profile import UserProfileService
+    from .helpers.event_tag_utils import EventTags
+
+
+class Optimizely:
+    """ Class encapsulating all SDK functionality. """
+
+    def __init__(
+            self,
+            datafile: Optional[str] = None,
+            event_dispatcher: Optional[CustomEventDispatcher] = None,
+            logger: Optional[_logging.Logger] = None,
+            error_handler: Optional[BaseErrorHandler] = None,
+            skip_json_validation: Optional[bool] = False,
+            user_profile_service: Optional[UserProfileService] = None,
+            sdk_key: Optional[str] = None,
+            config_manager: Optional[BaseConfigManager] = None,
+            notification_center: Optional[NotificationCenter] = None,
+            event_processor: Optional[BaseEventProcessor] = None,
+            datafile_access_token: Optional[str] = None,
+            default_decide_options: Optional[list[str]] = None,
+            event_processor_options: Optional[dict[str, Any]] = None,
+            settings: Optional[OptimizelySdkSettings] = None
+    ) -> None:
+        """ Optimizely init method for managing Custom projects.
+
+        Args:
+          datafile: Optional JSON string representing the project. Must provide at least one of datafile or sdk_key.
+          event_dispatcher: Provides a dispatch_event method which if given a URL and params sends a request to it.
+          logger: Optional component which provides a log method to log messages. By default nothing would be logged.
+          error_handler: Optional component which provides a handle_error method to handle exceptions.
+                         By default all exceptions will be suppressed.
+          skip_json_validation: Optional boolean param which allows skipping JSON schema validation upon object
+          invocation.
+                                By default JSON schema validation will be performed.
+          user_profile_service: Optional component which provides methods to store and manage user profiles.
+          sdk_key: Optional string uniquely identifying the datafile corresponding to project and environment
+          combination.
+                   Must provide at least one of datafile or sdk_key.
+          config_manager: Optional component which implements optimizely.config_manager.BaseConfigManager.
+          notification_center: Optional instance of notification_center.NotificationCenter. Useful when providing own
+                               config_manager.BaseConfigManager implementation which can be using the
+                               same NotificationCenter instance.
+          event_processor: Optional component which processes the given event(s).
+                           By default optimizely.event.event_processor.BatchEventProcessor is used
+                           which batches events. To simply forward events to the event dispatcher
+                           configure and use optimizely.event.event_processor.ForwardingEventProcessor.
+          datafile_access_token: Optional string used to fetch authenticated datafile for a secure project environment.
+          default_decide_options: Optional list of decide options used with the decide APIs.
+          event_processor_options: Optional dict of options to be passed to the default batch event processor.
+          settings: Optional instance of OptimizelySdkSettings for sdk configuration.
+        """
+        self.logger_name = '.'.join([__name__, self.__class__.__name__])
+        self.is_valid = True
+        self.event_dispatcher = event_dispatcher or EventDispatcher
+        self.logger = _logging.adapt_logger(logger or _logging.NoOpLogger())
+        self.error_handler = error_handler or NoOpErrorHandler
+        self.config_manager: BaseConfigManager = config_manager  # type: ignore[assignment]
+        self.notification_center = notification_center or NotificationCenter(self.logger)
+        event_processor_defaults = {
+            'batch_size': 1,
+            'flush_interval': 30,
+            'timeout_interval': 5,
+            'start_on_init': True
+        }
+        if event_processor_options:
+            event_processor_defaults.update(event_processor_options)
+
+        self.event_processor = event_processor or BatchEventProcessor(
+            self.event_dispatcher,
+            logger=self.logger,
+            notification_center=self.notification_center,
+            **event_processor_defaults  # type: ignore[arg-type]
+        )
+        self.default_decide_options: list[str]
+
+        if default_decide_options is None:
+            self.default_decide_options = []
+        else:
+            self.default_decide_options = default_decide_options
+
+        if isinstance(self.default_decide_options, list):
+            self.default_decide_options = self.default_decide_options[:]
+        else:
+            self.logger.debug('Provided default decide options is not a list.')
+            self.default_decide_options = []
+
+        self.sdk_settings: OptimizelySdkSettings = settings  # type: ignore[assignment]
+
+        try:
+            self._validate_instantiation_options()
+        except exceptions.InvalidInputException as error:
+            self.is_valid = False
+            # We actually want to log this error to stderr, so make sure the logger
+            # has a handler capable of doing that.
+            self.logger = _logging.reset_logger(self.logger_name)
+            self.logger.exception(str(error))
+            return
+
+        config_manager_options: dict[str, Any] = {
+            'datafile': datafile,
+            'logger': self.logger,
+            'error_handler': self.error_handler,
+            'notification_center': self.notification_center,
+            'skip_json_validation': skip_json_validation,
+        }
+
+        if not self.config_manager:
+            if sdk_key:
+                config_manager_options['sdk_key'] = sdk_key
+                if datafile_access_token:
+                    config_manager_options['datafile_access_token'] = datafile_access_token
+                    self.config_manager = AuthDatafilePollingConfigManager(**config_manager_options)
+                else:
+                    self.config_manager = PollingConfigManager(**config_manager_options)
+            else:
+                self.config_manager = StaticConfigManager(**config_manager_options)
+
+        self.odp_manager: OdpManager
+        self._setup_odp(self.config_manager.get_sdk_key())
+
+        self.event_builder = event_builder.EventBuilder()
+        self.decision_service = decision_service.DecisionService(self.logger, user_profile_service)
+
+    def _validate_instantiation_options(self) -> None:
+        """ Helper method to validate all instantiation parameters.
+
+        Raises:
+          Exception if provided instantiation options are valid.
+        """
+        if self.config_manager and not validator.is_config_manager_valid(self.config_manager):
+            raise exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('config_manager'))
+
+        if not validator.is_event_dispatcher_valid(self.event_dispatcher):
+            raise exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('event_dispatcher'))
+
+        if not validator.is_logger_valid(self.logger):
+            raise exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('logger'))
+
+        if not validator.is_error_handler_valid(self.error_handler):
+            raise exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('error_handler'))
+
+        if not validator.is_notification_center_valid(self.notification_center):
+            raise exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('notification_center'))
+
+        if not validator.is_event_processor_valid(self.event_processor):
+            raise exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('event_processor'))
+
+        if not isinstance(self.sdk_settings, OptimizelySdkSettings):
+            if self.sdk_settings is not None:
+                self.logger.debug('Provided sdk_settings is not an OptimizelySdkSettings instance.')
+            self.sdk_settings = OptimizelySdkSettings()
+
+        if self.sdk_settings.segments_cache:
+            if not validator.is_segments_cache_valid(self.sdk_settings.segments_cache):
+                raise exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('segments_cache'))
+
+        if self.sdk_settings.odp_segment_manager:
+            if not validator.is_segment_manager_valid(self.sdk_settings.odp_segment_manager):
+                raise exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('segment_manager'))
+
+        if self.sdk_settings.odp_event_manager:
+            if not validator.is_event_manager_valid(self.sdk_settings.odp_event_manager):
+                raise exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('event_manager'))
+
+    def _validate_user_inputs(
+        self, attributes: Optional[UserAttributes] = None, event_tags: Optional[EventTags] = None
+    ) -> bool:
+        """ Helper method to validate user inputs.
+
+        Args:
+          attributes: Dict representing user attributes.
+          event_tags: Dict representing metadata associated with an event.
+
+        Returns:
+          Boolean True if inputs are valid. False otherwise.
+
+        """
+
+        if attributes and not validator.are_attributes_valid(attributes):
+            self.logger.error('Provided attributes are in an invalid format.')
+            self.error_handler.handle_error(exceptions.InvalidAttributeException(enums.Errors.INVALID_ATTRIBUTE_FORMAT))
+            return False
+
+        if event_tags and not validator.are_event_tags_valid(event_tags):
+            self.logger.error('Provided event tags are in an invalid format.')
+            self.error_handler.handle_error(exceptions.InvalidEventTagException(enums.Errors.INVALID_EVENT_TAG_FORMAT))
+            return False
+
+        return True
+
+    def _send_impression_event(
+        self, project_config: project_config.ProjectConfig, experiment: Optional[entities.Experiment],
+        variation: Optional[entities.Variation], flag_key: str, rule_key: str, rule_type: str,
+        enabled: bool, user_id: str, attributes: Optional[UserAttributes]
+    ) -> None:
+        """ Helper method to send impression event.
+
+        Args:
+          project_config: Instance of ProjectConfig.
+          experiment: Experiment for which impression event is being sent.
+          variation: Variation picked for user for the given experiment.
+          flag_key: key for a feature flag.
+          rule_key: key for an experiment.
+          rule_type: type for the source.
+          enabled: boolean representing if feature is enabled
+          user_id: ID for user.
+          attributes: Dict representing user attributes and values which need to be recorded.
+        """
+        if not experiment:
+            experiment = entities.Experiment.get_default()
+
+        variation_id = variation.id if variation is not None else None
+        user_event = user_event_factory.UserEventFactory.create_impression_event(
+            project_config, experiment, variation_id, flag_key, rule_key, rule_type, enabled, user_id, attributes
+        )
+
+        if user_event is None:
+            self.logger.error('Cannot process None event.')
+            return
+
+        self.event_processor.process(user_event)
+
+        # Kept for backward compatibility.
+        # This notification is deprecated and new Decision notifications
+        # are sent via their respective method calls.
+        if len(self.notification_center.notification_listeners[enums.NotificationTypes.ACTIVATE]) > 0:
+            log_event = event_factory.EventFactory.create_log_event(user_event, self.logger)
+            self.notification_center.send_notifications(
+                enums.NotificationTypes.ACTIVATE, experiment, user_id, attributes, variation, log_event.__dict__,
+            )
+
+    def _get_feature_variable_for_type(
+        self, project_config: project_config.ProjectConfig, feature_key: str, variable_key: str,
+        variable_type: Optional[str], user_id: str, attributes: Optional[UserAttributes]
+    ) -> Any:
+        """ Helper method to determine value for a certain variable attached to a feature flag based on
+        type of variable.
+
+        Args:
+          project_config: Instance of ProjectConfig.
+          feature_key: Key of the feature whose variable's value is being accessed.
+          variable_key: Key of the variable whose value is to be accessed.
+          variable_type: Type of variable which could be one of boolean/double/integer/string.
+          user_id: ID for user.
+          attributes: Dict representing user attributes.
+
+        Returns:
+          Value of the variable. None if:
+          - Feature key is invalid.
+          - Variable key is invalid.
+          - Mismatch with type of variable.
+        """
+        if not validator.is_non_empty_string(feature_key):
+            self.logger.error(enums.Errors.INVALID_INPUT.format('feature_key'))
+            return None
+
+        if not validator.is_non_empty_string(variable_key):
+            self.logger.error(enums.Errors.INVALID_INPUT.format('variable_key'))
+            return None
+
+        if not isinstance(user_id, str):
+            self.logger.error(enums.Errors.INVALID_INPUT.format('user_id'))
+            return None
+
+        if not self._validate_user_inputs(attributes):
+            return None
+
+        feature_flag = project_config.get_feature_from_key(feature_key)
+        if not feature_flag:
+            return None
+
+        variable = project_config.get_variable_for_feature(feature_key, variable_key)
+        if not variable:
+            return None
+
+        # For non-typed method, use type of variable; else, return None if type differs
+        variable_type = variable_type or variable.type
+        if variable.type != variable_type:
+            self.logger.warning(
+                f'Requested variable type "{variable_type}", but variable is of '
+                f'type "{variable.type}". Use correct API to retrieve value. Returning None.'
+            )
+            return None
+
+        feature_enabled = False
+        source_info = {}
+        variable_value = variable.defaultValue
+
+        user_context = OptimizelyUserContext(self, self.logger, user_id, attributes, False)
+
+        decision, _ = self.decision_service.get_variation_for_feature(project_config, feature_flag, user_context)
+
+        if decision.variation:
+
+            feature_enabled = decision.variation.featureEnabled
+            if feature_enabled:
+                variable_value = project_config.get_variable_value_for_variation(variable, decision.variation)
+                self.logger.info(
+                    f'Got variable value "{variable_value}" for '
+                    f'variable "{variable_key}" of feature flag "{feature_key}".'
+                )
+            else:
+                self.logger.info(
+                    f'Feature "{feature_key}" is not enabled for user "{user_id}". '
+                    f'Returning the default variable value "{variable_value}".'
+                )
+        else:
+            self.logger.info(
+                f'User "{user_id}" is not in any variation or rollout rule. '
+                f'Returning default value for variable "{variable_key}" of feature flag "{feature_key}".'
+            )
+
+        if decision.source == enums.DecisionSources.FEATURE_TEST:
+            source_info = {
+                'experiment_key': decision.experiment.key if decision.experiment else None,
+                'variation_key': decision.variation.key if decision.variation else None,
+            }
+
+        try:
+            actual_value = project_config.get_typecast_value(variable_value, variable_type)
+        except:
+            self.logger.error('Unable to cast value. Returning None.')
+            actual_value = None
+
+        self.notification_center.send_notifications(
+            enums.NotificationTypes.DECISION,
+            enums.DecisionNotificationTypes.FEATURE_VARIABLE,
+            user_id,
+            attributes or {},
+            {
+                'feature_key': feature_key,
+                'feature_enabled': feature_enabled,
+                'source': decision.source,
+                'variable_key': variable_key,
+                'variable_value': actual_value,
+                'variable_type': variable_type,
+                'source_info': source_info,
+            },
+        )
+        return actual_value
+
+    def _get_all_feature_variables_for_type(
+        self, project_config: project_config.ProjectConfig, feature_key: str,
+        user_id: str, attributes: Optional[UserAttributes],
+    ) -> Optional[dict[str, Any]]:
+        """ Helper method to determine value for all variables attached to a feature flag.
+
+        Args:
+          project_config: Instance of ProjectConfig.
+          feature_key: Key of the feature whose variable's value is being accessed.
+          user_id: ID for user.
+          attributes: Dict representing user attributes.
+
+        Returns:
+          Dictionary of all variables. None if:
+          - Feature key is invalid.
+        """
+        if not validator.is_non_empty_string(feature_key):
+            self.logger.error(enums.Errors.INVALID_INPUT.format('feature_key'))
+            return None
+
+        if not isinstance(user_id, str):
+            self.logger.error(enums.Errors.INVALID_INPUT.format('user_id'))
+            return None
+
+        if not self._validate_user_inputs(attributes):
+            return None
+
+        feature_flag = project_config.get_feature_from_key(feature_key)
+        if not feature_flag:
+            return None
+
+        feature_enabled = False
+        source_info = {}
+
+        user_context = OptimizelyUserContext(self, self.logger, user_id, attributes, False)
+
+        decision, _ = self.decision_service.get_variation_for_feature(project_config, feature_flag, user_context)
+
+        if decision.variation:
+
+            feature_enabled = decision.variation.featureEnabled
+            if feature_enabled:
+                self.logger.info(
+                    f'Feature "{feature_key}" is enabled for user "{user_id}".'
+                )
+            else:
+                self.logger.info(
+                    f'Feature "{feature_key}" is not enabled for user "{user_id}".'
+                )
+        else:
+            self.logger.info(
+                f'User "{user_id}" is not in any variation or rollout rule. '
+                f'Returning default value for all variables of feature flag "{feature_key}".'
+            )
+
+        all_variables = {}
+        for variable_key, variable in feature_flag.variables.items():
+            variable_value = variable.defaultValue
+            if feature_enabled:
+                variable_value = project_config.get_variable_value_for_variation(variable, decision.variation)
+                self.logger.debug(
+                    f'Got variable value "{variable_value}" for '
+                    f'variable "{variable_key}" of feature flag "{feature_key}".'
+                )
+
+            try:
+                actual_value = project_config.get_typecast_value(variable_value, variable.type)
+            except:
+                self.logger.error('Unable to cast value. Returning None.')
+                actual_value = None
+
+            all_variables[variable_key] = actual_value
+
+        if decision.source == enums.DecisionSources.FEATURE_TEST:
+            source_info = {
+                'experiment_key': decision.experiment.key if decision.experiment else None,
+                'variation_key': decision.variation.key if decision.variation else None,
+            }
+
+        self.notification_center.send_notifications(
+            enums.NotificationTypes.DECISION,
+            enums.DecisionNotificationTypes.ALL_FEATURE_VARIABLES,
+            user_id,
+            attributes or {},
+            {
+                'feature_key': feature_key,
+                'feature_enabled': feature_enabled,
+                'variable_values': all_variables,
+                'source': decision.source,
+                'source_info': source_info,
+            },
+        )
+        return all_variables
+
+    def activate(self, experiment_key: str, user_id: str, attributes: Optional[UserAttributes] = None) -> Optional[str]:
+        """ Buckets visitor and sends impression event to Optimizely.
+
+        Args:
+          experiment_key: Experiment which needs to be activated.
+          user_id: ID for user.
+          attributes: Dict representing user attributes and values which need to be recorded.
+
+        Returns:
+          Variation key representing the variation the user will be bucketed in.
+          None if user is not in experiment or if experiment is not Running.
+        """
+
+        if not self.is_valid:
+            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('activate'))
+            return None
+
+        if not validator.is_non_empty_string(experiment_key):
+            self.logger.error(enums.Errors.INVALID_INPUT.format('experiment_key'))
+            return None
+
+        if not isinstance(user_id, str):
+            self.logger.error(enums.Errors.INVALID_INPUT.format('user_id'))
+            return None
+
+        project_config = self.config_manager.get_config()
+        if not project_config:
+            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('activate'))
+            return None
+
+        variation_key = self.get_variation(experiment_key, user_id, attributes)
+
+        if not variation_key:
+            self.logger.info(f'Not activating user "{user_id}".')
+            return None
+
+        experiment = project_config.get_experiment_from_key(experiment_key)
+        variation = project_config.get_variation_from_key(experiment_key, variation_key)
+        if not variation or not experiment:
+            self.logger.info(f'Not activating user "{user_id}".')
+            return None
+
+        # Create and dispatch impression event
+        self.logger.info(f'Activating user "{user_id}" in experiment "{experiment.key}".')
+        self._send_impression_event(project_config, experiment, variation, '', experiment.key,
+                                    enums.DecisionSources.EXPERIMENT, True, user_id, attributes)
+
+        return variation.key
+
+    def track(
+        self, event_key: str, user_id: str,
+        attributes: Optional[UserAttributes] = None,
+        event_tags: Optional[EventTags] = None
+    ) -> None:
+        """ Send conversion event to Optimizely.
+
+        Args:
+          event_key: Event key representing the event which needs to be recorded.
+          user_id: ID for user.
+          attributes: Dict representing visitor attributes and values which need to be recorded.
+          event_tags: Dict representing metadata associated with the event.
+        """
+
+        if not self.is_valid:
+            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('track'))
+            return
+
+        if not validator.is_non_empty_string(event_key):
+            self.logger.error(enums.Errors.INVALID_INPUT.format('event_key'))
+            return
+
+        if not isinstance(user_id, str):
+            self.logger.error(enums.Errors.INVALID_INPUT.format('user_id'))
+            return
+
+        if not self._validate_user_inputs(attributes, event_tags):
+            return
+
+        project_config = self.config_manager.get_config()
+        if not project_config:
+            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('track'))
+            return
+
+        event = project_config.get_event(event_key)
+        if not event:
+            self.logger.info(f'Not tracking user "{user_id}" for event "{event_key}".')
+            return
+
+        user_event = user_event_factory.UserEventFactory.create_conversion_event(
+            project_config, event_key, user_id, attributes, event_tags
+        )
+
+        if user_event is None:
+            self.logger.error('Cannot process None event.')
+            return
+
+        self.event_processor.process(user_event)
+        self.logger.info(f'Tracking event "{event_key}" for user "{user_id}".')
+
+        if len(self.notification_center.notification_listeners[enums.NotificationTypes.TRACK]) > 0:
+            log_event = event_factory.EventFactory.create_log_event(user_event, self.logger)
+            self.notification_center.send_notifications(
+                enums.NotificationTypes.TRACK, event_key, user_id, attributes, event_tags, log_event.__dict__,
+            )
+
+    def get_variation(
+        self, experiment_key: str, user_id: str, attributes: Optional[UserAttributes] = None
+    ) -> Optional[str]:
+        """ Gets variation where user will be bucketed.
+
+        Args:
+          experiment_key: Experiment for which user variation needs to be determined.
+          user_id: ID for user.
+          attributes: Dict representing user attributes.
+
+        Returns:
+          Variation key representing the variation the user will be bucketed in.
+          None if user is not in experiment or if experiment is not Running.
+        """
+
+        if not self.is_valid:
+            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('get_variation'))
+            return None
+
+        if not validator.is_non_empty_string(experiment_key):
+            self.logger.error(enums.Errors.INVALID_INPUT.format('experiment_key'))
+            return None
+
+        if not isinstance(user_id, str):
+            self.logger.error(enums.Errors.INVALID_INPUT.format('user_id'))
+            return None
+
+        project_config = self.config_manager.get_config()
+        if not project_config:
+            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('get_variation'))
+            return None
+
+        experiment = project_config.get_experiment_from_key(experiment_key)
+        variation_key = None
+
+        if not experiment:
+            self.logger.info(f'Experiment key "{experiment_key}" is invalid. Not activating user "{user_id}".')
+            return None
+
+        if not self._validate_user_inputs(attributes):
+            return None
+
+        user_context = OptimizelyUserContext(self, self.logger, user_id, attributes, False)
+
+        variation, _ = self.decision_service.get_variation(project_config, experiment, user_context)
+        if variation:
+            variation_key = variation.key
+
+        if project_config.is_feature_experiment(experiment.id):
+            decision_notification_type = enums.DecisionNotificationTypes.FEATURE_TEST
+        else:
+            decision_notification_type = enums.DecisionNotificationTypes.AB_TEST
+
+        self.notification_center.send_notifications(
+            enums.NotificationTypes.DECISION,
+            decision_notification_type,
+            user_id,
+            attributes or {},
+            {'experiment_key': experiment_key, 'variation_key': variation_key},
+        )
+
+        return variation_key
+
+    def is_feature_enabled(self, feature_key: str, user_id: str, attributes: Optional[UserAttributes] = None) -> bool:
+        """ Returns true if the feature is enabled for the given user.
+
+        Args:
+          feature_key: The key of the feature for which we are determining if it is enabled or not for the given user.
+          user_id: ID for user.
+          attributes: Dict representing user attributes.
+
+        Returns:
+          True if the feature is enabled for the user. False otherwise.
+        """
+
+        if not self.is_valid:
+            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('is_feature_enabled'))
+            return False
+
+        if not validator.is_non_empty_string(feature_key):
+            self.logger.error(enums.Errors.INVALID_INPUT.format('feature_key'))
+            return False
+
+        if not isinstance(user_id, str):
+            self.logger.error(enums.Errors.INVALID_INPUT.format('user_id'))
+            return False
+
+        if not self._validate_user_inputs(attributes):
+            return False
+
+        project_config = self.config_manager.get_config()
+        if not project_config:
+            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('is_feature_enabled'))
+            return False
+
+        feature = project_config.get_feature_from_key(feature_key)
+        if not feature:
+            return False
+
+        feature_enabled = False
+        source_info = {}
+
+        user_context = OptimizelyUserContext(self, self.logger, user_id, attributes, False)
+
+        decision, _ = self.decision_service.get_variation_for_feature(project_config, feature, user_context)
+        is_source_experiment = decision.source == enums.DecisionSources.FEATURE_TEST
+        is_source_rollout = decision.source == enums.DecisionSources.ROLLOUT
+
+        if decision.variation:
+            if decision.variation.featureEnabled is True:
+                feature_enabled = True
+
+        if (is_source_rollout or not decision.variation) and project_config.get_send_flag_decisions_value():
+            self._send_impression_event(
+                project_config, decision.experiment, decision.variation, feature.key, decision.experiment.key if
+                decision.experiment else '', decision.source, feature_enabled, user_id, attributes
+            )
+
+        # Send event if Decision came from an experiment.
+        if is_source_experiment and decision.variation and decision.experiment:
+            source_info = {
+                'experiment_key': decision.experiment.key,
+                'variation_key': decision.variation.key,
+            }
+            self._send_impression_event(
+                project_config, decision.experiment, decision.variation, feature.key, decision.experiment.key,
+                decision.source, feature_enabled, user_id, attributes
+            )
+
+        if feature_enabled:
+            self.logger.info(f'Feature "{feature_key}" is enabled for user "{user_id}".')
+        else:
+            self.logger.info(f'Feature "{feature_key}" is not enabled for user "{user_id}".')
+
+        self.notification_center.send_notifications(
+            enums.NotificationTypes.DECISION,
+            enums.DecisionNotificationTypes.FEATURE,
+            user_id,
+            attributes or {},
+            {
+                'feature_key': feature_key,
+                'feature_enabled': feature_enabled,
+                'source': decision.source,
+                'source_info': source_info,
+            },
+        )
+
+        return feature_enabled
+
+    def get_enabled_features(self, user_id: str, attributes: Optional[UserAttributes] = None) -> list[str]:
+        """ Returns the list of features that are enabled for the user.
+
+        Args:
+          user_id: ID for user.
+          attributes: Dict representing user attributes.
+
+        Returns:
+          A list of the keys of the features that are enabled for the user.
+        """
+
+        enabled_features: list[str] = []
+        if not self.is_valid:
+            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('get_enabled_features'))
+            return enabled_features
+
+        if not isinstance(user_id, str):
+            self.logger.error(enums.Errors.INVALID_INPUT.format('user_id'))
+            return enabled_features
+
+        if not self._validate_user_inputs(attributes):
+            return enabled_features
+
+        project_config = self.config_manager.get_config()
+        if not project_config:
+            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('get_enabled_features'))
+            return enabled_features
+
+        for feature in project_config.feature_key_map.values():
+            if self.is_feature_enabled(feature.key, user_id, attributes):
+                enabled_features.append(feature.key)
+
+        return enabled_features
+
+    def get_feature_variable(
+        self, feature_key: str, variable_key: str, user_id: str, attributes: Optional[UserAttributes] = None
+    ) -> Any:
+        """ Returns value for a variable attached to a feature flag.
+
+        Args:
+          feature_key: Key of the feature whose variable's value is being accessed.
+          variable_key: Key of the variable whose value is to be accessed.
+          user_id: ID for user.
+          attributes: Dict representing user attributes.
+
+        Returns:
+          Value of the variable. None if:
+          - Feature key is invalid.
+          - Variable key is invalid.
+        """
+        project_config = self.config_manager.get_config()
+        if not project_config:
+            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('get_feature_variable'))
+            return None
+
+        return self._get_feature_variable_for_type(project_config, feature_key, variable_key, None, user_id, attributes)
+
+    def get_feature_variable_boolean(
+        self, feature_key: str, variable_key: str, user_id: str, attributes: Optional[UserAttributes] = None
+    ) -> Optional[bool]:
+        """ Returns value for a certain boolean variable attached to a feature flag.
+
+        Args:
+          feature_key: Key of the feature whose variable's value is being accessed.
+          variable_key: Key of the variable whose value is to be accessed.
+          user_id: ID for user.
+          attributes: Dict representing user attributes.
+
+        Returns:
+          Boolean value of the variable. None if:
+          - Feature key is invalid.
+          - Variable key is invalid.
+          - Mismatch with type of variable.
+        """
+
+        variable_type = entities.Variable.Type.BOOLEAN
+        project_config = self.config_manager.get_config()
+        if not project_config:
+            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('get_feature_variable_boolean'))
+            return None
+
+        return self._get_feature_variable_for_type(  # type: ignore[no-any-return]
+            project_config, feature_key, variable_key, variable_type, user_id, attributes,
+        )
+
+    def get_feature_variable_double(
+        self, feature_key: str, variable_key: str, user_id: str, attributes: Optional[UserAttributes] = None
+    ) -> Optional[float]:
+        """ Returns value for a certain double variable attached to a feature flag.
+
+        Args:
+          feature_key: Key of the feature whose variable's value is being accessed.
+          variable_key: Key of the variable whose value is to be accessed.
+          user_id: ID for user.
+          attributes: Dict representing user attributes.
+
+        Returns:
+          Double value of the variable. None if:
+          - Feature key is invalid.
+          - Variable key is invalid.
+          - Mismatch with type of variable.
+        """
+
+        variable_type = entities.Variable.Type.DOUBLE
+        project_config = self.config_manager.get_config()
+        if not project_config:
+            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('get_feature_variable_double'))
+            return None
+
+        return self._get_feature_variable_for_type(  # type: ignore[no-any-return]
+            project_config, feature_key, variable_key, variable_type, user_id, attributes,
+        )
+
+    def get_feature_variable_integer(
+        self, feature_key: str, variable_key: str, user_id: str, attributes: Optional[UserAttributes] = None
+    ) -> Optional[int]:
+        """ Returns value for a certain integer variable attached to a feature flag.
+
+        Args:
+          feature_key: Key of the feature whose variable's value is being accessed.
+          variable_key: Key of the variable whose value is to be accessed.
+          user_id: ID for user.
+          attributes: Dict representing user attributes.
+
+        Returns:
+          Integer value of the variable. None if:
+          - Feature key is invalid.
+          - Variable key is invalid.
+          - Mismatch with type of variable.
+        """
+
+        variable_type = entities.Variable.Type.INTEGER
+        project_config = self.config_manager.get_config()
+        if not project_config:
+            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('get_feature_variable_integer'))
+            return None
+
+        return self._get_feature_variable_for_type(  # type: ignore[no-any-return]
+            project_config, feature_key, variable_key, variable_type, user_id, attributes,
+        )
+
+    def get_feature_variable_string(
+        self, feature_key: str, variable_key: str, user_id: str, attributes: Optional[UserAttributes] = None
+    ) -> Optional[str]:
+        """ Returns value for a certain string variable attached to a feature.
+
+        Args:
+          feature_key: Key of the feature whose variable's value is being accessed.
+          variable_key: Key of the variable whose value is to be accessed.
+          user_id: ID for user.
+          attributes: Dict representing user attributes.
+
+        Returns:
+          String value of the variable. None if:
+          - Feature key is invalid.
+          - Variable key is invalid.
+          - Mismatch with type of variable.
+        """
+
+        variable_type = entities.Variable.Type.STRING
+        project_config = self.config_manager.get_config()
+        if not project_config:
+            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('get_feature_variable_string'))
+            return None
+
+        return self._get_feature_variable_for_type(  # type: ignore[no-any-return]
+            project_config, feature_key, variable_key, variable_type, user_id, attributes,
+        )
+
+    def get_feature_variable_json(
+        self, feature_key: str, variable_key: str, user_id: str, attributes: Optional[UserAttributes] = None
+    ) -> Optional[dict[str, Any]]:
+        """ Returns value for a certain JSON variable attached to a feature.
+
+        Args:
+          feature_key: Key of the feature whose variable's value is being accessed.
+          variable_key: Key of the variable whose value is to be accessed.
+          user_id: ID for user.
+          attributes: Dict representing user attributes.
+
+        Returns:
+          Dictionary object of the variable. None if:
+          - Feature key is invalid.
+          - Variable key is invalid.
+          - Mismatch with type of variable.
+        """
+
+        variable_type = entities.Variable.Type.JSON
+        project_config = self.config_manager.get_config()
+        if not project_config:
+            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('get_feature_variable_json'))
+            return None
+
+        return self._get_feature_variable_for_type(  # type: ignore[no-any-return]
+            project_config, feature_key, variable_key, variable_type, user_id, attributes,
+        )
+
+    def get_all_feature_variables(
+        self, feature_key: str, user_id: str, attributes: Optional[UserAttributes] = None
+    ) -> Optional[dict[str, Any]]:
+        """ Returns dictionary of all variables and their corresponding values in the context of a feature.
+
+        Args:
+          feature_key: Key of the feature whose variable's value is being accessed.
+          user_id: ID for user.
+          attributes: Dict representing user attributes.
+
+        Returns:
+          Dictionary mapping variable key to variable value. None if:
+          - Feature key is invalid.
+        """
+
+        project_config = self.config_manager.get_config()
+        if not project_config:
+            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('get_all_feature_variables'))
+            return None
+
+        return self._get_all_feature_variables_for_type(
+            project_config, feature_key, user_id, attributes,
+        )
+
+    def set_forced_variation(self, experiment_key: str, user_id: str, variation_key: Optional[str]) -> bool:
+        """ Force a user into a variation for a given experiment.
+
+        Args:
+         experiment_key: A string key identifying the experiment.
+         user_id: The user ID.
+         variation_key: A string variation key that specifies the variation which the user.
+         will be forced into. If null, then clear the existing experiment-to-variation mapping.
+
+        Returns:
+          A boolean value that indicates if the set completed successfully.
+        """
+
+        if not self.is_valid:
+            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('set_forced_variation'))
+            return False
+
+        if not validator.is_non_empty_string(experiment_key):
+            self.logger.error(enums.Errors.INVALID_INPUT.format('experiment_key'))
+            return False
+
+        if not isinstance(user_id, str):
+            self.logger.error(enums.Errors.INVALID_INPUT.format('user_id'))
+            return False
+
+        project_config = self.config_manager.get_config()
+        if not project_config:
+            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('set_forced_variation'))
+            return False
+
+        return self.decision_service.set_forced_variation(project_config, experiment_key, user_id, variation_key)
+
+    def get_forced_variation(self, experiment_key: str, user_id: str) -> Optional[str]:
+        """ Gets the forced variation for a given user and experiment.
+
+        Args:
+          experiment_key: A string key identifying the experiment.
+          user_id: The user ID.
+
+        Returns:
+          The forced variation key. None if no forced variation key.
+        """
+
+        if not self.is_valid:
+            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('get_forced_variation'))
+            return None
+
+        if not validator.is_non_empty_string(experiment_key):
+            self.logger.error(enums.Errors.INVALID_INPUT.format('experiment_key'))
+            return None
+
+        if not isinstance(user_id, str):
+            self.logger.error(enums.Errors.INVALID_INPUT.format('user_id'))
+            return None
+
+        project_config = self.config_manager.get_config()
+        if not project_config:
+            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('get_forced_variation'))
+            return None
+
+        forced_variation, _ = self.decision_service.get_forced_variation(project_config, experiment_key, user_id)
+        return forced_variation.key if forced_variation else None
+
+    def get_optimizely_config(self) -> Optional[OptimizelyConfig]:
+        """ Gets OptimizelyConfig instance for the current project config.
+
+        Returns:
+            OptimizelyConfig instance. None if the optimizely instance is invalid or
+            project config isn't available.
+        """
+        if not self.is_valid:
+            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('get_optimizely_config'))
+            return None
+
+        project_config = self.config_manager.get_config()
+        if not project_config:
+            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('get_optimizely_config'))
+            return None
+
+        # Customized Config Manager may not have optimizely_config defined.
+        if hasattr(self.config_manager, 'optimizely_config'):
+            return self.config_manager.optimizely_config
+
+        return OptimizelyConfigService(project_config).get_config()
+
+    def create_user_context(
+        self, user_id: str, attributes: Optional[UserAttributes] = None
+    ) -> Optional[OptimizelyUserContext]:
+        """
+        We do not check for is_valid here as a user context can be created successfully
+        even when the SDK is not fully configured.
+
+        Args:
+            user_id: string to use as user id for user context
+            attributes: dictionary of attributes or None
+
+        Returns:
+            UserContext instance or None if the user id or attributes are invalid.
+        """
+        if not isinstance(user_id, str):
+            self.logger.error(enums.Errors.INVALID_INPUT.format('user_id'))
+            return None
+
+        if attributes is not None and type(attributes) is not dict:
+            self.logger.error(enums.Errors.INVALID_INPUT.format('attributes'))
+            return None
+
+        return OptimizelyUserContext(self, self.logger, user_id, attributes, True)
+
+    def _decide(
+        self, user_context: Optional[OptimizelyUserContext], key: str,
+        decide_options: Optional[list[str]] = None
+    ) -> OptimizelyDecision:
+        """
+        decide calls optimizely decide with feature key provided
+        Args:
+            user_context: UserContent with userid and attributes
+            key: feature key
+            decide_options: list of OptimizelyDecideOption
+
+        Returns:
+            Decision object
+        """
+
+        # raising on user context as it is internal and not provided directly by the user.
+        if not isinstance(user_context, OptimizelyUserContext):
+            raise exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('user_context'))
+
+        reasons = []
+
+        # check if SDK is ready
+        if not self.is_valid:
+            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('decide'))
+            reasons.append(OptimizelyDecisionMessage.SDK_NOT_READY)
+            return OptimizelyDecision(flag_key=key, user_context=user_context, reasons=reasons)
+
+        # validate that key is a string
+        if not isinstance(key, str):
+            self.logger.error('Key parameter is invalid')
+            reasons.append(OptimizelyDecisionMessage.FLAG_KEY_INVALID.format(key))
+            return OptimizelyDecision(flag_key=key, user_context=user_context, reasons=reasons)
+
+        # validate that key maps to a feature flag
+        config = self.config_manager.get_config()
+        if not config:
+            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('decide'))
+            reasons.append(OptimizelyDecisionMessage.SDK_NOT_READY)
+            return OptimizelyDecision(flag_key=key, user_context=user_context, reasons=reasons)
+
+        feature_flag = config.get_feature_from_key(key)
+        if feature_flag is None:
+            self.logger.error(f"No feature flag was found for key '{key}'.")
+            reasons.append(OptimizelyDecisionMessage.FLAG_KEY_INVALID.format(key))
+            return OptimizelyDecision(flag_key=key, user_context=user_context, reasons=reasons)
+
+        # merge decide_options and default_decide_options
+        if isinstance(decide_options, list):
+            decide_options += self.default_decide_options
+        else:
+            self.logger.debug('Provided decide options is not an array. Using default decide options.')
+            decide_options = self.default_decide_options
+
+        # Create Optimizely Decision Result.
+        user_id = user_context.user_id
+        attributes = user_context.get_user_attributes()
+        variation_key = None
+        variation = None
+        feature_enabled = False
+        rule_key = None
+        flag_key = key
+        all_variables = {}
+        experiment = None
+        decision_source = DecisionSources.ROLLOUT
+        source_info: dict[str, Any] = {}
+        decision_event_dispatched = False
+
+        # Check forced decisions first
+        optimizely_decision_context = OptimizelyUserContext.OptimizelyDecisionContext(flag_key=key, rule_key=rule_key)
+        forced_decision_response = self.decision_service.validated_forced_decision(config,
+                                                                                   optimizely_decision_context,
+                                                                                   user_context)
+        variation, decision_reasons = forced_decision_response
+        reasons += decision_reasons
+
+        if variation:
+            decision = Decision(None, variation, enums.DecisionSources.FEATURE_TEST)
+        else:
+            # Regular decision
+            decision, decision_reasons = self.decision_service.get_variation_for_feature(config,
+                                                                                         feature_flag,
+                                                                                         user_context, decide_options)
+
+            reasons += decision_reasons
+
+        # Fill in experiment and variation if returned (rollouts can have featureEnabled variables as well.)
+        if decision.experiment is not None:
+            experiment = decision.experiment
+            source_info["experiment"] = experiment
+            rule_key = experiment.key if experiment else None
+        if decision.variation is not None:
+            variation = decision.variation
+            variation_key = variation.key
+            feature_enabled = variation.featureEnabled
+            decision_source = decision.source
+            source_info["variation"] = variation
+
+        # Send impression event if Decision came from a feature
+        # test and decide options doesn't include disableDecisionEvent
+        if OptimizelyDecideOption.DISABLE_DECISION_EVENT not in decide_options:
+            if decision_source == DecisionSources.FEATURE_TEST or config.send_flag_decisions:
+                self._send_impression_event(config, experiment, variation, flag_key, rule_key or '',
+                                            decision_source, feature_enabled,
+                                            user_id, attributes)
+
+                decision_event_dispatched = True
+
+        # Generate all variables map if decide options doesn't include excludeVariables
+        if OptimizelyDecideOption.EXCLUDE_VARIABLES not in decide_options:
+            for variable_key, variable in feature_flag.variables.items():
+                variable_value = variable.defaultValue
+                if feature_enabled:
+                    variable_value = config.get_variable_value_for_variation(variable, decision.variation)
+                    self.logger.debug(
+                        f'Got variable value "{variable_value}" for '
+                        f'variable "{variable_key}" of feature flag "{flag_key}".'
+                    )
+
+                try:
+                    actual_value = config.get_typecast_value(variable_value, variable.type)
+                except:
+                    self.logger.error('Unable to cast value. Returning None.')
+                    actual_value = None
+
+                all_variables[variable_key] = actual_value
+
+        should_include_reasons = OptimizelyDecideOption.INCLUDE_REASONS in decide_options
+
+        # Send notification
+        self.notification_center.send_notifications(
+            enums.NotificationTypes.DECISION,
+            enums.DecisionNotificationTypes.FLAG,
+            user_id,
+            attributes or {},
+            {
+                'flag_key': flag_key,
+                'enabled': feature_enabled,
+                'variables': all_variables,
+                'variation_key': variation_key,
+                'rule_key': rule_key,
+                'reasons': reasons if should_include_reasons else [],
+                'decision_event_dispatched': decision_event_dispatched
+
+            },
+        )
+
+        return OptimizelyDecision(variation_key=variation_key, enabled=feature_enabled, variables=all_variables,
+                                  rule_key=rule_key, flag_key=flag_key,
+                                  user_context=user_context, reasons=reasons if should_include_reasons else []
+                                  )
+
+    def _decide_all(
+        self,
+        user_context: Optional[OptimizelyUserContext],
+        decide_options: Optional[list[str]] = None
+    ) -> dict[str, OptimizelyDecision]:
+        """
+        decide_all will return a decision for every feature key in the current config
+        Args:
+            user_context: UserContent object
+            decide_options: Array of DecisionOption
+
+        Returns:
+            A dictionary of feature key to Decision
+        """
+        # raising on user context as it is internal and not provided directly by the user.
+        if not isinstance(user_context, OptimizelyUserContext):
+            raise exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('user_context'))
+
+        # check if SDK is ready
+        if not self.is_valid:
+            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('decide_all'))
+            return {}
+
+        config = self.config_manager.get_config()
+        if not config:
+            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('decide'))
+            return {}
+
+        keys = []
+        for f in config.feature_flags:
+            keys.append(f['key'])
+        return self._decide_for_keys(user_context, keys, decide_options)
+
+    def _decide_for_keys(
+        self,
+        user_context: Optional[OptimizelyUserContext],
+        keys: list[str],
+        decide_options: Optional[list[str]] = None
+    ) -> dict[str, OptimizelyDecision]:
+        """
+        Args:
+            user_context: UserContent
+            keys: list of feature keys to run decide on.
+            decide_options: an array of DecisionOption objects
+
+        Returns:
+            An dictionary of feature key to Decision
+        """
+        # raising on user context as it is internal and not provided directly by the user.
+        if not isinstance(user_context, OptimizelyUserContext):
+            raise exceptions.InvalidInputException(enums.Errors.INVALID_INPUT.format('user_context'))
+
+        # check if SDK is ready
+        if not self.is_valid:
+            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('decide_for_keys'))
+            return {}
+
+        # merge decide_options and default_decide_options
+        merged_decide_options: list[str] = []
+        if isinstance(decide_options, list):
+            merged_decide_options = decide_options[:]
+            merged_decide_options += self.default_decide_options
+        else:
+            self.logger.debug('Provided decide options is not an array. Using default decide options.')
+            merged_decide_options = self.default_decide_options
+
+        enabled_flags_only = OptimizelyDecideOption.ENABLED_FLAGS_ONLY in merged_decide_options
+
+        decisions = {}
+        for key in keys:
+            decision = self._decide(user_context, key, decide_options)
+            if enabled_flags_only and not decision.enabled:
+                continue
+            decisions[key] = decision
+        return decisions
+
+    def _setup_odp(self, sdk_key: Optional[str]) -> None:
+        """
+        - Make sure odp manager is instantiated with provided parameters or defaults.
+        - Set up listener to update odp_config when datafile is updated.
+        - Manually call callback in case datafile was received before the listener was registered.
+        """
+
+        # no need to instantiate a cache if a custom cache or segment manager is provided.
+        if (
+            not self.sdk_settings.odp_disabled and
+            not self.sdk_settings.odp_segment_manager and
+            not self.sdk_settings.segments_cache
+        ):
+            self.sdk_settings.segments_cache = LRUCache(
+                self.sdk_settings.segments_cache_size,
+                self.sdk_settings.segments_cache_timeout_in_secs
+            )
+
+        self.odp_manager = OdpManager(
+            self.sdk_settings.odp_disabled,
+            self.sdk_settings.segments_cache,
+            self.sdk_settings.odp_segment_manager,
+            self.sdk_settings.odp_event_manager,
+            self.sdk_settings.fetch_segments_timeout,
+            self.sdk_settings.odp_event_timeout,
+            self.sdk_settings.odp_flush_interval,
+            self.logger,
+        )
+
+        if self.sdk_settings.odp_disabled:
+            return
+
+        internal_notification_center = _NotificationCenterRegistry.get_notification_center(sdk_key, self.logger)
+        if internal_notification_center:
+            internal_notification_center.add_notification_listener(
+                enums.NotificationTypes.OPTIMIZELY_CONFIG_UPDATE,
+                self._update_odp_config_on_datafile_update
+            )
+
+        self._update_odp_config_on_datafile_update()
+
+    def _update_odp_config_on_datafile_update(self) -> None:
+        config = None
+
+        if isinstance(self.config_manager, PollingConfigManager):
+            # can not use get_config here because callback is fired before _config_ready event is set
+            # and that would be a deadlock
+            config = self.config_manager._config
+        elif self.config_manager:
+            config = self.config_manager.get_config()
+
+        if not config:
+            return
+
+        self.odp_manager.update_odp_config(
+            config.public_key_for_odp,
+            config.host_for_odp,
+            config.all_segments
+        )
+
+    def _identify_user(self, user_id: str) -> None:
+        if not self.is_valid:
+            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('identify_user'))
+            return
+
+        config = self.config_manager.get_config()
+        if not config:
+            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('identify_user'))
+            return
+
+        self.odp_manager.identify_user(user_id)
+
+    def _fetch_qualified_segments(self, user_id: str, options: Optional[list[str]] = None) -> Optional[list[str]]:
+        if not self.is_valid:
+            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('fetch_qualified_segments'))
+            return None
+
+        config = self.config_manager.get_config()
+        if not config:
+            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('fetch_qualified_segments'))
+            return None
+
+        return self.odp_manager.fetch_qualified_segments(user_id, options or [])
+
+    def send_odp_event(
+        self,
+        action: str,
+        identifiers: dict[str, str],
+        type: str = enums.OdpManagerConfig.EVENT_TYPE,
+        data: Optional[dict[str, str | int | float | bool | None]] = None
+    ) -> None:
+        """
+        Send an event to the ODP server.
+
+        Args:
+            action: The event action name. Cannot be None or empty string.
+            identifiers: A dictionary for identifiers. The caller must provide at least one key-value pair.
+            type: The event type. Default 'fullstack'.
+            data: An optional dictionary for associated data. The default event data will be added to this data
+            before sending to the ODP server.
+        """
+        if not self.is_valid:
+            self.logger.error(enums.Errors.INVALID_OPTIMIZELY.format('send_odp_event'))
+            return
+
+        if action is None or action == "":
+            self.logger.error(enums.Errors.ODP_INVALID_ACTION)
+            return
+
+        if not identifiers or not isinstance(identifiers, dict):
+            self.logger.error('ODP events must have at least one key-value pair in identifiers.')
+            return
+
+        if type is None or type == "":
+            type = enums.OdpManagerConfig.EVENT_TYPE
+
+        config = self.config_manager.get_config()
+        if not config:
+            self.logger.error(enums.Errors.INVALID_PROJECT_CONFIG.format('send_odp_event'))
+            return
+
+        self.odp_manager.send_event(type, action, identifiers, data or {})
+
+    def close(self) -> None:
+        if callable(getattr(self.event_processor, 'stop', None)):
+            self.event_processor.stop()  # type: ignore[attr-defined]
+        if self.is_valid:
+            self.odp_manager.close()
+        if callable(getattr(self.config_manager, 'stop', None)):
+            self.config_manager.stop()  # type: ignore[attr-defined]
```

### Comparing `optimizely-sdk-4.1.1/optimizely/optimizely_config.py` & `optimizely-sdk-5.0.0b0/optimizely/optimizely_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,501 +1,534 @@
-# Copyright 2020-2021, Optimizely
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import copy
-from .helpers.condition import ConditionOperatorTypes
-
-from .project_config import ProjectConfig
-
-
-class OptimizelyConfig(object):
-    def __init__(self, revision, experiments_map, features_map, datafile=None,
-                 sdk_key=None, environment_key=None, attributes=None, events=None,
-                 audiences=None):
-        self.revision = revision
-
-        # This experiments_map is for experiments of legacy projects only.
-        # For flag projects, experiment keys are not guaranteed to be unique
-        # across multiple flags, so this map may not include all experiments
-        # when keys conflict.
-        self.experiments_map = experiments_map
-
-        self.features_map = features_map
-        self._datafile = datafile
-        self.sdk_key = sdk_key or ''
-        self.environment_key = environment_key or ''
-        self.attributes = attributes or []
-        self.events = events or []
-        self.audiences = audiences or []
-
-    def get_datafile(self):
-        """ Get the datafile associated with OptimizelyConfig.
-
-        Returns:
-            A JSON string representation of the environment's datafile.
-        """
-        return self._datafile
-
-
-class OptimizelyExperiment(object):
-    def __init__(self, id, key, variations_map, audiences=''):
-        self.id = id
-        self.key = key
-        self.variations_map = variations_map
-        self.audiences = audiences
-
-
-class OptimizelyFeature(object):
-    def __init__(self, id, key, experiments_map, variables_map):
-        self.id = id
-        self.key = key
-
-        # This experiments_map is now deprecated,
-        # Please use delivery_rules and experiment_rules
-        self.experiments_map = experiments_map
-
-        self.variables_map = variables_map
-        self.delivery_rules = []
-        self.experiment_rules = []
-
-
-class OptimizelyVariation(object):
-    def __init__(self, id, key, feature_enabled, variables_map):
-        self.id = id
-        self.key = key
-        self.feature_enabled = feature_enabled
-        self.variables_map = variables_map
-
-
-class OptimizelyVariable(object):
-    def __init__(self, id, key, variable_type, value):
-        self.id = id
-        self.key = key
-        self.type = variable_type
-        self.value = value
-
-
-class OptimizelyAttribute(object):
-    def __init__(self, id, key):
-        self.id = id
-        self.key = key
-
-
-class OptimizelyEvent(object):
-    def __init__(self, id, key, experiment_ids):
-        self.id = id
-        self.key = key
-        self.experiment_ids = experiment_ids
-
-
-class OptimizelyAudience(object):
-    def __init__(self, id, name, conditions):
-        self.id = id
-        self.name = name
-        self.conditions = conditions
-
-
-class OptimizelyConfigService(object):
-    """ Class encapsulating methods to be used in creating instance of OptimizelyConfig. """
-
-    def __init__(self, project_config):
-        """
-        Args:
-            project_config ProjectConfig
-        """
-        self.is_valid = True
-
-        if not isinstance(project_config, ProjectConfig):
-            self.is_valid = False
-            return
-
-        self._datafile = project_config.to_datafile()
-        self.experiments = project_config.experiments
-        self.feature_flags = project_config.feature_flags
-        self.groups = project_config.groups
-        self.revision = project_config.revision
-        self.sdk_key = project_config.sdk_key
-        self.environment_key = project_config.environment_key
-        self.attributes = project_config.attributes
-        self.events = project_config.events
-        self.rollouts = project_config.rollouts
-
-        self._create_lookup_maps()
-
-        '''
-            Merging typed_audiences with audiences from project_config.
-            The typed_audiences has higher precedence.
-        '''
-        optly_typed_audiences = []
-        id_lookup_dict = {}
-        for typed_audience in project_config.typed_audiences:
-            optly_audience = OptimizelyAudience(
-                typed_audience.get('id'),
-                typed_audience.get('name'),
-                typed_audience.get('conditions')
-            )
-            optly_typed_audiences.append(optly_audience)
-            id_lookup_dict[typed_audience.get('id')] = typed_audience.get('id')
-
-        for old_audience in project_config.audiences:
-            # check if old_audience.id exists in new_audiences.id from typed_audiences
-            if old_audience.get('id') not in id_lookup_dict and old_audience.get('id') != "$opt_dummy_audience":
-                # Convert audiences lists to OptimizelyAudience array
-                optly_audience = OptimizelyAudience(
-                    old_audience.get('id'),
-                    old_audience.get('name'),
-                    old_audience.get('conditions')
-                )
-                optly_typed_audiences.append(optly_audience)
-
-        self.audiences = optly_typed_audiences
-
-    def replace_ids_with_names(self, conditions, audiences_map):
-        '''
-            Gets conditions and audiences_map [id:name]
-
-            Returns:
-                a string of conditions with id's swapped with names
-                or empty string if no conditions found.
-
-        '''
-        if conditions is not None:
-            return self.stringify_conditions(conditions, audiences_map)
-        else:
-            return ''
-
-    def lookup_name_from_id(self, audience_id, audiences_map):
-        '''
-            Gets and audience ID and audiences map
-
-            Returns:
-                The name corresponding to the ID
-                or '' if not found.
-        '''
-        name = None
-        try:
-            name = audiences_map[audience_id]
-        except KeyError:
-            name = audience_id
-
-        return name
-
-    def stringify_conditions(self, conditions, audiences_map):
-        '''
-            Gets a list of conditions from an entities.Experiment
-            and an audiences_map [id:name]
-
-            Returns:
-                A string of conditions and names for the provided
-                list of conditions.
-        '''
-        ARGS = ConditionOperatorTypes.operators
-        operand = 'OR'
-        conditions_str = ''
-        length = len(conditions)
-
-        # Edge cases for lengths 0, 1 or 2
-        if length == 0:
-            return ''
-        if length == 1 and conditions[0] not in ARGS:
-            return '"' + self.lookup_name_from_id(conditions[0], audiences_map) + '"'
-        if length == 2 and conditions[0] in ARGS and \
-            type(conditions[1]) is not list and \
-                conditions[1] not in ARGS:
-            if conditions[0] != "not":
-                return '"' + self.lookup_name_from_id(conditions[1], audiences_map) + '"'
-            else:
-                return conditions[0].upper() + \
-                    ' "' + self.lookup_name_from_id(conditions[1], audiences_map) + '"'
-        # If length is 2 (where the one elemnt is a list) or greater
-        if length > 1:
-            for i in range(length):
-                # Operand is handled here and made Upper Case
-                if conditions[i] in ARGS:
-                    operand = conditions[i].upper()
-                else:
-                    # Check if element is a list or not
-                    if type(conditions[i]) == list:
-                        # Check if at the end or not to determine where to add the operand
-                        # Recursive call to call stringify on embedded list
-                        if i + 1 < length:
-                            conditions_str += '(' + self.stringify_conditions(conditions[i], audiences_map) + ') '
-                        else:
-                            conditions_str += operand + \
-                                ' (' + self.stringify_conditions(conditions[i], audiences_map) + ')'
-                    # If the item is not a list, we process as an audience ID and retrieve the name
-                    else:
-                        audience_name = self.lookup_name_from_id(conditions[i], audiences_map)
-                        if audience_name is not None:
-                            # Below handles all cases for one ID or greater
-                            if i + 1 < length - 1:
-                                conditions_str += '"' + audience_name + '" ' + operand + ' '
-                            elif i + 1 == length:
-                                conditions_str += operand + ' "' + audience_name + '"'
-                            else:
-                                conditions_str += '"' + audience_name + '" '
-
-        return conditions_str or ''
-
-    def get_config(self):
-        """ Gets instance of OptimizelyConfig
-
-        Returns:
-            Optimizely Config instance or None if OptimizelyConfigService is invalid.
-        """
-
-        if not self.is_valid:
-            return None
-
-        experiments_key_map, experiments_id_map = self._get_experiments_maps()
-        features_map = self._get_features_map(experiments_id_map)
-
-        return OptimizelyConfig(
-            self.revision,
-            experiments_key_map,
-            features_map,
-            self._datafile,
-            self.sdk_key,
-            self.environment_key,
-            self._get_attributes_list(self.attributes),
-            self._get_events_list(self.events),
-            self.audiences
-        )
-
-    def _create_lookup_maps(self):
-        """ Creates lookup maps to avoid redundant iteration of config objects.  """
-
-        self.exp_id_to_feature_map = {}
-        self.feature_key_variable_key_to_variable_map = {}
-        self.feature_key_variable_id_to_variable_map = {}
-        self.feature_id_variable_id_to_feature_variables_map = {}
-        self.feature_id_variable_key_to_feature_variables_map = {}
-
-        for feature in self.feature_flags:
-            for experiment_id in feature['experimentIds']:
-                self.exp_id_to_feature_map[experiment_id] = feature
-
-            variables_key_map = {}
-            variables_id_map = {}
-            for variable in feature.get('variables', []):
-                opt_variable = OptimizelyVariable(
-                    variable['id'], variable['key'], variable['type'], variable['defaultValue']
-                )
-                variables_key_map[variable['key']] = opt_variable
-                variables_id_map[variable['id']] = opt_variable
-
-            self.feature_id_variable_id_to_feature_variables_map[feature['id']] = variables_id_map
-            self.feature_id_variable_key_to_feature_variables_map[feature['id']] = variables_key_map
-            self.feature_key_variable_key_to_variable_map[feature['key']] = variables_key_map
-            self.feature_key_variable_id_to_variable_map[feature['key']] = variables_id_map
-
-    def _get_variables_map(self, experiment, variation, feature_id=None):
-        """ Gets variables map for given experiment and variation.
-
-        Args:
-            experiment dict -- Experiment parsed from the datafile.
-            variation dict -- Variation of the given experiment.
-
-        Returns:
-            dict - Map of variable key to OptimizelyVariable for the given variation.
-        """
-        variables_map = {}
-
-        feature_flag = self.exp_id_to_feature_map.get(experiment['id'], None)
-        if feature_flag is None and feature_id is None:
-            return {}
-
-        # set default variables for each variation
-        if feature_id:
-            variables_map = copy.deepcopy(self.feature_id_variable_key_to_feature_variables_map[feature_id])
-        else:
-            variables_map = copy.deepcopy(self.feature_key_variable_key_to_variable_map[feature_flag['key']])
-
-            # set variation specific variable value if any
-            if variation.get('featureEnabled'):
-                for variable in variation.get('variables', []):
-                    feature_variable = self.feature_key_variable_id_to_variable_map[feature_flag['key']][variable['id']]
-                    variables_map[feature_variable.key].value = variable['value']
-
-        return variables_map
-
-    def _get_variations_map(self, experiment, feature_id=None):
-        """ Gets variation map for the given experiment.
-
-        Args:
-            experiment dict -- Experiment parsed from the datafile.
-
-        Returns:
-            dict -- Map of variation key to OptimizelyVariation.
-        """
-        variations_map = {}
-
-        for variation in experiment.get('variations', []):
-            variables_map = self._get_variables_map(experiment, variation, feature_id)
-            feature_enabled = variation.get('featureEnabled', None)
-
-            optly_variation = OptimizelyVariation(
-                variation['id'], variation['key'], feature_enabled, variables_map
-            )
-
-            variations_map[variation['key']] = optly_variation
-
-        return variations_map
-
-    def _get_all_experiments(self):
-        """ Gets all experiments in the project config.
-
-        Returns:
-            list -- List of dicts of experiments.
-        """
-        experiments = self.experiments
-
-        for group in self.groups:
-            experiments = experiments + group['experiments']
-
-        return experiments
-
-    def _get_experiments_maps(self):
-        """ Gets maps for all the experiments in the project config and
-        updates the experiment with updated experiment audiences string.
-
-        Returns:
-            dict, dict -- experiment key/id to OptimizelyExperiment maps.
-        """
-        # Key map is required for the OptimizelyConfig response.
-        experiments_key_map = {}
-        # Id map comes in handy to figure out feature experiment.
-        experiments_id_map = {}
-        # Audiences map to use for updating experiments with new audience conditions string
-        audiences_map = {}
-
-        # Build map from OptimizelyAudience array
-        for optly_audience in self.audiences:
-            audiences_map[optly_audience.id] = optly_audience.name
-
-        all_experiments = self._get_all_experiments()
-        for exp in all_experiments:
-            optly_exp = OptimizelyExperiment(
-                exp['id'], exp['key'], self._get_variations_map(exp)
-            )
-            # Updating each OptimizelyExperiment
-            audiences = self.replace_ids_with_names(exp.get('audienceConditions', []), audiences_map)
-            optly_exp.audiences = audiences or ''
-
-            experiments_key_map[exp['key']] = optly_exp
-            experiments_id_map[exp['id']] = optly_exp
-
-        return experiments_key_map, experiments_id_map
-
-    def _get_features_map(self, experiments_id_map):
-        """ Gets features map for the project config.
-
-        Args:
-            experiments_id_map dict -- experiment id to OptimizelyExperiment map
-
-        Returns:
-            dict -- feaure key to OptimizelyFeature map
-        """
-        features_map = {}
-        experiment_rules = []
-
-        for feature in self.feature_flags:
-
-            delivery_rules = self._get_delivery_rules(self.rollouts, feature.get('rolloutId'), feature['id'])
-            experiment_rules = []
-
-            exp_map = {}
-            for experiment_id in feature.get('experimentIds', []):
-                optly_exp = experiments_id_map[experiment_id]
-                exp_map[optly_exp.key] = optly_exp
-                experiment_rules.append(optly_exp)
-
-            variables_map = self.feature_key_variable_key_to_variable_map[feature['key']]
-
-            optly_feature = OptimizelyFeature(
-                feature['id'], feature['key'], exp_map, variables_map
-            )
-            optly_feature.experiment_rules = experiment_rules
-            optly_feature.delivery_rules = delivery_rules
-
-            features_map[feature['key']] = optly_feature
-
-        return features_map
-
-    def _get_delivery_rules(self, rollouts, rollout_id, feature_id):
-        """ Gets an array of rollouts for the project config
-
-        returns:
-            an array of OptimizelyExperiments as delivery rules.
-        """
-        # Return list for delivery rules
-        delivery_rules = []
-        # Audiences map to use for updating experiments with new audience conditions string
-        audiences_map = {}
-
-        # Gets a rollout based on provided rollout_id
-        rollout = [rollout for rollout in rollouts if rollout.get('id') == rollout_id]
-
-        if rollout:
-            rollout = rollout[0]
-            # Build map from OptimizelyAudience array
-            for optly_audience in self.audiences:
-                audiences_map[optly_audience.id] = optly_audience.name
-
-            # Get the experiments for that rollout
-            experiments = rollout.get('experiments')
-            if experiments:
-                for experiment in experiments:
-                    optly_exp = OptimizelyExperiment(
-                        experiment['id'], experiment['key'], self._get_variations_map(experiment, feature_id)
-                    )
-                    audiences = self.replace_ids_with_names(experiment.get('audienceConditions', []), audiences_map)
-                    optly_exp.audiences = audiences
-
-                    delivery_rules.append(optly_exp)
-
-        return delivery_rules
-
-    def _get_attributes_list(self, attributes):
-        """ Gets attributes list for the project config
-
-        Returns:
-            List - OptimizelyAttributes
-        """
-        attributes_list = []
-
-        for attribute in attributes:
-            optly_attribute = OptimizelyAttribute(
-                attribute['id'],
-                attribute['key']
-            )
-            attributes_list.append(optly_attribute)
-
-        return attributes_list
-
-    def _get_events_list(self, events):
-        """ Gets events list for the project_config
-
-        Returns:
-            List - OptimizelyEvents
-        """
-        events_list = []
-
-        for event in events:
-            optly_event = OptimizelyEvent(
-                event['id'],
-                event['key'],
-                event['experimentIds']
-            )
-            events_list.append(optly_event)
-
-        return events_list
+# Copyright 2020-2022, Optimizely
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from __future__ import annotations
+import copy
+from typing import Any, Optional
+
+from .helpers.condition import ConditionOperatorTypes
+from .helpers.types import VariationDict, ExperimentDict, RolloutDict, AttributeDict, EventDict
+from .project_config import ProjectConfig
+
+
+class OptimizelyConfig:
+    def __init__(
+        self, revision: str,
+        experiments_map: dict[str, OptimizelyExperiment],
+        features_map: dict[str, OptimizelyFeature],
+        datafile: Optional[str] = None,
+        sdk_key: Optional[str] = None,
+        environment_key: Optional[str] = None,
+        attributes: Optional[list[OptimizelyAttribute]] = None,
+        events: Optional[list[OptimizelyEvent]] = None,
+        audiences: Optional[list[OptimizelyAudience]] = None
+    ):
+        self.revision = revision
+
+        # This experiments_map is for experiments of legacy projects only.
+        # For flag projects, experiment keys are not guaranteed to be unique
+        # across multiple flags, so this map may not include all experiments
+        # when keys conflict.
+        self.experiments_map = experiments_map
+
+        self.features_map = features_map
+        self._datafile = datafile
+        self.sdk_key = sdk_key or ''
+        self.environment_key = environment_key or ''
+        self.attributes = attributes or []
+        self.events = events or []
+        self.audiences = audiences or []
+
+    def get_datafile(self) -> Optional[str]:
+        """ Get the datafile associated with OptimizelyConfig.
+
+        Returns:
+            A JSON string representation of the environment's datafile.
+        """
+        return self._datafile
+
+
+class OptimizelyExperiment:
+    def __init__(self, id: str, key: str, variations_map: dict[str, OptimizelyVariation], audiences: str = ''):
+        self.id = id
+        self.key = key
+        self.variations_map = variations_map
+        self.audiences = audiences
+
+
+class OptimizelyFeature:
+    def __init__(
+        self,
+        id: str,
+        key: str,
+        experiments_map: dict[str, OptimizelyExperiment],
+        variables_map: dict[str, OptimizelyVariable]
+    ):
+        self.id = id
+        self.key = key
+
+        # This experiments_map is now deprecated,
+        # Please use delivery_rules and experiment_rules
+        self.experiments_map = experiments_map
+
+        self.variables_map = variables_map
+        self.delivery_rules: list[OptimizelyExperiment] = []
+        self.experiment_rules: list[OptimizelyExperiment] = []
+
+
+class OptimizelyVariation:
+    def __init__(
+        self, id: str, key: str, feature_enabled: Optional[bool], variables_map: dict[str, OptimizelyVariable]
+    ):
+        self.id = id
+        self.key = key
+        self.feature_enabled = feature_enabled
+        self.variables_map = variables_map
+
+
+class OptimizelyVariable:
+    def __init__(self, id: str, key: str, variable_type: str, value: Any):
+        self.id = id
+        self.key = key
+        self.type = variable_type
+        self.value = value
+
+
+class OptimizelyAttribute:
+    def __init__(self, id: str, key: str):
+        self.id = id
+        self.key = key
+
+
+class OptimizelyEvent:
+    def __init__(self, id: str, key: str, experiment_ids: list[str]):
+        self.id = id
+        self.key = key
+        self.experiment_ids = experiment_ids
+
+
+class OptimizelyAudience:
+    def __init__(self, id: Optional[str], name: Optional[str], conditions: Optional[list[Any] | str]):
+        self.id = id
+        self.name = name
+        self.conditions = conditions
+
+
+class OptimizelyConfigService:
+    """ Class encapsulating methods to be used in creating instance of OptimizelyConfig. """
+
+    def __init__(self, project_config: ProjectConfig):
+        """
+        Args:
+            project_config ProjectConfig
+        """
+        self.is_valid = True
+
+        if not isinstance(project_config, ProjectConfig):
+            self.is_valid = False
+            return
+
+        self._datafile = project_config.to_datafile()
+        self.experiments = project_config.experiments
+        self.feature_flags = project_config.feature_flags
+        self.groups = project_config.groups
+        self.revision = project_config.revision
+        self.sdk_key = project_config.sdk_key
+        self.environment_key = project_config.environment_key
+        self.attributes = project_config.attributes
+        self.events = project_config.events
+        self.rollouts = project_config.rollouts
+
+        self._create_lookup_maps()
+
+        '''
+            Merging typed_audiences with audiences from project_config.
+            The typed_audiences has higher precedence.
+        '''
+        optly_typed_audiences: list[OptimizelyAudience] = []
+        id_lookup_dict = {}
+        for typed_audience in project_config.typed_audiences:
+            optly_audience = OptimizelyAudience(
+                typed_audience.get('id'),
+                typed_audience.get('name'),
+                typed_audience.get('conditions')
+            )
+            optly_typed_audiences.append(optly_audience)
+            id_lookup_dict[typed_audience.get('id')] = typed_audience.get('id')
+
+        for old_audience in project_config.audiences:
+            # check if old_audience.id exists in new_audiences.id from typed_audiences
+            if old_audience.get('id') not in id_lookup_dict and old_audience.get('id') != "$opt_dummy_audience":
+                # Convert audiences lists to OptimizelyAudience array
+                optly_audience = OptimizelyAudience(
+                    old_audience.get('id'),
+                    old_audience.get('name'),
+                    old_audience.get('conditions')
+                )
+                optly_typed_audiences.append(optly_audience)
+
+        self.audiences = optly_typed_audiences
+
+    def replace_ids_with_names(self, conditions: str | list[Any], audiences_map: dict[str, str]) -> str:
+        '''
+            Gets conditions and audiences_map [id:name]
+
+            Returns:
+                a string of conditions with id's swapped with names
+                or empty string if no conditions found.
+
+        '''
+        if conditions is not None:
+            return self.stringify_conditions(conditions, audiences_map)
+        else:
+            return ''
+
+    def lookup_name_from_id(self, audience_id: str, audiences_map: dict[str, str]) -> str:
+        '''
+            Gets and audience ID and audiences map
+
+            Returns:
+                The name corresponding to the ID
+                or '' if not found.
+        '''
+        name = None
+        try:
+            name = audiences_map[audience_id]
+        except KeyError:
+            name = audience_id
+
+        return name
+
+    def stringify_conditions(self, conditions: str | list[Any], audiences_map: dict[str, str]) -> str:
+        '''
+            Gets a list of conditions from an entities.Experiment
+            and an audiences_map [id:name]
+
+            Returns:
+                A string of conditions and names for the provided
+                list of conditions.
+        '''
+        ARGS = ConditionOperatorTypes.operators
+        operand = 'OR'
+        conditions_str = ''
+        length = len(conditions)
+
+        # Edge cases for lengths 0, 1 or 2
+        if length == 0:
+            return ''
+        if length == 1 and conditions[0] not in ARGS:
+            return '"' + self.lookup_name_from_id(conditions[0], audiences_map) + '"'
+        if length == 2 and conditions[0] in ARGS and \
+            type(conditions[1]) is not list and \
+                conditions[1] not in ARGS:
+            if conditions[0] != "not":
+                return '"' + self.lookup_name_from_id(conditions[1], audiences_map) + '"'
+            else:
+                return conditions[0].upper() + \
+                    ' "' + self.lookup_name_from_id(conditions[1], audiences_map) + '"'
+        # If length is 2 (where the one elemnt is a list) or greater
+        if length > 1:
+            for i in range(length):
+                # Operand is handled here and made Upper Case
+                if conditions[i] in ARGS:
+                    operand = conditions[i].upper()
+                else:
+                    # Check if element is a list or not
+                    if type(conditions[i]) == list:
+                        # Check if at the end or not to determine where to add the operand
+                        # Recursive call to call stringify on embedded list
+                        if i + 1 < length:
+                            conditions_str += '(' + self.stringify_conditions(conditions[i], audiences_map) + ') '
+                        else:
+                            conditions_str += operand + \
+                                ' (' + self.stringify_conditions(conditions[i], audiences_map) + ')'
+                    # If the item is not a list, we process as an audience ID and retrieve the name
+                    else:
+                        audience_name = self.lookup_name_from_id(conditions[i], audiences_map)
+                        if audience_name is not None:
+                            # Below handles all cases for one ID or greater
+                            if i + 1 < length - 1:
+                                conditions_str += '"' + audience_name + '" ' + operand + ' '
+                            elif i + 1 == length:
+                                conditions_str += operand + ' "' + audience_name + '"'
+                            else:
+                                conditions_str += '"' + audience_name + '" '
+
+        return conditions_str or ''
+
+    def get_config(self) -> Optional[OptimizelyConfig]:
+        """ Gets instance of OptimizelyConfig
+
+        Returns:
+            Optimizely Config instance or None if OptimizelyConfigService is invalid.
+        """
+
+        if not self.is_valid:
+            return None
+
+        experiments_key_map, experiments_id_map = self._get_experiments_maps()
+        features_map = self._get_features_map(experiments_id_map)
+
+        return OptimizelyConfig(
+            self.revision,
+            experiments_key_map,
+            features_map,
+            self._datafile,
+            self.sdk_key,
+            self.environment_key,
+            self._get_attributes_list(self.attributes),
+            self._get_events_list(self.events),
+            self.audiences
+        )
+
+    def _create_lookup_maps(self) -> None:
+        """ Creates lookup maps to avoid redundant iteration of config objects.  """
+
+        self.exp_id_to_feature_map = {}
+        self.feature_key_variable_key_to_variable_map = {}
+        self.feature_key_variable_id_to_variable_map = {}
+        self.feature_id_variable_id_to_feature_variables_map = {}
+        self.feature_id_variable_key_to_feature_variables_map = {}
+
+        for feature in self.feature_flags:
+            for experiment_id in feature['experimentIds']:
+                self.exp_id_to_feature_map[experiment_id] = feature
+
+            variables_key_map = {}
+            variables_id_map = {}
+            for variable in feature.get('variables', []):
+                opt_variable = OptimizelyVariable(
+                    variable['id'], variable['key'], variable['type'], variable['defaultValue']
+                )
+                variables_key_map[variable['key']] = opt_variable
+                variables_id_map[variable['id']] = opt_variable
+
+            self.feature_id_variable_id_to_feature_variables_map[feature['id']] = variables_id_map
+            self.feature_id_variable_key_to_feature_variables_map[feature['id']] = variables_key_map
+            self.feature_key_variable_key_to_variable_map[feature['key']] = variables_key_map
+            self.feature_key_variable_id_to_variable_map[feature['key']] = variables_id_map
+
+    def _get_variables_map(
+        self, experiment: ExperimentDict, variation: VariationDict, feature_id: Optional[str] = None
+    ) -> dict[str, OptimizelyVariable]:
+        """ Gets variables map for given experiment and variation.
+
+        Args:
+            experiment dict -- Experiment parsed from the datafile.
+            variation dict -- Variation of the given experiment.
+
+        Returns:
+            dict - Map of variable key to OptimizelyVariable for the given variation.
+        """
+        variables_map: dict[str, OptimizelyVariable] = {}
+
+        feature_flag = self.exp_id_to_feature_map.get(experiment['id'], None)
+        if feature_flag is None and feature_id is None:
+            return {}
+
+        # set default variables for each variation
+        if feature_id:
+            variables_map = copy.deepcopy(self.feature_id_variable_key_to_feature_variables_map[feature_id])
+        elif feature_flag:
+            variables_map = copy.deepcopy(self.feature_key_variable_key_to_variable_map[feature_flag['key']])
+
+            # set variation specific variable value if any
+            if variation.get('featureEnabled'):
+                feature_variables_map = self.feature_key_variable_id_to_variable_map[feature_flag['key']]
+                for variable in variation.get('variables', []):
+                    feature_variable = feature_variables_map.get(variable['id'])
+                    if feature_variable:
+                        variables_map[feature_variable.key].value = variable['value']
+
+        return variables_map
+
+    def _get_variations_map(
+        self, experiment: ExperimentDict, feature_id: Optional[str] = None
+    ) -> dict[str, OptimizelyVariation]:
+        """ Gets variation map for the given experiment.
+
+        Args:
+            experiment dict -- Experiment parsed from the datafile.
+
+        Returns:
+            dict -- Map of variation key to OptimizelyVariation.
+        """
+        variations_map: dict[str, OptimizelyVariation] = {}
+
+        for variation in experiment.get('variations', []):
+            variables_map = self._get_variables_map(experiment, variation, feature_id)
+            feature_enabled = variation.get('featureEnabled', None)
+
+            optly_variation = OptimizelyVariation(
+                variation['id'], variation['key'], feature_enabled, variables_map
+            )
+
+            variations_map[variation['key']] = optly_variation
+
+        return variations_map
+
+    def _get_all_experiments(self) -> list[ExperimentDict]:
+        """ Gets all experiments in the project config.
+
+        Returns:
+            list -- List of dicts of experiments.
+        """
+        experiments = self.experiments
+
+        for group in self.groups:
+            experiments = experiments + group['experiments']
+
+        return experiments
+
+    def _get_experiments_maps(self) -> tuple[dict[str, OptimizelyExperiment], dict[str, OptimizelyExperiment]]:
+        """ Gets maps for all the experiments in the project config and
+        updates the experiment with updated experiment audiences string.
+
+        Returns:
+            dict, dict -- experiment key/id to OptimizelyExperiment maps.
+        """
+        # Key map is required for the OptimizelyConfig response.
+        experiments_key_map = {}
+        # Id map comes in handy to figure out feature experiment.
+        experiments_id_map = {}
+        # Audiences map to use for updating experiments with new audience conditions string
+        audiences_map: dict[str, str] = {}
+
+        # Build map from OptimizelyAudience array
+        for optly_audience in self.audiences:
+            audience_id = optly_audience.id
+            audience_name = optly_audience.name
+            if audience_id is not None:
+                audiences_map[audience_id] = audience_name if audience_name is not None else ''
+
+        all_experiments = self._get_all_experiments()
+        for exp in all_experiments:
+            optly_exp = OptimizelyExperiment(
+                exp['id'], exp['key'], self._get_variations_map(exp)
+            )
+            # Updating each OptimizelyExperiment
+            audiences = self.replace_ids_with_names(exp.get('audienceConditions', []), audiences_map)
+            optly_exp.audiences = audiences or ''
+
+            experiments_key_map[exp['key']] = optly_exp
+            experiments_id_map[exp['id']] = optly_exp
+
+        return experiments_key_map, experiments_id_map
+
+    def _get_features_map(self, experiments_id_map: dict[str, OptimizelyExperiment]) -> dict[str, OptimizelyFeature]:
+        """ Gets features map for the project config.
+
+        Args:
+            experiments_id_map dict -- experiment id to OptimizelyExperiment map
+
+        Returns:
+            dict -- feaure key to OptimizelyFeature map
+        """
+        features_map = {}
+        experiment_rules: list[OptimizelyExperiment] = []
+
+        for feature in self.feature_flags:
+
+            delivery_rules = self._get_delivery_rules(self.rollouts, feature.get('rolloutId'), feature['id'])
+            experiment_rules = []
+
+            exp_map = {}
+            for experiment_id in feature.get('experimentIds', []):
+                optly_exp = experiments_id_map[experiment_id]
+                exp_map[optly_exp.key] = optly_exp
+                experiment_rules.append(optly_exp)
+
+            variables_map = self.feature_key_variable_key_to_variable_map[feature['key']]
+
+            optly_feature = OptimizelyFeature(
+                feature['id'], feature['key'], exp_map, variables_map
+            )
+            optly_feature.experiment_rules = experiment_rules
+            optly_feature.delivery_rules = delivery_rules
+
+            features_map[feature['key']] = optly_feature
+
+        return features_map
+
+    def _get_delivery_rules(
+        self, rollouts: list[RolloutDict], rollout_id: Optional[str], feature_id: str
+    ) -> list[OptimizelyExperiment]:
+        """ Gets an array of rollouts for the project config
+
+        returns:
+            an array of OptimizelyExperiments as delivery rules.
+        """
+        # Return list for delivery rules
+        delivery_rules = []
+        # Audiences map to use for updating experiments with new audience conditions string
+        audiences_map: dict[str, str] = {}
+
+        # Gets a rollout based on provided rollout_id
+        rollout = [rollout for rollout in rollouts if rollout.get('id') == rollout_id]
+
+        if rollout:
+            found_rollout = rollout[0]
+            # Build map from OptimizelyAudience array
+            for optly_audience in self.audiences:
+                audience_id = optly_audience.id
+                audience_name = optly_audience.name
+                if audience_id is not None:
+                    audiences_map[audience_id] = audience_name if audience_name is not None else ''
+
+            # Get the experiments for that rollout
+            experiments = found_rollout.get('experiments')
+            if experiments:
+                for experiment in experiments:
+                    optly_exp = OptimizelyExperiment(
+                        experiment['id'], experiment['key'], self._get_variations_map(experiment, feature_id)
+                    )
+                    audiences = self.replace_ids_with_names(experiment.get('audienceConditions', []), audiences_map)
+                    optly_exp.audiences = audiences
+
+                    delivery_rules.append(optly_exp)
+
+        return delivery_rules
+
+    def _get_attributes_list(self, attributes: list[AttributeDict]) -> list[OptimizelyAttribute]:
+        """ Gets attributes list for the project config
+
+        Returns:
+            List - OptimizelyAttributes
+        """
+        attributes_list = []
+
+        for attribute in attributes:
+            optly_attribute = OptimizelyAttribute(
+                attribute['id'],
+                attribute['key']
+            )
+            attributes_list.append(optly_attribute)
+
+        return attributes_list
+
+    def _get_events_list(self, events: list[EventDict]) -> list[OptimizelyEvent]:
+        """ Gets events list for the project_config
+
+        Returns:
+            List - OptimizelyEvents
+        """
+        events_list = []
+
+        for event in events:
+            optly_event = OptimizelyEvent(
+                event['id'],
+                event['key'],
+                event['experimentIds']
+            )
+            events_list.append(optly_event)
+
+        return events_list
```

### Comparing `optimizely-sdk-4.1.1/optimizely/optimizely_factory.py` & `optimizely-sdk-5.0.0b0/optimizely/optimizely_factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,164 +1,180 @@
-# Copyright 2021, Optimizely
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-from . import logger as optimizely_logger
-from .config_manager import PollingConfigManager
-from .error_handler import NoOpErrorHandler
-from .event.event_processor import BatchEventProcessor
-from .event_dispatcher import EventDispatcher
-from .notification_center import NotificationCenter
-from .optimizely import Optimizely
-
-
-class OptimizelyFactory(object):
-    """ Optimizely factory to provides basic utility to instantiate the Optimizely
-        SDK with a minimal number of configuration options."""
-
-    max_event_batch_size = None
-    max_event_flush_interval = None
-    polling_interval = None
-    blocking_timeout = None
-
-    @staticmethod
-    def set_batch_size(batch_size):
-        """ Convenience method for setting the maximum number of events contained within a batch.
-        Args:
-          batch_size: Sets size of event_queue.
-         """
-
-        OptimizelyFactory.max_event_batch_size = batch_size
-        return OptimizelyFactory.max_event_batch_size
-
-    @staticmethod
-    def set_flush_interval(flush_interval):
-        """ Convenience method for setting the maximum time interval in milliseconds between event dispatches.
-        Args:
-          flush_interval: Time interval between event dispatches.
-         """
-
-        OptimizelyFactory.max_event_flush_interval = flush_interval
-        return OptimizelyFactory.max_event_flush_interval
-
-    @staticmethod
-    def set_polling_interval(polling_interval):
-        """ Method to set frequency at which datafile has to be polled.
-            Args:
-              polling_interval: Time in seconds after which to update datafile.
-        """
-        OptimizelyFactory.polling_interval = polling_interval
-        return OptimizelyFactory.polling_interval
-
-    @staticmethod
-    def set_blocking_timeout(blocking_timeout):
-        """ Method to set time in seconds to block the config call until config has been initialized.
-            Args:
-              blocking_timeout: Time in seconds to block the config call.
-       """
-        OptimizelyFactory.blocking_timeout = blocking_timeout
-        return OptimizelyFactory.blocking_timeout
-
-    @staticmethod
-    def default_instance(sdk_key, datafile=None):
-        """ Returns a new optimizely instance..
-          Args:
-            sdk_key:  Required string uniquely identifying the fallback datafile corresponding to project.
-            datafile: Optional JSON string datafile.
-        """
-        error_handler = NoOpErrorHandler()
-        logger = optimizely_logger.NoOpLogger()
-        notification_center = NotificationCenter(logger)
-
-        config_manager_options = {
-            'sdk_key': sdk_key,
-            'update_interval': OptimizelyFactory.polling_interval,
-            'blocking_timeout': OptimizelyFactory.blocking_timeout,
-            'datafile': datafile,
-            'logger': logger,
-            'error_handler': error_handler,
-            'notification_center': notification_center,
-        }
-
-        config_manager = PollingConfigManager(**config_manager_options)
-
-        event_processor = BatchEventProcessor(
-            event_dispatcher=EventDispatcher(),
-            logger=logger,
-            batch_size=OptimizelyFactory.max_event_batch_size,
-            flush_interval=OptimizelyFactory.max_event_flush_interval,
-            notification_center=notification_center,
-        )
-
-        optimizely = Optimizely(
-            datafile, None, logger, error_handler, None, None, sdk_key, config_manager, notification_center,
-            event_processor
-        )
-        return optimizely
-
-    @staticmethod
-    def default_instance_with_config_manager(config_manager):
-        return Optimizely(
-            config_manager=config_manager
-        )
-
-    @staticmethod
-    def custom_instance(sdk_key, datafile=None, event_dispatcher=None, logger=None, error_handler=None,
-                        skip_json_validation=None, user_profile_service=None, config_manager=None,
-                        notification_center=None):
-        """ Returns a new optimizely instance.
-             if max_event_batch_size and max_event_flush_interval are None then default batch_size and flush_interval
-             will be used to setup BatchEventProcessor.
-
-             Args:
-               sdk_key: Required string uniquely identifying the fallback datafile corresponding to project.
-               datafile: Optional JSON string datafile.
-               event_dispatcher: Optional EventDispatcher interface provides a dispatch_event method which if given a
-                                 URL and params sends a request to it.
-               logger: Optional Logger interface provides a log method to log messages.
-                       By default nothing would be logged.
-               error_handler: Optional ErrorHandler interface which provides a handle_error method to handle exceptions.
-                              By default all exceptions will be suppressed.
-               skip_json_validation: Optional boolean param to skip JSON schema validation of the provided datafile.
-               user_profile_service: Optional UserProfileService interface provides methods to store and retrieve
-                                     user profiles.
-               config_manager: Optional ConfigManager interface responds to 'config' method.
-               notification_center: Optional Instance of NotificationCenter.
-        """
-
-        error_handler = error_handler or NoOpErrorHandler()
-        logger = logger or optimizely_logger.NoOpLogger()
-        notification_center = notification_center if isinstance(notification_center,
-                                                                NotificationCenter) else NotificationCenter(logger)
-
-        event_processor = BatchEventProcessor(
-            event_dispatcher=event_dispatcher or EventDispatcher(),
-            logger=logger,
-            batch_size=OptimizelyFactory.max_event_batch_size,
-            flush_interval=OptimizelyFactory.max_event_flush_interval,
-            notification_center=notification_center,
-        )
-
-        config_manager_options = {
-            'sdk_key': sdk_key,
-            'update_interval': OptimizelyFactory.polling_interval,
-            'blocking_timeout': OptimizelyFactory.blocking_timeout,
-            'datafile': datafile,
-            'logger': logger,
-            'error_handler': error_handler,
-            'skip_json_validation': skip_json_validation,
-            'notification_center': notification_center,
-        }
-        config_manager = config_manager or PollingConfigManager(**config_manager_options)
-
-        return Optimizely(
-            datafile, event_dispatcher, logger, error_handler, skip_json_validation, user_profile_service,
-            sdk_key, config_manager, notification_center, event_processor
-        )
+# Copyright 2021-2022, Optimizely
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+from __future__ import annotations
+from typing import TYPE_CHECKING, Optional
+
+from optimizely.helpers.sdk_settings import OptimizelySdkSettings
+
+from . import logger as optimizely_logger
+from .config_manager import BaseConfigManager, PollingConfigManager
+from .error_handler import BaseErrorHandler, NoOpErrorHandler
+from .event.event_processor import BatchEventProcessor
+from .event_dispatcher import EventDispatcher, CustomEventDispatcher
+from .notification_center import NotificationCenter
+from .optimizely import Optimizely
+
+if TYPE_CHECKING:
+    # prevent circular dependenacy by skipping import at runtime
+    from .user_profile import UserProfileService
+
+
+class OptimizelyFactory:
+    """ Optimizely factory to provides basic utility to instantiate the Optimizely
+        SDK with a minimal number of configuration options."""
+
+    max_event_batch_size: Optional[int] = None
+    max_event_flush_interval: Optional[int] = None
+    polling_interval: Optional[float] = None
+    blocking_timeout: Optional[int] = None
+
+    @staticmethod
+    def set_batch_size(batch_size: int) -> int:
+        """ Convenience method for setting the maximum number of events contained within a batch.
+        Args:
+          batch_size: Sets size of event_queue.
+         """
+
+        OptimizelyFactory.max_event_batch_size = batch_size
+        return OptimizelyFactory.max_event_batch_size
+
+    @staticmethod
+    def set_flush_interval(flush_interval: int) -> int:
+        """ Convenience method for setting the maximum time interval in milliseconds between event dispatches.
+        Args:
+          flush_interval: Time interval between event dispatches.
+         """
+
+        OptimizelyFactory.max_event_flush_interval = flush_interval
+        return OptimizelyFactory.max_event_flush_interval
+
+    @staticmethod
+    def set_polling_interval(polling_interval: int) -> int:
+        """ Method to set frequency at which datafile has to be polled.
+            Args:
+              polling_interval: Time in seconds after which to update datafile.
+        """
+        OptimizelyFactory.polling_interval = polling_interval
+        return OptimizelyFactory.polling_interval
+
+    @staticmethod
+    def set_blocking_timeout(blocking_timeout: int) -> int:
+        """ Method to set time in seconds to block the config call until config has been initialized.
+            Args:
+              blocking_timeout: Time in seconds to block the config call.
+       """
+        OptimizelyFactory.blocking_timeout = blocking_timeout
+        return OptimizelyFactory.blocking_timeout
+
+    @staticmethod
+    def default_instance(sdk_key: str, datafile: Optional[str] = None) -> Optimizely:
+        """ Returns a new optimizely instance..
+          Args:
+            sdk_key:  Required string uniquely identifying the fallback datafile corresponding to project.
+            datafile: Optional JSON string datafile.
+        """
+        error_handler = NoOpErrorHandler()
+        logger = optimizely_logger.NoOpLogger()
+        notification_center = NotificationCenter(logger)
+
+        config_manager = PollingConfigManager(
+            sdk_key=sdk_key,
+            update_interval=OptimizelyFactory.polling_interval,
+            blocking_timeout=OptimizelyFactory.blocking_timeout,
+            datafile=datafile,
+            logger=logger,
+            error_handler=error_handler,
+            notification_center=notification_center
+        )
+
+        event_processor = BatchEventProcessor(
+            event_dispatcher=EventDispatcher(),
+            logger=logger,
+            batch_size=OptimizelyFactory.max_event_batch_size,
+            flush_interval=OptimizelyFactory.max_event_flush_interval,
+            notification_center=notification_center,
+        )
+
+        optimizely = Optimizely(
+            datafile, None, logger, error_handler, None, None, sdk_key, config_manager, notification_center,
+            event_processor
+        )
+        return optimizely
+
+    @staticmethod
+    def default_instance_with_config_manager(config_manager: BaseConfigManager) -> Optimizely:
+        return Optimizely(
+            config_manager=config_manager
+        )
+
+    @staticmethod
+    def custom_instance(
+        sdk_key: str,
+        datafile: Optional[str] = None,
+        event_dispatcher: Optional[CustomEventDispatcher] = None,
+        logger: Optional[optimizely_logger.Logger] = None,
+        error_handler: Optional[BaseErrorHandler] = None,
+        skip_json_validation: Optional[bool] = None,
+        user_profile_service: Optional[UserProfileService] = None,
+        config_manager: Optional[BaseConfigManager] = None,
+        notification_center: Optional[NotificationCenter] = None,
+        settings: Optional[OptimizelySdkSettings] = None
+    ) -> Optimizely:
+        """ Returns a new optimizely instance.
+             if max_event_batch_size and max_event_flush_interval are None then default batch_size and flush_interval
+             will be used to setup BatchEventProcessor.
+
+             Args:
+               sdk_key: Required string uniquely identifying the fallback datafile corresponding to project.
+               datafile: Optional JSON string datafile.
+               event_dispatcher: Optional EventDispatcher interface provides a dispatch_event method which if given a
+                                 URL and params sends a request to it.
+               logger: Optional Logger interface provides a log method to log messages.
+                       By default nothing would be logged.
+               error_handler: Optional ErrorHandler interface which provides a handle_error method to handle exceptions.
+                              By default all exceptions will be suppressed.
+               skip_json_validation: Optional boolean param to skip JSON schema validation of the provided datafile.
+               user_profile_service: Optional UserProfileService interface provides methods to store and retrieve
+                                     user profiles.
+               config_manager: Optional ConfigManager interface responds to 'config' method.
+               notification_center: Optional Instance of NotificationCenter.
+               settings: Optional Instance of OptimizelySdkSettings.
+        """
+
+        error_handler = error_handler or NoOpErrorHandler()
+        logger = logger or optimizely_logger.NoOpLogger()
+        notification_center = notification_center if isinstance(notification_center,
+                                                                NotificationCenter) else NotificationCenter(logger)
+
+        event_processor = BatchEventProcessor(
+            event_dispatcher=event_dispatcher or EventDispatcher(),
+            logger=logger,
+            batch_size=OptimizelyFactory.max_event_batch_size,
+            flush_interval=OptimizelyFactory.max_event_flush_interval,
+            notification_center=notification_center,
+        )
+
+        config_manager = config_manager or PollingConfigManager(
+            sdk_key=sdk_key,
+            update_interval=OptimizelyFactory.polling_interval,
+            blocking_timeout=OptimizelyFactory.blocking_timeout,
+            datafile=datafile,
+            logger=logger,
+            error_handler=error_handler,
+            skip_json_validation=skip_json_validation,
+            notification_center=notification_center,
+        )
+
+        return Optimizely(
+            datafile, event_dispatcher, logger, error_handler, skip_json_validation, user_profile_service,
+            sdk_key, config_manager, notification_center, event_processor, settings=settings
+        )
```

### Comparing `optimizely-sdk-4.1.1/optimizely/version.py` & `optimizely-sdk-5.0.0b0/optimizely/odp/optimizely_odp_option.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,25 @@
-# Copyright 2016-2020, 2022-2023, Optimizely
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-version_info = (4, 1, 1)
-__version__ = '.'.join(str(v) for v in version_info)
+# Copyright 2022, Optimizely
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from sys import version_info
+
+if version_info < (3, 8):
+    from typing_extensions import Final
+else:
+    from typing import Final  # type: ignore
+
+
+class OptimizelyOdpOption:
+    """Options for the OdpSegmentManager."""
+    IGNORE_CACHE: Final = 'IGNORE_CACHE'
+    RESET_CACHE: Final = 'RESET_CACHE'
```

### Comparing `optimizely-sdk-4.1.1/optimizely_sdk.egg-info/PKG-INFO` & `optimizely-sdk-5.0.0b0/optimizely_sdk.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,683 +1,717 @@
-Metadata-Version: 2.1
-Name: optimizely-sdk
-Version: 4.1.1
-Summary: Python SDK for Optimizely Feature Experimentation, Optimizely Full Stack (legacy), and Optimizely Rollouts.
-Home-page: https://github.com/optimizely/python-sdk
-Author: Optimizely
-Author-email: developers@optimizely.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
-Optimizely Feature Experimentation is A/B testing and feature management for product development teams. Experiment in any application. Make every feature on your roadmap an opportunity to learn. Learn more at https://www.optimizely.com/products/experiment/feature-experimentation/ or see our documentation at https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/welcome. # Optimizely Python SDK
-
-[![PyPI version](https://badge.fury.io/py/optimizely-sdk.svg)](https://pypi.org/project/optimizely-sdk)
-[![Build Status](https://travis-ci.org/optimizely/python-sdk.svg?branch=master)](https://travis-ci.org/optimizely/python-sdk)
-[![Coverage Status](https://coveralls.io/repos/github/optimizely/python-sdk/badge.svg)](https://coveralls.io/github/optimizely/python-sdk)
-[![Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](http://www.apache.org/licenses/LICENSE-2.0)
-
-This repository houses the Python SDK for use with Optimizely Feature Experimentation and Optimizely Full Stack (legacy).
-
-Optimizely Feature Experimentation is an A/B testing and feature management tool for product development teams that enables you to experiment at every step. Using Optimizely Feature Experimentation allows for every feature on your roadmap to be an opportunity to discover hidden insights. Learn more at [Optimizely.com](https://www.optimizely.com/products/experiment/feature-experimentation/), or see the [developer documentation](https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/welcome).
-
-Optimizely Rollouts is [free feature flags](https://www.optimizely.com/free-feature-flagging/) for development teams. You can easily roll out and roll back features in any application without code deploys, mitigating risk for every feature on your roadmap.
-
-## Get Started
-
-Refer to the [Python SDK's developer documentation](https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/python-sdk) for detailed instructions on getting started with using the SDK.
-
-### Requirements
-
-Version `4.0+`: Python 3.7+, PyPy 3.7+
-
-Version `3.0+`: Python 2.7+, PyPy 3.4+
-
-### Install the SDK
-
-The SDK is available through [PyPi](https://pypi.python.org/pypi?name=optimizely-sdk&:action=display).
-
-To install:
-
-    pip install optimizely-sdk
-
-### Feature Management Access
-
-To access the Feature Management configuration in the Optimizely
-dashboard, please contact your Optimizely customer success manager.
-
-## Use the Python SDK
-
-### Initialization
-
-You can initialize the Optimizely instance in three ways: with a datafile, by providing an sdk_key, or by providing an implementation of
-[BaseConfigManager](https://github.com/optimizely/python-sdk/tree/master/optimizely/config_manager.py#L32).
-Each method is described below.
-
-1.  Initialize Optimizely with a datafile. This datafile will be used as
-    the source of ProjectConfig throughout the life of Optimizely instance:
-
-        optimizely.Optimizely(
-          datafile
-        )
-
-2.  Initialize Optimizely by providing an \'sdk_key\'. This will
-    initialize a PollingConfigManager that makes an HTTP GET request to
-    the URL (formed using your provided sdk key and the
-    default datafile CDN URL template) to asynchronously download the
-    project datafile at regular intervals and update ProjectConfig when
-    a new datafile is received. A hard-coded datafile can also be
-    provided along with the sdk_key that will be used
-    initially before any update:
-
-        optimizely.Optimizely(
-          sdk_key='put_your_sdk_key_here'
-        )
-
-    If providing a datafile, the initialization will look like:
-
-        optimizely.Optimizely(
-          datafile=datafile,
-          sdk_key='put_your_sdk_key_here'
-        )
-
-3.  Initialize Optimizely by providing a ConfigManager that implements
-    [BaseConfigManager](https://github.com/optimizely/python-sdk/tree/master/optimizely/config_manager.py#L34).
-    You may use our [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L150) or
-    [AuthDatafilePollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L375) as needed:
-
-        optimizely.Optimizely(
-          config_manager=custom_config_manager
-        )
-
-### PollingConfigManager
-
-The [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L150) asynchronously polls for
-datafiles from a specified URL at regular intervals by making HTTP requests.
-
-    polling_config_manager = PollingConfigManager(
-        sdk_key=None,
-        datafile=None,
-        update_interval=None,
-        url=None,
-        url_template=None,
-        logger=None,
-        error_handler=None,
-        notification_center=None,
-        skip_json_validation=False
-    )
-
-**Note**: You must provide either the sdk_key or URL. If
-you provide both, the URL takes precedence.
-
-**sdk_key** The sdk_key is used to compose the outbound
-HTTP request to the default datafile location on the Optimizely CDN.
-
-**datafile** You can provide an initial datafile to bootstrap the
-`ProjectConfigManager` so that it can be used immediately. The initial
-datafile also serves as a fallback datafile if HTTP connection cannot be
-established. The initial datafile will be discarded after the first
-successful datafile poll.
-
-**update_interval** The update_interval is used to specify a fixed
-delay in seconds between consecutive HTTP requests for the datafile.
-
-**url** The target URL from which to request the datafile.
-
-**url_template** A string with placeholder `{sdk_key}` can be provided
-so that this template along with the provided sdk key is
-used to form the target URL.
-
-You may also provide your own logger, error_handler, or
-notification_center.
-
-### AuthDatafilePollingConfigManager
-
-The [AuthDatafilePollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L375)
-implements `PollingConfigManager` and asynchronously polls for authenticated datafiles from a specified URL at regular intervals
-by making HTTP requests.
-
-    auth_datafile_polling_config_manager = AuthDatafilePollingConfigManager(
-        datafile_access_token,
-        *args,
-        **kwargs
-    )
-
-**Note**: To use [AuthDatafilePollingConfigManager](#authdatafilepollingconfigmanager), you must create a secure environment for
-your project and generate an access token for your datafile.
-
-**datafile_access_token** The datafile_access_token is attached to the outbound HTTP request header to authorize the request and fetch the datafile.
-
-### Advanced configuration
-
-The following properties can be set to override the default
-configurations for [PollingConfigManager](#pollingconfigmanager) and [AuthDatafilePollingConfigManager](#authdatafilepollingconfigmanager).
-
-| **Property Name** |                                                                                    **Default Value**                                                                                    |                        **Description**                         |
-| :---------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------: |
-|      sdk_key      |                                                                                          None                                                                                           |                   Optimizely project SDK key                   |
-|     datafile      |                                                                                          None                                                                                           | Initial datafile, typically sourced from a local cached source |
-|  update_interval  |                                                                                        5 minutes                                                                                        |          Fixed delay between fetches for the datafile          |
-|        url        |                                                                                          None                                                                                           |      Custom URL location from which to fetch the datafile      |
-|   url_template    | `PollingConfigManager:`<br/>https://cdn.optimizely.com/datafiles/{sdk_key}.json<br/>`AuthDatafilePollingConfigManager:`<br/>https://config.optimizely.com/datafiles/auth/{sdk_key}.json |             Parameterized datafile URL by SDK key              |
-
-A notification signal will be triggered whenever a _new_ datafile is
-fetched and Project Config is updated. To subscribe to these
-notifications, use:
-
-```
-notification_center.add_notification_listener(NotificationTypes.OPTIMIZELY_CONFIG_UPDATE, update_callback)
-```
-
-For Further details see the Optimizely [Feature Experimentation documentation](https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/welcome)
-to learn how to set up your first Python project and use the SDK.
-
-## SDK Development
-
-### Building the SDK
-
-Build and install the SDK with pip, using the following command:
-
-    pip install -e .
-
-### Unit Tests
-
-#### Running all tests
-
-To get test dependencies installed, use a modified version of the
-install command:
-
-    pip install -e '.[test]'
-
-You can run all unit tests with:
-
-    pytest
-
-#### Running all tests in a file
-
-To run all tests under a particular test file you can use the following
-command:
-
-    pytest tests.<file_name_without_extension>
-
-For example, to run all tests under `test_event_builder`, the command would be:
-
-    pytest tests/test_event_builder.py
-
-#### Running all tests under a class
-
-To run all tests under a particular class of tests you can use the
-following command:
-
-    pytest tests/<file_name_with_extension>::ClassName
-
-For example, to run all tests under `test_event_builder.EventTest`, the command
-would be:
-
-    pytest tests/test_event_builder.py::EventTest
-
-#### Running a single test
-
-To run a single test you can use the following command:
-
-    pytest tests/<file_name_with_extension>::ClassName::test_name
-
-For example, to run `test_event_builder.EventTest.test_init`, the command
-would be:
-
-    pytest tests/test_event_builder.py::EventTest::test_init
-
-### Contributing
-
-Please see [CONTRIBUTING](https://github.com/optimizely/python-sdk/blob/master/CONTRIBUTING.md).
-
-### Credits
-
-This software incorporates code from the following open source projects:
-
-requests (Apache-2.0 License: https://github.com/psf/requests/blob/master/LICENSE)
-
-pyOpenSSL (Apache-2.0 License https://github.com/pyca/pyopenssl/blob/main/LICENSE)
-
-cryptography (Apache-2.0 https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE)
-
-idna (BSD 3-Clause License https://github.com/kjd/idna/blob/master/LICENSE.md)
-
-### Other Optimizely SDKs
-
-- Agent - https://github.com/optimizely/agent
-
-- Android - https://github.com/optimizely/android-sdk
-
-- C# - https://github.com/optimizely/csharp-sdk
-
-- Flutter - https://github.com/optimizely/optimizely-flutter-sdk
-
-- Go - https://github.com/optimizely/go-sdk
-
-- Java - https://github.com/optimizely/java-sdk
-
-- JavaScript - https://github.com/optimizely/javascript-sdk
-
-- PHP - https://github.com/optimizely/php-sdk
-
-- Python - https://github.com/optimizely/python-sdk
-
-- React - https://github.com/optimizely/react-sdk
-
-- Ruby - https://github.com/optimizely/ruby-sdk
-
-- Swift - https://github.com/optimizely/swift-sdk
-# Optimizely Python SDK Changelog
-
-## 4.1.1
-March 10th, 2023
-
-We updated our README.md and other non-functional code to reflect that this SDK supports both Optimizely Feature Experimentation and Optimizely Full Stack. ([#420](https://github.com/optimizely/python-sdk/pull/420))
-
-## 4.1.0
-July 7th, 2022
-
-### Bug Fixes
-* Fix error log formatting for flag key ([#381](https://github.com/optimizely/python-sdk/pull/381))
-* Fix invalid datafile returned from `ProjectConfig.to_datafile` and `OptimizelyConfig.get_datafile` ([#321](https://github.com/optimizely/python-sdk/pull/321), [#384](https://github.com/optimizely/python-sdk/pull/384))
-
-
-## 4.0.0
-January 12th, 2022
-
-### New Features
-* Add a set of new APIs for overriding and managing user-level flag, experiment and delivery rule decisions. These methods can be used for QA and automated testing purposes. They are an extension of the OptimizelyUserContext interface ([#361](https://github.com/optimizely/python-sdk/pull/361), [#365](https://github.com/optimizely/python-sdk/pull/365), [#369](https://github.com/optimizely/python-sdk/pull/369)):
-	- setForcedDecision
-	- getForcedDecision
-	- removeForcedDecision
-	- removeAllForcedDecisions
-
-* For details, refer to our documentation pages: [OptimizelyUserContext](https://docs.developers.optimizely.com/full-stack/v4.0/docs/optimizelyusercontext-python) and [Forced Decision methods](https://docs.developers.optimizely.com/full-stack/v4.0/docs/forced-decision-methods-python).
-
-### Breaking Changes:
-
-* Support for `Python v3.4` has been dropped as of this release due to a security vulnerability with `PyYAML <v5.4`. ([#366](https://github.com/optimizely/python-sdk/pull/366))
-* We no longer support `Python v2.7, v3.5, and v3.6` including `PyPy` as of this release. ([#377](https://github.com/optimizely/python-sdk/pull/373))
-* We now support `Python v3.7 and above` including `PyPy3`.
-
-## 3.10.0
-September 16th, 2021
-
-### New Features
-* Added new public properties to OptimizelyConfig.
-  - sdk_key and environment_key [#338] (https://github.com/optimizely/python-sdk/pull/338)
-  - attributes and events [#339] (https://github.com/optimizely/python-sdk/pull/339)
-  - experiment_rules, delivery_rules, audiences and audiences in OptimizelyExperiment
-    - [#342] (https://github.com/optimizely/python-sdk/pull/342)
-    - [#351] (https://github.com/optimizely/python-sdk/pull/351/files)
-* For details please refer to our documentation page:
-  - Python-sdk: [https://docs.developers.optimizely.com/full-stack/docs/optimizelyconfig-python]
-
-* OptimizelyFeature.experiments_map of OptimizelyConfig is now deprecated. Please use OptimizelyFeature.experiment_rules and OptimizelyFeature.delivery_rules. [#360] (https://github.com/optimizely/python-sdk/pull/360)
-
-### Bug Fixes
-* Fix event processor negative timeout interval when retrieving events from queue. [#356] (https://github.com/optimizely/python-sdk/pull/356)
-
-## 3.9.1
-July 14th, 2021
-
-### Bug Fixes:
-* Fixed issue with serving incorrect variation in projects containing multiple flags with duplicate keys. [#347] (https://github.com/optimizely/python-sdk/pull/347)
-* Fixed issue with serving incorrect variation in create_impression_event in user_event_factory.py. [#350] (https://github.com/optimizely/python-sdk/pull/350)
-
-## 3.9.0
-June 1st, 2021
-
-### New Features
-* Added support for multiple concurrent prioritized experiments per flag. [#322](https://github.com/optimizely/python-sdk/pull/322)
-
-## 3.8.0
-February 12th, 2021
-
-### New Features
-* New Features
-Introducing a new primary interface for retrieving feature flag status, configuration and associated experiment decisions for users ([#309](https://github.com/optimizely/python-sdk/pull/309)). The new `OptimizelyUserContext` class is instantiated with `create_user_context` and exposes the following APIs to get `OptimizelyDecision`:
-
-    - set_attribute
-    - decide
-    - decide_all
-    - decide_for_keys
-    - track_event
-
-For details, refer to our documentation page: https://docs.developers.optimizely.com/full-stack/v4.0/docs/python-sdk.
-
-## 3.7.1
-November 19th, 2020
-
-### Bug Fixes:
-* Added "enabled" field to decision metadata structure. [#306](https://github.com/optimizely/python-sdk/pull/306)
-
-## 3.7.0
-November 2nd, 2020
-
-### New Features
-* Added support for upcoming application-controlled introduction of tracking for non-experiment Flag decisions. [#300](https://github.com/optimizely/python-sdk/pull/300)
-
-## 3.6.0
-October 1st, 2020
-
-### New Features:
-* Version targeting using semantic version syntax. [#293](https://github.com/optimizely/python-sdk/pull/293)
-* Datafile accessor API added to access current config as a JSON string. [#283](https://github.com/optimizely/python-sdk/pull/283)
-
-### Bug Fixes:
-* Fixed package installation for Python 3.4 and pypy. [#298](https://github.com/optimizely/python-sdk/pull/298)
-
-## 3.5.2
-July 14th, 2020
-
-### Bug Fixes:
-* Fixed handling of network and no status code errors when polling for datafile in `PollingConfigManager` and `AuthDatafilePollingConfigManager`. ([#287](https://github.com/optimizely/python-sdk/pull/287))
-
-## 3.5.1
-July 10th, 2020
-
-### Bug Fixes:
-* Fixed HTTP request exception handling in `PollingConfigManager`. ([#285](https://github.com/optimizely/python-sdk/pull/285))
-
-## 3.5.0
-July 9th, 2020
-
-### New Features:
-* Introduced 2 APIs to interact with feature variables:
-  * `get_feature_variable_json` allows you to get value for JSON variables related to a feature.
-  * `get_all_feature_variables` gets values for all variables under a feature.
-* Added support for fetching authenticated datafiles. `AuthDatafilePollingConfigManager` is a new config manager that allows you to poll for a datafile belonging to a secure environment. You can create a client by setting the `datafile_access_token`.
-
-### Bug Fixes:
-* Fixed log messages for targeted rollouts evaluation. ([#268](https://github.com/optimizely/python-sdk/pull/268))
-
-## 3.4.2
-June 11th, 2020
-
-### Bug Fixes:
-* Adjusted log level for audience evaluation logs. ([#267](https://github.com/optimizely/python-sdk/pull/267))
-
-## 3.4.1
-March 19th, 2020
-
-### Bug Fixes:
-* Updated `jsonschema` to address [installation issue](https://github.com/optimizely/python-sdk/issues/232).
-
-## 3.4.0
-January 27th, 2020
-
-### New Features:
-* Added a new API to get project configuration static data.
-  * Call `get_optimizely_config()` to get a snapshot of project configuration static data.
-  * It returns an `OptimizelyConfig` instance which includes a datafile revision number, all experiments, and feature flags mapped by their key values.
-  * Added caching for `get_optimizely_config()` - `OptimizelyConfig` object will be cached and reused for the lifetime of the datafile.
-  * For details, refer to our documentation page: [https://docs.developers.optimizely.com/full-stack/docs/optimizelyconfig-python](https://docs.developers.optimizely.com/full-stack/docs/optimizelyconfig-python).
-
-
-## 3.3.1
-December 16th, 2019
-
-### Bug Fixes:
-* Fixed [installation issue](https://github.com/optimizely/python-sdk/issues/220) on Windows. ([#224](https://github.com/optimizely/python-sdk/pull/224))
-* Fixed batch event processor deadline reset issue. ([#227](https://github.com/optimizely/python-sdk/pull/227))
-* Added more batch event processor debug messages. ([#227](https://github.com/optimizely/python-sdk/pull/227))
-
-## 3.3.0
-October 28th, 2019
-
-### New Features:
-* Added support for event batching via the event processor.
-  * Events generated by methods like `activate`, `track`, and `is_feature_enabled` will be held in a queue until the configured batch size is reached, or the configured flush interval has elapsed. Then, they will be batched into a single payload and sent to the event dispatcher.
-  * To configure event batching, set the `batch_size` and `flush_interval` properties when initializing instance of [BatchEventProcessor](https://github.com/optimizely/python-sdk/blob/3.3.x/optimizely/event/event_processor.py#L45).
-  * Event batching is disabled by default. You can pass in instance of `BatchEventProcessor` when creating `Optimizely` instance to enable event batching.
-  * Users can subscribe to `LogEvent` notification to be notified of whenever a payload consisting of a batch of user events is handed off to the event dispatcher to send to Optimizely's backend.
-* Introduced blocking timeout in `PollingConfigManager`. By default, calls to `get_config` will block for maximum of 10 seconds until config is available.
-
-### Bug Fixes:
-* Fixed incorrect log message when numeric metric is not used. ([#217](https://github.com/optimizely/python-sdk/pull/217))
-
-## 3.2.0
-August 27th, 2019
-
-### New Features:
-* Added support for automatic datafile management via [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151):
-  * The [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151) is an implementation of the [BaseConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L32).
-  * Users may provide one of datafile or SDK key (sdk_key) or both to `optimizely.Optimizely`. Based on that, the SDK will use the [StaticConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L73) or the [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151). Refer to the [README](README.md) for more instructions.
-  * An initial datafile can be provided to the `PollingConfigManager` to bootstrap before making HTTP requests for the hosted datafile.
-  * Requests for the datafile are made in a separate thread and are scheduled with fixed delay.
-  * Configuration updates can be subscribed to by adding the OPTIMIZELY_CONFIG_UPDATE notification listener.
-* Introduced `Optimizely.get_feature_variable` API.  ([#191](https://github.com/optimizely/python-sdk/pull/191))
-
-### Deprecated:
-
-* `NotificationCenter.clear_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
-* `NotificationCenter.clear_all_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_all_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
-
-## 3.2.0b1
-July 26th, 2019
-
-### New Features:
-* Added support for automatic datafile management via [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151):
-  * The [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151) is an implementation of the [BaseConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L32).
-  * Users may provide one of datafile or SDK key (sdk_key) or both to `optimizely.Optimizely`. Based on that, the SDK will use the [StaticConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L73) or the [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151). Refer to the [README](README.md) for more instructions.
-  * An initial datafile can be provided to the `PollingConfigManager` to bootstrap before making HTTP requests for the hosted datafile.
-  * Requests for the datafile are made in a separate thread and are scheduled with fixed delay.
-  * Configuration updates can be subscribed to by adding the OPTIMIZELY_CONFIG_UPDATE notification listener.
-* Introduced `Optimizely.get_feature_variable` API.  ([#191](https://github.com/optimizely/python-sdk/pull/191))
-
-### Deprecated:
-
-* `NotificationCenter.clear_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
-* `NotificationCenter.clear_all_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_all_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
-
-## 3.1.0
-May 3rd, 2019
-
-### New Features:
-* Introduced Decision notification listener to be able to record:
-  * Variation assignments for users activated in an experiment.
-  * Feature access for users.
-  * Feature variable value for users.
-
-### Bug Fixes:
-* Feature variable APIs now return default variable value when featureEnabled property is false.  ([#171](https://github.com/optimizely/python-sdk/pull/171))
-
-### Deprecated:
-* Activate notification listener is deprecated as of this release.  Recommendation is to use the new Decision notification listener.  Activate notification listener will be removed in the next major release.
-
-## 3.0.0
-March 1st, 2019
-
-The 3.0 release improves event tracking and supports additional audience
-targeting functionality.
-
-### New Features:
-* Event tracking:
-  * The `track` method now dispatches its conversion event *unconditionally*, without first determining whether the user is targeted by a known experiment that uses the event. This may increase outbound network traffic.
-  * In Optimizely results, conversion events sent by 3.0 SDKs don\'t explicitly name the experiments and variations that are currently targeted to the user. Instead, conversions are automatically attributed to variations that the user has previously seen, as long as those variations were served via 3.0 SDKs or by other clients capable of automatic attribution, and as long as our backend actually received the impression events for those variations.
-  * Altogether, this allows you to track conversion events and attribute them to variations even when you don't know all of a user's attribute values, and even if the user's attribute values or the experiment's configuration have changed such that the user is no longer affected by the experiment. As a result, **you may observe an increase in the conversion rate for previously-instrumented events.** If that is undesirable, you can reset the results of previously-running experiments after upgrading to the 3.0 SDK.  -   This will also allow you to attribute events to variations from other Optimizely projects in your account, even though those experiments don't appear in the same datafile.
-  * Note that for results segmentation in Optimizely results, the user attribute values from one event are automatically applied to all other events in the same session, as long as the events in question were actually received by our backend. This behavior was already in place and is not affected by the 3.0 release.
-* Support for all types of attribute values, not just strings.
-  * All values are passed through to notification listeners.
-  * Strings, booleans, and valid numbers are passed to the event dispatcher and can be used for Optimizely results segmentation.  A valid number is a finite float or numbers.Integral in the inclusive range \[-2 ^ 53, 2 ^ 53\].
-  * Strings, booleans, and valid numbers are relevant for audience conditions.
-* Support for additional matchers in audience conditions:
-  * An `exists` matcher that passes if the user has a non-null value for the targeted user attribute and fails otherwise.
-  * A `substring` matcher that resolves if the user has a string value for the targeted attribute.
-    * `gt` (greater than) and `lt` (less than) matchers that resolve if the user has a valid number value for the targeted attribute.  A valid number is a finite float or numbers.Integral in the inclusive range \[-2 ^ 53, 2 ^ 53\].
-    * The original (`exact`) matcher can now be used to target booleans and valid numbers, not just strings.
-* Support for A/B tests, feature tests, and feature rollouts whose audiences are combined using `"and"` and `"not"` operators, not just the `"or"` operator.
-* Datafile-version compatibility check: The SDK will remain uninitialized (i.e., will gracefully fail to activate experiments and features) if given a datafile version greater than 4.
-* Updated Pull Request template and commit message guidelines.
-
-### Breaking Changes:
-* Conversion events sent by 3.0 SDKs don\'t explicitly name the experiments and variations that are currently targeted to the user, so these events are unattributed in raw events data export. You must use the new *results* export to determine the variations to which events have been attributed.
-* Previously, notification listeners were only given string-valued user attributes because only strings could be passed into various method calls. That is no longer the case. You may pass non-string attribute values, and if you do, you must update your notification listeners to be able to receive whatever values you pass in.
-
-### Bug Fixes:
-* Experiments and features can no longer activate when a negatively targeted attribute has a missing, null, or malformed value.
-  * Audience conditions (except for the new `exists` matcher) no longer resolve to `false` when they fail to find an legitimate value for the targeted user attribute. The result remains `null` (unknown). Therefore, an audience that negates such a condition (using the `"not"` operator) can no longer resolve to `true` unless there is an unrelated branch in the condition tree that itself resolves to `true`.
-* Updated the default event dispatcher to log an error if the request resolves to HTTP 4xx or 5xx.  ([#140](https://github.com/optimizely/python-sdk/pull/140))
-* All methods now validate that user IDs are strings and that experiment keys, feature keys, feature variable keys, and event keys are non-empty strings.
-
-## 2.1.1
-August 21st, 2018
-
-* Fix: record conversions for all experiments using an event when using track([#136](https://github.com/optimizely/python-sdk/pull/136)).
-
-## 2.1.0
-July 2nd, 2018
-
-* Introduced support for bot filtering ([#121](https://github.com/optimizely/python-sdk/pull/121)).
-* Overhauled logging to use standard Python logging ([#123](https://github.com/optimizely/python-sdk/pull/123)).
-
-## 2.0.1
-June 19th, 2018
-
-* Fix: send impression event for Feature Test when Feature is disabled ([#128](https://github.com/optimizely/python-sdk/pull/128)).
-
-## 2.0.0
-April 12th, 2018
-
-This major release introduces APIs for Feature Management. It also
-introduces some breaking changes listed below.
-
-### New Features
-* Introduced the `is_feature_enabled` API to determine whether to show a feature to a user or not.
-
-```
-    is_enabled = optimizel_client.is_feature_enabled('my_feature_key', 'my_user', user_attributes)
-```
-
-* All enabled features for the user can be retrieved by calling:
-
-```
-    enabled_features = optimizely_client.get_enabled_features('my_user', user_attributes)
-```
-* Introduced Feature Variables to configure or parameterize a feature.  There are four variable types: `String`, `Integer`, `Double`, `Boolean`.
-
-```
-    string_variable = optimizely_client.get_feature_variable_string('my_feature_key', 'string_variable_key', 'my_user')
-    integer_variable = optimizely_client.get_feature_variable_integer('my_feature_key', 'integer_variable_key', 'my_user')
-    double_variable = optimizely_client.get_feature_variable_double('my_feature_key', 'double_variable_key', 'my_user')
-    boolean_variable = optimizely_client.get_feature_variable_boolean('my_feature_key', 'boolean_variable_key', 'my_user')
-```
-
-### Breaking changes
-* The `track` API with revenue value as a stand-alone parameter has been removed. The revenue value should be passed in as an entry in the event tags dict. The key for the revenue tag is `revenue` and the passed in value will be treated by Optimizely as the value for computing results.
-
-```
-    event_tags = {
-      'revenue': 1200
-    }
-
-    optimizely_client.track('event_key', 'my_user', user_attributes, event_tags)
-```
-
-## 2.0.0b1
-March 29th, 2018
-
-This beta release introduces APIs for Feature Management. It also
-introduces some breaking changes listed below.
-
-### New Features
-* Introduced the `is_feature_enabled` API to determine whether to show a feature to a user or not.
-```
-    is_enabled = optimizel_client.is_feature_enabled('my_feature_key', 'my_user', user_attributes)
-```
-
-* All enabled features for the user can be retrieved by calling:
-
-```
-    enabled_features = optimizely_client.get_enabled_features('my_user', user_attributes)
-```
-
-* Introduced Feature Variables to configure or parameterize a feature.  There are four variable types: `String`, `Integer`, `Double`, `Boolean`.
-
-```
-    string_variable = optimizely_client.get_feature_variable_string('my_feature_key', 'string_variable_key', 'my_user')
-    integer_variable = optimizely_client.get_feature_variable_integer('my_feature_key', 'integer_variable_key', 'my_user')
-    double_variable = optimizely_client.get_feature_variable_double('my_feature_key', 'double_variable_key', 'my_user')
-    boolean_variable = optimizely_client.get_feature_variable_boolean('my_feature_key', 'boolean_variable_key', 'my_user')
-```
-
-### Breaking changes
-* The `track` API with revenue value as a stand-alone parameter has been removed. The revenue value should be passed in as an entry in the event tags dict. The key for the revenue tag is `revenue` and the passed in value will be treated by Optimizely as the value for computing results.
-
-```
-    event_tags = {
-      'revenue': 1200
-    }
-
-    optimizely_client.track('event_key', 'my_user', user_attributes, event_tags)
-```
-
-## 1.4.0
-
-* Added support for IP anonymization.
-* Added support for notification listeners.
-* Added support for bucketing ID.
-* Updated mmh3 to handle installation failures on Windows 10.
-
-## 1.3.0
-
-* Introduced support for forced bucketing.
-* Introduced support for numeric metrics.
-* Updated event builder to support new endpoint.
-
-## 1.2.1
-
-* Removed older feature flag parsing.
-
-## 1.2.0
-
-* Added user profile service.
-
-## 1.1.1
-
-* Updated datafile parsing to be able to handle additional fields.
-* Deprecated Classic project support.
-
-## 1.1.0
-
-* Included datafile revision information in log events.
-* Added event tags to track API to allow users to pass in event metadata.
-* Deprecated the `event_value` parameter from the track method. Should use `event_tags` to pass in event value instead.
-* Updated event logging endpoint to logx.optimizely.com.
-
-## 1.0.0
-
-* Introduced support for Full Stack projects in Optimizely X. No breaking changes from previous version.
-* Introduced more graceful exception handling in instantiation and core methods.
-* Updated whitelisting to precede audience matching.
-
-## 0.1.3
-
-* Added support for v2 endpoint and datafile.
-* Updated dispatch_event to consume an Event object instead of url and params. The Event object comprises of four properties: url (string representing URL to dispatch event to), params (dict representing the params to be set for the event), http_verb (one of 'GET' or 'POST') and headers (header values to be sent along).
-* Fixed issue with tracking events for experiments in groups.
-
-## 0.1.2
-
-* Updated requirements file.
-
-## 0.1.1
-
-* Introduced option to skip JSON schema validation.
-
-## 0.1.0
-
-* Beta release of the Python SDK for server-side testing.
+Metadata-Version: 2.1
+Name: optimizely-sdk
+Version: 5.0.0b0
+Summary: Python SDK for Optimizely Feature Experimentation, Optimizely Full Stack (legacy), and Optimizely Rollouts.
+Home-page: https://github.com/optimizely/python-sdk
+Author: Optimizely
+Author-email: developers@optimizely.com
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
+Optimizely Feature Experimentation is A/B testing and feature management for product development teams. Experiment in any application. Make every feature on your roadmap an opportunity to learn. Learn more at https://www.optimizely.com/products/experiment/feature-experimentation/ or see our documentation at https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/welcome. # Optimizely Python SDK
+
+[![PyPI version](https://badge.fury.io/py/optimizely-sdk.svg)](https://pypi.org/project/optimizely-sdk)
+[![Build Status](https://github.com/optimizely/python-sdk/actions/workflows/python.yml/badge.svg?branch=master)](https://github.com/optimizely/python-sdk/actions/workflows/python.yml?query=branch%3Amaster)
+[![Coverage Status](https://coveralls.io/repos/github/optimizely/python-sdk/badge.svg)](https://coveralls.io/github/optimizely/python-sdk)
+[![Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](http://www.apache.org/licenses/LICENSE-2.0)
+
+This repository houses the Python SDK for use with Optimizely Feature Experimentation and Optimizely Full Stack (legacy).
+
+Optimizely Feature Experimentation is an A/B testing and feature management tool for product development teams that enables you to experiment at every step. Using Optimizely Feature Experimentation allows for every feature on your roadmap to be an opportunity to discover hidden insights. Learn more at [Optimizely.com](https://www.optimizely.com/products/experiment/feature-experimentation/), or see the [developer documentation](https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/welcome).
+
+Optimizely Rollouts is [free feature flags](https://www.optimizely.com/free-feature-flagging/) for development teams. You can easily roll out and roll back features in any application without code deploys, mitigating risk for every feature on your roadmap.
+
+## Get Started
+
+Refer to the [Python SDK's developer documentation](https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/python-sdk) for detailed instructions on getting started with using the SDK.
+
+### Requirements
+
+Version `4.0+`: Python 3.7+, PyPy 3.7+
+
+Version `3.0+`: Python 2.7+, PyPy 3.4+
+
+### Install the SDK
+
+The SDK is available through [PyPi](https://pypi.python.org/pypi?name=optimizely-sdk&:action=display).
+
+To install:
+
+    pip install optimizely-sdk
+
+### Feature Management Access
+
+To access the Feature Management configuration in the Optimizely
+dashboard, please contact your Optimizely customer success manager.
+
+## Use the Python SDK
+
+### Initialization
+
+You can initialize the Optimizely instance in three ways: with a datafile, by providing an sdk_key, or by providing an implementation of
+[BaseConfigManager](https://github.com/optimizely/python-sdk/tree/master/optimizely/config_manager.py#L32).
+Each method is described below.
+
+1.  Initialize Optimizely with a datafile. This datafile will be used as
+    the source of ProjectConfig throughout the life of Optimizely instance:
+
+        optimizely.Optimizely(
+          datafile
+        )
+
+2.  Initialize Optimizely by providing an \'sdk_key\'. This will
+    initialize a PollingConfigManager that makes an HTTP GET request to
+    the URL (formed using your provided sdk key and the
+    default datafile CDN URL template) to asynchronously download the
+    project datafile at regular intervals and update ProjectConfig when
+    a new datafile is received. A hard-coded datafile can also be
+    provided along with the sdk_key that will be used
+    initially before any update:
+
+        optimizely.Optimizely(
+          sdk_key='put_your_sdk_key_here'
+        )
+
+    If providing a datafile, the initialization will look like:
+
+        optimizely.Optimizely(
+          datafile=datafile,
+          sdk_key='put_your_sdk_key_here'
+        )
+
+3.  Initialize Optimizely by providing a ConfigManager that implements
+    [BaseConfigManager](https://github.com/optimizely/python-sdk/tree/master/optimizely/config_manager.py#L34).
+    You may use our [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L150) or
+    [AuthDatafilePollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L375) as needed:
+
+        optimizely.Optimizely(
+          config_manager=custom_config_manager
+        )
+
+### PollingConfigManager
+
+The [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L150) asynchronously polls for
+datafiles from a specified URL at regular intervals by making HTTP requests.
+
+    polling_config_manager = PollingConfigManager(
+        sdk_key=None,
+        datafile=None,
+        update_interval=None,
+        url=None,
+        url_template=None,
+        logger=None,
+        error_handler=None,
+        notification_center=None,
+        skip_json_validation=False
+    )
+
+**Note**: You must provide either the sdk_key or URL. If
+you provide both, the URL takes precedence.
+
+**sdk_key** The sdk_key is used to compose the outbound
+HTTP request to the default datafile location on the Optimizely CDN.
+
+**datafile** You can provide an initial datafile to bootstrap the
+`ProjectConfigManager` so that it can be used immediately. The initial
+datafile also serves as a fallback datafile if HTTP connection cannot be
+established. The initial datafile will be discarded after the first
+successful datafile poll.
+
+**update_interval** The update_interval is used to specify a fixed
+delay in seconds between consecutive HTTP requests for the datafile.
+
+**url** The target URL from which to request the datafile.
+
+**url_template** A string with placeholder `{sdk_key}` can be provided
+so that this template along with the provided sdk key is
+used to form the target URL.
+
+You may also provide your own logger, error_handler, or
+notification_center.
+
+### AuthDatafilePollingConfigManager
+
+The [AuthDatafilePollingConfigManager](https://github.com/optimizely/python-sdk/blob/master/optimizely/config_manager.py#L375)
+implements `PollingConfigManager` and asynchronously polls for authenticated datafiles from a specified URL at regular intervals
+by making HTTP requests.
+
+    auth_datafile_polling_config_manager = AuthDatafilePollingConfigManager(
+        datafile_access_token,
+        *args,
+        **kwargs
+    )
+
+**Note**: To use [AuthDatafilePollingConfigManager](#authdatafilepollingconfigmanager), you must create a secure environment for
+your project and generate an access token for your datafile.
+
+**datafile_access_token** The datafile_access_token is attached to the outbound HTTP request header to authorize the request and fetch the datafile.
+
+### Advanced configuration
+
+The following properties can be set to override the default
+configurations for [PollingConfigManager](#pollingconfigmanager) and [AuthDatafilePollingConfigManager](#authdatafilepollingconfigmanager).
+
+| **Property Name** |                                                                                    **Default Value**                                                                                    |                        **Description**                         |
+| :---------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------: |
+|      sdk_key      |                                                                                          None                                                                                           |                   Optimizely project SDK key                   |
+|     datafile      |                                                                                          None                                                                                           | Initial datafile, typically sourced from a local cached source |
+|  update_interval  |                                                                                        5 minutes                                                                                        |          Fixed delay between fetches for the datafile          |
+|        url        |                                                                                          None                                                                                           |      Custom URL location from which to fetch the datafile      |
+|   url_template    | `PollingConfigManager:`<br/>https://cdn.optimizely.com/datafiles/{sdk_key}.json<br/>`AuthDatafilePollingConfigManager:`<br/>https://config.optimizely.com/datafiles/auth/{sdk_key}.json |             Parameterized datafile URL by SDK key              |
+
+A notification signal will be triggered whenever a _new_ datafile is
+fetched and Project Config is updated. To subscribe to these
+notifications, use:
+
+```
+notification_center.add_notification_listener(NotificationTypes.OPTIMIZELY_CONFIG_UPDATE, update_callback)
+```
+
+For Further details see the Optimizely [Feature Experimentation documentation](https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/welcome)
+to learn how to set up your first Python project and use the SDK.
+
+## SDK Development
+
+### Building the SDK
+
+Build and install the SDK with pip, using the following command:
+
+    pip install -e .
+
+### Unit Tests
+
+#### Running all tests
+
+To get test dependencies installed, use a modified version of the
+install command:
+
+    pip install -e '.[test]'
+
+You can run all unit tests with:
+
+    pytest
+
+#### Running all tests in a file
+
+To run all tests under a particular test file you can use the following
+command:
+
+    pytest tests.<file_name_without_extension>
+
+For example, to run all tests under `test_event_builder`, the command would be:
+
+    pytest tests/test_event_builder.py
+
+#### Running all tests under a class
+
+To run all tests under a particular class of tests you can use the
+following command:
+
+    pytest tests/<file_name_with_extension>::ClassName
+
+For example, to run all tests under `test_event_builder.EventTest`, the command
+would be:
+
+    pytest tests/test_event_builder.py::EventTest
+
+#### Running a single test
+
+To run a single test you can use the following command:
+
+    pytest tests/<file_name_with_extension>::ClassName::test_name
+
+For example, to run `test_event_builder.EventTest.test_init`, the command
+would be:
+
+    pytest tests/test_event_builder.py::EventTest::test_init
+
+### Contributing
+
+Please see [CONTRIBUTING](https://github.com/optimizely/python-sdk/blob/master/CONTRIBUTING.md).
+
+### Credits
+
+This software incorporates code from the following open source projects:
+
+requests (Apache-2.0 License: https://github.com/psf/requests/blob/master/LICENSE)
+
+pyOpenSSL (Apache-2.0 License https://github.com/pyca/pyopenssl/blob/main/LICENSE)
+
+cryptography (Apache-2.0 https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE)
+
+idna (BSD 3-Clause License https://github.com/kjd/idna/blob/master/LICENSE.md)
+
+### Other Optimizely SDKs
+
+- Agent - https://github.com/optimizely/agent
+
+- Android - https://github.com/optimizely/android-sdk
+
+- C# - https://github.com/optimizely/csharp-sdk
+
+- Flutter - https://github.com/optimizely/optimizely-flutter-sdk
+
+- Go - https://github.com/optimizely/go-sdk
+
+- Java - https://github.com/optimizely/java-sdk
+
+- JavaScript - https://github.com/optimizely/javascript-sdk
+
+- PHP - https://github.com/optimizely/php-sdk
+
+- Python - https://github.com/optimizely/python-sdk
+
+- React - https://github.com/optimizely/react-sdk
+
+- Ruby - https://github.com/optimizely/ruby-sdk
+
+- Swift - https://github.com/optimizely/swift-sdk
+# Optimizely Python SDK Changelog
+
+## 5.0.0-beta
+Apr 28th, 2023
+
+### New Features  
+
+The 5.0.0-beta release introduces a new primary feature, [Advanced Audience Targeting]( https://docs.developers.optimizely.com/feature-experimentation/docs/optimizely-data-platform-advanced-audience-targeting) enabled through integration with [Optimizely Data Platform (ODP)](https://docs.developers.optimizely.com/optimizely-data-platform/docs) ([#395](https://github.com/optimizely/python-sdk/pull/395), [#398](https://github.com/optimizely/python-sdk/pull/398), [#402](https://github.com/optimizely/python-sdk/pull/402), [#403](https://github.com/optimizely/python-sdk/pull/403), [#405](https://github.com/optimizely/python-sdk/pull/405)).  
+
+You can use ODP, a high-performance [Customer Data Platform (CDP)]( https://www.optimizely.com/optimization-glossary/customer-data-platform/), to easily create complex real-time segments (RTS) using first-party and 50+ third-party data sources out of the box. You can create custom schemas that support the user attributes important for your business, and stitch together user behavior done on different devices to better understand and target your customers for personalized user experiences. ODP can be used as a single source of truth for these segments in any Optimizely or 3rd party tool. 
+
+With ODP accounts integrated into Optimizely projects, you can build audiences using segments pre-defined in ODP. The SDK will fetch the segments for given users and make decisions using the segments. For access to ODP audience targeting in your Feature Experimentation account, please contact your Optimizely Customer Success Manager. 
+
+This version includes the following changes: 
+
+* New API added to `OptimizelyUserContext`: 
+
+  * `fetchQualifiedSegments()`: this API will retrieve user segments from the ODP server. The fetched segments will be used for audience evaluation. The fetched data will be stored in the local cache to avoid repeated network delays.
+  * When an `OptimizelyUserContext` is created, the SDK will automatically send an identify request to the ODP server to facilitate observing user activities. 
+
+* New APIs added to `OptimizelyClient`: 
+
+  * `sendOdpEvent()`: customers can build/send arbitrary ODP events that will bind user identifiers and data to user profiles in ODP.
+
+For details, refer to our documentation pages:  
+
+* [Advanced Audience Targeting](https://docs.developers.optimizely.com/feature-experimentation/docs/optimizely-data-platform-advanced-audience-targeting)  
+* [Server SDK Support](https://docs.developers.optimizely.com/feature-experimentation/v1.0/docs/advanced-audience-targeting-for-server-side-sdks) 
+* [Initialize Python SDK](https://docs.developers.optimizely.com/feature-experimentation/docs/initialize-sdk-python) 
+* [OptimizelyUserContext Python SDK](https://docs.developers.optimizely.com/feature-experimentation/docs/wip-fsodp-optimizelyusercontext-python) 
+* [Advanced Audience Targeting segment qualification methods](https://docs.developers.optimizely.com/feature-experimentation/v1.0/docs/advanced-audience-targeting-segment-qualification-methods-python) 
+* [Send Optimizely Data Platform data using Advanced Audience Targeting](https://docs.developers.optimizely.com/feature-experimentation/v1.0/docs/send-odp-data-using-advanced-audience-targeting-python) 
+
+### Breaking Changes 
+
+* `ODPManager` in the SDK is enabled by default. Unless an ODP account is integrated into the Optimizely projects, most `ODPManager` functions will be ignored. If needed, `ODPManager` can be disabled when `OptimizelyClient` is instantiated. 
+* `BaseConfigManager` abstract class now requires a get_sdk_key method. ([#413](https://github.com/optimizely/python-sdk/pull/413))
+* `PollingConfigManager` requires either the sdk_key parameter or datafile containing an sdkKey. ([#413](https://github.com/optimizely/python-sdk/pull/413))
+* Asynchronous `BatchEventProcessor` is now the default event processor. ([#378](https://github.com/optimizely/python-sdk/pull/378))
+
+## 4.1.1
+March 10th, 2023
+
+We updated our README.md and other non-functional code to reflect that this SDK supports both Optimizely Feature Experimentation and Optimizely Full Stack. ([#420](https://github.com/optimizely/python-sdk/pull/420))
+
+## 4.1.0
+July 7th, 2022
+
+### Bug Fixes
+* Fix invalid datafile returned from `ProjectConfig.to_datafile` and `OptimizelyConfig.get_datafile` ([#321](https://github.com/optimizely/python-sdk/pull/321), [#384](https://github.com/optimizely/python-sdk/pull/384))
+
+## 4.0.0
+January 12th, 2022
+
+### New Features
+* Add a set of new APIs for overriding and managing user-level flag, experiment and delivery rule decisions. These methods can be used for QA and automated testing purposes. They are an extension of the OptimizelyUserContext interface ([#361](https://github.com/optimizely/python-sdk/pull/361), [#365](https://github.com/optimizely/python-sdk/pull/365), [#369](https://github.com/optimizely/python-sdk/pull/369)):
+	- setForcedDecision
+	- getForcedDecision
+	- removeForcedDecision
+	- removeAllForcedDecisions
+
+* For details, refer to our documentation pages: [OptimizelyUserContext](https://docs.developers.optimizely.com/full-stack/v4.0/docs/optimizelyusercontext-python) and [Forced Decision methods](https://docs.developers.optimizely.com/full-stack/v4.0/docs/forced-decision-methods-python).
+
+### Breaking Changes:
+
+* Support for `Python v3.4` has been dropped as of this release due to a security vulnerability with `PyYAML <v5.4`. ([#366](https://github.com/optimizely/python-sdk/pull/366))
+* We no longer support `Python v2.7, v3.5, and v3.6` including `PyPy` as of this release. ([#377](https://github.com/optimizely/python-sdk/pull/373))
+* We now support `Python v3.7 and above` including `PyPy3`.
+
+## 3.10.0
+September 16th, 2021
+
+### New Features
+* Added new public properties to OptimizelyConfig.
+  - sdk_key and environment_key [#338] (https://github.com/optimizely/python-sdk/pull/338)
+  - attributes and events [#339] (https://github.com/optimizely/python-sdk/pull/339)
+  - experiment_rules, delivery_rules, audiences and audiences in OptimizelyExperiment
+    - [#342] (https://github.com/optimizely/python-sdk/pull/342)
+    - [#351] (https://github.com/optimizely/python-sdk/pull/351/files)
+* For details please refer to our documentation page:
+  - Python-sdk: [https://docs.developers.optimizely.com/full-stack/docs/optimizelyconfig-python]
+
+* OptimizelyFeature.experiments_map of OptimizelyConfig is now deprecated. Please use OptimizelyFeature.experiment_rules and OptimizelyFeature.delivery_rules. [#360] (https://github.com/optimizely/python-sdk/pull/360)
+
+### Bug Fixes
+* Fix event processor negative timeout interval when retrieving events from queue. [#356] (https://github.com/optimizely/python-sdk/pull/356)
+
+## 3.9.1
+July 14th, 2021
+
+### Bug Fixes:
+* Fixed issue with serving incorrect variation in projects containing multiple flags with duplicate keys. [#347] (https://github.com/optimizely/python-sdk/pull/347)
+* Fixed issue with serving incorrect variation in create_impression_event in user_event_factory.py. [#350] (https://github.com/optimizely/python-sdk/pull/350)
+
+## 3.9.0
+June 1st, 2021
+
+### New Features
+* Added support for multiple concurrent prioritized experiments per flag. [#322](https://github.com/optimizely/python-sdk/pull/322)
+
+## 3.8.0
+February 12th, 2021
+
+### New Features
+* New Features
+Introducing a new primary interface for retrieving feature flag status, configuration and associated experiment decisions for users ([#309](https://github.com/optimizely/python-sdk/pull/309)). The new `OptimizelyUserContext` class is instantiated with `create_user_context` and exposes the following APIs to get `OptimizelyDecision`:
+
+    - set_attribute
+    - decide
+    - decide_all
+    - decide_for_keys
+    - track_event
+
+For details, refer to our documentation page: https://docs.developers.optimizely.com/full-stack/v4.0/docs/python-sdk.
+
+## 3.7.1
+November 19th, 2020
+
+### Bug Fixes:
+* Added "enabled" field to decision metadata structure. [#306](https://github.com/optimizely/python-sdk/pull/306)
+
+## 3.7.0
+November 2nd, 2020
+
+### New Features
+* Added support for upcoming application-controlled introduction of tracking for non-experiment Flag decisions. [#300](https://github.com/optimizely/python-sdk/pull/300)
+
+## 3.6.0
+October 1st, 2020
+
+### New Features:
+* Version targeting using semantic version syntax. [#293](https://github.com/optimizely/python-sdk/pull/293)
+* Datafile accessor API added to access current config as a JSON string. [#283](https://github.com/optimizely/python-sdk/pull/283)
+
+### Bug Fixes:
+* Fixed package installation for Python 3.4 and pypy. [#298](https://github.com/optimizely/python-sdk/pull/298)
+
+## 3.5.2
+July 14th, 2020
+
+### Bug Fixes:
+* Fixed handling of network and no status code errors when polling for datafile in `PollingConfigManager` and `AuthDatafilePollingConfigManager`. ([#287](https://github.com/optimizely/python-sdk/pull/287))
+
+## 3.5.1
+July 10th, 2020
+
+### Bug Fixes:
+* Fixed HTTP request exception handling in `PollingConfigManager`. ([#285](https://github.com/optimizely/python-sdk/pull/285))
+
+## 3.5.0
+July 9th, 2020
+
+### New Features:
+* Introduced 2 APIs to interact with feature variables:
+  * `get_feature_variable_json` allows you to get value for JSON variables related to a feature.
+  * `get_all_feature_variables` gets values for all variables under a feature.
+* Added support for fetching authenticated datafiles. `AuthDatafilePollingConfigManager` is a new config manager that allows you to poll for a datafile belonging to a secure environment. You can create a client by setting the `datafile_access_token`.
+
+### Bug Fixes:
+* Fixed log messages for targeted rollouts evaluation. ([#268](https://github.com/optimizely/python-sdk/pull/268))
+
+## 3.4.2
+June 11th, 2020
+
+### Bug Fixes:
+* Adjusted log level for audience evaluation logs. ([#267](https://github.com/optimizely/python-sdk/pull/267))
+
+## 3.4.1
+March 19th, 2020
+
+### Bug Fixes:
+* Updated `jsonschema` to address [installation issue](https://github.com/optimizely/python-sdk/issues/232).
+
+## 3.4.0
+January 27th, 2020
+
+### New Features:
+* Added a new API to get project configuration static data.
+  * Call `get_optimizely_config()` to get a snapshot of project configuration static data.
+  * It returns an `OptimizelyConfig` instance which includes a datafile revision number, all experiments, and feature flags mapped by their key values.
+  * Added caching for `get_optimizely_config()` - `OptimizelyConfig` object will be cached and reused for the lifetime of the datafile.
+  * For details, refer to our documentation page: [https://docs.developers.optimizely.com/full-stack/docs/optimizelyconfig-python](https://docs.developers.optimizely.com/full-stack/docs/optimizelyconfig-python).
+
+
+## 3.3.1
+December 16th, 2019
+
+### Bug Fixes:
+* Fixed [installation issue](https://github.com/optimizely/python-sdk/issues/220) on Windows. ([#224](https://github.com/optimizely/python-sdk/pull/224))
+* Fixed batch event processor deadline reset issue. ([#227](https://github.com/optimizely/python-sdk/pull/227))
+* Added more batch event processor debug messages. ([#227](https://github.com/optimizely/python-sdk/pull/227))
+
+## 3.3.0
+October 28th, 2019
+
+### New Features:
+* Added support for event batching via the event processor.
+  * Events generated by methods like `activate`, `track`, and `is_feature_enabled` will be held in a queue until the configured batch size is reached, or the configured flush interval has elapsed. Then, they will be batched into a single payload and sent to the event dispatcher.
+  * To configure event batching, set the `batch_size` and `flush_interval` properties when initializing instance of [BatchEventProcessor](https://github.com/optimizely/python-sdk/blob/3.3.x/optimizely/event/event_processor.py#L45).
+  * Event batching is disabled by default. You can pass in instance of `BatchEventProcessor` when creating `Optimizely` instance to enable event batching.
+  * Users can subscribe to `LogEvent` notification to be notified of whenever a payload consisting of a batch of user events is handed off to the event dispatcher to send to Optimizely's backend.
+* Introduced blocking timeout in `PollingConfigManager`. By default, calls to `get_config` will block for maximum of 10 seconds until config is available.
+
+### Bug Fixes:
+* Fixed incorrect log message when numeric metric is not used. ([#217](https://github.com/optimizely/python-sdk/pull/217))
+
+## 3.2.0
+August 27th, 2019
+
+### New Features:
+* Added support for automatic datafile management via [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151):
+  * The [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151) is an implementation of the [BaseConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L32).
+  * Users may provide one of datafile or SDK key (sdk_key) or both to `optimizely.Optimizely`. Based on that, the SDK will use the [StaticConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L73) or the [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151). Refer to the [README](README.md) for more instructions.
+  * An initial datafile can be provided to the `PollingConfigManager` to bootstrap before making HTTP requests for the hosted datafile.
+  * Requests for the datafile are made in a separate thread and are scheduled with fixed delay.
+  * Configuration updates can be subscribed to by adding the OPTIMIZELY_CONFIG_UPDATE notification listener.
+* Introduced `Optimizely.get_feature_variable` API.  ([#191](https://github.com/optimizely/python-sdk/pull/191))
+
+### Deprecated:
+
+* `NotificationCenter.clear_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
+* `NotificationCenter.clear_all_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_all_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
+
+## 3.2.0b1
+July 26th, 2019
+
+### New Features:
+* Added support for automatic datafile management via [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151):
+  * The [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151) is an implementation of the [BaseConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L32).
+  * Users may provide one of datafile or SDK key (sdk_key) or both to `optimizely.Optimizely`. Based on that, the SDK will use the [StaticConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L73) or the [PollingConfigManager](https://github.com/optimizely/python-sdk/blob/3.2.x/optimizely/config_manager.py#L151). Refer to the [README](README.md) for more instructions.
+  * An initial datafile can be provided to the `PollingConfigManager` to bootstrap before making HTTP requests for the hosted datafile.
+  * Requests for the datafile are made in a separate thread and are scheduled with fixed delay.
+  * Configuration updates can be subscribed to by adding the OPTIMIZELY_CONFIG_UPDATE notification listener.
+* Introduced `Optimizely.get_feature_variable` API.  ([#191](https://github.com/optimizely/python-sdk/pull/191))
+
+### Deprecated:
+
+* `NotificationCenter.clear_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
+* `NotificationCenter.clear_all_notifications` is deprecated as of this release. Please use `NotificationCenter.clear_all_notification_listeners`.  ([#182](https://github.com/optimizely/python-sdk/pull/182))
+
+## 3.1.0
+May 3rd, 2019
+
+### New Features:
+* Introduced Decision notification listener to be able to record:
+  * Variation assignments for users activated in an experiment.
+  * Feature access for users.
+  * Feature variable value for users.
+
+### Bug Fixes:
+* Feature variable APIs now return default variable value when featureEnabled property is false.  ([#171](https://github.com/optimizely/python-sdk/pull/171))
+
+### Deprecated:
+* Activate notification listener is deprecated as of this release.  Recommendation is to use the new Decision notification listener.  Activate notification listener will be removed in the next major release.
+
+## 3.0.0
+March 1st, 2019
+
+The 3.0 release improves event tracking and supports additional audience
+targeting functionality.
+
+### New Features:
+* Event tracking:
+  * The `track` method now dispatches its conversion event *unconditionally*, without first determining whether the user is targeted by a known experiment that uses the event. This may increase outbound network traffic.
+  * In Optimizely results, conversion events sent by 3.0 SDKs don\'t explicitly name the experiments and variations that are currently targeted to the user. Instead, conversions are automatically attributed to variations that the user has previously seen, as long as those variations were served via 3.0 SDKs or by other clients capable of automatic attribution, and as long as our backend actually received the impression events for those variations.
+  * Altogether, this allows you to track conversion events and attribute them to variations even when you don't know all of a user's attribute values, and even if the user's attribute values or the experiment's configuration have changed such that the user is no longer affected by the experiment. As a result, **you may observe an increase in the conversion rate for previously-instrumented events.** If that is undesirable, you can reset the results of previously-running experiments after upgrading to the 3.0 SDK.  -   This will also allow you to attribute events to variations from other Optimizely projects in your account, even though those experiments don't appear in the same datafile.
+  * Note that for results segmentation in Optimizely results, the user attribute values from one event are automatically applied to all other events in the same session, as long as the events in question were actually received by our backend. This behavior was already in place and is not affected by the 3.0 release.
+* Support for all types of attribute values, not just strings.
+  * All values are passed through to notification listeners.
+  * Strings, booleans, and valid numbers are passed to the event dispatcher and can be used for Optimizely results segmentation.  A valid number is a finite float or numbers.Integral in the inclusive range \[-2 ^ 53, 2 ^ 53\].
+  * Strings, booleans, and valid numbers are relevant for audience conditions.
+* Support for additional matchers in audience conditions:
+  * An `exists` matcher that passes if the user has a non-null value for the targeted user attribute and fails otherwise.
+  * A `substring` matcher that resolves if the user has a string value for the targeted attribute.
+    * `gt` (greater than) and `lt` (less than) matchers that resolve if the user has a valid number value for the targeted attribute.  A valid number is a finite float or numbers.Integral in the inclusive range \[-2 ^ 53, 2 ^ 53\].
+    * The original (`exact`) matcher can now be used to target booleans and valid numbers, not just strings.
+* Support for A/B tests, feature tests, and feature rollouts whose audiences are combined using `"and"` and `"not"` operators, not just the `"or"` operator.
+* Datafile-version compatibility check: The SDK will remain uninitialized (i.e., will gracefully fail to activate experiments and features) if given a datafile version greater than 4.
+* Updated Pull Request template and commit message guidelines.
+
+### Breaking Changes:
+* Conversion events sent by 3.0 SDKs don\'t explicitly name the experiments and variations that are currently targeted to the user, so these events are unattributed in raw events data export. You must use the new *results* export to determine the variations to which events have been attributed.
+* Previously, notification listeners were only given string-valued user attributes because only strings could be passed into various method calls. That is no longer the case. You may pass non-string attribute values, and if you do, you must update your notification listeners to be able to receive whatever values you pass in.
+
+### Bug Fixes:
+* Experiments and features can no longer activate when a negatively targeted attribute has a missing, null, or malformed value.
+  * Audience conditions (except for the new `exists` matcher) no longer resolve to `false` when they fail to find an legitimate value for the targeted user attribute. The result remains `null` (unknown). Therefore, an audience that negates such a condition (using the `"not"` operator) can no longer resolve to `true` unless there is an unrelated branch in the condition tree that itself resolves to `true`.
+* Updated the default event dispatcher to log an error if the request resolves to HTTP 4xx or 5xx.  ([#140](https://github.com/optimizely/python-sdk/pull/140))
+* All methods now validate that user IDs are strings and that experiment keys, feature keys, feature variable keys, and event keys are non-empty strings.
+
+## 2.1.1
+August 21st, 2018
+
+* Fix: record conversions for all experiments using an event when using track([#136](https://github.com/optimizely/python-sdk/pull/136)).
+
+## 2.1.0
+July 2nd, 2018
+
+* Introduced support for bot filtering ([#121](https://github.com/optimizely/python-sdk/pull/121)).
+* Overhauled logging to use standard Python logging ([#123](https://github.com/optimizely/python-sdk/pull/123)).
+
+## 2.0.1
+June 19th, 2018
+
+* Fix: send impression event for Feature Test when Feature is disabled ([#128](https://github.com/optimizely/python-sdk/pull/128)).
+
+## 2.0.0
+April 12th, 2018
+
+This major release introduces APIs for Feature Management. It also
+introduces some breaking changes listed below.
+
+### New Features
+* Introduced the `is_feature_enabled` API to determine whether to show a feature to a user or not.
+
+```
+    is_enabled = optimizel_client.is_feature_enabled('my_feature_key', 'my_user', user_attributes)
+```
+
+* All enabled features for the user can be retrieved by calling:
+
+```
+    enabled_features = optimizely_client.get_enabled_features('my_user', user_attributes)
+```
+* Introduced Feature Variables to configure or parameterize a feature.  There are four variable types: `String`, `Integer`, `Double`, `Boolean`.
+
+```
+    string_variable = optimizely_client.get_feature_variable_string('my_feature_key', 'string_variable_key', 'my_user')
+    integer_variable = optimizely_client.get_feature_variable_integer('my_feature_key', 'integer_variable_key', 'my_user')
+    double_variable = optimizely_client.get_feature_variable_double('my_feature_key', 'double_variable_key', 'my_user')
+    boolean_variable = optimizely_client.get_feature_variable_boolean('my_feature_key', 'boolean_variable_key', 'my_user')
+```
+
+### Breaking changes
+* The `track` API with revenue value as a stand-alone parameter has been removed. The revenue value should be passed in as an entry in the event tags dict. The key for the revenue tag is `revenue` and the passed in value will be treated by Optimizely as the value for computing results.
+
+```
+    event_tags = {
+      'revenue': 1200
+    }
+
+    optimizely_client.track('event_key', 'my_user', user_attributes, event_tags)
+```
+
+## 2.0.0b1
+March 29th, 2018
+
+This beta release introduces APIs for Feature Management. It also
+introduces some breaking changes listed below.
+
+### New Features
+* Introduced the `is_feature_enabled` API to determine whether to show a feature to a user or not.
+```
+    is_enabled = optimizel_client.is_feature_enabled('my_feature_key', 'my_user', user_attributes)
+```
+
+* All enabled features for the user can be retrieved by calling:
+
+```
+    enabled_features = optimizely_client.get_enabled_features('my_user', user_attributes)
+```
+
+* Introduced Feature Variables to configure or parameterize a feature.  There are four variable types: `String`, `Integer`, `Double`, `Boolean`.
+
+```
+    string_variable = optimizely_client.get_feature_variable_string('my_feature_key', 'string_variable_key', 'my_user')
+    integer_variable = optimizely_client.get_feature_variable_integer('my_feature_key', 'integer_variable_key', 'my_user')
+    double_variable = optimizely_client.get_feature_variable_double('my_feature_key', 'double_variable_key', 'my_user')
+    boolean_variable = optimizely_client.get_feature_variable_boolean('my_feature_key', 'boolean_variable_key', 'my_user')
+```
+
+### Breaking changes
+* The `track` API with revenue value as a stand-alone parameter has been removed. The revenue value should be passed in as an entry in the event tags dict. The key for the revenue tag is `revenue` and the passed in value will be treated by Optimizely as the value for computing results.
+
+```
+    event_tags = {
+      'revenue': 1200
+    }
+
+    optimizely_client.track('event_key', 'my_user', user_attributes, event_tags)
+```
+
+## 1.4.0
+
+* Added support for IP anonymization.
+* Added support for notification listeners.
+* Added support for bucketing ID.
+* Updated mmh3 to handle installation failures on Windows 10.
+
+## 1.3.0
+
+* Introduced support for forced bucketing.
+* Introduced support for numeric metrics.
+* Updated event builder to support new endpoint.
+
+## 1.2.1
+
+* Removed older feature flag parsing.
+
+## 1.2.0
+
+* Added user profile service.
+
+## 1.1.1
+
+* Updated datafile parsing to be able to handle additional fields.
+* Deprecated Classic project support.
+
+## 1.1.0
+
+* Included datafile revision information in log events.
+* Added event tags to track API to allow users to pass in event metadata.
+* Deprecated the `event_value` parameter from the track method. Should use `event_tags` to pass in event value instead.
+* Updated event logging endpoint to logx.optimizely.com.
+
+## 1.0.0
+
+* Introduced support for Full Stack projects in Optimizely X. No breaking changes from previous version.
+* Introduced more graceful exception handling in instantiation and core methods.
+* Updated whitelisting to precede audience matching.
+
+## 0.1.3
+
+* Added support for v2 endpoint and datafile.
+* Updated dispatch_event to consume an Event object instead of url and params. The Event object comprises of four properties: url (string representing URL to dispatch event to), params (dict representing the params to be set for the event), http_verb (one of 'GET' or 'POST') and headers (header values to be sent along).
+* Fixed issue with tracking events for experiments in groups.
+
+## 0.1.2
+
+* Updated requirements file.
+
+## 0.1.1
+
+* Introduced option to skip JSON schema validation.
+
+## 0.1.0
+
+* Beta release of the Python SDK for server-side testing.
```

### Comparing `optimizely-sdk-4.1.1/setup.py` & `optimizely-sdk-5.0.0b0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,60 @@
-import os
-
-from setuptools import setup
-from setuptools import find_packages
-
-here = os.path.join(os.path.dirname(__file__))
-
-
-__version__ = None
-with open(os.path.join(here, 'optimizely', 'version.py')) as _file:
-    exec(_file.read())
-
-with open(os.path.join(here, 'requirements', 'core.txt')) as _file:
-    REQUIREMENTS = _file.read().splitlines()
-
-with open(os.path.join(here, 'requirements', 'test.txt')) as _file:
-    TEST_REQUIREMENTS = _file.read().splitlines()
-    TEST_REQUIREMENTS = list(set(REQUIREMENTS + TEST_REQUIREMENTS))
-
-with open(os.path.join(here, 'README.md')) as _file:
-    README = _file.read()
-
-with open(os.path.join(here, 'CHANGELOG.md')) as _file:
-    CHANGELOG = _file.read()
-
-about_text = (
-    'Optimizely Feature Experimentation is A/B testing and feature management for product development teams. '
-    'Experiment in any application. Make every feature on your roadmap an opportunity to learn. '
-    'Learn more at https://www.optimizely.com/products/experiment/feature-experimentation/ or see our documentation at '
-    'https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/welcome. '
-)
-
-setup(
-    name='optimizely-sdk',
-    version=__version__,
-    description='Python SDK for Optimizely Feature Experimentation, Optimizely Full Stack (legacy), '
-    'and Optimizely Rollouts.',
-    long_description=about_text + README + CHANGELOG,
-    long_description_content_type='text/markdown',
-    author='Optimizely',
-    author_email='developers@optimizely.com',
-    url='https://github.com/optimizely/python-sdk',
-    classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Environment :: Web Environment',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: Apache Software License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-    ],
-    packages=find_packages(exclude=['docs', 'tests']),
-    extras_require={'test': TEST_REQUIREMENTS},
-    install_requires=REQUIREMENTS,
-    tests_require=TEST_REQUIREMENTS,
-    test_suite='tests',
-)
+import os
+
+from setuptools import setup
+from setuptools import find_packages
+
+here = os.path.join(os.path.dirname(__file__))
+
+
+__version__ = None
+with open(os.path.join(here, 'optimizely', 'version.py')) as _file:
+    exec(_file.read())
+
+with open(os.path.join(here, 'requirements', 'core.txt')) as _file:
+    REQUIREMENTS = _file.read().splitlines()
+
+with open(os.path.join(here, 'requirements', 'test.txt')) as _file:
+    TEST_REQUIREMENTS = _file.read().splitlines()
+    TEST_REQUIREMENTS = list(set(REQUIREMENTS + TEST_REQUIREMENTS))
+
+with open(os.path.join(here, 'README.md')) as _file:
+    README = _file.read()
+
+with open(os.path.join(here, 'CHANGELOG.md')) as _file:
+    CHANGELOG = _file.read()
+
+about_text = (
+    'Optimizely Feature Experimentation is A/B testing and feature management for product development teams. '
+    'Experiment in any application. Make every feature on your roadmap an opportunity to learn. '
+    'Learn more at https://www.optimizely.com/products/experiment/feature-experimentation/ or see our documentation at '
+    'https://docs.developers.optimizely.com/experimentation/v4.0.0-full-stack/docs/welcome. '
+)
+
+setup(
+    name='optimizely-sdk',
+    version=__version__,
+    description='Python SDK for Optimizely Feature Experimentation, Optimizely Full Stack (legacy), '
+    'and Optimizely Rollouts.',
+    long_description=about_text + README + CHANGELOG,
+    long_description_content_type='text/markdown',
+    author='Optimizely',
+    author_email='developers@optimizely.com',
+    url='https://github.com/optimizely/python-sdk',
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+        'Environment :: Web Environment',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: Apache Software License',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+    ],
+    packages=find_packages(exclude=['docs', 'tests']),
+    extras_require={'test': TEST_REQUIREMENTS},
+    install_requires=REQUIREMENTS,
+    tests_require=TEST_REQUIREMENTS,
+    test_suite='tests',
+)
```

