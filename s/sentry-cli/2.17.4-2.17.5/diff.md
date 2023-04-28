# Comparing `tmp/sentry_cli-2.17.4.tar.gz` & `tmp/sentry_cli-2.17.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_cli-2.17.4.tar", last modified: Thu Apr 20 09:59:23 2023, max compression
+gzip compressed data, was "sentry_cli-2.17.5.tar", last modified: Fri Apr 28 07:57:03 2023, max compression
```

## Comparing `sentry_cli-2.17.4.tar` & `sentry_cli-2.17.5.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.669736 sentry_cli-2.17.4/
--rw-r--r--   0 runner    (1001) docker     (123)    80821 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-20 09:59:23.669736 sentry_cli-2.17.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.657736 sentry_cli-2.17.4/sentry_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-20 09:59:23.000000 sentry_cli-2.17.4/sentry_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-20 09:59:23.000000 sentry_cli-2.17.4/sentry_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:59:23.000000 sentry_cli-2.17.4/sentry_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:59:23.000000 sentry_cli-2.17.4/sentry_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-20 09:59:23.669736 sentry_cli-2.17.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.657736 sentry_cli-2.17.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)    87341 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/api.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/bashsupport.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.657736 sentry_cli-2.17.4/src/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/bash_hook.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.657736 sentry_cli-2.17.4/src/commands/debug_files/
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/debug_files/bundle_jvm.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/debug_files/bundle_sources.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/debug_files/check.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/debug_files/find.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/debug_files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/debug_files/print_sources.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/debug_files/upload.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.661736 sentry_cli-2.17.4/src/commands/deploys/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/deploys/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/deploys/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/deploys/new.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.661736 sentry_cli-2.17.4/src/commands/events/
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/events/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/events/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.661736 sentry_cli-2.17.4/src/commands/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/files/delete.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/files/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/files/upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/info.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.661736 sentry_cli-2.17.4/src/commands/issues/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/issues/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/issues/mute.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/issues/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/issues/unresolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/login.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.661736 sentry_cli-2.17.4/src/commands/monitors/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/monitors/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/monitors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/monitors/run.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.661736 sentry_cli-2.17.4/src/commands/organizations/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/organizations/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/organizations/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.661736 sentry_cli-2.17.4/src/commands/projects/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/projects/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/projects/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.661736 sentry_cli-2.17.4/src/commands/react_native/
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/react_native/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/react_native/gradle.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/react_native/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/react_native/xcode.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.665736 sentry_cli-2.17.4/src/commands/releases/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/releases/archive.rs
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/releases/delete.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/releases/finalize.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/releases/info.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/releases/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/releases/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/releases/new.rs
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/releases/propose_version.rs
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/releases/restore.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/releases/set_commits.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.665736 sentry_cli-2.17.4/src/commands/repos/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/repos/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/repos/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/send_envelope.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/send_event.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.665736 sentry_cli-2.17.4/src/commands/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/sourcemaps/explain.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/sourcemaps/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/sourcemaps/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/sourcemaps/upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/uninstall.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/update.rs
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/upload_dif.rs
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/upload_dsym.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/commands/upload_proguard.rs
--rw-r--r--   0 runner    (1001) docker     (123)    20882 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/config.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/constants.rs
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.669736 sentry_cli-2.17.4/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/android.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/args.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/chunks.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/codepush.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/cordova.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/dif.rs
--rw-r--r--   0 runner    (1001) docker     (123)    72539 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/dif_upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/enc.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/event.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/file_search.rs
--rw-r--r--   0 runner    (1001) docker     (123)    16926 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/file_upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/formatting.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/fs.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/http.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/logging.rs
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/progress.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/releases.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/retry.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.669736 sentry_cli-2.17.4/src/utils/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:59:23.669736 sentry_cli-2.17.4/src/utils/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (123)    36190 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/sourcemaps.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/system.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/ui.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/update.rs
--rw-r--r--   0 runner    (1001) docker     (123)    36048 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/vcs.rs
--rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-04-20 09:58:58.000000 sentry_cli-2.17.4/src/utils/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.853531 sentry_cli-2.17.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    80821 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-28 07:57:03.853531 sentry_cli-2.17.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.841531 sentry_cli-2.17.5/sentry_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-28 07:57:03.000000 sentry_cli-2.17.5/sentry_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-28 07:57:03.000000 sentry_cli-2.17.5/sentry_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 07:57:03.000000 sentry_cli-2.17.5/sentry_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 07:57:03.000000 sentry_cli-2.17.5/sentry_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-28 07:57:03.853531 sentry_cli-2.17.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.845531 sentry_cli-2.17.5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    87341 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/api.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/bashsupport.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.845531 sentry_cli-2.17.5/src/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/bash_hook.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.845531 sentry_cli-2.17.5/src/commands/debug_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/debug_files/bundle_jvm.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/debug_files/bundle_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/debug_files/check.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/debug_files/find.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/debug_files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/debug_files/print_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/debug_files/upload.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.845531 sentry_cli-2.17.5/src/commands/deploys/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/deploys/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/deploys/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/deploys/new.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.845531 sentry_cli-2.17.5/src/commands/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/events/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/events/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.845531 sentry_cli-2.17.5/src/commands/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/files/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/files/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/files/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/info.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.845531 sentry_cli-2.17.5/src/commands/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/issues/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/issues/mute.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/issues/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/issues/unresolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/login.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.845531 sentry_cli-2.17.5/src/commands/monitors/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/monitors/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/monitors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/monitors/run.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.845531 sentry_cli-2.17.5/src/commands/organizations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/organizations/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/organizations/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.849531 sentry_cli-2.17.5/src/commands/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/projects/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/projects/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.849531 sentry_cli-2.17.5/src/commands/react_native/
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/react_native/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/react_native/gradle.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/react_native/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/react_native/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.849531 sentry_cli-2.17.5/src/commands/releases/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/releases/archive.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/releases/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/releases/finalize.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/releases/info.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/releases/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/releases/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/releases/new.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/releases/propose_version.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/releases/restore.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/releases/set_commits.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.849531 sentry_cli-2.17.5/src/commands/repos/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/repos/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/repos/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/send_envelope.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/send_event.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.849531 sentry_cli-2.17.5/src/commands/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/sourcemaps/explain.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/sourcemaps/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/sourcemaps/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/sourcemaps/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/uninstall.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/upload_dif.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/upload_dsym.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/commands/upload_proguard.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    20882 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/config.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/constants.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.853531 sentry_cli-2.17.5/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/android.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/args.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/chunks.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/codepush.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/cordova.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/dif.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    72539 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/dif_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/enc.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/event.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/file_search.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    17036 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/file_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/formatting.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/fs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/http.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/logging.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/progress.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/releases.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/retry.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.853531 sentry_cli-2.17.5/src/utils/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:57:03.853531 sentry_cli-2.17.5/src/utils/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    36411 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/sourcemaps.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/system.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/ui.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    36048 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/vcs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-04-28 07:56:49.000000 sentry_cli-2.17.5/src/utils/xcode.rs
```

### Comparing `sentry_cli-2.17.4/Cargo.lock` & `sentry_cli-2.17.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2191,15 +2191,15 @@
  "once_cell",
  "regex",
  "sentry-core",
 ]
 
 [[package]]
 name = "sentry-cli"
