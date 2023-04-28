# Comparing `tmp/instawow-2.2.0.tar.gz` & `tmp/instawow-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instawow-2.2.0.tar", max compression
+gzip compressed data, was "instawow-2.3.0.tar", max compression
```

## Comparing `instawow-2.2.0.tar` & `instawow-2.3.0.tar`

### file list

```diff
@@ -1,121 +1,121 @@
--rw-r--r--   0        0        0    35147 2019-12-02 23:23:41.000000 instawow-2.2.0/COPYING
--rw-r--r--   0        0        0     7232 2022-09-11 11:09:45.272521 instawow-2.2.0/README.rst
--rw-r--r--   0        0        0        0 2021-09-26 23:03:02.610144 instawow-2.2.0/gui-webview/src/instawow_gui/__init__.py
--rw-r--r--   0        0        0     4374 2023-04-15 10:43:33.025204 instawow-2.2.0/gui-webview/src/instawow_gui/app.py
--rw-r--r--   0        0        0       27 2021-06-12 09:49:57.192616 instawow-2.2.0/gui-webview/src/instawow_gui/frontend/.gitignore
--rw-r--r--   0        0        0        0 2021-06-12 09:49:57.192724 instawow-2.2.0/gui-webview/src/instawow_gui/frontend/__init__.py
--rw-r--r--   0        0        0      415 2023-04-22 10:09:21.216534 instawow-2.2.0/gui-webview/src/instawow_gui/frontend/index.html
--rw-r--r--   0        0        0    19643 2023-04-22 10:09:31.184620 instawow-2.2.0/gui-webview/src/instawow_gui/frontend/svelte-bundle.css
--rw-r--r--   0        0        0   494619 2023-04-22 10:09:31.185238 instawow-2.2.0/gui-webview/src/instawow_gui/frontend/svelte-bundle.js
--rw-r--r--   0        0        0    27256 2023-04-19 21:34:51.388261 instawow-2.2.0/gui-webview/src/instawow_gui/json_rpc_server.py
--rw-r--r--   0        0        0        0 2021-09-18 16:01:49.335972 instawow-2.2.0/gui-webview/src/instawow_gui/py.typed
--rw-r--r--   0        0        0        0 2021-06-12 09:49:57.193550 instawow-2.2.0/gui-webview/src/instawow_gui/resources/__init__.py
--rw-r--r--   0        0        0   133998 2021-06-12 09:49:57.194686 instawow-2.2.0/gui-webview/src/instawow_gui/resources/instawow_gui.icns
--rw-r--r--   0        0        0     8736 2021-06-12 09:49:57.195656 instawow-2.2.0/gui-webview/src/instawow_gui/resources/instawow_gui.ico
--rw-r--r--   0        0        0    60410 2021-06-12 09:49:57.197567 instawow-2.2.0/gui-webview/src/instawow_gui/resources/instawow_gui.png
--rw-r--r--   0        0        0     3775 2023-04-22 10:10:13.919108 instawow-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      213 2023-04-13 13:01:04.746899 instawow-2.2.0/src/instawow/__init__.py
--rw-r--r--   0        0        0      480 2023-02-10 14:46:48.188526 instawow-2.2.0/src/instawow/__main__.py
--rw-r--r--   0        0        0     2775 2022-12-15 05:55:39.666760 instawow-2.2.0/src/instawow/_addon_hashing.py
--rw-r--r--   0        0        0     9904 2023-04-19 15:05:25.729293 instawow-2.2.0/src/instawow/_cli_prompts.py
--rw-r--r--   0        0        0     7760 2023-02-01 10:07:51.063301 instawow-2.2.0/src/instawow/_custom_slpp.py
--rw-r--r--   0        0        0     3427 2023-04-16 14:08:11.800604 instawow-2.2.0/src/instawow/_http_cache_db.py
--rw-r--r--   0        0        0      842 2023-04-17 17:43:24.869397 instawow-2.2.0/src/instawow/_import_wrapper.py
--rw-r--r--   0        0        0        0 2021-06-12 09:49:57.208218 instawow-2.2.0/src/instawow/_migrations/__init__.py
--rw-r--r--   0        0        0     1623 2021-06-12 09:49:57.208876 instawow-2.2.0/src/instawow/_migrations/alembic.ini
--rw-r--r--   0        0        0     1261 2023-02-10 14:46:48.159866 instawow-2.2.0/src/instawow/_migrations/env.py
--rw-r--r--   0        0        0      494 2021-06-12 09:49:57.209309 instawow-2.2.0/src/instawow/_migrations/script.py.mako
--rw-r--r--   0        0        0      567 2023-02-10 14:46:48.144898 instawow-2.2.0/src/instawow/_migrations/versions/2bfcfe824fe0_remove_pkgoptions_strategy_constraint.py
--rw-r--r--   0        0        0      615 2023-02-10 14:46:48.148613 instawow-2.2.0/src/instawow/_migrations/versions/3b37d2faccd2_add_missing_unique_constraint.py
--rw-r--r--   0        0        0      771 2023-02-10 14:46:48.142255 instawow-2.2.0/src/instawow/_migrations/versions/43aa3610e92a_populate_version_table_from_installed_pkgs.py
--rw-r--r--   0        0        0     1330 2023-02-10 14:46:48.148806 instawow-2.2.0/src/instawow/_migrations/versions/58a8306c3a5b_make_basenames.py
--rw-r--r--   0        0        0      752 2023-02-10 14:46:48.137514 instawow-2.2.0/src/instawow/_migrations/versions/7204944522b1_add_dependency_table.py
--rw-r--r--   0        0        0      769 2023-02-10 14:46:48.139872 instawow-2.2.0/src/instawow/_migrations/versions/75f69831f74f_replace_curse_strategies.py
--rw-r--r--   0        0        0      858 2023-02-10 14:46:48.133648 instawow-2.2.0/src/instawow/_migrations/versions/764fa963cc71_add_changelog_column.py
--rw-r--r--   0        0        0     3242 2023-02-10 14:46:48.157600 instawow-2.2.0/src/instawow/_migrations/versions/8f6ba74cfa82_rename_origin_column.py
--rw-r--r--   0        0        0     2601 2023-02-10 14:46:48.153141 instawow-2.2.0/src/instawow/_migrations/versions/98716a7301f8_renovate_pkg_options.py
--rw-r--r--   0        0        0      814 2023-02-10 14:46:48.145012 instawow-2.2.0/src/instawow/_migrations/versions/9b8df9661cdb_add_pkg_version_log_fk.py
--rw-r--r--   0        0        0        0 2021-06-12 09:49:57.211018 instawow-2.2.0/src/instawow/_migrations/versions/__init__.py
--rw-r--r--   0        0        0      784 2023-02-10 14:46:48.139232 instawow-2.2.0/src/instawow/_migrations/versions/d3f542de5ff4_add_version_log_table.py
--rw-r--r--   0        0        0     3847 2023-02-10 14:46:48.143020 instawow-2.2.0/src/instawow/_migrations/versions/e13430219249_add_cascade.py
--rw-r--r--   0        0        0     1266 2023-02-10 14:46:48.135782 instawow-2.2.0/src/instawow/_migrations/versions/e4921edb1154_replace_uq_with_pk_constraint.py
--rw-r--r--   0        0        0     1231 2023-02-10 14:46:48.147304 instawow-2.2.0/src/instawow/_migrations/versions/e4ae835a34be_change_pkg_options_strategy_checks.py
--rw-r--r--   0        0        0      556 2023-02-10 14:46:48.146303 instawow-2.2.0/src/instawow/_migrations/versions/f3f9957de30c_drop_file_id.py
--rw-r--r--   0        0        0        0 2022-08-14 14:15:56.303799 instawow-2.2.0/src/instawow/_sources/__init__.py
--rw-r--r--   0        0        0    14338 2023-04-10 23:13:29.001702 instawow-2.2.0/src/instawow/_sources/cfcore.py
--rw-r--r--   0        0        0    16388 2023-04-19 22:34:59.730527 instawow-2.2.0/src/instawow/_sources/github.py
--rw-r--r--   0        0        0     2335 2023-04-10 23:13:27.566255 instawow-2.2.0/src/instawow/_sources/instawow.py
--rw-r--r--   0        0        0     7782 2023-04-10 23:13:28.412152 instawow-2.2.0/src/instawow/_sources/tukui.py
--rw-r--r--   0        0        0     6824 2022-12-18 21:54:41.548677 instawow-2.2.0/src/instawow/_sources/wago.py
--rw-r--r--   0        0        0     8708 2023-04-10 23:13:28.429759 instawow-2.2.0/src/instawow/_sources/wowi.py
--rw-r--r--   0        0        0     1317 2023-04-22 10:10:13.924559 instawow-2.2.0/src/instawow/_version.py
--rw-r--r--   0        0        0      120 2022-12-15 17:34:52.403485 instawow-2.2.0/src/instawow/_wa_templates/CHANGELOG.md
--rw-r--r--   0        0        0    18046 2021-06-12 09:49:57.216042 instawow-2.2.0/src/instawow/_wa_templates/COPYING.WeakAuras-Companion
--rw-r--r--   0        0        0      223 2021-12-05 22:28:54.088794 instawow-2.2.0/src/instawow/_wa_templates/README
--rw-r--r--   0        0        0      360 2022-12-15 06:04:29.919814 instawow-2.2.0/src/instawow/_wa_templates/WeakAurasCompanion.toc
--rw-r--r--   0        0        0        0 2021-06-12 09:49:57.216549 instawow-2.2.0/src/instawow/_wa_templates/__init__.py
--rw-r--r--   0        0        0      418 2022-12-15 06:04:29.919169 instawow-2.2.0/src/instawow/_wa_templates/data.lua
--rw-r--r--   0        0        0     1059 2023-04-22 08:30:05.257712 instawow-2.2.0/src/instawow/_wa_templates/init.lua
--rw-r--r--   0        0        0     3733 2023-04-17 22:51:34.488709 instawow-2.2.0/src/instawow/cataloguer.py
--rw-r--r--   0        0        0    41753 2023-04-19 22:32:19.925511 instawow-2.2.0/src/instawow/cli.py
--rw-r--r--   0        0        0     3702 2023-04-09 11:42:24.821116 instawow-2.2.0/src/instawow/common.py
--rw-r--r--   0        0        0    12195 2023-04-19 22:39:20.139646 instawow-2.2.0/src/instawow/config.py
--rw-r--r--   0        0        0     4949 2023-04-17 22:42:46.703539 instawow-2.2.0/src/instawow/db.py
--rw-r--r--   0        0        0     1657 2023-04-10 23:11:08.500874 instawow-2.2.0/src/instawow/github_auth.py
--rw-r--r--   0        0        0     3166 2023-04-10 23:13:28.902227 instawow-2.2.0/src/instawow/http.py
--rw-r--r--   0        0        0    28602 2023-04-19 22:54:57.977209 instawow-2.2.0/src/instawow/manager.py
--rw-r--r--   0        0        0     6900 2023-04-14 00:50:10.921100 instawow-2.2.0/src/instawow/matchers.py
--rw-r--r--   0        0        0     3826 2023-04-17 22:43:42.642098 instawow-2.2.0/src/instawow/models.py
--rw-r--r--   0        0        0     1194 2023-04-17 17:43:06.947727 instawow-2.2.0/src/instawow/plugins.py
--rw-r--r--   0        0        0        0 2021-09-18 22:38:54.214209 instawow-2.2.0/src/instawow/py.typed
--rw-r--r--   0        0        0     5355 2023-04-19 23:13:42.409688 instawow-2.2.0/src/instawow/resolvers.py
--rw-r--r--   0        0        0     4016 2023-01-14 09:18:02.366070 instawow-2.2.0/src/instawow/results.py
--rw-r--r--   0        0        0     8994 2023-04-19 22:44:32.270341 instawow-2.2.0/src/instawow/utils.py
--rw-r--r--   0        0        0    12526 2023-04-22 09:14:01.757277 instawow-2.2.0/src/instawow/wa_updater.py
--rw-r--r--   0        0        0        0 2022-10-01 14:46:03.853827 instawow-2.2.0/tests/__init__.py
--rw-r--r--   0        0        0     3895 2023-04-15 10:35:01.565813 instawow-2.2.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2019-09-13 12:49:54.000000 instawow-2.2.0/tests/fixtures/FakeAddon/FakeAddon.lua
--rw-r--r--   0        0        0      116 2019-09-13 12:49:54.000000 instawow-2.2.0/tests/fixtures/FakeAddon/FakeAddon.toc
--rw-r--r--   0        0        0     8799 2022-12-15 05:52:01.534031 instawow-2.2.0/tests/fixtures/http/__init__.py
--rw-r--r--   0        0        0  4816882 2022-08-31 22:25:56.442109 instawow-2.2.0/tests/fixtures/http/base-catalogue-v7.compact.json
--rw-r--r--   0        0        0   210360 2022-08-31 20:23:48.857256 instawow-2.2.0/tests/fixtures/http/curse-addon--all.json
--rw-r--r--   0        0        0      113 2022-08-31 20:23:50.334581 instawow-2.2.0/tests/fixtures/http/curse-addon-changelog.json
--rw-r--r--   0        0        0    71851 2022-08-31 20:23:49.676910 instawow-2.2.0/tests/fixtures/http/curse-addon-files.json
--rw-r--r--   0        0        0      115 2022-08-31 20:24:16.713339 instawow-2.2.0/tests/fixtures/http/github-oauth-login-access-token.json
--rw-r--r--   0        0        0      187 2022-08-31 20:24:16.643118 instawow-2.2.0/tests/fixtures/http/github-oauth-login-device-code.json
--rw-r--r--   0        0        0      376 2022-08-31 20:24:09.661693 instawow-2.2.0/tests/fixtures/http/github-release-molinari-release-json.json
--rw-r--r--   0        0        0     6036 2022-08-31 20:24:08.368219 instawow-2.2.0/tests/fixtures/http/github-release-molinari.json
--rw-r--r--   0        0        0     1895 2022-08-31 20:24:14.230192 instawow-2.2.0/tests/fixtures/http/github-release-no-assets.json
--rw-r--r--   0        0        0     8518 2022-08-31 20:24:11.947838 instawow-2.2.0/tests/fixtures/http/github-release-no-release-json.json
--rw-r--r--   0        0        0      398 2022-08-31 20:24:06.271014 instawow-2.2.0/tests/fixtures/http/github-release-release-json-release-json.json
--rw-r--r--   0        0        0     8128 2022-08-31 20:24:04.451313 instawow-2.2.0/tests/fixtures/http/github-release-release-json.json
--rw-r--r--   0        0        0     6715 2022-08-31 20:24:07.258377 instawow-2.2.0/tests/fixtures/http/github-repo-molinari.json
--rw-r--r--   0        0        0     6813 2022-08-31 20:24:10.657644 instawow-2.2.0/tests/fixtures/http/github-repo-no-release-json.json
--rw-r--r--   0        0        0     6740 2022-08-31 20:24:13.112037 instawow-2.2.0/tests/fixtures/http/github-repo-no-releases.json
--rw-r--r--   0        0        0     5508 2022-08-31 20:24:02.620371 instawow-2.2.0/tests/fixtures/http/github-repo-release-json.json
--rwxr-xr-x   0        0        0     4643 2022-10-04 08:31:31.924694 instawow-2.2.0/tests/fixtures/http/regen.sh
--rw-r--r--   0        0        0      742 2022-09-12 20:30:46.898294 instawow-2.2.0/tests/fixtures/http/tukui-classic-addons.json
--rw-r--r--   0        0        0      754 2022-09-12 20:30:49.198297 instawow-2.2.0/tests/fixtures/http/tukui-classic-wotlk-addons.json
--rw-r--r--   0        0        0      738 2022-09-12 20:30:45.511712 instawow-2.2.0/tests/fixtures/http/tukui-retail-addons.json
--rw-r--r--   0        0        0      790 2022-09-12 20:30:43.625964 instawow-2.2.0/tests/fixtures/http/tukui-ui--elvui.json
--rw-r--r--   0        0        0      716 2022-09-12 20:30:41.827769 instawow-2.2.0/tests/fixtures/http/tukui-ui--tukui.json
--rw-r--r--   0        0        0      938 2022-10-04 08:31:13.687772 instawow-2.2.0/tests/fixtures/http/wago-match-addons.json
--rw-r--r--   0        0        0     2126 2022-08-31 20:23:52.860250 instawow-2.2.0/tests/fixtures/http/wowi-filedetails.json
--rw-r--r--   0        0        0      924 2022-08-31 20:23:51.724107 instawow-2.2.0/tests/fixtures/http/wowi-filelist.json
--rw-r--r--   0        0        0     1326 2023-02-10 14:46:48.151173 instawow-2.2.0/tests/plugin/instawow_test_plugin.py
--rw-r--r--   0        0        0       92 2022-06-02 10:31:06.427153 instawow-2.2.0/tests/plugin/pyproject.toml
--rw-r--r--   0        0        0      237 2023-02-10 14:46:48.152376 instawow-2.2.0/tests/plugin/setup.py
--rw-r--r--   0        0        0     5553 2023-04-22 09:14:58.522978 instawow-2.2.0/tests/test__slpp.py
--rw-r--r--   0        0        0     9802 2023-01-14 09:18:02.341111 instawow-2.2.0/tests/test__sources.py
--rw-r--r--   0        0        0     3124 2023-04-13 13:04:19.565989 instawow-2.2.0/tests/test__version.py
--rw-r--r--   0        0        0    17242 2023-04-18 22:28:54.194396 instawow-2.2.0/tests/test_cli.py
--rw-r--r--   0        0        0     2192 2022-12-15 05:55:39.677042 instawow-2.2.0/tests/test_common.py
--rw-r--r--   0        0        0     3676 2022-12-15 05:52:01.537348 instawow-2.2.0/tests/test_config.py
--rw-r--r--   0        0        0      422 2022-12-15 05:44:18.270434 instawow-2.2.0/tests/test_github_oauth_flow.py
--rw-r--r--   0        0        0     3134 2023-01-04 01:40:34.984676 instawow-2.2.0/tests/test_github_zip_parsing.py
--rw-r--r--   0        0        0     4404 2023-01-04 01:39:11.965442 instawow-2.2.0/tests/test_json_rpc_api.py
--rw-r--r--   0        0        0    10677 2023-04-15 10:24:48.644729 instawow-2.2.0/tests/test_manager.py
--rw-r--r--   0        0        0     3813 2023-01-04 01:37:47.785586 instawow-2.2.0/tests/test_matchers.py
--rw-r--r--   0        0        0     4491 2023-01-04 01:37:53.376282 instawow-2.2.0/tests/test_utils.py
--rw-r--r--   0        0        0     3483 2023-04-10 10:46:56.823221 instawow-2.2.0/tests/test_wa_updater.py
--rw-r--r--   0        0        0     8980 1970-01-01 00:00:00.000000 instawow-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35147 2019-12-02 23:23:41.000000 instawow-2.3.0/COPYING
+-rw-r--r--   0        0        0     7232 2022-09-11 11:09:45.272521 instawow-2.3.0/README.rst
+-rw-r--r--   0        0        0        0 2021-09-26 23:03:02.610144 instawow-2.3.0/gui-webview/src/instawow_gui/__init__.py
+-rw-r--r--   0        0        0     4374 2023-04-15 10:43:33.025204 instawow-2.3.0/gui-webview/src/instawow_gui/app.py
+-rw-r--r--   0        0        0       27 2021-06-12 09:49:57.192616 instawow-2.3.0/gui-webview/src/instawow_gui/frontend/.gitignore
+-rw-r--r--   0        0        0        0 2021-06-12 09:49:57.192724 instawow-2.3.0/gui-webview/src/instawow_gui/frontend/__init__.py
+-rw-r--r--   0        0        0      415 2023-04-28 13:11:02.176641 instawow-2.3.0/gui-webview/src/instawow_gui/frontend/index.html
+-rw-r--r--   0        0        0    19643 2023-04-28 13:11:10.163467 instawow-2.3.0/gui-webview/src/instawow_gui/frontend/svelte-bundle.css
+-rw-r--r--   0        0        0   494633 2023-04-28 13:11:10.162925 instawow-2.3.0/gui-webview/src/instawow_gui/frontend/svelte-bundle.js
+-rw-r--r--   0        0        0    27256 2023-04-19 21:34:51.388261 instawow-2.3.0/gui-webview/src/instawow_gui/json_rpc_server.py
+-rw-r--r--   0        0        0        0 2021-09-18 16:01:49.335972 instawow-2.3.0/gui-webview/src/instawow_gui/py.typed
+-rw-r--r--   0        0        0        0 2021-06-12 09:49:57.193550 instawow-2.3.0/gui-webview/src/instawow_gui/resources/__init__.py
+-rw-r--r--   0        0        0   133998 2021-06-12 09:49:57.194686 instawow-2.3.0/gui-webview/src/instawow_gui/resources/instawow_gui.icns
+-rw-r--r--   0        0        0     8736 2021-06-12 09:49:57.195656 instawow-2.3.0/gui-webview/src/instawow_gui/resources/instawow_gui.ico
+-rw-r--r--   0        0        0    60410 2021-06-12 09:49:57.197567 instawow-2.3.0/gui-webview/src/instawow_gui/resources/instawow_gui.png
+-rw-r--r--   0        0        0     3775 2023-04-28 13:11:36.067733 instawow-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      213 2023-04-13 13:01:04.746899 instawow-2.3.0/src/instawow/__init__.py
+-rw-r--r--   0        0        0      480 2023-02-10 14:46:48.188526 instawow-2.3.0/src/instawow/__main__.py
+-rw-r--r--   0        0        0     2775 2022-12-15 05:55:39.666760 instawow-2.3.0/src/instawow/_addon_hashing.py
+-rw-r--r--   0        0        0     9904 2023-04-19 15:05:25.729293 instawow-2.3.0/src/instawow/_cli_prompts.py
+-rw-r--r--   0        0        0     7760 2023-02-01 10:07:51.063301 instawow-2.3.0/src/instawow/_custom_slpp.py
+-rw-r--r--   0        0        0     3427 2023-04-16 14:08:11.800604 instawow-2.3.0/src/instawow/_http_cache_db.py
+-rw-r--r--   0        0        0      842 2023-04-17 17:43:24.869397 instawow-2.3.0/src/instawow/_import_wrapper.py
+-rw-r--r--   0        0        0        0 2021-06-12 09:49:57.208218 instawow-2.3.0/src/instawow/_migrations/__init__.py
+-rw-r--r--   0        0        0     1623 2021-06-12 09:49:57.208876 instawow-2.3.0/src/instawow/_migrations/alembic.ini
+-rw-r--r--   0        0        0     1261 2023-02-10 14:46:48.159866 instawow-2.3.0/src/instawow/_migrations/env.py
+-rw-r--r--   0        0        0      494 2021-06-12 09:49:57.209309 instawow-2.3.0/src/instawow/_migrations/script.py.mako
+-rw-r--r--   0        0        0      567 2023-04-26 09:53:54.276530 instawow-2.3.0/src/instawow/_migrations/versions/2bfcfe824fe0_remove_pkgoptions_strategy_constraint.py
+-rw-r--r--   0        0        0      615 2023-02-10 14:46:48.148613 instawow-2.3.0/src/instawow/_migrations/versions/3b37d2faccd2_add_missing_unique_constraint.py
+-rw-r--r--   0        0        0      771 2023-02-10 14:46:48.142255 instawow-2.3.0/src/instawow/_migrations/versions/43aa3610e92a_populate_version_table_from_installed_pkgs.py
+-rw-r--r--   0        0        0     1330 2023-02-10 14:46:48.148806 instawow-2.3.0/src/instawow/_migrations/versions/58a8306c3a5b_make_basenames.py
+-rw-r--r--   0        0        0      752 2023-02-10 14:46:48.137514 instawow-2.3.0/src/instawow/_migrations/versions/7204944522b1_add_dependency_table.py
+-rw-r--r--   0        0        0      769 2023-02-10 14:46:48.139872 instawow-2.3.0/src/instawow/_migrations/versions/75f69831f74f_replace_curse_strategies.py
+-rw-r--r--   0        0        0      858 2023-02-10 14:46:48.133648 instawow-2.3.0/src/instawow/_migrations/versions/764fa963cc71_add_changelog_column.py
+-rw-r--r--   0        0        0     3242 2023-02-10 14:46:48.157600 instawow-2.3.0/src/instawow/_migrations/versions/8f6ba74cfa82_rename_origin_column.py
+-rw-r--r--   0        0        0     2601 2023-02-10 14:46:48.153141 instawow-2.3.0/src/instawow/_migrations/versions/98716a7301f8_renovate_pkg_options.py
+-rw-r--r--   0        0        0      814 2023-02-10 14:46:48.145012 instawow-2.3.0/src/instawow/_migrations/versions/9b8df9661cdb_add_pkg_version_log_fk.py
+-rw-r--r--   0        0        0        0 2021-06-12 09:49:57.211018 instawow-2.3.0/src/instawow/_migrations/versions/__init__.py
+-rw-r--r--   0        0        0      784 2023-02-10 14:46:48.139232 instawow-2.3.0/src/instawow/_migrations/versions/d3f542de5ff4_add_version_log_table.py
+-rw-r--r--   0        0        0     3847 2023-02-10 14:46:48.143020 instawow-2.3.0/src/instawow/_migrations/versions/e13430219249_add_cascade.py
+-rw-r--r--   0        0        0     1266 2023-02-10 14:46:48.135782 instawow-2.3.0/src/instawow/_migrations/versions/e4921edb1154_replace_uq_with_pk_constraint.py
+-rw-r--r--   0        0        0     1231 2023-02-10 14:46:48.147304 instawow-2.3.0/src/instawow/_migrations/versions/e4ae835a34be_change_pkg_options_strategy_checks.py
+-rw-r--r--   0        0        0      556 2023-02-10 14:46:48.146303 instawow-2.3.0/src/instawow/_migrations/versions/f3f9957de30c_drop_file_id.py
+-rw-r--r--   0        0        0        0 2022-08-14 14:15:56.303799 instawow-2.3.0/src/instawow/_sources/__init__.py
+-rw-r--r--   0        0        0    14338 2023-04-10 23:13:29.001702 instawow-2.3.0/src/instawow/_sources/cfcore.py
+-rw-r--r--   0        0        0    16430 2023-04-28 10:06:44.626478 instawow-2.3.0/src/instawow/_sources/github.py
+-rw-r--r--   0        0        0     2335 2023-04-10 23:13:27.566255 instawow-2.3.0/src/instawow/_sources/instawow.py
+-rw-r--r--   0        0        0     7782 2023-04-10 23:13:28.412152 instawow-2.3.0/src/instawow/_sources/tukui.py
+-rw-r--r--   0        0        0     6824 2022-12-18 21:54:41.548677 instawow-2.3.0/src/instawow/_sources/wago.py
+-rw-r--r--   0        0        0     8708 2023-04-10 23:13:28.429759 instawow-2.3.0/src/instawow/_sources/wowi.py
+-rw-r--r--   0        0        0     1317 2023-04-28 13:11:36.069812 instawow-2.3.0/src/instawow/_version.py
+-rw-r--r--   0        0        0      120 2022-12-15 17:34:52.403485 instawow-2.3.0/src/instawow/_wa_templates/CHANGELOG.md
+-rw-r--r--   0        0        0    18046 2021-06-12 09:49:57.216042 instawow-2.3.0/src/instawow/_wa_templates/COPYING.WeakAuras-Companion
+-rw-r--r--   0        0        0      223 2021-12-05 22:28:54.088794 instawow-2.3.0/src/instawow/_wa_templates/README
+-rw-r--r--   0        0        0      360 2022-12-15 06:04:29.919814 instawow-2.3.0/src/instawow/_wa_templates/WeakAurasCompanion.toc
+-rw-r--r--   0        0        0        0 2021-06-12 09:49:57.216549 instawow-2.3.0/src/instawow/_wa_templates/__init__.py
+-rw-r--r--   0        0        0      418 2022-12-15 06:04:29.919169 instawow-2.3.0/src/instawow/_wa_templates/data.lua
+-rw-r--r--   0        0        0     1059 2023-04-22 08:30:05.257712 instawow-2.3.0/src/instawow/_wa_templates/init.lua
+-rw-r--r--   0        0        0     3733 2023-04-17 22:51:34.488709 instawow-2.3.0/src/instawow/cataloguer.py
+-rw-r--r--   0        0        0    41889 2023-04-28 11:05:44.360754 instawow-2.3.0/src/instawow/cli.py
+-rw-r--r--   0        0        0     3702 2023-04-09 11:42:24.821116 instawow-2.3.0/src/instawow/common.py
+-rw-r--r--   0        0        0    12195 2023-04-19 22:39:20.139646 instawow-2.3.0/src/instawow/config.py
+-rw-r--r--   0        0        0     4949 2023-04-28 10:55:47.175112 instawow-2.3.0/src/instawow/db.py
+-rw-r--r--   0        0        0     1657 2023-04-10 23:11:08.500874 instawow-2.3.0/src/instawow/github_auth.py
+-rw-r--r--   0        0        0     3166 2023-04-10 23:13:28.902227 instawow-2.3.0/src/instawow/http.py
+-rw-r--r--   0        0        0    28694 2023-04-28 11:33:33.840087 instawow-2.3.0/src/instawow/manager.py
+-rw-r--r--   0        0        0     6900 2023-04-14 00:50:10.921100 instawow-2.3.0/src/instawow/matchers.py
+-rw-r--r--   0        0        0     3769 2023-04-28 10:12:09.936604 instawow-2.3.0/src/instawow/models.py
+-rw-r--r--   0        0        0     1194 2023-04-17 17:43:06.947727 instawow-2.3.0/src/instawow/plugins.py
+-rw-r--r--   0        0        0        0 2021-09-18 22:38:54.214209 instawow-2.3.0/src/instawow/py.typed
+-rw-r--r--   0        0        0     5355 2023-04-19 23:13:42.409688 instawow-2.3.0/src/instawow/resolvers.py
+-rw-r--r--   0        0        0     4156 2023-04-28 11:21:49.123394 instawow-2.3.0/src/instawow/results.py
+-rw-r--r--   0        0        0     8994 2023-04-28 11:33:33.841850 instawow-2.3.0/src/instawow/utils.py
+-rw-r--r--   0        0        0    12526 2023-04-22 09:14:01.757277 instawow-2.3.0/src/instawow/wa_updater.py
+-rw-r--r--   0        0        0        0 2022-10-01 14:46:03.853827 instawow-2.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     3895 2023-04-15 10:35:01.565813 instawow-2.3.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2019-09-13 12:49:54.000000 instawow-2.3.0/tests/fixtures/FakeAddon/FakeAddon.lua
+-rw-r--r--   0        0        0      116 2019-09-13 12:49:54.000000 instawow-2.3.0/tests/fixtures/FakeAddon/FakeAddon.toc
+-rw-r--r--   0        0        0     8799 2022-12-15 05:52:01.534031 instawow-2.3.0/tests/fixtures/http/__init__.py
+-rw-r--r--   0        0        0  4816882 2022-08-31 22:25:56.442109 instawow-2.3.0/tests/fixtures/http/base-catalogue-v7.compact.json
+-rw-r--r--   0        0        0   210360 2022-08-31 20:23:48.857256 instawow-2.3.0/tests/fixtures/http/curse-addon--all.json
+-rw-r--r--   0        0        0      113 2022-08-31 20:23:50.334581 instawow-2.3.0/tests/fixtures/http/curse-addon-changelog.json
+-rw-r--r--   0        0        0    71851 2022-08-31 20:23:49.676910 instawow-2.3.0/tests/fixtures/http/curse-addon-files.json
+-rw-r--r--   0        0        0      115 2022-08-31 20:24:16.713339 instawow-2.3.0/tests/fixtures/http/github-oauth-login-access-token.json
+-rw-r--r--   0        0        0      187 2022-08-31 20:24:16.643118 instawow-2.3.0/tests/fixtures/http/github-oauth-login-device-code.json
+-rw-r--r--   0        0        0      376 2022-08-31 20:24:09.661693 instawow-2.3.0/tests/fixtures/http/github-release-molinari-release-json.json
+-rw-r--r--   0        0        0     6036 2022-08-31 20:24:08.368219 instawow-2.3.0/tests/fixtures/http/github-release-molinari.json
+-rw-r--r--   0        0        0     1895 2022-08-31 20:24:14.230192 instawow-2.3.0/tests/fixtures/http/github-release-no-assets.json
+-rw-r--r--   0        0        0     8518 2022-08-31 20:24:11.947838 instawow-2.3.0/tests/fixtures/http/github-release-no-release-json.json
+-rw-r--r--   0        0        0      398 2022-08-31 20:24:06.271014 instawow-2.3.0/tests/fixtures/http/github-release-release-json-release-json.json
+-rw-r--r--   0        0        0     8128 2022-08-31 20:24:04.451313 instawow-2.3.0/tests/fixtures/http/github-release-release-json.json
+-rw-r--r--   0        0        0     6715 2022-08-31 20:24:07.258377 instawow-2.3.0/tests/fixtures/http/github-repo-molinari.json
+-rw-r--r--   0        0        0     6813 2022-08-31 20:24:10.657644 instawow-2.3.0/tests/fixtures/http/github-repo-no-release-json.json
+-rw-r--r--   0        0        0     6740 2022-08-31 20:24:13.112037 instawow-2.3.0/tests/fixtures/http/github-repo-no-releases.json
+-rw-r--r--   0        0        0     5508 2022-08-31 20:24:02.620371 instawow-2.3.0/tests/fixtures/http/github-repo-release-json.json
+-rwxr-xr-x   0        0        0     4643 2022-10-04 08:31:31.924694 instawow-2.3.0/tests/fixtures/http/regen.sh
+-rw-r--r--   0        0        0      742 2022-09-12 20:30:46.898294 instawow-2.3.0/tests/fixtures/http/tukui-classic-addons.json
+-rw-r--r--   0        0        0      754 2022-09-12 20:30:49.198297 instawow-2.3.0/tests/fixtures/http/tukui-classic-wotlk-addons.json
+-rw-r--r--   0        0        0      738 2022-09-12 20:30:45.511712 instawow-2.3.0/tests/fixtures/http/tukui-retail-addons.json
+-rw-r--r--   0        0        0      790 2022-09-12 20:30:43.625964 instawow-2.3.0/tests/fixtures/http/tukui-ui--elvui.json
+-rw-r--r--   0        0        0      716 2022-09-12 20:30:41.827769 instawow-2.3.0/tests/fixtures/http/tukui-ui--tukui.json
+-rw-r--r--   0        0        0      938 2022-10-04 08:31:13.687772 instawow-2.3.0/tests/fixtures/http/wago-match-addons.json
+-rw-r--r--   0        0        0     2126 2022-08-31 20:23:52.860250 instawow-2.3.0/tests/fixtures/http/wowi-filedetails.json
+-rw-r--r--   0        0        0      924 2022-08-31 20:23:51.724107 instawow-2.3.0/tests/fixtures/http/wowi-filelist.json
+-rw-r--r--   0        0        0     1326 2023-02-10 14:46:48.151173 instawow-2.3.0/tests/plugin/instawow_test_plugin.py
+-rw-r--r--   0        0        0       92 2022-06-02 10:31:06.427153 instawow-2.3.0/tests/plugin/pyproject.toml
+-rw-r--r--   0        0        0      237 2023-02-10 14:46:48.152376 instawow-2.3.0/tests/plugin/setup.py
+-rw-r--r--   0        0        0     5553 2023-04-22 09:14:58.522978 instawow-2.3.0/tests/test__slpp.py
+-rw-r--r--   0        0        0     9802 2023-01-14 09:18:02.341111 instawow-2.3.0/tests/test__sources.py
+-rw-r--r--   0        0        0     3124 2023-04-13 13:04:19.565989 instawow-2.3.0/tests/test__version.py
+-rw-r--r--   0        0        0    17242 2023-04-18 22:28:54.194396 instawow-2.3.0/tests/test_cli.py
+-rw-r--r--   0        0        0     2192 2022-12-15 05:55:39.677042 instawow-2.3.0/tests/test_common.py
+-rw-r--r--   0        0        0     3676 2022-12-15 05:52:01.537348 instawow-2.3.0/tests/test_config.py
+-rw-r--r--   0        0        0      422 2022-12-15 05:44:18.270434 instawow-2.3.0/tests/test_github_oauth_flow.py
+-rw-r--r--   0        0        0     3134 2023-01-04 01:40:34.984676 instawow-2.3.0/tests/test_github_zip_parsing.py
+-rw-r--r--   0        0        0     4404 2023-01-04 01:39:11.965442 instawow-2.3.0/tests/test_json_rpc_api.py
+-rw-r--r--   0        0        0    11675 2023-04-28 10:32:37.028087 instawow-2.3.0/tests/test_manager.py
+-rw-r--r--   0        0        0     3813 2023-01-04 01:37:47.785586 instawow-2.3.0/tests/test_matchers.py
+-rw-r--r--   0        0        0     4491 2023-01-04 01:37:53.376282 instawow-2.3.0/tests/test_utils.py
+-rw-r--r--   0        0        0     3483 2023-04-10 10:46:56.823221 instawow-2.3.0/tests/test_wa_updater.py
+-rw-r--r--   0        0        0     8980 1970-01-01 00:00:00.000000 instawow-2.3.0/PKG-INFO
```

### Comparing `instawow-2.2.0/COPYING` & `instawow-2.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/README.rst` & `instawow-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/gui-webview/src/instawow_gui/app.py` & `instawow-2.3.0/gui-webview/src/instawow_gui/app.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/gui-webview/src/instawow_gui/frontend/svelte-bundle.css` & `instawow-2.3.0/gui-webview/src/instawow_gui/frontend/svelte-bundle.css`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/gui-webview/src/instawow_gui/frontend/svelte-bundle.js` & `instawow-2.3.0/gui-webview/src/instawow_gui/frontend/svelte-bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2787,15 +2787,16 @@
                     message: t
                 }
             })
         }
     }
     const Br = e => ({
         source: e.source,
-        alias: e.id,
+        alias: e.slug,
+        id: e.id,
         strategies: Object.fromEntries(Object.entries(e.options).map((([t, r]) => [t, r ? t === Ir.version_eq && r ? e.version : r : null])))
     });
     var Ur = {},
         Vr = {};
     ! function(e) {
         var t = nt && nt.__awaiter || function(e, t, r, n) {
                 return new(r || (r = Promise))((function(i, o) {
@@ -19413,25 +19414,25 @@
                 e && O(t)
             }
         }
     }
 
     function ad(e) {
         let t, r, n, i, o, s, a = e[0].source + "",
-            l = e[0].id + "",
+            l = e[0].slug + "",
             u = e[4] === of.Expanded && ld(e);
         return {
             c() {
                 t = S("li"), r = C(a), n = C(":"), i = C(l), o = L(), u && u.c(), s = N(), F(t, "class", "defn svelte-n5lp8")
             },
             m(e, a) {
                 A(e, t, a), q(t, r), q(t, n), q(t, i), A(e, o, a), u && u.m(e, a), A(e, s, a)
             },
             p(e, t) {
-                1 & t && a !== (a = e[0].source + "") && B(r, a), 1 & t && l !== (l = e[0].id + "") && B(i, l), e[4] === of.Expanded ? u ? u.p(e, t) : (u = ld(e), u.c(), u.m(s.parentNode, s)) : u && (u.d(1), u = null)
+                1 & t && a !== (a = e[0].source + "") && B(r, a), 1 & t && l !== (l = e[0].slug + "") && B(i, l), e[4] === of.Expanded ? u ? u.p(e, t) : (u = ld(e), u.c(), u.m(s.parentNode, s)) : u && (u.d(1), u = null)
             },
             d(e) {
                 e && O(t), e && O(o), u && u.d(e), e && O(s)
             }
         }
     }
```

