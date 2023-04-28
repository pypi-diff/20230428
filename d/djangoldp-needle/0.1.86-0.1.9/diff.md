# Comparing `tmp/djangoldp_needle-0.1.86.tar.gz` & `tmp/djangoldp_needle-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_needle-0.1.86.tar", last modified: Fri Apr 28 07:24:34 2023, max compression
+gzip compressed data, was "dist/djangoldp_needle-0.1.9.tar", last modified: Thu Jan  5 15:11:29 2023, max compression
```

## Comparing `djangoldp_needle-0.1.86.tar` & `djangoldp_needle-0.1.9.tar`

### file list

```diff
@@ -1,154 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:24:34.000000 djangoldp_needle-0.1.86/
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:24:34.000000 djangoldp_needle-0.1.86/djangoldp_needle/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:24:34.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/test_first_annotation_on_user_creation.py
--rw-rw-rw-   0 root         (0) root         (0)     3002 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/test_user_contact.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16392 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/test_annotation_target_add.py
--rw-rw-rw-   0 root         (0) root         (0)     5325 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/test_booklets_list.py
--rw-rw-rw-   0 root         (0) root         (0)     2196 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/test_booklets_quit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:24:34.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:24:34.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/target_url/
--rw-rw-rw-   0 root         (0) root         (0)     4305 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/target_url/links_with_not_found.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/target_url/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11721 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/target_url/links_with_dates.py
--rw-rw-rw-   0 root         (0) root         (0)    15329 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/target_url/links.py
--rw-rw-rw-   0 root         (0) root         (0)      642 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/target_url/links_with_timeout.py
--rw-rw-rw-   0 root         (0) root         (0)     1747 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/target_url/realsites.py
--rw-rw-rw-   0 root         (0) root         (0)    17166 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/target_url/links_with_redirect.py
--rw-rw-rw-   0 root         (0) root         (0)     4538 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/target_url/links_with_error.py
--rw-rw-rw-   0 root         (0) root         (0)     4184 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/target_url/needlerealsites.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:24:34.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/parsing/
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/parsing/base_valid.20221103.html
--rw-rw-rw-   0 root         (0) root         (0)   613961 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/parsing/lemonde-1.html
--rw-rw-rw-   0 root         (0) root         (0)   289885 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/parsing/theconversation-1.html
--rw-rw-rw-   0 root         (0) root         (0)   126155 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/parsing/internetactu-1.html
--rw-rw-rw-   0 root         (0) root         (0)   306075 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/parsing/lemonde.20221103.html
--rw-rw-rw-   0 root         (0) root         (0)   181484 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/parsing/theconversation.20221103.html
--rw-rw-rw-   0 root         (0) root         (0)   149029 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/parsing/reporterre-1.html
--rw-rw-rw-   0 root         (0) root         (0)   127161 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/parsing/laviedesidees-1.html
--rw-rw-rw-   0 root         (0) root         (0)   369446 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/parsing/latribune-1.html
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/parsing/base_invalid.20221103.html
--rw-rw-rw-   0 root         (0) root         (0)   232761 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/parsing/fredcavazza-1.html
--rw-rw-rw-   0 root         (0) root         (0)   118533 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/data/parsing/blogdumoderateur-1.html
--rw-rw-rw-   0 root         (0) root         (0)     2343 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/test_date_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2470 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/test_booklets_add.py
--rw-rw-rw-   0 root         (0) root         (0)    10168 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/test_annotation_activity.py
--rw-rw-rw-   0 root         (0) root         (0)     2841 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/test_annotation_import.py
--rw-rw-rw-   0 root         (0) root         (0)    10327 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/test_annotation_intersection.py
--rw-rw-rw-   0 root         (0) root         (0)     8159 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/test_annotation_yarn.py
--rw-rw-rw-   0 root         (0) root         (0)     4198 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/test_booklets_invitation.py
--rw-rw-rw-   0 root         (0) root         (0)     1590 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/tests/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:24:34.000000 djangoldp_needle-0.1.86/djangoldp_needle/templates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/templates/email.txt
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     2009 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/djangoldp_urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:24:34.000000 djangoldp_needle-0.1.86/djangoldp_needle/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:24:34.000000 djangoldp_needle-0.1.86/djangoldp_needle/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/management/commands/importneedledata.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-04-28 07:24:32.000000 djangoldp_needle-0.1.86/djangoldp_needle/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:24:34.000000 djangoldp_needle-0.1.86/djangoldp_needle/request_parser/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:24:34.000000 djangoldp_needle-0.1.86/djangoldp_needle/request_parser/parsers/
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/request_parser/parsers/linkIcon.py
--rw-rw-rw-   0 root         (0) root         (0)     2306 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/request_parser/parsers/opengraph.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/request_parser/parsers/urlParser.py
--rw-rw-rw-   0 root         (0) root         (0)      357 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/request_parser/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/request_parser/parsers/abstract_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2328 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/request_parser/parsers/metaProp.py
--rw-rw-rw-   0 root         (0) root         (0)     3571 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/request_parser/parsers/itemProp.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/request_parser/parsers/linkCanonicalProp.py
--rw-rw-rw-   0 root         (0) root         (0)    25244 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/request_parser/parsers/jsonld.py
--rw-rw-rw-   0 root         (0) root         (0)      808 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/request_parser/parsers/lastChanceParser.py
--rw-rw-rw-   0 root         (0) root         (0)      611 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/request_parser/parsers/titleTag.py
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/request_parser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/request_parser/webdriver_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6029 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/request_parser/request_parser.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:24:34.000000 djangoldp_needle-0.1.86/djangoldp_needle/views/
--rw-rw-rw-   0 root         (0) root         (0)    12144 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/views/annotation.py
--rw-rw-rw-   0 root         (0) root         (0)      461 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/views/user.py
--rw-rw-rw-   0 root         (0) root         (0)      651 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/views/annotation_intersections.py
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/views/needle_user_profile.py
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/views/needle_activity.py
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/views/contact_message.py
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/views/booklet.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/views/annotation_intersection_read.py
--rw-rw-rw-   0 root         (0) root         (0)    10838 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/views/annotation_target.py
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/views/needle_user_follow.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/views/tag.py
--rw-rw-rw-   0 root         (0) root         (0)     1002 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/views/booklet_invitation.py
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/views/booklet_quit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:24:34.000000 djangoldp_needle-0.1.86/djangoldp_needle/permissions/
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/permissions/annotation.py
--rw-rw-rw-   0 root         (0) root         (0)      531 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/permissions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/permissions/needle_user_profile.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/permissions/needle_activity.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/permissions/contact_message.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/permissions/_base.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/permissions/booklet.py
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/permissions/annotation_intersection_read.py
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/permissions/annotation_target.py
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/permissions/needle_user_follow.py
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/permissions/tag.py
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/djangoldp_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:24:34.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      413 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0004_annotationtarget_image.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0019_auto_20230208_1213.py
--rw-rw-rw-   0 root         (0) root         (0)      422 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0012_needleactivity_activity_type.py
--rw-rw-rw-   0 root         (0) root         (0)     2622 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1852 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0013_needleuserprofile.py
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0029_auto_20230411_1211.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0009_activity_subtitle.py
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0015_auto_20230112_1339.py
--rw-rw-rw-   0 root         (0) root         (0)      404 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0006_auto_20221101_1846.py
--rw-rw-rw-   0 root         (0) root         (0)     1543 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0002_tag.py
--rw-rw-rw-   0 root         (0) root         (0)      465 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0018_auto_20230129_1617.py
--rw-rw-rw-   0 root         (0) root         (0)      543 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0014_auto_20230105_1238.py
--rw-rw-rw-   0 root         (0) root         (0)      408 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0022_annotation_annotation_date.py
--rw-rw-rw-   0 root         (0) root         (0)      584 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0007_auto_20221114_1643.py
--rw-rw-rw-   0 root         (0) root         (0)     1992 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0023_booklet.py
--rw-rw-rw-   0 root         (0) root         (0)     1854 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0011_auto_20221125_1015.py
--rw-rw-rw-   0 root         (0) root         (0)      432 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0028_annotationtarget_annotation_target_date.py
--rw-rw-rw-   0 root         (0) root         (0)     1846 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0017_annotationintersectionread.py
--rw-rw-rw-   0 root         (0) root         (0)     1970 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0025_needleuserfollow.py
--rw-rw-rw-   0 root         (0) root         (0)     1699 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0019_contactmessage.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0024_auto_20230328_0814.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0020_contactmessage_creation_date.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0021_merge_20230213_1548.py
--rw-rw-rw-   0 root         (0) root         (0)      519 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0027_needleuserfollow_creation_date.py
--rw-rw-rw-   0 root         (0) root         (0)      399 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0003_annotation_tags.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0005_annotationtarget_title.py
--rw-rw-rw-   0 root         (0) root         (0)     1635 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0008_activity.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0010_activity_read.py
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0026_auto_20230331_1603.py
--rw-rw-rw-   0 root         (0) root         (0)     1129 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/migrations/0016_auto_20230123_1741.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:24:34.000000 djangoldp_needle-0.1.86/djangoldp_needle/models/
--rw-rw-rw-   0 root         (0) root         (0)     2885 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/models/annotation.py
--rw-rw-rw-   0 root         (0) root         (0)     7197 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/models/activity_signal_receiver.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/models/needle_user_profile.py
--rw-rw-rw-   0 root         (0) root         (0)     1216 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/models/needle_activity.py
--rw-rw-rw-   0 root         (0) root         (0)     1489 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/models/contact_message.py
--rw-rw-rw-   0 root         (0) root         (0)     1037 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/models/booklet.py
--rw-rw-rw-   0 root         (0) root         (0)     1185 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/models/annotation_intersection_read.py
--rw-rw-rw-   0 root         (0) root         (0)      830 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/models/annotation_target.py
--rw-rw-rw-   0 root         (0) root         (0)     1346 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/models/needle_user_follow.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/djangoldp_needle/models/tag.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/setup.py
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-04-28 07:24:11.000000 djangoldp_needle-0.1.86/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-04-28 07:24:34.000000 djangoldp_needle-0.1.86/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      521 2023-04-28 07:24:34.000000 djangoldp_needle-0.1.86/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:24:34.000000 djangoldp_needle-0.1.86/djangoldp_needle.egg-info/
--rw-r--r--   0 root         (0) root         (0)      521 2023-04-28 07:24:34.000000 djangoldp_needle-0.1.86/djangoldp_needle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 07:24:34.000000 djangoldp_needle-0.1.86/djangoldp_needle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     6552 2023-04-28 07:24:34.000000 djangoldp_needle-0.1.86/djangoldp_needle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-28 07:24:34.000000 djangoldp_needle-0.1.86/djangoldp_needle.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      142 2023-04-28 07:24:34.000000 djangoldp_needle-0.1.86/djangoldp_needle.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 15:11:29.000000 djangoldp_needle-0.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)      194 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 15:11:29.000000 djangoldp_needle-0.1.9/djangoldp_needle/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 15:11:29.000000 djangoldp_needle-0.1.9/djangoldp_needle/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4967 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/tests/test_annotation_add.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/tests/test_first_annotation_on_user_creation.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7084 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/tests/test_annotation_target_add.py
+-rw-rw-rw-   0 root         (0) root         (0)    10736 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/tests/test_annotation_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/tests/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      782 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/djangoldp_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-05 15:11:27.000000 djangoldp_needle-0.1.9/djangoldp_needle/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 15:11:29.000000 djangoldp_needle-0.1.9/djangoldp_needle/request_parser/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 15:11:29.000000 djangoldp_needle-0.1.9/djangoldp_needle/request_parser/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/request_parser/parsers/opengraph.py
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/request_parser/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/request_parser/parsers/abstract_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/request_parser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/request_parser/request_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 15:11:29.000000 djangoldp_needle-0.1.9/djangoldp_needle/views/
+-rw-rw-rw-   0 root         (0) root         (0)     1696 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/views/annotation_target_intersection.py
+-rw-rw-rw-   0 root         (0) root         (0)     3392 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/views/annotation.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/views/needle_user_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)      570 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/views/needle_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)     2216 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/views/annotation_target.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/views/tag.py
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/djangoldp_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 15:11:29.000000 djangoldp_needle-0.1.9/djangoldp_needle/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      413 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/migrations/0004_annotationtarget_image.py
+-rw-rw-rw-   0 root         (0) root         (0)      422 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/migrations/0012_needleactivity_activity_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     2622 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1852 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/migrations/0013_needleuserprofile.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/migrations/0009_activity_subtitle.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      404 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/migrations/0006_auto_20221101_1846.py
+-rw-rw-rw-   0 root         (0) root         (0)     1543 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/migrations/0002_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)      543 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/migrations/0014_auto_20230105_1238.py
+-rw-rw-rw-   0 root         (0) root         (0)      584 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/migrations/0007_auto_20221114_1643.py
+-rw-rw-rw-   0 root         (0) root         (0)     1854 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/migrations/0011_auto_20221125_1015.py
+-rw-rw-rw-   0 root         (0) root         (0)      399 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/migrations/0003_annotation_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/migrations/0005_annotationtarget_title.py
+-rw-rw-rw-   0 root         (0) root         (0)     1635 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/migrations/0008_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/migrations/0010_activity_read.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 15:11:29.000000 djangoldp_needle-0.1.9/djangoldp_needle/models/
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/models/annotation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3641 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/models/activity_signal_receiver.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      803 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/models/needle_user_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/models/needle_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/models/annotation_target.py
+-rw-rw-rw-   0 root         (0) root         (0)      624 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/djangoldp_needle/models/tag.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-01-05 15:11:12.000000 djangoldp_needle-0.1.9/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      571 2023-01-05 15:11:29.000000 djangoldp_needle-0.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      399 2023-01-05 15:11:29.000000 djangoldp_needle-0.1.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-05 15:11:29.000000 djangoldp_needle-0.1.9/djangoldp_needle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-01-05 15:11:29.000000 djangoldp_needle-0.1.9/djangoldp_needle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-05 15:11:29.000000 djangoldp_needle-0.1.9/djangoldp_needle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     2287 2023-01-05 15:11:29.000000 djangoldp_needle-0.1.9/djangoldp_needle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-01-05 15:11:29.000000 djangoldp_needle-0.1.9/djangoldp_needle.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2023-01-05 15:11:29.000000 djangoldp_needle-0.1.9/djangoldp_needle.egg-info/requires.txt
```

### Comparing `djangoldp_needle-0.1.86/djangoldp_needle/tests/test_first_annotation_on_user_creation.py` & `djangoldp_needle-0.1.9/djangoldp_needle/tests/test_first_annotation_on_user_creation.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.86/djangoldp_needle/tests/test_annotation_activity.py` & `djangoldp_needle-0.1.9/djangoldp_needle/tests/test_annotation_activity.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             "target": {
                 "@id": target.urlid
             }
         })
 
     def test_annotation_activity_create_first_annotation_new_annotation_target_activity(
             self):