-version = "2.17.4"
+version = "2.17.5"
 dependencies = [
  "anyhow",
  "anylog",
  "backoff",
  "backtrace",
  "brotli2",
  "bytecount",
```

### Comparing `sentry_cli-2.17.4/Cargo.toml` & `sentry_cli-2.17.5/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [package]
 authors = ["Armin Ronacher <armin.ronacher@active-4.com>"]
 build = "build.rs"
 name = "sentry-cli"
-version = "2.17.4"
+version = "2.17.5"
 edition = "2021"
 rust-version = "1.65"
 
 [dependencies]
 anylog = "0.6.3"
 anyhow = { version = "1.0.69", features = ["backtrace"] }
 backoff = "0.4.0"
```

### Comparing `sentry_cli-2.17.4/LICENSE` & `sentry_cli-2.17.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/PKG-INFO` & `sentry_cli-2.17.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry_cli
-Version: 2.17.4
+Version: 2.17.5
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry_cli Version: 2.17.4 Summary: A command line
+Metadata-Version: 2.1 Name: sentry_cli Version: 2.17.5 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.17.4/README.md` & `sentry_cli-2.17.5/README.md`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/build.rs` & `sentry_cli-2.17.5/build.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/sentry_cli.egg-info/PKG-INFO` & `sentry_cli-2.17.5/sentry_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-cli
-Version: 2.17.4
+Version: 2.17.5
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry-cli Version: 2.17.4 Summary: A command line
+Metadata-Version: 2.1 Name: sentry-cli Version: 2.17.5 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.17.4/sentry_cli.egg-info/SOURCES.txt` & `sentry_cli-2.17.5/sentry_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/setup.cfg` & `sentry_cli-2.17.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/setup.py` & `sentry_cli-2.17.5/setup.py`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/api.rs` & `sentry_cli-2.17.5/src/api.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/bashsupport.sh` & `sentry_cli-2.17.5/src/bashsupport.sh`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/bash_hook.rs` & `sentry_cli-2.17.5/src/commands/bash_hook.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/debug_files/bundle_jvm.rs` & `sentry_cli-2.17.5/src/commands/debug_files/bundle_jvm.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/debug_files/bundle_sources.rs` & `sentry_cli-2.17.5/src/commands/debug_files/bundle_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/debug_files/check.rs` & `sentry_cli-2.17.5/src/commands/debug_files/check.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/debug_files/find.rs` & `sentry_cli-2.17.5/src/commands/debug_files/find.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/debug_files/mod.rs` & `sentry_cli-2.17.5/src/commands/debug_files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/debug_files/print_sources.rs` & `sentry_cli-2.17.5/src/commands/debug_files/print_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/debug_files/upload.rs` & `sentry_cli-2.17.5/src/commands/debug_files/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/deploys/list.rs` & `sentry_cli-2.17.5/src/commands/deploys/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/deploys/mod.rs` & `sentry_cli-2.17.5/src/commands/deploys/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/deploys/new.rs` & `sentry_cli-2.17.5/src/commands/deploys/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/events/list.rs` & `sentry_cli-2.17.5/src/commands/events/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/events/mod.rs` & `sentry_cli-2.17.5/src/commands/events/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/files/delete.rs` & `sentry_cli-2.17.5/src/commands/files/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/files/list.rs` & `sentry_cli-2.17.5/src/commands/files/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/files/mod.rs` & `sentry_cli-2.17.5/src/commands/files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/files/upload.rs` & `sentry_cli-2.17.5/src/commands/files/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/info.rs` & `sentry_cli-2.17.5/src/commands/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/issues/mod.rs` & `sentry_cli-2.17.5/src/commands/issues/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/issues/mute.rs` & `sentry_cli-2.17.5/src/commands/issues/mute.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/issues/resolve.rs` & `sentry_cli-2.17.5/src/commands/issues/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/issues/unresolve.rs` & `sentry_cli-2.17.5/src/commands/issues/unresolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/login.rs` & `sentry_cli-2.17.5/src/commands/login.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/mod.rs` & `sentry_cli-2.17.5/src/commands/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/monitors/list.rs` & `sentry_cli-2.17.5/src/commands/monitors/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/monitors/mod.rs` & `sentry_cli-2.17.5/src/commands/monitors/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/monitors/run.rs` & `sentry_cli-2.17.5/src/commands/monitors/run.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/organizations/list.rs` & `sentry_cli-2.17.5/src/commands/organizations/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/organizations/mod.rs` & `sentry_cli-2.17.5/src/commands/organizations/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/projects/list.rs` & `sentry_cli-2.17.5/src/commands/projects/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/projects/mod.rs` & `sentry_cli-2.17.5/src/commands/projects/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/react_native/appcenter.rs` & `sentry_cli-2.17.5/src/commands/react_native/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/react_native/gradle.rs` & `sentry_cli-2.17.5/src/commands/react_native/gradle.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/react_native/mod.rs` & `sentry_cli-2.17.5/src/commands/react_native/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/react_native/xcode.rs` & `sentry_cli-2.17.5/src/commands/react_native/xcode.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/releases/archive.rs` & `sentry_cli-2.17.5/src/commands/releases/archive.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/releases/delete.rs` & `sentry_cli-2.17.5/src/commands/releases/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/releases/finalize.rs` & `sentry_cli-2.17.5/src/commands/releases/finalize.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/releases/info.rs` & `sentry_cli-2.17.5/src/commands/releases/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/releases/list.rs` & `sentry_cli-2.17.5/src/commands/releases/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/releases/mod.rs` & `sentry_cli-2.17.5/src/commands/releases/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/releases/new.rs` & `sentry_cli-2.17.5/src/commands/releases/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/releases/restore.rs` & `sentry_cli-2.17.5/src/commands/releases/restore.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/releases/set_commits.rs` & `sentry_cli-2.17.5/src/commands/releases/set_commits.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/repos/list.rs` & `sentry_cli-2.17.5/src/commands/repos/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/repos/mod.rs` & `sentry_cli-2.17.5/src/commands/repos/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/send_envelope.rs` & `sentry_cli-2.17.5/src/commands/send_envelope.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/send_event.rs` & `sentry_cli-2.17.5/src/commands/send_event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/sourcemaps/explain.rs` & `sentry_cli-2.17.5/src/commands/sourcemaps/explain.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/sourcemaps/inject.rs` & `sentry_cli-2.17.5/src/commands/sourcemaps/inject.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/sourcemaps/mod.rs` & `sentry_cli-2.17.5/src/commands/sourcemaps/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/sourcemaps/resolve.rs` & `sentry_cli-2.17.5/src/commands/sourcemaps/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/sourcemaps/upload.rs` & `sentry_cli-2.17.5/src/commands/sourcemaps/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/uninstall.rs` & `sentry_cli-2.17.5/src/commands/uninstall.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/update.rs` & `sentry_cli-2.17.5/src/commands/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/commands/upload_proguard.rs` & `sentry_cli-2.17.5/src/commands/upload_proguard.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/config.rs` & `sentry_cli-2.17.5/src/config.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/constants.rs` & `sentry_cli-2.17.5/src/constants.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/android.rs` & `sentry_cli-2.17.5/src/utils/android.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/appcenter.rs` & `sentry_cli-2.17.5/src/utils/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/args.rs` & `sentry_cli-2.17.5/src/utils/args.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/chunks.rs` & `sentry_cli-2.17.5/src/utils/chunks.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/codepush.rs` & `sentry_cli-2.17.5/src/utils/codepush.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/cordova.rs` & `sentry_cli-2.17.5/src/utils/cordova.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/dif.rs` & `sentry_cli-2.17.5/src/utils/dif.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/dif_upload.rs` & `sentry_cli-2.17.5/src/utils/dif_upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/enc.rs` & `sentry_cli-2.17.5/src/utils/enc.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/event.rs` & `sentry_cli-2.17.5/src/utils/event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/file_search.rs` & `sentry_cli-2.17.5/src/utils/file_search.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/file_upload.rs` & `sentry_cli-2.17.5/src/utils/file_upload.rs`

 * *Files 1% similar despite different names*

```diff
@@ -461,14 +461,20 @@
         style(files.len()).yellow(),
         match files.len() {
             1 => "file",
             _ => "files",
         }
     );
 
+    println!(
+        "{} Bundle ID: {}",
+        style(">").dim(),
+        style(debug_id).yellow(),
+    );
+
     Ok(archive)
 }
 
 fn url_to_bundle_path(url: &str) -> Result<String> {
     let base = Url::parse("http://~").unwrap();
     let url = if let Some(rest) = url.strip_prefix("~/") {
         base.join(rest)?
```

### Comparing `sentry_cli-2.17.4/src/utils/formatting.rs` & `sentry_cli-2.17.5/src/utils/formatting.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/fs.rs` & `sentry_cli-2.17.5/src/utils/fs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/http.rs` & `sentry_cli-2.17.5/src/utils/http.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/logging.rs` & `sentry_cli-2.17.5/src/utils/logging.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/progress.rs` & `sentry_cli-2.17.5/src/utils/progress.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/releases.rs` & `sentry_cli-2.17.5/src/utils/releases.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/retry.rs` & `sentry_cli-2.17.5/src/utils/retry.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap` & `sentry_cli-2.17.5/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap` & `sentry_cli-2.17.5/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap` & `sentry_cli-2.17.5/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap` & `sentry_cli-2.17.5/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/sourcemaps/inject.rs` & `sentry_cli-2.17.5/src/utils/sourcemaps/inject.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/sourcemaps.rs` & `sentry_cli-2.17.5/src/utils/sourcemaps.rs`

 * *Files 1% similar despite different names*

```diff
@@ -388,15 +388,20 @@
                 continue;
             }
 
             let mut pieces = Vec::new();
 
             if source.ty == SourceFileType::MinifiedSource {
                 if let Some(sm_ref) = get_sourcemap_ref(source) {
-                    pieces.push(format!("sourcemap at {}", style(sm_ref.get_url()).cyan()));
+                    let sm_url = sm_ref.get_url();
+                    if sm_url.starts_with("data:") {
+                        pieces.push("embedded sourcemap".to_string());
+                    } else {
+                        pieces.push(format!("sourcemap at {}", style(sm_url).cyan()));
+                    };
                 } else {
                     pieces.push("no sourcemap ref".into());
                 }
             }
             if let Some((_, debug_id)) = source.headers.iter().find(|x| x.0 == "debug-id") {
                 pieces.push(format!("debug id {}", style(debug_id).yellow()));
             }
```

### Comparing `sentry_cli-2.17.4/src/utils/system.rs` & `sentry_cli-2.17.5/src/utils/system.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/ui.rs` & `sentry_cli-2.17.5/src/utils/ui.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/update.rs` & `sentry_cli-2.17.5/src/utils/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/vcs.rs` & `sentry_cli-2.17.5/src/utils/vcs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.4/src/utils/xcode.rs` & `sentry_cli-2.17.5/src/utils/xcode.rs`

 * *Files identical despite different names*