### Comparing `instawow-2.2.0/gui-webview/src/instawow_gui/json_rpc_server.py` & `instawow-2.3.0/gui-webview/src/instawow_gui/json_rpc_server.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/gui-webview/src/instawow_gui/resources/instawow_gui.icns` & `instawow-2.3.0/gui-webview/src/instawow_gui/resources/instawow_gui.icns`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/gui-webview/src/instawow_gui/resources/instawow_gui.ico` & `instawow-2.3.0/gui-webview/src/instawow_gui/resources/instawow_gui.ico`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/gui-webview/src/instawow_gui/resources/instawow_gui.png` & `instawow-2.3.0/gui-webview/src/instawow_gui/resources/instawow_gui.png`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/pyproject.toml` & `instawow-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 substitution.files = ["src/instawow/_version.py"]
 
 [tool.poetry]
 name = "instawow"
-version = "2.2.0"
+version = "2.3.0"
 description = "World of Warcraft add-on manager"
 license = "GPL-3.0-or-later"
 authors = [
   "layday <layday@protonmail.com>",
 ]
 readme = "README.rst"
 urls.homepage = "http://github.com/layday/instawow"
```

### Comparing `instawow-2.2.0/src/instawow/_addon_hashing.py` & `instawow-2.3.0/src/instawow/_addon_hashing.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_cli_prompts.py` & `instawow-2.3.0/src/instawow/_cli_prompts.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_custom_slpp.py` & `instawow-2.3.0/src/instawow/_custom_slpp.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_http_cache_db.py` & `instawow-2.3.0/src/instawow/_http_cache_db.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_import_wrapper.py` & `instawow-2.3.0/src/instawow/_import_wrapper.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_migrations/alembic.ini` & `instawow-2.3.0/src/instawow/_migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_migrations/env.py` & `instawow-2.3.0/src/instawow/_migrations/env.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_migrations/versions/2bfcfe824fe0_remove_pkgoptions_strategy_constraint.py` & `instawow-2.3.0/src/instawow/_migrations/versions/2bfcfe824fe0_remove_pkgoptions_strategy_constraint.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_migrations/versions/3b37d2faccd2_add_missing_unique_constraint.py` & `instawow-2.3.0/src/instawow/_migrations/versions/3b37d2faccd2_add_missing_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_migrations/versions/43aa3610e92a_populate_version_table_from_installed_pkgs.py` & `instawow-2.3.0/src/instawow/_migrations/versions/43aa3610e92a_populate_version_table_from_installed_pkgs.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_migrations/versions/58a8306c3a5b_make_basenames.py` & `instawow-2.3.0/src/instawow/_migrations/versions/58a8306c3a5b_make_basenames.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_migrations/versions/7204944522b1_add_dependency_table.py` & `instawow-2.3.0/src/instawow/_migrations/versions/7204944522b1_add_dependency_table.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_migrations/versions/75f69831f74f_replace_curse_strategies.py` & `instawow-2.3.0/src/instawow/_migrations/versions/75f69831f74f_replace_curse_strategies.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_migrations/versions/764fa963cc71_add_changelog_column.py` & `instawow-2.3.0/src/instawow/_migrations/versions/764fa963cc71_add_changelog_column.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_migrations/versions/8f6ba74cfa82_rename_origin_column.py` & `instawow-2.3.0/src/instawow/_migrations/versions/8f6ba74cfa82_rename_origin_column.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_migrations/versions/98716a7301f8_renovate_pkg_options.py` & `instawow-2.3.0/src/instawow/_migrations/versions/98716a7301f8_renovate_pkg_options.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_migrations/versions/9b8df9661cdb_add_pkg_version_log_fk.py` & `instawow-2.3.0/src/instawow/_migrations/versions/9b8df9661cdb_add_pkg_version_log_fk.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_migrations/versions/d3f542de5ff4_add_version_log_table.py` & `instawow-2.3.0/src/instawow/_migrations/versions/d3f542de5ff4_add_version_log_table.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_migrations/versions/e13430219249_add_cascade.py` & `instawow-2.3.0/src/instawow/_migrations/versions/e13430219249_add_cascade.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_migrations/versions/e4921edb1154_replace_uq_with_pk_constraint.py` & `instawow-2.3.0/src/instawow/_migrations/versions/e4921edb1154_replace_uq_with_pk_constraint.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_migrations/versions/e4ae835a34be_change_pkg_options_strategy_checks.py` & `instawow-2.3.0/src/instawow/_migrations/versions/e4ae835a34be_change_pkg_options_strategy_checks.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_migrations/versions/f3f9957de30c_drop_file_id.py` & `instawow-2.3.0/src/instawow/_migrations/versions/f3f9957de30c_drop_file_id.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_sources/cfcore.py` & `instawow-2.3.0/src/instawow/_sources/cfcore.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_sources/github.py` & `instawow-2.3.0/src/instawow/_sources/github.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     find_addon_zip_tocs,
 )
 
 
 # Not exhaustive (as you might've guessed).  Reference:
 # https://docs.github.com/en/rest/reference/repos
 class _GithubRepo(TypedDict):