-
+        print("test_annotation_activity_create_first_annotation_new_annotation_target_activity")
         user1 = self.buildUser('user1')
         target1 = self.buildAnnotationTarget('target1')
 
         self.client.force_authenticate(user1)
         self.client.post(
             "/users/user1/yarn/",
             content_type='application/ld+json',
@@ -62,15 +62,15 @@
             NeedleActivity.objects.filter(creator=user1,
                                           activity_type=ACTIVITY_TYPE_FIRST_ANNOTATION_WITHOUT_CONNECTIONS)
 
         self.assertEqual(1, result_needle_activity.count())
 
     def test_annotation_activity_create_first_annotation_already_exist_annotation_target_activity(
             self):
-
+        print("test_annotation_activity_create_first_annotation_already_exist_annotation_target_activity")
         user1 = self.buildUser('user1')
         user2 = self.buildUser('user2')
         target1 = self.buildAnnotationTarget('target1')
 
         self.client.force_authenticate(user1)
         self.client.post(
             "/users/user1/yarn/",
@@ -88,15 +88,15 @@
             NeedleActivity.objects.filter(creator=user2,
                                           activity_type=ACTIVITY_TYPE_FIRST_ANNOTATION_WITH_CONNECTIONS)
 
         self.assertEqual(1, result_needle_activity.count())
 
     def test_annotation_activity_create_two_annotations_not_and_already_exists_annotation_target_activity(
             self):
-
+        print("test_annotation_activity_create_two_annotations_not_and_already_exists_annotation_target_activity")
         user1 = self.buildUser('user1')
         user2 = self.buildUser('user2')
         target1 = self.buildAnnotationTarget('target1')
         target2 = self.buildAnnotationTarget('target2')
 
         self.client.force_authenticate(user1)
         self.client.post(
@@ -129,15 +129,15 @@
         )
 
         self.assertEqual(1, result_needle_activity_without.count())
         self.assertEqual(1, result_needle_activity_with.count())
 
     def test_annotation_activity_create_two_annotations_already_and_not_exists_annotation_target_activity(
             self):
-
+        print("test_annotation_activity_create_two_annotations_already_and_not_exists_annotation_target_activity")
         user1 = self.buildUser('user1')
         user2 = self.buildUser('user2')
         target1 = self.buildAnnotationTarget('target1')
         target2 = self.buildAnnotationTarget('target2')
 
         self.client.force_authenticate(user1)
         self.client.post(
@@ -170,14 +170,16 @@
         )
 
         self.assertEqual(1, result_needle_activity_without.count())
         self.assertEqual(1, result_needle_activity_with.count())
 
     def test_annotation_activity_create_two_annotations_already_and_not_exists_annotation_target_activity_two_times(
             self):
+        print(
+            "test_annotation_activity_create_two_annotations_already_and_not_exists_annotation_target_activity_two_times")
         user1 = self.buildUser('user1')
         user2 = self.buildUser('user2')
         target1 = self.buildAnnotationTarget('target1')
         target2 = self.buildAnnotationTarget('target2')
         target3 = self.buildAnnotationTarget('target3')
         target4 = self.buildAnnotationTarget('target4')
```

### Comparing `djangoldp_needle-0.1.86/djangoldp_needle/tests/test_annotation_import.py` & `djangoldp_needle-0.1.9/djangoldp_needle/views/annotation_target.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-import requests_mock
-from django.db import transaction
-from djangoldp_account.models import LDPUser
-from rest_framework.test import APITestCase, APIClient, APITransactionTestCase
-import json
-from pkg_resources import resource_string
+from django.core.exceptions import ObjectDoesNotExist
+from djangoldp.views import LDPViewSet, JSONLDParser, NoCSRFAuthentication
+from rest_framework import status
 import requests as requestsLib
+
+from ..models import AnnotationTarget, NeedleActivity
+from ..models.needle_activity import ACTIVITY_TYPE_FIRST_ANNOTATION_WITHOUT_CONNECTIONS
+from rest_framework.views import APIView, Response
+
 from ..request_parser import RequestParser
-from ..views.annotation_target import AnnotationTargetViewset
-from ..models import AnnotationTarget, Annotation, NeedleActivity
 
-from ..models.needle_activity import ACTIVITY_TYPE_FIRST_ANNOTATION_WITH_CONNECTIONS, \
-    ACTIVITY_TYPE_FIRST_ANNOTATION_WITHOUT_CONNECTIONS, ACTIVITY_TYPE_NEW_USER
 
-from ..management.commands.needle_old_data import needleImportDatas
-from ..views.annotation import import_external_annotation
-import time
-
-class TestAnnotationImport(APITestCase):
-
-    def setUp(self):
-        self.client = APIClient()
-
-    def _test_import_old_needle_data(self):
-        user_name = "Chenille_30011407"
-        user_email="test@test.test"
-        user_creation_date="2014-02-18 20:54:54"
-        target_url="https://www.nouvelobs.com/monde/20160129.OBS3681/l-etat-islamique-est-une-revolution-par-scott-atran.html"
-        target_title="L'Etat islamique est une révolution, par Scott Atran - L'Obs"
-        target_creation_date="2016-02-03 14:27:20"
-        annotation_description="c'est la description"
-        annotation_date="2016-02-03 14:27:20"
-        annotation_tags="anthropologie  radicalisation"
-
-        annotation = import_external_annotation(user_name, user_email, user_creation_date, target_url, target_title,
-                                   target_creation_date, annotation_description, annotation_date, annotation_tags,
-                                   " ", None)
-        self.assertEqual(user_name, annotation.creator.username)
-        self.assertEqual(user_email, annotation.creator.email)
-        self.assertEqual(annotation_description, annotation.description)
-        self.assertEqual(target_url, annotation.target.target)
-        self.assertEqual(2, annotation.tags.count())
-        annotation = Annotation.objects.get(target=annotation.target, creator=annotation.creator)
-        self.assertEqual(user_name, annotation.creator.username)
-        self.assertEqual(user_email, annotation.creator.email)
-        self.assertEqual(annotation_description, annotation.description)
-        self.assertEqual(target_url, annotation.target.target)
-        self.assertEqual(2, annotation.tags.count())
-        self.assertEqual('2016', annotation.annotation_date.strftime('%Y'))
-        self.assertEqual('02', annotation.annotation_date.strftime('%m'))
-
-
-    def test_import_old_needle_data(self):
-        annotationTargetViewset = AnnotationTargetViewset()
-        annotation_target = annotationTargetViewset.parse_target("http://ujomusic.com/")
-        self.assertIsNotNone(annotation_target.target)
+class AnnotationTargetViewset(LDPViewSet):
+    def create(self, request, *args, **kwargs):
+        self.check_model_permissions(request)
+        target = request.data['target']
+        try:
+            targets_in_db = AnnotationTarget.objects.get(target=target)
+        except ObjectDoesNotExist:
+            try:
+                new_annotation = self.parse_target(target)
+                return self.save_annotation_target(request, new_annotation)
+
+            except Exception as e:
+                return self.generate_invalide_response()
+
+        return self.generate_success_response(status.HTTP_200_OK, targets_in_db)
+
+    def parse_target(self, target):
+        targetRequestResponse = requestsLib.get(target)
+
+        if targetRequestResponse.status_code != 200:
+            raise Exception
+
+        parser = RequestParser()
+        (result, annotation_target) = parser.parse(target, targetRequestResponse.content)
+        if not result:
+            raise Exception
+
+        return annotation_target
+
+    def generate_success_response(self, status, target):
+        response_serializer = self.get_serializer()
+        data = response_serializer.to_representation(target)
+        headers = self.get_success_headers(data)
+        return Response(data, status=status, headers=headers)
+
+    def generate_invalide_response(self):
+        return Response({'URL': ['Le lien est invalide']}, status=status.HTTP_400_BAD_REQUEST)
+
+    def save_annotation_target(self, request, annotation_target):
+        annotation_target.save()
+        response_serializer = self.get_serializer()
+        data = response_serializer.to_representation(annotation_target)
+        headers = self.get_success_headers(data)
+        return Response(data, status=status.HTTP_201_CREATED, headers=headers)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `djangoldp_needle-0.1.86/djangoldp_needle/tests/runner.py` & `djangoldp_needle-0.1.9/djangoldp_needle/tests/runner.py`

 * *Files 26% similar despite different names*

```diff
@@ -33,20 +33,13 @@
 from django.test.runner import DiscoverRunner
 
 test_runner = DiscoverRunner(verbosity=1)
 
 failures = test_runner.run_tests([
     'djangoldp_needle.tests.test_first_annotation_on_user_creation',
     'djangoldp_needle.tests.test_annotation_target_add',
-    'djangoldp_needle.tests.test_annotation_yarn',
-    'djangoldp_needle.tests.test_annotation_activity',
-    'djangoldp_needle.tests.test_date_parser',
-    'djangoldp_needle.tests.test_annotation_intersection',
-    'djangoldp_needle.tests.test_user_contact',
-    'djangoldp_needle.tests.test_booklets_add',
-    'djangoldp_needle.tests.test_booklets_list',
-    'djangoldp_needle.tests.test_booklets_quit',
-    'djangoldp_needle.tests.test_booklets_invitation',
+    'djangoldp_needle.tests.test_annotation_add',
+    'djangoldp_needle.tests.test_annotation_activity'
 ])
 if failures:
     sys.exit(failures)
```

### Comparing `djangoldp_needle-0.1.86/djangoldp_needle/request_parser/parsers/urlParser.py` & `djangoldp_needle-0.1.9/djangoldp_needle/request_parser/parsers/opengraph.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 from . import AbstractParser
 from ...models import AnnotationTarget
-import re
-import datetime
-
-class URLParser(AbstractParser):
-
 
+class OpenGraph(AbstractParser):
     def parse(self, annotation_target: AnnotationTarget, target_url, bs_document, previous_parse_result):
-
-
-
-        if annotation_target.publication_date is None:
-
-            if annotation_target.target is not None:
-                date = self.parsedatefromurl(annotation_target.target)
-
-            if date is None:
-                date = self.parsedatefromurl(target_url)
-
-            if date:
-                annotation_target.publication_date = date.isoformat()
+        # Does not change result if previous parse match
+        if previous_parse_result:
+            return previous_parse_result
+
+        og_url = bs_document.head.find('meta', property="og:url")
+        if og_url is None:
+            return False
+
+        og_image = bs_document.head.find('meta', property="og:image")
+        if og_image is None:
+            return False
+
+        og_title = bs_document.head.find('meta', property="og:title")
+        if og_title is None:
+            return False
+
+        annotation_target.target = og_url['content']
+        annotation_target.image = og_image['content']
+        annotation_target.title = og_title['content']
 
         return True
 
-    def parsedatefromurl(self, urlString):
-        if urlString:
-            p = re.compile("http(s){0,1}:\/\/.*\/((20[0-9][0-9])\/([0-1]{0,1}[0-9])\/([0-2]{0,1}[0-9]))\/.*")
-            result = p.search(urlString)
-            if result:
-                date = result.group(2)
-                date = datetime.datetime.strptime(date, "%Y/%m/%d")
-                return date
-        return None
```

### Comparing `djangoldp_needle-0.1.86/djangoldp_needle/migrations/0001_initial.py` & `djangoldp_needle-0.1.9/djangoldp_needle/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.86/djangoldp_needle/migrations/0013_needleuserprofile.py` & `djangoldp_needle-0.1.9/djangoldp_needle/migrations/0013_needleuserprofile.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.86/djangoldp_needle/migrations/0015_auto_20230112_1339.py` & `djangoldp_needle-0.1.9/djangoldp_needle/migrations/0007_auto_20221114_1643.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-# Generated by Django 2.2.28 on 2023-01-12 13:39
+# Generated by Django 2.2.28 on 2022-11-14 16:43
 
-from django.conf import settings
 from django.db import migrations, models
-import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('djangoldp_needle', '0014_auto_20230105_1238'),
+        ('djangoldp_needle', '0006_auto_20221101_1846'),
     ]
 
     operations = [
-        migrations.RemoveField(
-            model_name='needleuserprofile',
-            name='id',
+        migrations.AddField(
+            model_name='annotation',
+            name='description',
+            field=models.TextField(null=True),
         ),
         migrations.AlterField(
-            model_name='needleuserprofile',
-            name='creator',
-            field=models.OneToOneField(on_delete=django.db.models.deletion.CASCADE, primary_key=True, serialize=False, to=settings.AUTH_USER_MODEL),
+            model_name='annotation',
+            name='tags',
+            field=models.ManyToManyField(blank=True, to='djangoldp_needle.Tag'),
         ),
     ]
```

### Comparing `djangoldp_needle-0.1.86/djangoldp_needle/migrations/0002_tag.py` & `djangoldp_needle-0.1.9/djangoldp_needle/migrations/0002_tag.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.86/djangoldp_needle/migrations/0014_auto_20230105_1238.py` & `djangoldp_needle-0.1.9/djangoldp_needle/migrations/0014_auto_20230105_1238.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.86/djangoldp_needle/migrations/0023_booklet.py` & `djangoldp_needle-0.1.9/djangoldp_needle/migrations/0011_auto_20221125_1015.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-# Generated by Django 2.2.28 on 2023-03-21 12:37
+# Generated by Django 2.2.28 on 2022-11-25 10:15
 
 from django.conf import settings
 from django.db import migrations, models
+import django.db.models.deletion
 import djangoldp.fields
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
-        ('djangoldp_needle', '0022_annotation_annotation_date'),
+        ('djangoldp_needle', '0010_activity_read'),
     ]
 
     operations = [
         migrations.CreateModel(
-            name='Booklet',
+            name='NeedleActivity',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('urlid', djangoldp.fields.LDPUrlField(blank=True, null=True, unique=True)),
                 ('is_backlink', models.BooleanField(default=False, help_text='set automatically to indicate the Model is a backlink')),
                 ('allow_create_backlink', models.BooleanField(default=True, help_text='set to False to disable backlink creation after Model save')),
-                ('title', models.CharField(max_length=160)),
-                ('abstract', models.CharField(max_length=4096, null=True)),
-                ('accessibility_public', models.BooleanField()),
-                ('collaboration_allowed', models.BooleanField()),
-                ('cover', models.IntegerField()),
-                ('annotations', models.ManyToManyField(to='djangoldp_needle.Annotation')),
-                ('contributors', models.ManyToManyField(related_name='boolket_contributor', to=settings.AUTH_USER_MODEL)),
-                ('owners', models.ManyToManyField(related_name='boolket_owner', to=settings.AUTH_USER_MODEL)),
-                ('tags', models.ManyToManyField(to='djangoldp_needle.Tag')),
+                ('creation_date', models.DateTimeField(auto_now_add=True)),
+                ('title', models.CharField(max_length=255)),
+                ('subtitle', models.CharField(default='', max_length=1024)),
+                ('content', models.TextField(max_length=4096)),
+                ('read', models.BooleanField(default=False)),
+                ('creator', models.ForeignKey(null=True, on_delete=django.db.models.deletion.CASCADE, related_name='needle_activities', to=settings.AUTH_USER_MODEL)),
             ],
             options={
                 'abstract': False,
                 'default_permissions': ['add', 'change', 'delete', 'view', 'control'],
-                'rdf_type': 'hd:annotation',
+                'rdf_type': 'hd:activity',
+                'owner_field': 'creator',
                 'depth': 0,
-                'authenticated_perms': ['add', 'view', 'edit'],
             },
         ),
+        migrations.DeleteModel(
+            name='Activity',
+        ),
     ]