+    id: int  # Unique, stable repository ID
     name: str  # the repo in user-or-org/repo
     full_name: str  # user-or-org/repo
     description: str | None
     html_url: str
 
 
 class _GithubRelease(TypedDict):
@@ -390,15 +391,15 @@
                 break
 
         else:
             raise R.PkgFilesNotMatching(defn.strategies)
 
         return models.Pkg(
             source=self.metadata.id,
-            id=project['full_name'],
+            id=str(project['id']),
             slug=project['full_name'].lower(),
             name=project['name'],
             description=project['description'] or '',
             url=project['html_url'],
             download_url=matching_asset['url'],
             date_published=iso8601.parse_date(release['published_at']),
             version=release['tag_name'],
```

### Comparing `instawow-2.2.0/src/instawow/_sources/instawow.py` & `instawow-2.3.0/src/instawow/_sources/instawow.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_sources/tukui.py` & `instawow-2.3.0/src/instawow/_sources/tukui.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_sources/wago.py` & `instawow-2.3.0/src/instawow/_sources/wago.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_sources/wowi.py` & `instawow-2.3.0/src/instawow/_sources/wowi.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_version.py` & `instawow-2.3.0/src/instawow/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from datetime import timedelta
 
 from typing_extensions import TypedDict
 
 from . import config
 
-__version__ = '2.2.0'
+__version__ = '2.3.0'
 
 
 class _SimpleApiProject(TypedDict):
     versions: list[str]
 
 
 async def is_outdated(global_config: config.GlobalConfig) -> tuple[bool, str]:
```

### Comparing `instawow-2.2.0/src/instawow/_wa_templates/COPYING.WeakAuras-Companion` & `instawow-2.3.0/src/instawow/_wa_templates/COPYING.WeakAuras-Companion`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/_wa_templates/init.lua` & `instawow-2.3.0/src/instawow/_wa_templates/init.lua`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/cataloguer.py` & `instawow-2.3.0/src/instawow/cataloguer.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/cli.py` & `instawow-2.3.0/src/instawow/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -770,15 +770,18 @@
                 (
                     sa.select(db.pkg).filter(
                         sa.or_(
                             *(
                                 db.pkg.c.slug.contains(d.alias)
                                 if d.source == '*'
                                 else (db.pkg.c.source == d.source)
-                                & ((db.pkg.c.id == d.alias) | (db.pkg.c.slug == d.alias))
+                                & (
+                                    (db.pkg.c.id == d.alias)
+                                    | (sa.func.lower(db.pkg.c.slug) == sa.func.lower(d.alias))
+                                )
                                 for d in addons
                             )
                         )
                     )
                     if addons
                     else sa.select(db.pkg)
                 ).order_by(db.pkg.c.source, sa.func.lower(db.pkg.c.name))
```

### Comparing `instawow-2.2.0/src/instawow/common.py` & `instawow-2.3.0/src/instawow/common.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/config.py` & `instawow-2.3.0/src/instawow/config.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/db.py` & `instawow-2.3.0/src/instawow/db.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/github_auth.py` & `instawow-2.3.0/src/instawow/github_auth.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/http.py` & `instawow-2.3.0/src/instawow/http.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/manager.py` & `instawow-2.3.0/src/instawow/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,30 +295,30 @@
                 connection.execute(
                     sa.select(sa.text('1'))
                     .select_from(db.pkg)
                     .where(
                         db.pkg.c.source == defn.source,
                         (db.pkg.c.id == defn.alias)
                         | (db.pkg.c.id == defn.id)
-                        | (db.pkg.c.slug == defn.alias),
+                        | (sa.func.lower(db.pkg.c.slug) == sa.func.lower(defn.alias)),
                     )
                 ).scalar()
                 == 1
             )
 
     def get_pkg(self, defn: Defn, partial_match: bool = False) -> models.Pkg | None:
         "Retrieve a package from the database."
         with self.database.connect() as connection:
             maybe_row_mapping = (
                 connection.execute(
                     sa.select(db.pkg).where(
                         db.pkg.c.source == defn.source,
                         (db.pkg.c.id == defn.alias)
                         | (db.pkg.c.id == defn.id)
-                        | (db.pkg.c.slug == defn.alias),
+                        | (sa.func.lower(db.pkg.c.slug) == sa.func.lower(defn.alias)),
                     )
                 )
                 .mappings()
                 .one_or_none()
             )
             if maybe_row_mapping is None and partial_match:
                 maybe_row_mapping = (
@@ -685,32 +685,31 @@
         "Install packages from a definition list."
         # We'll weed out installed deps from the results after resolving -
         # doing it this way isn't particularly efficient but avoids having to
         # deal with local state in ``resolve``
         resolve_results = await self.resolve(
             [d for d in defns if not self.check_pkg_exists(d)], with_deps=True
         )
-        pkgs, resolve_errors = bucketise_results(
-            (d, r) for d, r in resolve_results.items() if not self.check_pkg_exists(d)
-        )
+        pkgs, resolve_errors = bucketise_results(resolve_results.items())
+        new_pkgs = {d: p for d, p in pkgs.items() if not self.check_pkg_exists(p.to_defn())}
         archive_paths, download_errors = bucketise_results(
             zip(
-                pkgs,
+                new_pkgs,
                 await gather(
-                    (self._download_pkg_archive(r) for r in pkgs.values()),
+                    (self._download_pkg_archive(r) for r in new_pkgs.values()),
                     capture_manager_exc_async,
                 ),
             )
         )
         results = (
             dict.fromkeys(defns, R.PkgAlreadyInstalled())
             | resolve_errors
             | download_errors
             | {
-                d: await capture_manager_exc_async(self._install_pkg(pkgs[d], a, replace))
+                d: await capture_manager_exc_async(self._install_pkg(new_pkgs[d], a, replace))
                 for d, a in archive_paths.items()
             }
         )
         return results
 
     @_with_lock(_StandardLocks.MutatePkgs)
     async def update(
```

### Comparing `instawow-2.2.0/src/instawow/matchers.py` & `instawow-2.3.0/src/instawow/matchers.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/models.py` & `instawow-2.3.0/src/instawow/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-from collections.abc import Mapping
 from datetime import datetime
 
 import sqlalchemy as sa
 from attrs import asdict, frozen
 from cattrs import Converter
 from typing_extensions import Self
 
@@ -58,17 +57,15 @@
     changelog_url: str
     options: PkgOptions  # pkg_options
     folders: list[PkgFolder] = []  # pkg_folder
     deps: list[PkgDep] = []  # pkg_dep
     logged_versions: list[PkgLoggedVersion] = []  # pkg_version_log
 
     @classmethod
-    def from_row_mapping(
-        cls, connection: sa.Connection, row_mapping: Mapping[str, object]
-    ) -> Self:
+    def from_row_mapping(cls, connection: sa.Connection, row_mapping: sa.RowMapping) -> Self:
         source_and_id = {'pkg_source': row_mapping['source'], 'pkg_id': row_mapping['id']}
         return _db_pkg_converter.structure(
             {
                 **row_mapping,
                 'options': connection.execute(sa.select(db.pkg_options).filter_by(**source_and_id))
                 .mappings()
                 .one(),
```

### Comparing `instawow-2.2.0/src/instawow/plugins.py` & `instawow-2.3.0/src/instawow/plugins.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/resolvers.py` & `instawow-2.3.0/src/instawow/resolvers.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/results.py` & `instawow-2.3.0/src/instawow/results.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,18 @@
     def __init__(self, old_pkg: models.Pkg, new_pkg: models.Pkg) -> None:
         super().__init__()
         self.old_pkg = old_pkg
         self.new_pkg = new_pkg
 
     @property
     def message(self) -> str:
-        return f'updated {self.old_pkg.version} to {self.new_pkg.version}'
+        message = f'updated {self.old_pkg.version} to {self.new_pkg.version}'
+        if self.old_pkg.slug != self.new_pkg.slug:
+            message += f' with new slug {self.new_pkg.slug!r}'
+        return message
 
 
 class PkgRemoved(ManagerResult, _SuccessResult):
     def __init__(self, old_pkg: models.Pkg) -> None:
         super().__init__()
         self.old_pkg = old_pkg
```

### Comparing `instawow-2.2.0/src/instawow/utils.py` & `instawow-2.3.0/src/instawow/utils.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/src/instawow/wa_updater.py` & `instawow-2.3.0/src/instawow/wa_updater.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/conftest.py` & `instawow-2.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/fixtures/http/__init__.py` & `instawow-2.3.0/tests/fixtures/http/__init__.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/fixtures/http/base-catalogue-v7.compact.json` & `instawow-2.3.0/tests/fixtures/http/base-catalogue-v7.compact.json`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/fixtures/http/curse-addon--all.json` & `instawow-2.3.0/tests/fixtures/http/curse-addon--all.json`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/fixtures/http/curse-addon-files.json` & `instawow-2.3.0/tests/fixtures/http/curse-addon-files.json`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/fixtures/http/github-release-molinari.json` & `instawow-2.3.0/tests/fixtures/http/github-release-molinari.json`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/fixtures/http/github-release-no-assets.json` & `instawow-2.3.0/tests/fixtures/http/github-release-no-assets.json`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/fixtures/http/github-release-no-release-json.json` & `instawow-2.3.0/tests/fixtures/http/github-release-no-release-json.json`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/fixtures/http/github-release-release-json.json` & `instawow-2.3.0/tests/fixtures/http/github-release-release-json.json`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/fixtures/http/github-repo-molinari.json` & `instawow-2.3.0/tests/fixtures/http/github-repo-molinari.json`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/fixtures/http/github-repo-no-release-json.json` & `instawow-2.3.0/tests/fixtures/http/github-repo-no-release-json.json`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/fixtures/http/github-repo-no-releases.json` & `instawow-2.3.0/tests/fixtures/http/github-repo-no-releases.json`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/fixtures/http/github-repo-release-json.json` & `instawow-2.3.0/tests/fixtures/http/github-repo-release-json.json`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/fixtures/http/regen.sh` & `instawow-2.3.0/tests/fixtures/http/regen.sh`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/fixtures/http/tukui-classic-addons.json` & `instawow-2.3.0/tests/fixtures/http/tukui-classic-addons.json`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/fixtures/http/tukui-classic-wotlk-addons.json` & `instawow-2.3.0/tests/fixtures/http/tukui-classic-wotlk-addons.json`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/fixtures/http/tukui-retail-addons.json` & `instawow-2.3.0/tests/fixtures/http/tukui-retail-addons.json`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/fixtures/http/tukui-ui--elvui.json` & `instawow-2.3.0/tests/fixtures/http/tukui-ui--elvui.json`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/fixtures/http/tukui-ui--tukui.json` & `instawow-2.3.0/tests/fixtures/http/tukui-ui--tukui.json`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/fixtures/http/wago-match-addons.json` & `instawow-2.3.0/tests/fixtures/http/wago-match-addons.json`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/fixtures/http/wowi-filedetails.json` & `instawow-2.3.0/tests/fixtures/http/wowi-filedetails.json`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/fixtures/http/wowi-filelist.json` & `instawow-2.3.0/tests/fixtures/http/wowi-filelist.json`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/plugin/instawow_test_plugin.py` & `instawow-2.3.0/tests/plugin/instawow_test_plugin.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/test__slpp.py` & `instawow-2.3.0/tests/test__slpp.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/test__sources.py` & `instawow-2.3.0/tests/test__sources.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/test__version.py` & `instawow-2.3.0/tests/test__version.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/test_cli.py` & `instawow-2.3.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/test_common.py` & `instawow-2.3.0/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/test_config.py` & `instawow-2.3.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/test_github_zip_parsing.py` & `instawow-2.3.0/tests/test_github_zip_parsing.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/test_json_rpc_api.py` & `instawow-2.3.0/tests/test_json_rpc_api.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/test_manager.py` & `instawow-2.3.0/tests/test_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import datetime
 from pathlib import Path
 
 import pytest
 from aiohttp import ClientError
+from attrs import evolve
 
 from instawow import results as R
 from instawow.common import Defn, Flavour, Strategy
 from instawow.manager import Manager
 from instawow.models import Pkg
 
 
@@ -136,14 +137,41 @@
     result = await iw_manager.install([wowi_defn], replace=False)
     assert type(result[wowi_defn]) is R.PkgConflictsWithInstalled
 
     result = await iw_manager.install([wowi_defn], replace=True)
     assert type(result[wowi_defn]) is R.PkgConflictsWithInstalled
 
 
+async def test_install_recognises_renamed_pkg_from_id(
+    monkeypatch: pytest.MonkeyPatch, iw_manager: Manager
+):
+    old_defn = Defn('curse', 'molinari')
+    new_defn = Defn('curse', 'molinarifico')
+
+    result = await iw_manager.install([old_defn], replace=False)
+    assert type(result[old_defn]) is R.PkgInstalled
+
+    result = await iw_manager.install([old_defn], replace=False)
+    assert type(result[old_defn]) is R.PkgAlreadyInstalled
+
+    result = await iw_manager.install([new_defn], replace=False)
+    assert type(result[new_defn]) is R.PkgNonexistent
+
+    async def resolve(defns, with_deps=False):
+        result = await orig_resolve([old_defn])
+        pkg = evolve(result[old_defn], slug=new_defn.alias)
+        return {new_defn: pkg}
+
+    orig_resolve = iw_manager.resolve
+    monkeypatch.setattr(iw_manager, 'resolve', resolve)
+
+    result = await iw_manager.install([new_defn], replace=False)
+    assert type(result[new_defn]) is R.PkgAlreadyInstalled
+
+
 async def test_update_lifecycle_while_varying_retain_defn_strategy(iw_manager: Manager):
     defn = Defn('curse', 'molinari')
     versioned_defn = defn.with_version('80000.57-Release')
 
     result = (await iw_manager.install([defn], replace=False))[defn]
     assert type(result) is R.PkgInstalled
```

### Comparing `instawow-2.2.0/tests/test_matchers.py` & `instawow-2.3.0/tests/test_matchers.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/test_utils.py` & `instawow-2.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/tests/test_wa_updater.py` & `instawow-2.3.0/tests/test_wa_updater.py`

 * *Files identical despite different names*

### Comparing `instawow-2.2.0/PKG-INFO` & `instawow-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instawow
-Version: 2.2.0
+Version: 2.3.0
 Summary: World of Warcraft add-on manager
 License: GPL-3.0-or-later
 Author: layday
 Author-email: layday@protonmail.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