```

### Comparing `djangoldp_needle-0.1.86/djangoldp_needle/migrations/0011_auto_20221125_1015.py` & `djangoldp_needle-0.1.9/djangoldp_needle/migrations/0008_activity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,37 @@
-# Generated by Django 2.2.28 on 2022-11-25 10:15
+# Generated by Django 2.2.28 on 2022-11-18 13:54
 
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 import djangoldp.fields
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
-        ('djangoldp_needle', '0010_activity_read'),
+        ('djangoldp_needle', '0007_auto_20221114_1643'),
     ]
 
     operations = [
         migrations.CreateModel(
-            name='NeedleActivity',
+            name='Activity',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('urlid', djangoldp.fields.LDPUrlField(blank=True, null=True, unique=True)),
                 ('is_backlink', models.BooleanField(default=False, help_text='set automatically to indicate the Model is a backlink')),
                 ('allow_create_backlink', models.BooleanField(default=True, help_text='set to False to disable backlink creation after Model save')),
                 ('creation_date', models.DateTimeField(auto_now_add=True)),
                 ('title', models.CharField(max_length=255)),
-                ('subtitle', models.CharField(default='', max_length=1024)),
                 ('content', models.TextField(max_length=4096)),
-                ('read', models.BooleanField(default=False)),
-                ('creator', models.ForeignKey(null=True, on_delete=django.db.models.deletion.CASCADE, related_name='needle_activities', to=settings.AUTH_USER_MODEL)),
+                ('creator', models.ForeignKey(null=True, on_delete=django.db.models.deletion.CASCADE, related_name='activities', to=settings.AUTH_USER_MODEL)),
             ],
             options={
                 'abstract': False,
                 'default_permissions': ['add', 'change', 'delete', 'view', 'control'],
                 'rdf_type': 'hd:activity',
                 'owner_field': 'creator',
                 'depth': 0,
             },
         ),
-        migrations.DeleteModel(
-            name='Activity',
-        ),
     ]
```

### Comparing `djangoldp_needle-0.1.86/djangoldp_needle/models/needle_user_profile.py` & `djangoldp_needle-0.1.9/djangoldp_needle/models/needle_user_profile.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 from django.conf import settings
 from django.db import models
 from djangoldp.models import Model
 
-from ..permissions import NeedleUserProfilePermissions
-
 
 class NeedleUserProfile(Model):
-    creator = models.OneToOneField(settings.AUTH_USER_MODEL,
-                                   related_name='needle_user_profile',
-                                   on_delete=models.CASCADE,
-                                   primary_key=True
-                                   )
-
-    activity_crossed_yarn_last_date = models.DateField()
-    activity_followed_yarn_last_date = models.DateField()
-    activity_pads_last_date = models.DateField()
+    creator = models.ForeignKey(settings.AUTH_USER_MODEL,
+                                related_name='needle_user_profiles',
+                                null=True,
+                                on_delete=models.CASCADE
+                                )
+
+    activity_crossed_yarn_last_date = models.DateTimeField(auto_now_add=True)
+    activity_followed_yarn_last_date = models.DateTimeField(auto_now_add=True)
+    activity_pads_last_date = models.DateTimeField(auto_now_add=True)
 
     name = models.CharField(max_length=16)
 
-
     class Meta(Model.Meta):
         rdf_type = 'hd:user_profile'
         owner_field = 'creator'
         owner_perms = ['view', 'change']
-        permission_classes = [NeedleUserProfilePermissions]
```

### Comparing `djangoldp_needle-0.1.86/djangoldp_needle/models/needle_activity.py` & `djangoldp_needle-0.1.9/djangoldp_needle/models/needle_activity.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from django.conf import settings
 from django.db import models
 from djangoldp.models import Model
 
-from ..permissions import NeedleActivityPermissions
-
 ACTIVITY_TYPE_NEW_USER = "ACTIVITY_TYPE_NEW_USER";
 ACTIVITY_TYPE_FIRST_ANNOTATION_WITH_CONNECTIONS = "ACTIVITY_TYPE_FIRST_ANNOTATION_WITH_CONNECTIONS";
 ACTIVITY_TYPE_FIRST_ANNOTATION_WITHOUT_CONNECTIONS = "ACTIVITY_TYPE_FIRST_ANNOTATION_WITHOUT_CONNECTIONS";
 
 
 class NeedleActivity(Model):
     creator = models.ForeignKey(settings.AUTH_USER_MODEL,
@@ -22,8 +20,7 @@
     activity_type = models.TextField(max_length=255, default="")
     read = models.BooleanField(default=False)
 
     class Meta(Model.Meta):
         rdf_type = 'hd:activity'
         owner_field = 'creator'
         owner_perms = ['view', 'change']
-        permission_classes = [NeedleActivityPermissions]
```

### Comparing `djangoldp_needle-0.1.86/djangoldp_needle/models/booklet.py` & `djangoldp_needle-0.1.9/djangoldp_needle/models/annotation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from django.conf import settings
 from django.db import models
 from djangoldp.models import Model
-from . import Annotation, Tag
-from ..permissions import BookletPermissions
+from .annotation_target import AnnotationTarget
+from . import Tag
 
-
-class Booklet(Model):
-    owners = models.ManyToManyField(settings.AUTH_USER_MODEL, related_name="boolket_owner")
-    contributors = models.ManyToManyField(settings.AUTH_USER_MODEL, related_name="boolket_contributor")
-    annotations = models.ManyToManyField(Annotation, related_name="booklets")
-    title = models.CharField(max_length=160)
-    abstract = models.CharField(max_length=4096, null=True)
-    accessibility_public = models.BooleanField()
-    collaboration_allowed = models.BooleanField()
-    tags = models.ManyToManyField(Tag)
-    cover = models.IntegerField()
+class Annotation(Model):
+    creator = models.ForeignKey(settings.AUTH_USER_MODEL,
+                                related_name='yarn',
+                                null=True,
+                               on_delete=models.SET_NULL
+                                )
+    creation_date = models.DateTimeField(auto_now_add=True)
+    target = models.ForeignKey(AnnotationTarget, null=True, on_delete=models.SET_NULL, related_name='annotations')
+    tags = models.ManyToManyField(Tag, blank=True)
+    description = models.TextField(null=True)
 
     class Meta(Model.Meta):
         rdf_type = 'hd:annotation'
         #rdf_context = 'https://www.w3.org/ns/anno.jsonld'
-        owner_field = "owners"
-        owner_perms = []
-        authenticated_perms = []
-        anonymous_perms = []
-        permission_classes = [BookletPermissions]
+        authenticated_perms = ['add', 'view']
+        auto_author = 'creator'
+        owner_field = 'creator'
+        owner_perms = ['view', 'delete']
```

### Comparing `djangoldp_needle-0.1.86/djangoldp_needle/models/tag.py` & `djangoldp_needle-0.1.9/djangoldp_needle/models/tag.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from django.conf import settings
 from django.db import models
 from djangoldp.models import Model
 
-from ..permissions import TagPermissions
-
 
 class Tag(Model):
     creator = models.ForeignKey(settings.AUTH_USER_MODEL,
                                 related_name='tags',
                                 null=True,
                                 on_delete=models.SET_NULL
                                 )
     creation_date = models.DateTimeField(auto_now_add=True)
-    name = models.CharField(max_length=64)
+    name = models.CharField(max_length=16)
 
     class Meta(Model.Meta):
         rdf_type = 'hd:tag'
-        authenticated_perms = ['add', 'view']
+        authenticated_perms = ['add']
         owner_field = 'creator'
         owner_perms = ['view']
-        permission_classes = [TagPermissions]
```

### Comparing `djangoldp_needle-0.1.86/setup.cfg` & `djangoldp_needle-0.1.9/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -5,24 +5,22 @@
 long_description = file: README.md
 license = MIT
 classifiers = 
 	Programming Language :: Python :: 3
 
 [options]
 packages = find:
+include_package_data = True
 install_requires = 
 	djangoldp>=1.0
 	djangoldp_account
 	beautifulsoup4
 	requests
-	selenium==3.14.1
-	webdriver-manager
 
 [options.extras_require]
-include_package_data = True
 dev = 
 	requests-mock
 
 [semantic_release]
 version_source = tag
 version_variable = djangoldp_needle/__init__.py:__version__
 commit_parser = commit_parser.parse
```

