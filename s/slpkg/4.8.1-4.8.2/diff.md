# Comparing `tmp/slpkg-4.8.1.tar.gz` & `tmp/slpkg-4.8.2.tar.gz`

## Comparing `slpkg-4.8.1.tar` & `slpkg-4.8.2.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:26:51.000000 slpkg-4.8.1/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/filelists/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/filelists/multilib/
--rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-04-25 15:23:48.000000 slpkg-4.8.1/filelists/multilib/README.ERIC
--rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-04-25 15:23:48.000000 slpkg-4.8.1/filelists/multilib/glibc_packages.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)      831 2023-04-25 15:23:48.000000 slpkg-4.8.1/filelists/multilib/README
--rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-04-25 15:23:48.000000 slpkg-4.8.1/filelists/multilib/compat32.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-04-25 15:23:48.000000 slpkg-4.8.1/filelists/README
--rw-r--r--   0 dslackw   (1000) users      (100)     1189 2023-04-25 15:23:48.000000 slpkg-4.8.1/repositories.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/slackbuild/
--rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-04-25 15:23:48.000000 slpkg-4.8.1/slackbuild/slack-desc
--rw-r--r--   0 dslackw   (1000) users      (100)      432 2023-04-25 15:23:48.000000 slpkg-4.8.1/slackbuild/doinst.sh
--rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-04-25 15:23:48.000000 slpkg-4.8.1/slackbuild/README
--rwxr-xr-x   0 dslackw   (1000) users      (100)     4297 2023-04-25 15:23:48.000000 slpkg-4.8.1/slackbuild/slpkg.SlackBuild
--rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-04-25 15:23:48.000000 slpkg-4.8.1/setup.py
--rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-04-25 15:23:48.000000 slpkg-4.8.1/requirements.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/configs/
--rw-r--r--   0 dslackw   (1000) users      (100)     8285 2023-04-25 15:23:48.000000 slpkg-4.8.1/configs/repositories.toml
--rw-r--r--   0 dslackw   (1000) users      (100)      483 2023-04-25 15:23:48.000000 slpkg-4.8.1/configs/blacklist.toml
--rw-r--r--   0 dslackw   (1000) users      (100)     3731 2023-04-25 15:23:48.000000 slpkg-4.8.1/configs/slpkg.toml
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/tests/
--rw-r--r--   0 dslackw   (1000) users      (100)     2340 2023-04-25 15:23:48.000000 slpkg-4.8.1/tests/test_configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)      770 2023-04-25 15:23:48.000000 slpkg-4.8.1/tests/test_checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1891 2023-04-25 15:23:48.000000 slpkg-4.8.1/tests/test_utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1455 2023-04-25 15:23:48.000000 slpkg-4.8.1/tests/test_sbo_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)      255 2023-04-25 15:23:48.000000 slpkg-4.8.1/tests/test_blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)      898 2023-04-25 15:23:48.000000 slpkg-4.8.1/tests/test_colors.py
--rw-r--r--   0 dslackw   (1000) users      (100)      890 2023-04-25 15:23:48.000000 slpkg-4.8.1/tests/check_updates_test.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1567 2023-04-25 15:23:48.000000 slpkg-4.8.1/tests/test_upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1787 2023-04-25 15:23:48.000000 slpkg-4.8.1/tests/test_bin_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-04-25 15:23:48.000000 slpkg-4.8.1/LICENSE
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1773 2023-04-25 15:23:48.000000 slpkg-4.8.1/install.sh
--rw-r--r--   0 dslackw   (1000) users      (100)    45524 2023-04-25 15:23:48.000000 slpkg-4.8.1/ChangeLog.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/man/
--rw-r--r--   0 dslackw   (1000) users      (100)     8987 2023-04-25 15:23:48.000000 slpkg-4.8.1/man/slpkg.1
--rw-r--r--   0 dslackw   (1000) users      (100)     9918 2023-04-25 15:23:48.000000 slpkg-4.8.1/man/slpkg-fr.1
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/completion/
--rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-04-25 15:23:48.000000 slpkg-4.8.1/completion/slpkg
--rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-04-25 15:23:48.000000 slpkg-4.8.1/.gitignore
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/
--rw-r--r--   0 dslackw   (1000) users      (100)     4007 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/dialog_configs.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/binaries/
--rw-r--r--   0 dslackw   (1000) users      (100)     1623 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/binaries/required.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2110 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/binaries/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/binaries/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     9345 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/binaries/install.py
--rw-r--r--   0 dslackw   (1000) users      (100)    63301 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/install_data.py
--rw-r--r--   0 dslackw   (1000) users      (100)    26741 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/repositories.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2016 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/repo_info.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/sbos/
--rw-r--r--   0 dslackw   (1000) users      (100)     1368 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/sbos/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)    14622 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/sbos/slackbuild.py
--rw-r--r--   0 dslackw   (1000) users      (100)      974 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/sbos/dependencies.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/sbos/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)    30467 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/update_repository.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1395 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/progress_bar.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2476 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/downloader.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/models/
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/models/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2630 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/models/models.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/views/
--rw-r--r--   0 dslackw   (1000) users      (100)     6721 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/views/view_package.py
--rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/views/version.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6096 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/views/cli_menu.py
--rw-r--r--   0 dslackw   (1000) users      (100)     5053 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/views/ascii.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3810 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/views/help_commands.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/views/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     9528 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/views/views.py
--rw-r--r--   0 dslackw   (1000) users      (100)      387 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/error_messages.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3386 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1416 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/checksum.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2196 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/dialog_box.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4324 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)      902 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/clean_logs.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6462 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3607 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/dependees.py
--rw-r--r--   0 dslackw   (1000) users      (100)      587 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/toml_error_message.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4815 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/check_updates.py
--rw-r--r--   0 dslackw   (1000) users      (100)     5384 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/remove_packages.py
--rw-r--r--   0 dslackw   (1000) users      (100)      939 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2603 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/download_only.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2828 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/tracking.py
--rw-r--r--   0 dslackw   (1000) users      (100)      245 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/logging_config.py
--rw-r--r--   0 dslackw   (1000) users      (100)    29954 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/main.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1117 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/find_installed.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3206 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2610 2023-04-25 15:23:48.000000 slpkg-4.8.1/slpkg/search.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1354 2023-04-25 15:23:48.000000 slpkg-4.8.1/setup.cfg
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:26:48.000000 slpkg-4.8.1/slpkg.egg-info/
--rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-04-25 15:26:48.000000 slpkg-4.8.1/slpkg.egg-info/dependency_links.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1159 2023-04-25 15:26:48.000000 slpkg-4.8.1/slpkg.egg-info/SOURCES.txt
--rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-04-25 15:26:48.000000 slpkg-4.8.1/slpkg.egg-info/top_level.txt
--rw-r--r--   0 dslackw   (1000) users      (100)       77 2023-04-25 15:26:48.000000 slpkg-4.8.1/slpkg.egg-info/requires.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1262 2023-04-25 15:26:48.000000 slpkg-4.8.1/slpkg.egg-info/PKG-INFO
--rw-r--r--   0 dslackw   (1000) users      (100)     8518 2023-04-25 15:23:48.000000 slpkg-4.8.1/README.md
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/tools/
--rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-04-25 15:23:48.000000 slpkg-4.8.1/tools/gen_sbo_txt.sh
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-25 15:23:48.000000 slpkg-4.8.1/bin/
--rwxr-xr-x   0 dslackw   (1000) users      (100)    11352 2023-04-25 15:23:48.000000 slpkg-4.8.1/bin/slpkg_new-configs
--rwxr-xr-x   0 dslackw   (1000) users      (100)      184 2023-04-25 15:23:48.000000 slpkg-4.8.1/bin/slpkg
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:51:40.000000 slpkg-4.8.2/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/filelists/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/filelists/multilib/
+-rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-04-28 14:28:20.000000 slpkg-4.8.2/filelists/multilib/README.ERIC
+-rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-04-28 14:28:20.000000 slpkg-4.8.2/filelists/multilib/glibc_packages.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)      831 2023-04-28 14:28:20.000000 slpkg-4.8.2/filelists/multilib/README
+-rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-04-28 14:28:20.000000 slpkg-4.8.2/filelists/multilib/compat32.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-04-28 14:28:20.000000 slpkg-4.8.2/filelists/README
+-rw-r--r--   0 dslackw   (1000) users      (100)     1189 2023-04-28 14:28:20.000000 slpkg-4.8.2/repositories.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/slackbuild/
+-rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-04-28 14:28:20.000000 slpkg-4.8.2/slackbuild/slack-desc
+-rw-r--r--   0 dslackw   (1000) users      (100)      432 2023-04-28 14:28:20.000000 slpkg-4.8.2/slackbuild/doinst.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-04-28 14:28:20.000000 slpkg-4.8.2/slackbuild/README
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     4195 2023-04-28 14:28:20.000000 slpkg-4.8.2/slackbuild/slpkg.SlackBuild
+-rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-04-28 14:28:20.000000 slpkg-4.8.2/setup.py
+-rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-04-28 14:28:20.000000 slpkg-4.8.2/requirements.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/configs/
+-rw-r--r--   0 dslackw   (1000) users      (100)     8545 2023-04-28 14:28:20.000000 slpkg-4.8.2/configs/repositories.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)      483 2023-04-28 14:28:20.000000 slpkg-4.8.2/configs/blacklist.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)     3813 2023-04-28 14:28:20.000000 slpkg-4.8.2/configs/slpkg.toml
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/tests/
+-rw-r--r--   0 dslackw   (1000) users      (100)     2337 2023-04-28 14:28:20.000000 slpkg-4.8.2/tests/test_configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      770 2023-04-28 14:28:20.000000 slpkg-4.8.2/tests/test_checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1891 2023-04-28 14:28:20.000000 slpkg-4.8.2/tests/test_utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1455 2023-04-28 14:28:20.000000 slpkg-4.8.2/tests/test_sbo_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      255 2023-04-28 14:28:20.000000 slpkg-4.8.2/tests/test_blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      898 2023-04-28 14:28:20.000000 slpkg-4.8.2/tests/test_colors.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      890 2023-04-28 14:28:20.000000 slpkg-4.8.2/tests/check_updates_test.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1567 2023-04-28 14:28:20.000000 slpkg-4.8.2/tests/test_upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1787 2023-04-28 14:28:20.000000 slpkg-4.8.2/tests/test_bin_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-04-28 14:28:20.000000 slpkg-4.8.2/LICENSE
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1624 2023-04-28 14:28:20.000000 slpkg-4.8.2/install.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)    45800 2023-04-28 14:28:20.000000 slpkg-4.8.2/ChangeLog.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/man/
+-rw-r--r--   0 dslackw   (1000) users      (100)     9291 2023-04-28 14:28:20.000000 slpkg-4.8.2/man/slpkg.1
+-rw-r--r--   0 dslackw   (1000) users      (100)     9919 2023-04-28 14:28:20.000000 slpkg-4.8.2/man/slpkg-fr.1
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/completion/
+-rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-04-28 14:28:20.000000 slpkg-4.8.2/completion/slpkg
+-rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-04-28 14:28:20.000000 slpkg-4.8.2/.gitignore
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/
+-rw-r--r--   0 dslackw   (1000) users      (100)     4126 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/dialog_configs.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/binaries/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1623 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/binaries/required.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2110 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/binaries/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/binaries/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     8326 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/binaries/install.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    63301 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/install_data.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    26741 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/repositories.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2016 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/repo_info.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/sbos/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1368 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/sbos/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    13735 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/sbos/slackbuild.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      974 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/sbos/dependencies.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/sbos/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    30343 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/update_repository.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1524 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/progress_bar.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2518 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/downloader.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/models/
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/models/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2630 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/models/models.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/views/
+-rw-r--r--   0 dslackw   (1000) users      (100)     6716 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/views/view_package.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/views/version.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6208 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/views/cli_menu.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     5053 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/views/ascii.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3810 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/views/help_commands.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/views/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    10363 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/views/views.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      432 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/error_messages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3595 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1443 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/logging_deps.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    11552 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/new_configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3277 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/cleanings.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1916 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/checksum.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2584 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/dialog_box.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4460 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6888 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3592 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/dependees.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      587 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/toml_error_message.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     5595 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/check_updates.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     5458 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/remove_packages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      939 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2593 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/download_only.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2818 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/tracking.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      456 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/logging_config.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    30502 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/main.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1117 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/find_installed.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3371 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2605 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/search.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1471 2023-04-28 14:28:20.000000 slpkg-4.8.2/setup.cfg
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:51:34.000000 slpkg-4.8.2/slpkg.egg-info/
+-rw-r--r--   0 dslackw   (1000) users      (100)       86 2023-04-28 14:51:34.000000 slpkg-4.8.2/slpkg.egg-info/entry_points.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-04-28 14:51:34.000000 slpkg-4.8.2/slpkg.egg-info/dependency_links.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1233 2023-04-28 14:51:34.000000 slpkg-4.8.2/slpkg.egg-info/SOURCES.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-04-28 14:51:34.000000 slpkg-4.8.2/slpkg.egg-info/top_level.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)       77 2023-04-28 14:51:34.000000 slpkg-4.8.2/slpkg.egg-info/requires.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1262 2023-04-28 14:51:34.000000 slpkg-4.8.2/slpkg.egg-info/PKG-INFO
+-rw-r--r--   0 dslackw   (1000) users      (100)     8684 2023-04-28 14:28:20.000000 slpkg-4.8.2/README.md
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/tools/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-04-28 14:28:20.000000 slpkg-4.8.2/tools/gen_sbo_txt.sh
```

### Comparing `slpkg-4.8.1/filelists/multilib/README.ERIC` & `slpkg-4.8.2/filelists/multilib/README.ERIC`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/filelists/multilib/README` & `slpkg-4.8.2/filelists/multilib/README`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/filelists/multilib/compat32.pkgs` & `slpkg-4.8.2/filelists/multilib/compat32.pkgs`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/repositories.txt` & `slpkg-4.8.2/repositories.txt`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/slackbuild/slack-desc` & `slpkg-4.8.2/slackbuild/slack-desc`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/slackbuild/slpkg.SlackBuild` & `slpkg-4.8.2/slackbuild/slpkg.SlackBuild`

 * *Files 11% similar despite different names*

```diff
@@ -72,43 +72,40 @@
 
 set -e
 
 rm -rf $PKG
 mkdir -p $TMP $PKG $OUTPUT
 cd $TMP
 rm -rf $PRGNAM-$VERSION
-tar xvf $CWD/$PRGNAM-$VERSION.tar.gz || tar xvf $CWD/v$VERSION.tar.gz \
-    || tar xvf $CWD/$PRGNAM-$VERSION.tar.bz2 || unzip $CWD/$PRGNAM-$VERSION.zip \
-	|| unzip $CWD/v$VERSION.zip
+tar xvf $CWD/$PRGNAM-$VERSION.tar.gz || tar xvf $CWD/$PRGNAM-$VERSION.tar.bz2 || unzip $CWD/$PRGNAM-$VERSION.zip
 cd $PRGNAM-$VERSION
 chown -R root:root .
 find -L . \
  \( -perm 777 -o -perm 775 -o -perm 750 -o -perm 711 -o -perm 555 \
   -o -perm 511 \) -exec chmod 755 {} \; -o \
  \( -perm 666 -o -perm 664 -o -perm 640 -o -perm 600 -o -perm 444 \
   -o -perm 440 -o -perm 400 \) -exec chmod 644 {} \;
 
 python3 setup.py install --root=$PKG
 
+# Move executables to the /usr/sbin folder.
 mkdir -p $PKG/usr/sbin
-cp bin/slpkg $PKG/usr/sbin/slpkg
-cp bin/slpkg_new-configs $PKG/usr/sbin/slpkg_new-configs
+mv $PKG/usr/bin/slpkg $PKG/usr/sbin/slpkg
+mv $PKG/usr/bin/slpkg_new-configs $PKG/usr/sbin/slpkg_new-configs
+rm -rf $PKG/usr/bin
 
 find $PKG -print0 | xargs -0 file | grep -e "executable" -e "shared object" | grep ELF \
   | cut -f 1 -d : | xargs strip --strip-unneeded 2> /dev/null || true
 
 # Install configuration files and creating lib directory
 mkdir -p $PKG/etc/$PRGNAM
 install -D -m0644 configs/slpkg.toml $PKG/etc/slpkg/slpkg.toml.new
 install -D -m0644 configs/repositories.toml $PKG/etc/slpkg/repositories.toml.new
 install -D -m0644 configs/blacklist.toml $PKG/etc/slpkg/blacklist.toml.new
 
-mkdir -p $PKG/var/lib/$PRGNAM/repositories/ponce
-cp tools/gen_sbo_txt.sh $PKG/var/lib/$PRGNAM/repositories/ponce
-
 mkdir -p $PKG/usr/man/man1 & mkdir -p $PKG/usr/man/fr/man1
 cp man/slpkg.1 $PKG/usr/man/man1
 cp man/slpkg-fr.1 $PKG/usr/man/fr/man1/slpkg.1
 
 find $PKG/usr/man -type f -exec gzip -9 {} \;
 for i in $( find $PKG/usr/man -type l ) ; do ln -s $( readlink $i ).gz $i.gz; rm $i ; done
```

### Comparing `slpkg-4.8.1/configs/repositories.toml` & `slpkg-4.8.2/configs/repositories.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 # This is the general repositories configuration file of slpkg:
 # /etc/slpkg/repositories.toml
-# Date: 24/04/2023, Version: 4.8.1
+# Date: 26/04/2023, Version: 4.8.2
 
 # The philosophy behind this is to have two repositories for
 # Slackbuilds one for the Slackware stable and one for the -current
 # and many binaries for all versions.
 # Set 'true' to 'PONCE_REPO' to switch with the ponce repository.
 # Set 'true' to the binary repositories you want to enable.
 # Default is the 'sbo' Slackbuilds.org repository.
 
 # If you are going to use a local repository, set the mirror:
 # Example: ["file:///path/to/alien/repository/" ,"15.0/", "x86_64/"]
 # A binary local repository will must contain the files:
 # ChangeLog.txt, PACKAGES.TXT and CHECKSUMS.md5
 # A SlackBuilds repository will must contain the files:
 # SLACKBUILDS.TXT and ChangeLog.txt
-# Note: ponce repository needs the 'gen_sbo_txt.sh' tool from
-# the 'slpkg/tools/' folder, if the SLACKBUILDS.TXT missing.
 
 # After the mirror changed, you should update the database:
 # slpkg update or apply the option --bin-repo=<repo_name> for
 # binary repositories.
 
+# DO NOT CHANGE THE PATTERN OF THE MIRRORS, CHANGE ONLY WHAT YOU WANT.
+# Example: ["https://slackware.nl/people/alien/sbrepos/", "15.0/", "x86_64/"]
+# For Slackware -current users should be:
+# ["https://slackware.nl/people/alien/sbrepos/", "current/", "x86_64/"]
+# and NOT: ["https://slackware.nl/people/alien/sbrepos/current/x86_64/"]
+
 # Note: Before using a repository, make sure you have read about it.
-#       Some repositories are for -current only. Change the mirror if
-#       it is necessary. The mirror should end with a slash '/'.
+#       Some repositories are for -current only. Change the mirror
+#       if it is necessary. The mirror or every part of the mirror
+#       should end with a slash '/'.
 
 [REPOSITORIES]
 
 # SBo Repository for Slackware 15.0 stable.
 SBO_REPO_NAME = "sbo"
 SBO_REPO_MIRROR = ["https://slackbuilds.org/slackbuilds/15.0/"]
 SBO_REPO_SLACKBUILDS = "SLACKBUILDS.TXT"
@@ -71,15 +76,15 @@
 # Official repository for Slackware patches x86_64 15.0 stable.
 SLACK_PATCHES_REPO = false
 SLACK_PATCHES_REPO_NAME = "slack_patches"
 SLACK_PATCHES_REPO_MIRROR = ["https://slackware.uk/slackware/slackware64-15.0/", "patches/"]
 SLACK_PATCHES_REPO_PACKAGES = "PACKAGES.TXT"
 SLACK_PATCHES_REPO_CHECKSUMS = "CHECKSUMS.md5"
 SLACK_PATCHES_REPO_CHANGELOG = "ChangeLog.txt"
-SLACK_PATCHES_REPO_TAG = ""
+SLACK_PATCHES_REPO_TAG = "_slack15.0"
 
 # AlienBob Repository for Slackware x86_64 15.0 stable.
 # For Slackware x86_64 -current:
 # ["http://slackware.uk/people/alien/sbrepos/", "current/", "x86_64/"]
 ALIEN_REPO = false
 ALIEN_REPO_NAME = "alien"
 ALIEN_REPO_MIRROR = ["https://slackware.nl/people/alien/sbrepos/", "15.0/", "x86_64/"]
```

### Comparing `slpkg-4.8.1/configs/slpkg.toml` & `slpkg-4.8.2/configs/slpkg.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This is the general configuration file of slpkg:
 # /etc/slpkg/slpkg.toml
-# Date: 24/04/2023, Version: 4.8.1
+# Date: 24/04/2023, Version: 4.8.2
 
 [CONFIGS]
 
 # OS architecture by default.
 OS_ARCH = "x86_64"
 
 # Where the packages download.
@@ -40,42 +40,45 @@
 # Alternatively, you can use the option '--parallel'.
 PARALLEL_DOWNLOADS = false
 
 # Pass your file pattern here, if you want to work only with 'sbo' packages
 # add '*_SBo' pattern. Default is the '*'.
 FILE_PATTERN = "*"
 
+# Enable or disable the spinning bar. Default is true. [true/false]
+SPINNING_BAR = true
+
 # There are 5 predefined spinners for the progress bar.
 # Default is pixel. [spinner/pie/moon/line/pixel]
 PROGRESS_SPINNER = "pixel"
 
 # Choose color for the progress bar spinner.
 # Default is green. [green/violet/yellow/blue/cyan/grey/red]
 SPINNER_COLOR = "green"
 
 # Slackware command for install packages, instead, you can use 'installpkg'.
 # Normally upgradepkg only upgrades packages that are already installed
 # on the system, and will skip any packages that do not already have a
 # version installed. If --install- new is specified, the behavior is
 # modified to install new packages in addition to upgrading existing ones.
-# See: $ man upgradepkg.
+# See manpage of the upgradepkg.
 INSTALLPKG = "upgradepkg --install-new"
 
 # Slackware command to reinstall packages.
 # Upgradepkg usually skips packages if the exact same package (matching name,
 # version, arch, and build number) is already installed on the system. Use
 # the --reinstall option if you want to upgrade all packages even if the same
-# version is already installed. See: $ man upgradepkg.
+# version is already installed.
 REINSTALL = "upgradepkg --reinstall"
 
 # Slackware command to remove packages.
 #removepkg removes a previously installed Slackware package, while writing
 # a progress report to the standard output.  A package may be specified either
 # by the full package name (as you'd see listed in /var/lib/pkgtools/packages/),
-# or by the base package name. See: $ man removepkg.
+# or by the base package name. See manpage of the removepkg.
 REMOVEPKG = "removepkg"
 
 # You can choose a downloader among wget, curl and lftp.
 # Default is wget. [wget/wget2/curl/lftp]
 DOWNLOADER = "wget"
 
 # Wget downloader options.
```

### Comparing `slpkg-4.8.1/tests/test_configs.py` & `slpkg-4.8.2/tests/test_configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 
     def setUp(self):
         self.configs = Configs
 
     def test_configs(self):
         self.assertEqual('slpkg', self.configs.prog_name)
         self.assertEqual('x86_64', self.configs.os_arch)
-        self.assertEqual('/tmp/', self.configs.tmp_path)
+        self.assertEqual(Path('/tmp'), self.configs.tmp_path)
         self.assertEqual(Path('/tmp/slpkg'), self.configs.tmp_slpkg)
-        self.assertEqual('/tmp/slpkg/', self.configs.download_only_path)
+        self.assertEqual(Path('/tmp/slpkg/'), self.configs.download_only_path)
         self.assertEqual(Path('/var', 'lib', 'slpkg'), self.configs.lib_path)
         self.assertEqual(Path('/etc', 'slpkg'), self.configs.etc_path)
         self.assertEqual(Path('/var/lib/', 'slpkg', 'database'), self.configs.db_path)
         self.assertEqual(Path('/var', 'log', 'packages'), self.configs.log_packages)
 
         self.assertEqual('database.slpkg', self.configs.database_name)
         self.assertEqual('.pkgs', self.configs.file_list_suffix)
         self.assertEqual('upgradepkg --install-new', self.configs.installpkg)
-        self.assertEqual('upgradepkg --install-new --reinstall', self.configs.reinstall)
+        self.assertEqual('upgradepkg --reinstall', self.configs.reinstall)
         self.assertEqual('removepkg', self.configs.removepkg)
         self.assertEqual(True, self.configs.colors)
         self.assertEqual(True, self.configs.dialog)
         self.assertEqual('wget', self.configs.downloader)
         self.assertEqual('-c -q --progress=bar:force:noscroll --show-progress', self.configs.wget_options)
         self.assertEqual('', self.configs.curl_options)
         self.assertEqual('-c get -e', self.configs.lftp_get_options)
```

### Comparing `slpkg-4.8.1/tests/test_checks.py` & `slpkg-4.8.2/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/tests/test_utilities.py` & `slpkg-4.8.2/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/tests/test_sbo_queries.py` & `slpkg-4.8.2/tests/test_sbo_queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/tests/test_colors.py` & `slpkg-4.8.2/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/tests/check_updates_test.py` & `slpkg-4.8.2/tests/check_updates_test.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/tests/test_upgrade.py` & `slpkg-4.8.2/tests/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/tests/test_bin_queries.py` & `slpkg-4.8.2/tests/test_bin_queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/LICENSE` & `slpkg-4.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/install.sh` & `slpkg-4.8.2/install.sh`

 * *Files 12% similar despite different names*

```diff
@@ -26,18 +26,16 @@
 # Grab version from __metadata_.py file
 cat setup.cfg | grep "version =" | tr -d "[:space:]" | cut -c9-13 | tr , .
 }
 
 PRGNAM=slpkg
 VERSION=${VERSION:-$(__version)} 
 
-# Installation script.
-# With this script allows you to install the slpkg as a Slackware package binary file.
-ARCHIVES="$PRGNAM-$VERSION.tar.gz $PRGNAM-$VERSION.zip v$VERSION.tar.gz v$VERSION.zip \
-	      $PRGNAM-$VERSION.tar.bz2"
+ARCHIVES="$PRGNAM-$VERSION.tar.gz $PRGNAM-$VERSION.tar.bz2 $PRGNAM-$VERSION.zip"
+
 cd ..
 for file in $ARCHIVES; do
   if [ -f $file ]; then
     cp $file $PRGNAM-$VERSION/slackbuild
     cd $PRGNAM-$VERSION/slackbuild
     chmod +x $PRGNAM.SlackBuild
     ./$PRGNAM.SlackBuild
```

### Comparing `slpkg-4.8.1/ChangeLog.txt` & `slpkg-4.8.2/ChangeLog.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+4.8.2 - 25/04/2023
+Updated:
+- For exit status code
+- Packages summary for calculating the file sizes
+Added:
+- Disable or enable the spinning bar
+Fixed:
+- Slackware patches repository tag
+- For skip to download sources if the package is installed (Thanks to kingbeowulf LQ63)
+
 4.8.1 - 21/04/2023
 Updated:
 - For error messages
 - For repository updates (Thanks to rizitis)
 - For reinstall slackware command
 Fixed:
 - Double packages as main and as dependency for binaries repos
```

### Comparing `slpkg-4.8.1/man/slpkg.1` & `slpkg-4.8.2/man/slpkg.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-.TH slpkg 1 "Orestiada, Greece" "slpkg 4.7.8" dslackw
+.TH slpkg 1 "Orestiada, Greece" "slpkg 4.8.2" dslackw
 .SH NAME
 .P
 slpkg \- Package manager utility for Slackware.
 .SH SYNOPSIS
 .P
 slpkg \c
 [\fICOMMAND\fR] [\fIOPTIONS\fR] [\fIFILELIST|PACKAGES...\fR]
 .P
-slpkg [-h|-v] [-u, update] [-U, upgrade] [-c, check-updates] [-I, repo-info] [-g, configs] [-L, clean-logs]
-[-D, clean-tmp] [-T, clean-data] [-b, build] [-i, install] [-d, download]
+slpkg [-h|-v] [-u, update] [-U, upgrade] [-c, check-updates] [-I, repo-info] [-g, configs]
+[-L, clean-logs] [-D, clean-tmp] [-T, clean-data] [-b, build] [-i, install] [-d, download]
 [-R, remove] [-f, find] [-w, view] [-s, search] [-e, dependees] [-t, tracking] -y, --yes, -j, --jobs, -o, --resolve-off,
 -r, --reinstall, -k, --skip-installed, -E, --full-reverse, -S, --search, -n, --no-silent, -p, --pkg-version, -z,
 -G, --generate-only, -P, --parallel, -B, --bin-repo=[\fIREPO\fR], -z, --directory=[\fIPATH\fR]
 .SH DESCRIPTION
 .P
 Slpkg is a software package manager that installs, updates, and removes packages on Slackware based systems.
 It automatically computes dependencies and figures out what things should occur to install packages.
@@ -238,23 +238,33 @@
 You can apply the asterisk '*' instead of a package, to matching all the packages from a repository. You can't apply
 an asterisk to the '\fB-B, --bin-repos=\fR' option, except for the '\fB-s, search\fR', '\fB-u, update\fR' and '\fB-c, check-updates\fR' commands.
 
 Command clean-data, removes the local repository data and the database data.
 
 Note: There is currently no function to indicate the packages if the colors are disabled.
 .RE
+.SH EXIT STATUS
+.P
+0 Successful slpkg execution.
+.P
+1 Something wrong happened.
+.P
+20 No package found to be  downloaded,  installed,  reinstalled,  up‐graded, or removed.
+.RE
 .SH CONFIGURATION FILES
 .P
 Configuration file in the /etc/slpkg/slpkg.toml file.
 .P
 Repositories file in the /etc/slpkg/repositories.toml file.
 .P
 Blacklist file in the /etc/slpkg/blacklist.toml file.
 .P
-\fIslpkg_new-config\fR command it's managing the .new configuration files easily and fast. Move, copy or remove them.
+\fIslpkg_new-configs\fR command it's managing the .new configuration files easily and fast. Move, copy or remove them.
 .RE
 .SH REPORT BUGS
 .P
 Please report any found to: https://gitlab.com/dslackw/slpkg/-/issues.
+.P
+Note: With the issue, please reference the log file you will find in the /tmp/slpkg/logs/slpkg.log path and paste it too.
 .SH AUTHOR
 .P
 Dimitris Zlatanidis <dslackw@gmail.com>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `slpkg-4.8.1/man/slpkg-fr.1` & `slpkg-4.8.2/man/slpkg-fr.1`

 * *Files 1% similar despite different names*

```diff
@@ -241,15 +241,15 @@
 .P
 Fichier de \fBconfiguration\fP : /etc/slpkg/slpkg.toml
 .P
 Fichier des \fBdépôts\fP : /etc/slpkg/repositories.toml
 .P
 Fichier \fBblacklist\fP : /etc/slpkg/blacklist.toml
 .P
-\fIslpkg_new-config\fR permet de gérer les fichiers de configuration \fB.new\fP facilement et rapidement. Déplacez, copiez ou supprimez-les.
+\fIslpkg_new-configs\fR permet de gérer les fichiers de configuration \fB.new\fP facilement et rapidement. Déplacez, copiez ou supprimez-les.
 .RE
 .SH RAPPORT DE BOGUES
 .P
 Veuillez signaler tout bogue trouvé à \fBhttps://gitlab.com/dslackw/slpkg/-/issues\fP.
 .SH AUTEUR
 .P
 \fBDimitris Zlatanidis\fP <dslackw@gmail.com>
```

### Comparing `slpkg-4.8.1/completion/slpkg` & `slpkg-4.8.2/completion/slpkg`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/slpkg/dialog_configs.py` & `slpkg-4.8.2/slpkg/dialog_configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.orig_configs: list = []
         self.config_file: Path = Path(self.etc_path, f'{self.prog_name}.toml')
 
     def is_dialog_enabled(self) -> None:
         """ Checking if the dialog box is enabled by the user. """
         if not self.dialog:
             self.errors.raise_error_message(f"You should enable the dialog in the "
-                                            f"'{self.etc_path}/{self.prog_name}.toml' file")
+                                            f"'{self.etc_path}/{self.prog_name}.toml' file", exit_status=1)
 
     def edit(self) -> None:
         """ Read and write the configuration file. """
         self.is_dialog_enabled()
         elements: list = []
         height: int = 30
         width: int = 74
@@ -71,15 +71,16 @@
         """ Check for true of false values. """
         keys: list = [
             'COLORS',
             'DIALOG',
             'SILENT_MODE',
             'ASCII_CHARACTERS',
             'ASK_QUESTION',
-            'PARALLEL_DOWNLOADS'
+            'PARALLEL_DOWNLOADS',
+            'SPINNING_BAR'
         ]
         values: list = ['true', 'false']
 
         for key, value in zip(self.configs['CONFIGS'].keys(), tags):
 
             if key in keys and value not in values:
                 self.dialogbox.msgbox(f"\nError value for {key}. It must be 'true' or 'false'\n", height=7, width=60)
@@ -106,16 +107,18 @@
                 for key, value in zip(self.configs['CONFIGS'].keys(), tags):
 
                     if line.lstrip().startswith(f'{key} ='):
                         line = f'  {key} = "{value}"\n'
 
                     if line.lstrip().startswith(
 
-                            ('COLORS =', 'DIALOG =',
+                            ('COLORS =',
+                             'DIALOG =',
                              'SILENT_MODE =',
                              'ASCII_CHARACTERS =',
                              'ASK_QUESTION =',
-                             'PARALLEL_DOWNLOADS =')
+                             'PARALLEL_DOWNLOADS =',
+                             'SPINNING_BAR =')
                     ):
                         line: str = line.replace('"', '')
 
                 patch_toml.write(line)
```

### Comparing `slpkg-4.8.1/slpkg/binaries/required.py` & `slpkg-4.8.2/slpkg/binaries/required.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             self.repos.salixos_repo_name,
             self.repos.salixos_patches_repo_name,
             self.repos.salixos_extra_repo_name,
             self.repos.slackel_repo_name,
             self.repos.slint_repo_name
         ]
 
-        self.repo = self.data[name][11]
+        self.repo: str = data[name][11]
 
     def resolve(self) -> list:
         """ Resolve the dependencies. """
         required: list[str] = list(self.remove_deps(self.data[self.name][6].split()))
 
         # Resolve dependencies for some special repos.
         if self.repo in self.special_repos:
```

### Comparing `slpkg-4.8.1/slpkg/binaries/queries.py` & `slpkg-4.8.2/slpkg/binaries/queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/slpkg/binaries/install.py` & `slpkg-4.8.2/slpkg/binaries/install.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import os
 import time
 import subprocess
+from pathlib import Path
 from collections import OrderedDict
 from multiprocessing import Process
 
 from slpkg.configs import Configs
 from slpkg.checksum import Md5sum
 from slpkg.upgrade import Upgrade
 from slpkg.utilities import Utilities
 from slpkg.dialog_box import DialogBox
 from slpkg.downloader import Downloader
 from slpkg.views.views import ViewMessage
 from slpkg.progress_bar import ProgressBar
+from slpkg.logging_deps import LoggingDeps
 from slpkg.repositories import Repositories
 from slpkg.binaries.required import Required
-from slpkg.models.models import LogsDependencies
 from slpkg.models.models import session as Session
 
 
 class Packages(Configs):
 
     def __init__(self, data: dict, packages: list, flags: list, mode: str):
         __slots__ = 'data', 'packages', 'flags', 'mode'
@@ -31,39 +32,40 @@
         self.flags: list = flags
         self.mode: str = mode
 
         self.progress = ProgressBar()
         self.utils = Utilities()
         self.repos = Repositories()
         self.dialogbox = DialogBox()
-        self.upgrade = Upgrade(self.flags, self.data)
-        self.view_message = ViewMessage(self.flags, self.data)
+        self.logs_deps = LoggingDeps(flags, data)
+        self.upgrade = Upgrade(flags, data)
+        self.view_message = ViewMessage(flags, data)
         self.session = Session
 
         self.stderr = None
         self.stdout = None
         self.process_message: str = ''
 
         self.packages_requires: list = []
         self.install_order: list = []
         self.binary_packages: list = []
 
         self.option_for_reinstall: bool = self.utils.is_option(
-            ['-r', '--reinstall'], self.flags)
+            ['-r', '--reinstall'], flags)
 
         self.option_for_skip_installed: bool = self.utils.is_option(
-            ['-k', '--skip-installed'], self.flags)
+            ['-k', '--skip-installed'], flags)
 
         self.option_for_resolve_off: bool = self.utils.is_option(
-            ['-o', '--resolve-off'], self.flags)
+            ['-o', '--resolve-off'], flags)
 
         self.option_for_no_silent: bool = self.utils.is_option(
-            ['-n', '--no-silent'], self.flags)
+            ['-n', '--no-silent'], flags)
 
-        self.packages: list = self.utils.apply_package_pattern(self.data, self.packages)
+        self.packages: list = self.utils.apply_package_pattern(data, packages)
 
     def execute(self) -> None:
         self.dependencies()
 
         self.view_message.install_packages(self.packages, self.packages_requires, self.mode)
         self.view_message.question()
 
@@ -140,15 +142,15 @@
 
         return False
 
     def checksum(self) -> None:
         """ Packages checksums. """
         md5 = Md5sum(self.flags)
         for package in self.binary_packages:
-            name: str = self.utils.split_binary_pkg(package[:-4])[0]
+            name: str = self.utils.split_binary_pkg(Path(package).stem)[0]
             pkg_checksum: str = self.data[name][10]
             md5.check(self.tmp_slpkg, package, pkg_checksum)
 
     def install_packages(self) -> None:
         """ Install the packages. """
         for package in self.binary_packages:
 
@@ -162,35 +164,16 @@
                 slack_command: str = self.reinstall
 
             command: str = f'{slack_command} {self.tmp_slpkg}/{package}'
             self.process_message: str = f"package '{package}' to install"
             self.multi_process(command, package, message)
 
             if not self.option_for_resolve_off:
-                name: str = self.utils.split_binary_pkg(package[:-4])[0]
-                self.logging_installed_dependencies(name)
-
-    def logging_installed_dependencies(self, name: str) -> None:
-        """ Logging installed dependencies. """
-        exist = self.session.query(LogsDependencies.name).filter(
-            LogsDependencies.name == name).first()
-
-        requires: list = Required(self.data, name).resolve()
-
-        # Update the dependencies if exist else create it.
-        if exist:
-            self.session.query(
-                LogsDependencies).filter(
-                    LogsDependencies.name == name).update(
-                        {LogsDependencies.requires: ' '.join(requires)})
-
-        elif requires:
-            deps: list = LogsDependencies(name=name, requires=' '.join(requires))
-            self.session.add(deps)
-        self.session.commit()
+                name: str = self.utils.split_binary_pkg(Path(package).stem)[0]
+                self.logs_deps.logging(name)
 
     def multi_process(self, command: str, filename: str, message: str) -> None:
         """ Starting multiprocessing install/upgrade process. """
         if self.silent_mode and not self.option_for_no_silent:
 
             done: str = f' {self.byellow} Done{self.endc}'
             self.stderr = subprocess.DEVNULL
@@ -228,29 +211,22 @@
         height: int = 10
         width: int = 70
         list_height: int = 0
         choices: list = []
         title: str = ' Choose dependencies you want to install '
 
         for package in dependencies:
-            status: bool = False
+            status: bool = True
 
             repo_ver: str = self.data[package][0]
             help_text: str = f'Package: {package} {repo_ver}'
-            upgradable: bool = self.upgrade.is_package_upgradeable(package)
             installed: str = self.utils.is_package_installed(package)
 
-            if self.mode == 'upgrade' and upgradable:
-                status: bool = True
-
-            if self.mode == 'install' and upgradable:
-                status: bool = True
-
-            if self.mode == 'install' and not installed:
-                status: bool = True
+            if installed:
+                status: bool = False
 
             if self.option_for_reinstall:
                 status: bool = True
 
             choices += [(package, repo_ver, status, help_text)]
 
         text: str = f'There are {len(choices)} dependencies:'
```

### Comparing `slpkg-4.8.1/slpkg/install_data.py` & `slpkg-4.8.2/slpkg/install_data.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/slpkg/repositories.py` & `slpkg-4.8.2/slpkg/repositories.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/slpkg/repo_info.py` & `slpkg-4.8.2/slpkg/repo_info.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/slpkg/sbos/queries.py` & `slpkg-4.8.2/slpkg/sbos/queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/slpkg/sbos/slackbuild.py` & `slpkg-4.8.2/slpkg/sbos/slackbuild.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import os
 import time
 import shutil
+import logging
 import subprocess
 
 from pathlib import Path
 from collections import OrderedDict
 from multiprocessing import Process, cpu_count
 
 from slpkg.checksum import Md5sum
@@ -15,17 +16,18 @@
 from slpkg.upgrade import Upgrade
 from slpkg.utilities import Utilities
 from slpkg.dialog_box import DialogBox
 from slpkg.downloader import Downloader
 from slpkg.error_messages import Errors
 from slpkg.views.views import ViewMessage
 from slpkg.progress_bar import ProgressBar
+from slpkg.logging_deps import LoggingDeps
 from slpkg.repositories import Repositories
 from slpkg.sbos.dependencies import Requires
-from slpkg.models.models import LogsDependencies
+from slpkg.logging_config import LoggingConfig
 from slpkg.models.models import session as Session
 
 
 class Slackbuilds(Configs):
     """ Download build and install the SlackBuilds. """
 
     def __init__(self, data: dict, slackbuilds: list, flags: list, mode: str):
@@ -38,45 +40,51 @@
 
         self.session = Session
         self.errors = Errors()
         self.repos = Repositories()
         self.utils = Utilities()
         self.progress = ProgressBar()
         self.dialogbox = DialogBox()
-        self.upgrade = Upgrade(self.flags, data)
-        self.view_message = ViewMessage(self.flags, data)
+        self.logs_deps = LoggingDeps(flags, data)
+        self.upgrade = Upgrade(flags, data)
+        self.view_message = ViewMessage(flags, data)
 
         self.stderr = None
         self.stdout = None
         self.sbos: dict = {}
         self.install_order: list = []
         self.dependencies: list = []
         self.process_message: str = ''
 
         self.option_for_reinstall: bool = self.utils.is_option(
-            ['-r', '--reinstall'], self.flags)
+            ['-r', '--reinstall'], flags)
 
         self.option_for_skip_installed: bool = self.utils.is_option(
-            ['-k', '--skip-installed'], self.flags)
+            ['-k', '--skip-installed'], flags)
 
         self.option_for_resolve_off: bool = self.utils.is_option(
-            ['-o', '--resolve-off'], self.flags)
+            ['-o', '--resolve-off'], flags)
 
         self.option_for_jobs: bool = self.utils.is_option(
-            ['-j', '--jobs'], self.flags)
+            ['-j', '--jobs'], flags)
 
         self.option_for_no_silent: bool = self.utils.is_option(
-            ['-n', '--no-silent'], self.flags)
+            ['-n', '--no-silent'], flags)
 
-        self.slackbuilds: list = self.utils.apply_package_pattern(self.data, self.slackbuilds)
+        self.slackbuilds: list = self.utils.apply_package_pattern(data, slackbuilds)
 
         # Patch the TAG from configs.
         if self.repos.patch_repo_tag:
             self.repos.repo_tag = self.repos.patch_repo_tag
 
+        logging.basicConfig(filename=LoggingConfig.log_file,
+                            filemode=LoggingConfig.filemode,
+                            encoding=LoggingConfig.encoding,
+                            level=LoggingConfig.level)
+
     def execute(self) -> None:
         """ Starting build or install the slackbuilds. """
         self.creating_dictionary()
         self.creating_dependencies_for_build()
         self.creating_main_for_build()
         self.view_before_build()
 
@@ -151,19 +159,17 @@
         if self.utils.is_package_installed(name) and self.option_for_reinstall:
             return True
 
         return False
 
     def prepare_slackbuilds_for_build(self) -> None:
         """ Downloads files and sources. """
-        sources_urls: list = []
         sources: dict = {}
 
         for sbo in self.install_order:
-
             if self.continue_build_or_install(sbo):
 
                 build_path: Path = Path(self.build_path, sbo)
 
                 self.utils.remove_folder_if_exists(build_path)
                 location: str = self.data[sbo][0]
                 slackbuild = Path(self.build_path, sbo, f'{sbo}.SlackBuild')
@@ -176,28 +182,24 @@
                     path_sbo_repo_package = Path(self.repos.sbo_repo_path, location, sbo)
                     shutil.copytree(path_sbo_repo_package, build_path)
 
                 os.chmod(slackbuild, 0o775)
 
                 if self.os_arch == 'x86_64' and self.data[sbo][4]:
                     sources[sbo] = self.data[sbo][4].split()
-                    sources_urls += self.data[sbo][4].split()
                 else:
                     sources[sbo] = self.data[sbo][3].split()
-                    sources_urls += self.data[sbo][3].split()
 
-        # Download the sources.
         if sources:
-            for sbo, sbo_sources in sources.items():
-                down_urls = Downloader(Path(self.build_path, sbo), sbo_sources, self.flags)
+            for pkg, sbo_sources in sources.items():
+                down_urls = Downloader(Path(self.build_path, pkg), sbo_sources, self.flags)
                 down_urls.download()
 
-            print()  # New line here.
-
             self.checksum_downloads()
+        print()  # New line here.
 
     def checksum_downloads(self) -> None:
         """ Checking the correct checksums. """
         for sbo in self.install_order:
             path = Path(self.build_path, sbo)
 
             if self.os_arch == 'x86_64' and self.data[sbo][6]:
@@ -223,54 +225,34 @@
 
                 if self.mode in ['install', 'upgrade']:
 
                     pkg: str = self.package_for_install(sbo)
                     self.install_package(pkg)
 
                     if not self.option_for_resolve_off:
-                        self.logging_installed_dependencies(sbo)
+                        self.logs_deps.logging(sbo)
             else:
                 package: str = self.utils.is_package_installed(sbo)
                 version: str = self.utils.split_binary_pkg(package)[1]
                 self.view_message.view_skipping_packages(sbo, version)
 
     def patch_sbo_tag(self, sbo: str) -> None:
         """ Patching SBo TAG from the configuration file. """
         sbo_script: Path = Path(self.build_path, sbo, f'{sbo}.SlackBuild')
 
         if sbo_script.is_file() and self.repos.patch_repo_tag:
 
-            with open(sbo_script, 'r', encoding='utf-8') as f:
-                lines = f.readlines()
+            lines: list = self.utils.read_file(sbo_script)
 
             with open(sbo_script, 'w') as script:
                 for line in lines:
                     if line.startswith('TAG=$'):
                         line: str = f'TAG=${{TAG:-{self.repos.patch_repo_tag}}}\n'
                     script.write(line)
 
-    def logging_installed_dependencies(self, name: str) -> None:
-        """ Logging installed dependencies and used for remove. """
-        exist: tuple = self.session.query(LogsDependencies.name).filter(
-            LogsDependencies.name == name).first()
-
-        requires: list = Requires(self.data, name).resolve()
-
-        # Update the dependencies if exist else create it.
-        if exist:
-            self.session.query(
-                LogsDependencies).filter(
-                    LogsDependencies.name == name).update(
-                        {LogsDependencies.requires: ' '.join(requires)})
-
-        elif requires:
-            deps: list = LogsDependencies(name=name, requires=' '.join(requires))
-            self.session.add(deps)
-        self.session.commit()
-
     def install_package(self, package: str) -> None:
         """ Install the packages that before created in the tmp directory. """
         pkg: str = self.utils.split_binary_pkg(package)[0]
 
         execute: str = self.installpkg
         if self.option_for_reinstall and self.utils.is_package_installed(pkg):
             execute: str = self.reinstall
@@ -278,31 +260,33 @@
         message: str = f'{self.cyan}Installing{self.endc}'
         self.process_message: str = f"package '{pkg}' to install"
 
         if self.mode == 'upgrade':
             self.process_message: str = f"package '{pkg}' to upgrade"
             message: str = f'{self.cyan}Upgrade{self.endc}'
 
-        command: str = f'{execute} {self.tmp_path}{package}'
+        command: str = f'{execute} {self.tmp_path}/{package}'
 
         self.multi_process(command, package, message)
 
     def package_for_install(self, name: str) -> str:
         """ Returns the package for install. """
         package: str = ''
         version: str = self.data[name][2]
         pattern: str = f'{name}-{version}*{self.repos.repo_tag}*'
 
-        tmp: Path = Path(self.tmp_path)
-        packages: list = [file.name for file in tmp.glob(pattern)]
+        packages: list = [file.name for file in self.tmp_path.glob(pattern)]
 
         try:
             package: str = max(packages)
         except ValueError:
-            self.errors.raise_error_message(f"Package '{name}' not found for install")
+            logger = logging.getLogger(LoggingConfig.date)
+            logger.exception(f'{self.__class__.__name__}: '
+                             f'{self.__class__.package_for_install.__name__}')
+            self.errors.raise_error_message(f"Package '{name}' not found for install", exit_status=20)
 
         return package
 
     def build_the_script(self, path: Path, name: str) -> None:
         """ Run the .SlackBuild script. """
         folder: str = f'{Path(path, name)}/'
         execute: str = f'{folder}./{name}.SlackBuild'
@@ -366,33 +350,23 @@
         height: int = 10
         width: int = 70
         list_height: int = 0
         choices: list = []
         title: str = ' Choose dependencies you want to install '
 
         for package in dependencies:
-            status: bool = False
+            status: bool = True
 
             repo_ver: str = self.data[package][2]
             description: str = self.data[package][8]
             help_text: str = f'Description: {description}'
-            upgradable: bool = self.upgrade.is_package_upgradeable(package)
             installed: str = self.utils.is_package_installed(package)
 
-            if self.mode == 'build':
-                status: bool = True
-
-            if self.mode == 'upgrade':
-                status: bool = True
-
-            if self.mode == 'install' and upgradable:
-                status: bool = True
-
-            if self.mode == 'install' and not installed:
-                status: bool = True
+            if installed:
+                status: bool = False
 
             if self.option_for_reinstall:
                 status: bool = True
 
             choices += [(package, repo_ver, status, help_text)]
 
         text: str = f'There are {len(choices)} dependencies:'
```

### Comparing `slpkg-4.8.1/slpkg/sbos/dependencies.py` & `slpkg-4.8.2/slpkg/sbos/dependencies.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/slpkg/update_repository.py` & `slpkg-4.8.2/slpkg/update_repository.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,52 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import os
-import shutil
 from pathlib import Path
 from multiprocessing import Process, Queue
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.downloader import Downloader
 from slpkg.views.views import ViewMessage
 from slpkg.progress_bar import ProgressBar
 from slpkg.install_data import InstallData
 from slpkg.repositories import Repositories
 from slpkg.check_updates import CheckUpdates
 from slpkg.models.models import session as Session
-from slpkg.models.models import (Base, engine, SBoTable,
-                                 PonceTable, BinariesTable,
-                                 LastRepoUpdated)
+from slpkg.models.models import (SBoTable, PonceTable,
+                                 BinariesTable, LastRepoUpdated)
 
 
 class UpdateRepository(Configs):
     """ Deletes and install the data. """
 
     def __init__(self, flags: list, repo: str):
         __slots__ = 'flags', 'repo'
         super(Configs, self).__init__()
         self.flags: list = flags
         self.repo: str = repo
 
         self.session = Session
-        self.view = ViewMessage(self.flags)
+        self.view = ViewMessage(flags)
         self.repos = Repositories()
         self.progress = ProgressBar()
         self.utils = Utilities()
         self.data = InstallData()
 
-        self.check_updates = CheckUpdates(
-            self.flags, self.repo
-        )
+        self.check_updates = CheckUpdates(flags, repo)
 
         self.repos_for_update: dict = {}
 
         self.option_for_generate: bool = self.utils.is_option(
-            ['-G', '--generate-only'], self.flags)
+            ['-G', '--generate-only'], flags)
 
         self.option_for_binaries: bool = self.utils.is_option(
-            ['-B', '--bin-repo='], self.flags)
+            ['-B', '--bin-repo='], flags)
 
     def update_the_repositories(self) -> None:
         if not any(list(self.repos_for_update.values())) or self.repo == '*':
             self.view.question()
         else:
             print()
 
@@ -89,15 +85,15 @@
         print()
 
     def slack_repository(self):
         if not self.repos.slack_repo_mirror[0].startswith('file'):
             print(f"Downloading the '{self.green}{self.repos.slack_repo_name}{self.endc}"
                   f"' repository, please wait...\n")
             urls: list = []
-            self.make_dirs(self.repos.slack_repo_name)
+            self.utils.create_directory(self.repos.slack_repo_path)
 
             urls.append(f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_packages}')
             urls.append(f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_changelog}')
             urls.append(f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_checksums}')
 
             self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_packages)
             self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_changelog)
@@ -113,15 +109,15 @@
         print()
 
     def slack_extra_repository(self):
         if not self.repos.slack_extra_repo_mirror[0].startswith('file'):
             print(f"Downloading the '{self.green}{self.repos.slack_extra_repo_name}{self.endc}"
                   f"' repository, please wait...\n")
             urls: list = []
-            self.make_dirs(self.repos.slack_extra_repo_name)
+            self.utils.create_directory(self.repos.slack_extra_repo_path)
 
             urls.append(f'{"".join(self.repos.slack_extra_repo_mirror)}{self.repos.slack_extra_repo_packages}')
             urls.append(f'{self.repos.slack_extra_repo_mirror[0]}{self.repos.slack_extra_repo_changelog}')
             urls.append(f'{self.repos.slack_extra_repo_mirror[0]}{self.repos.slack_extra_repo_checksums}')
 
             self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path,
                                              self.repos.slack_extra_repo_packages)
@@ -140,15 +136,15 @@
         print()
 
     def slack_patches_repository(self):
         if not self.repos.slack_patches_repo_mirror[0].startswith('file'):
             print(f"Downloading the '{self.green}{self.repos.slack_patches_repo_name}{self.endc}"
                   f"' repository, please wait...\n")
             urls: list = []
-            self.make_dirs(self.repos.slack_patches_repo_name)
+            self.utils.create_directory(self.repos.slack_patches_repo_path)
 
             urls.append(f'{"".join(self.repos.slack_patches_repo_mirror)}{self.repos.slack_patches_repo_packages}')
             urls.append(f'{self.repos.slack_patches_repo_mirror[0]}{self.repos.slack_patches_repo_changelog}')
             urls.append(f'{self.repos.slack_patches_repo_mirror[0]}{self.repos.slack_patches_repo_checksums}')
 
             self.utils.remove_file_if_exists(self.repos.slack_patches_repo_path,
                                              self.repos.slack_patches_repo_packages)
@@ -167,15 +163,15 @@
         print()
 
     def alien_repository(self):
         if not self.repos.alien_repo_mirror[0].startswith('file'):
             print(f"Downloading the '{self.green}{self.repos.alien_repo_name}{self.endc}' "
                   f"repository, please wait...\n")
             urls: list = []
-            self.make_dirs(self.repos.alien_repo_name)
+            self.utils.create_directory(self.repos.alien_repo_path)
 
             urls.append(f'{"".join(self.repos.alien_repo_mirror)}{self.repos.alien_repo_packages}')
             urls.append(f'{self.repos.alien_repo_mirror[0]}{self.repos.alien_repo_changelog}')
             urls.append(f'{"".join(self.repos.alien_repo_mirror)}{self.repos.alien_repo_checksums}')
 
             self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_packages)
             self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_changelog)
@@ -191,15 +187,15 @@
         print()
 
     def multilib_repository(self) -> None:
         if not self.repos.multilib_repo_mirror[0].startswith('file'):
             print(f"Downloading the '{self.green}{self.repos.multilib_repo_name}{self.endc}' "
                   f"repository, please wait...\n")
             urls: list = []
-            self.make_dirs(self.repos.multilib_repo_name)
+            self.utils.create_directory(self.repos.multilib_repo_path)
 
             urls.append(f'{"".join(self.repos.multilib_repo_mirror)}{self.repos.multilib_repo_packages}')
             urls.append(f'{self.repos.multilib_repo_mirror[0]}{self.repos.multilib_repo_changelog}')
             urls.append(f'{self.repos.multilib_repo_mirror[0]}{self.repos.multilib_repo_checksums}')
 
             self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_packages)
             self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_changelog)
@@ -215,15 +211,15 @@
         print()
 
     def restricted_repository(self) -> None:
         if not self.repos.restricted_repo_mirror[0].startswith('file'):
             print(f"Downloading the '{self.green}{self.repos.restricted_repo_name}{self.endc}' "
                   f"repository, please wait...\n")
             urls: list = []
-            self.make_dirs(self.repos.restricted_repo_name)
+            self.utils.create_directory(self.repos.restricted_repo_path)
 
             urls.append(f'{"".join(self.repos.restricted_repo_mirror)}{self.repos.restricted_repo_packages}')
             urls.append(f'{self.repos.restricted_repo_mirror[0]}{self.repos.restricted_repo_changelog}')
             urls.append(f'{"".join(self.repos.restricted_repo_mirror)}{self.repos.restricted_repo_checksums}')
 
             self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_packages)
             self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_changelog)
@@ -239,15 +235,15 @@
         print()
 
     def gnome_repository(self) -> None:
         if not self.repos.gnome_repo_mirror[0].startswith('file'):
             print(f"Downloading the '{self.green}{self.repos.gnome_repo_name}{self.endc}' "
                   f"repository, please wait...\n")
             urls: list = []
-            self.make_dirs(self.repos.gnome_repo_name)
+            self.utils.create_directory(self.repos.gnome_repo_path)
 
             urls.append(f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_packages}')
             urls.append(f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_changelog}')
             urls.append(f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_checksums}')
 
             self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_packages)
             self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_changelog)
@@ -263,15 +259,15 @@
         print()
 
     def msb_repository(self) -> None:
         if not self.repos.msb_repo_mirror[0].startswith('file'):
             print(f"Downloading the '{self.green}{self.repos.msb_repo_name}{self.endc}' "
                   f"repository, please wait...\n")
             urls: list = []
-            self.make_dirs(self.repos.msb_repo_name)
+            self.utils.create_directory(self.repos.msb_repo_path)
 
             urls.append(f'{"".join(self.repos.msb_repo_mirror)}{self.repos.msb_repo_packages}')
             urls.append(f'{self.repos.msb_repo_mirror[0]}{self.repos.msb_repo_changelog}')
             urls.append(f'{self.repos.msb_repo_mirror[0]}{self.repos.msb_repo_checksums}')
 
             self.utils.remove_file_if_exists(self.repos.msb_repo_path,
                                              self.repos.msb_repo_packages)
@@ -290,15 +286,15 @@
         print()
 
     def csb_repository(self) -> None:
         if not self.repos.csb_repo_mirror[0].startswith('file'):
             print(f"Downloading the '{self.green}{self.repos.csb_repo_name}{self.endc}' "
                   f"repository, please wait...\n")
             urls: list = []
-            self.make_dirs(self.repos.csb_repo_name)
+            self.utils.create_directory(self.repos.csb_repo_path)
 
             urls.append(f'{"".join(self.repos.csb_repo_mirror)}{self.repos.csb_repo_packages}')
             urls.append(f'{self.repos.csb_repo_mirror[0]}{self.repos.csb_repo_changelog}')
             urls.append(f'{self.repos.csb_repo_mirror[0]}{self.repos.csb_repo_checksums}')
 
             self.utils.remove_file_if_exists(self.repos.csb_repo_path,
                                              self.repos.csb_repo_packages)
@@ -317,15 +313,15 @@
         print()
 
     def conraid_repository(self) -> None:
         if not self.repos.conraid_repo_mirror[0].startswith('file'):
             print(f"Downloading the '{self.green}{self.repos.conraid_repo_name}{self.endc}' "
                   f"repository, please wait...\n")
             urls: list = []
-            self.make_dirs(self.repos.conraid_repo_name)
+            self.utils.create_directory(self.repos.conraid_repo_path)
 
             urls.append(f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_packages}')
             urls.append(f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_changelog}')
             urls.append(f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_checksums}')
 
             self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_packages)
             self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_changelog)
@@ -341,15 +337,15 @@
         print()
 
     def slackonly_repository(self) -> None:
         if not self.repos.slackonly_repo_mirror[0].startswith('file'):
             print(f"Downloading the '{self.green}{self.repos.slackonly_repo_name}{self.endc}' "
                   f"repository, please wait...\n")
             urls: list = []
-            self.make_dirs(self.repos.slackonly_repo_name)
+            self.utils.create_directory(self.repos.slackonly_repo_path)
 
             urls.append(f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_packages}')
             urls.append(f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_changelog}')
             urls.append(f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_checksums}')
 
             self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_packages)
             self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_changelog)
@@ -365,15 +361,15 @@
         print()
 
     def salixos_repository(self) -> None:
         if not self.repos.salixos_repo_mirror[0].startswith('file'):
             print(f"Downloading the '{self.green}{self.repos.salixos_repo_name}{self.endc}' "
                   f"repository, please wait...\n")
             urls: list = []
-            self.make_dirs(self.repos.salixos_repo_name)
+            self.utils.create_directory(self.repos.salixos_repo_path)
 
             urls.append(f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_packages}')
             urls.append(f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_changelog}')
             urls.append(f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_checksums}')
 
             self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_packages)
             self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_changelog)
@@ -389,15 +385,15 @@
         print()
 
     def salixos_extra_repository(self) -> None:
         if not self.repos.salixos_extra_repo_mirror[0].startswith('file'):
             print(f"Downloading the '{self.green}{self.repos.salixos_extra_repo_name}{self.endc}' "
                   f"repository, please wait...\n")
             urls: list = []
-            self.make_dirs(self.repos.salixos_extra_repo_name)
+            self.utils.create_directory(self.repos.salixos_extra_repo_path)
 
             urls.append(f'{"".join(self.repos.salixos_extra_repo_mirror)}{self.repos.salixos_extra_repo_packages}')
             urls.append(f'{self.repos.salixos_extra_repo_mirror[0]}{self.repos.salixos_extra_repo_changelog}')
             urls.append(f'{self.repos.salixos_extra_repo_mirror[0]}{self.repos.salixos_extra_repo_checksums}')
 
             self.utils.remove_file_if_exists(self.repos.salixos_extra_repo_path,
                                              self.repos.salixos_extra_repo_packages)
@@ -416,15 +412,15 @@
         print()
 
     def salixos_patches_repository(self) -> None:
         if not self.repos.salixos_patches_repo_mirror[0].startswith('file'):
             print(f"Downloading the '{self.green}{self.repos.salixos_patches_repo_name}{self.endc}' "
                   f"repository, please wait...\n")
             urls: list = []
-            self.make_dirs(self.repos.salixos_patches_repo_name)
+            self.utils.create_directory(self.repos.slack_patches_repo_path)
 
             urls.append(f'{"".join(self.repos.salixos_patches_repo_mirror)}'
                         f'{self.repos.salixos_patches_repo_packages}')
             urls.append(f'{self.repos.salixos_patches_repo_mirror[0]}{self.repos.salixos_patches_repo_changelog}')
             urls.append(f'{self.repos.salixos_patches_repo_mirror[0]}{self.repos.salixos_patches_repo_checksums}')
 
             self.utils.remove_file_if_exists(self.repos.salixos_patches_repo_path,
@@ -444,15 +440,15 @@
         print()
 
     def slackel_repository(self) -> None:
         if not self.repos.slackel_repo_mirror[0].startswith('file'):
             print(f"Downloading the '{self.green}{self.repos.slackel_repo_name}{self.endc}' "
                   f"repository, please wait...\n")
             urls: list = []
-            self.make_dirs(self.repos.slackel_repo_name)
+            self.utils.create_directory(self.repos.slackel_repo_path)
 
             urls.append(f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_packages}')
             urls.append(f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_changelog}')
             urls.append(f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_checksums}')
 
             self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_packages)
             self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_changelog)
@@ -468,15 +464,15 @@
         print()
 
     def slint_repository(self) -> None:
         if not self.repos.slint_repo_mirror[0].startswith('file'):
             print(f"Downloading the '{self.green}{self.repos.slint_repo_name}{self.endc}' "
                   f"repository, please wait...\n")
             urls: list = []
-            self.make_dirs(self.repos.slint_repo_name)
+            self.utils.create_directory(self.repos.slint_repo_path)
 
             urls.append(f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_packages}')
             urls.append(f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_changelog}')
             urls.append(f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_checksums}')
 
             self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_packages)
             self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_changelog)
@@ -491,55 +487,62 @@
         self.data.install_slint_data()
         print()
 
     def slackbuild_repositories(self) -> None:
         """ Update the slackbuild repositories. """
         if self.repos.ponce_repo:
 
-            if not self.option_for_generate or not self.repos.ponce_repo_mirror[0].startswith('file'):
+            if not self.option_for_generate or self.repos.ponce_repo_mirror[0].startswith('file'):
                 print(f"Downloading the '{self.green}{self.repos.ponce_repo_name}"
                       f"{self.endc}' repository, please wait...\n")
-                self.make_dirs(self.repos.gnome_repo_name)
+
+                self.utils.create_directory(self.repos.ponce_repo_path)
                 self.utils.remove_file_if_exists(self.repos.ponce_repo_path, self.repos.ponce_repo_slackbuilds)
+
                 lftp_command: str = (f'lftp {self.lftp_mirror_options} {self.repos.ponce_repo_mirror[0]} '
                                      f'{self.repos.ponce_repo_path}')
+
                 self.utils.process(lftp_command)
 
             gen_script: Path = Path(self.repos.ponce_repo_path, 'gen_sbo_txt.sh')
-            if gen_script.is_file():
-                # Generating the ponce SLACKBUILDS.TXT file.
-                print(f'Generating the {self.repos.ponce_repo_slackbuilds} file... ', end='', flush=True)
-                os.chdir(self.repos.ponce_repo_path)
-                gen_command: str = f'./gen_sbo_txt.sh > {self.repos.ponce_repo_slackbuilds}'
-                self.utils.process(gen_command)
-                self.delete_last_updated(self.repos.ponce_repo_name)
-                print('\n')
+            if not gen_script.is_file():
+                with open(gen_script, 'w') as file:
+                    file.write(self.__class__.gen_sbo_script.__doc__)
+
+                os.chmod(gen_script, 0o775)
+
+            # Generating the ponce SLACKBUILDS.TXT file.
+            print(f'Generating the {self.repos.ponce_repo_slackbuilds} file... ', end='', flush=True)
+            os.chdir(self.repos.ponce_repo_path)
+            gen_command: str = f'./gen_sbo_txt.sh > {self.repos.ponce_repo_slackbuilds}'
+
+            self.utils.process(gen_command)
+            self.delete_last_updated(self.repos.ponce_repo_name)
+            print('\n')
 
         else:
 
             if not self.repos.sbo_repo_mirror[0].startswith('file'):
                 print(f"Downloading the '{self.green}{self.repos.sbo_repo_name}{self.endc}' "
                       f"repository, please wait...\n")
-                self.make_dirs(self.repos.sbo_repo_name)
+
+                self.utils.create_directory(self.repos.sbo_repo_path)
+
                 self.utils.remove_file_if_exists(self.repos.sbo_repo_path, self.repos.sbo_repo_slackbuilds)
                 self.utils.remove_file_if_exists(self.repos.sbo_repo_path, self.repos.sbo_repo_changelog)
+
                 lftp_command: str = (f'lftp {self.lftp_mirror_options} {self.repos.sbo_repo_mirror[0]} '
                                      f'{self.repos.sbo_repo_path}')
-                self.utils.process(lftp_command)
 
+                self.utils.process(lftp_command)
             self.delete_last_updated(self.repos.sbo_repo_name)
 
         self.delete_sbo_database_data()
         self.data.install_sbos_data()
 
-    def make_dirs(self, repo) -> None:
-        path = Path(self.repos.repositories_path, repo)
-        if not os.path.isdir(path):
-            os.makedirs(path)
-
     def check(self, queue) -> None:
         compare: dict = self.check_updates.check()
 
         print()
         for repo, comp in compare.items():
             if comp:
                 print(f"\n{self.endc}There are new updates available for the "
@@ -592,38 +595,34 @@
         self.session.commit()
 
     def delete_last_updated(self, repo) -> None:
         """ Deletes the last updated date. """
         self.session.query(LastRepoUpdated).where(LastRepoUpdated.repo == repo).delete()
         self.session.commit()
 
-    def drop_the_tables(self) -> None:
-        """ Drop all the tables from the database. """
-        print(f'\n{self.prog_name}: {self.blink}{self.bold}{self.bred}WARNING!{self.endc}: '
-              f'All the data from the database will be deleted!')
-        self.view.question()
-
-        tables: list = [
-            PonceTable.__table__,
-            SBoTable.__table__,
-            BinariesTable.__table__,
-            LastRepoUpdated.__table__
-        ]
-
-        Base.metadata.drop_all(bind=engine, tables=tables)
-
-        # Deletes local downloaded data.
-        self.delete_repositories_data()
-
-        print("Successfully cleared!\n\nYou need to run 'slpkg update' now.")
-
-    def delete_repositories_data(self):
-        """ Deletes local folders with the repository downloaded data. """
-        for repo in self.repos.repositories.keys():
-
-            repo_path: Path = Path(self.repos.repositories_path, repo)
-
-            if repo_path.exists():
-                shutil.rmtree(repo_path)
-                print(f"Deleted: '{repo_path}'")
+    def gen_sbo_script(self):
+        """#!/bin/bash
 
-        print()
+# gen_sbo_txt.sh is a script to build a SLACKBUILDS.TXT file.
+# Thanks to bassmadrigal from LQ forum.
+# https://www.linuxquestions.org/questions/slackware-14/script-for-building-a-slackbuilds-txt-4175598436/
+
+for i in */*; do
+
+  NAME=$(echo $i | cut -d "/" -f2)
+  FILES=$(ls $i)
+  source $i/${NAME}.info
+  DESCRIPTION=$(grep -m 1 $NAME $i/slack-desc | cut -d " " -f2-)
+
+  echo SLACKBUILD NAME: $NAME
+  echo SLACKBUILD LOCATION: ./$i
+  echo SLACKBUILD FILES: $FILES
+  echo SLACKBUILD VERSION: $VERSION
+  echo SLACKBUILD DOWNLOAD: $DOWNLOAD
+  echo SLACKBUILD DOWNLOAD_x86_64: $DOWNLOAD_x86_64
+  echo SLACKBUILD MD5SUM: $MD5SUM
+  echo SLACKBUILD MD5SUM_x86_64: $MD5SUM_x86_64
+  echo SLACKBUILD REQUIRES: $REQUIRES
+  echo SLACKBUILD SHORT DESCRIPTION: $DESCRIPTION
+  echo
+
+done"""
```

### Comparing `slpkg-4.8.1/slpkg/progress_bar.py` & `slpkg-4.8.2/slpkg/progress_bar.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,18 @@
         try:
             spinner = spinners[self.progress_spinner]
             color: str = colors[self.spinner_color]
         except KeyError:
             spinner = PixelSpinner
             color: str = self.endc
 
-        bar_spinner = spinner(f'{self.endc}{message} {filename} {color}')
-        # print('\033[F', end='', flush=True)
-        try:
-            while True:
-                time.sleep(0.1)
-                bar_spinner.next()
-        except KeyboardInterrupt:
-            raise SystemExit(1)
+        if self.spinning_bar:
+            bar_spinner = spinner(f'{self.endc}{message} {filename} {color}')
+            # print('\033[F', end='', flush=True)
+            try:
+                while True:
+                    time.sleep(0.1)
+                    bar_spinner.next()
+            except KeyboardInterrupt:
+                raise SystemExit(1)
+        else:
+            print(f'{message} ', end='', flush=True)
```

### Comparing `slpkg-4.8.1/slpkg/downloader.py` & `slpkg-4.8.2/slpkg/downloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import shutil
 from typing import Union
 from pathlib import Path
-from urllib.parse import unquote
 from multiprocessing import Process
+from urllib.parse import unquote, urlparse
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.error_messages import Errors
 
 
 class Downloader(Configs):
@@ -21,56 +21,55 @@
         self.urls: list = urls
         self.flags: list = flags
 
         self.errors = Errors()
         self.utils = Utilities()
 
         self.option_for_parallel: bool = self.utils.is_option(
-            ['-P', '--parallel'], self.flags)
+            ['-P', '--parallel'], flags)
 
     def download(self) -> None:
         """ Starting the processing for downloading. """
         process: list = []
 
         if self.parallel_downloads or self.option_for_parallel:
             for url in self.urls:
-                p1 = Process(target=self.tools, args=(url,))
+                p1 = Process(target=self.tool, args=(url,))
                 process.append(p1)
                 p1.start()
 
             for proc in process:
                 proc.join()
         else:
             for url in self.urls:
-                self.tools(url)
+                self.tool(url)
 
-    def tools(self, url: str) -> None:
-        """ Downloader tools wget, curl and lftp. """
+    def tool(self, url: str) -> None:
+        """ Downloader tools wget, wget2, curl and lftp. """
         command: str = ''
-        filename: str = url.split('/')[-1]
+        path: str = urlparse(url).path
+        filename: str = unquote(Path(path).name)
 
         if url.startswith('file'):
             shutil.copy2(url[7:], self.tmp_slpkg)
         else:
             if self.downloader in ['wget', 'wget2']:
                 command: str = f'{self.downloader} {self.wget_options} --directory-prefix={self.path} "{url}"'
 
             elif self.downloader == 'curl':
                 command: str = f'{self.downloader} {self.curl_options} "{url}" --output {self.path}/{filename}'
 
             elif self.downloader == 'lftp':
                 command: str = f'{self.downloader} {self.lftp_get_options} {url} -o {self.path}'
 
             else:
-                self.errors.raise_error_message(f"Downloader '{self.downloader}' not supported")
+                self.errors.raise_error_message(f"Downloader '{self.downloader}' not supported", exit_status=1)
 
         self.utils.process(command)
-        self.check_if_downloaded(url)
+        self.check_if_downloaded(url, filename)
 
-    def check_if_downloaded(self, url: str) -> None:
+    def check_if_downloaded(self, url: str, filename: str) -> None:
         """ Checks if the file downloaded. """
-        url: str = unquote(url)
-        file: str = url.split('/')[-1]
-        path_file: Path = Path(self.path, file)
+        path_file: Path = Path(self.path, filename)
 
         if not path_file.exists():
-            self.errors.raise_error_message(f"Download the '{file}' file")
+            self.errors.raise_error_message(f"Download the '{url}' file", exit_status=20)
```

### Comparing `slpkg-4.8.1/slpkg/models/models.py` & `slpkg-4.8.2/slpkg/models/models.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/slpkg/views/view_package.py` & `slpkg-4.8.2/slpkg/views/view_package.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         if self.repos.ponce_repo:
             self.sbo_table = PonceTable
             self.repo_url: str = self.repos.ponce_repo_mirror[0]
             self.repo_path: Path = self.repos.ponce_repo_path
             self.repo_tar_suffix: str = ''
 
         self.option_for_pkg_version: bool = self.utils.is_option(
-            ['-p', '--pkg-version'], self.flags)
+            ['-p', '--pkg-version'], flags)
 
     def slackbuild(self, data: dict, slackbuilds: list) -> None:
         """ View the packages from the repository. """
         slackbuilds: list = self.utils.apply_package_pattern(data, slackbuilds)
 
         for sbo in slackbuilds:
```

### Comparing `slpkg-4.8.1/slpkg/views/version.py` & `slpkg-4.8.2/slpkg/views/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 class Version:
     """ Print the version. """
 
     def __init__(self):
-        self.version_info: tuple = (4, 8, 1)
+        self.version_info: tuple = (4, 8, 2)
         self.version: str = '{0}.{1}.{2}'.format(*self.version_info)
         self.license: str = 'MIT License'
         self.author: str = 'Dimitris Zlatanidis (dslackw)'
         self.homepage: str = 'https://dslackw.gitlab.io/slpkg'
 
     def view(self) -> None:
         """ Prints the version. """
```

### Comparing `slpkg-4.8.1/slpkg/views/cli_menu.py` & `slpkg-4.8.2/slpkg/views/cli_menu.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 from typing import NoReturn
 from slpkg.configs import Configs
+from slpkg.views.version import Version
 
 
 class Usage(Configs):
 
     def __init__(self):
         super(Configs, self).__init__()
 
@@ -20,50 +21,51 @@
 
         print(args)
         raise SystemExit(1)
 
     def help_short(self, status: int) -> NoReturn:
         """ Prints the short menu. """
         args: str = (
-            f'Usage: {self.prog_name} [{self.cyan}COMMAND{self.endc}] [{self.yellow}OPTIONS{self.endc}] '
+            f'USAGE: {self.prog_name} [{self.cyan}COMMAND{self.endc}] [{self.yellow}OPTIONS{self.endc}] '
             f'[FILELIST|PACKAGES...]\n'
             f'\n  slpkg [{self.cyan}COMMAND{self.endc}] [-u, update, -U, upgrade, -c, check-updates, -I, repo-info]\n'
-            f'  slpkg [{self.cyan}COMMAND{self.endc}] [-L, clean-logs, -T, clean-data, -D, clean-tmp, -g, configs]\n'
-            f'  slpkg [{self.cyan}COMMAND{self.endc}] [-b, build, -i, install, -d, download [packages...]]\n'
-            f'  slpkg [{self.cyan}COMMAND{self.endc}] [-R, remove, -f, find, -w, view [packages...]]\n'
+            f'  slpkg [{self.cyan}COMMAND{self.endc}] [-g, configs, -L, clean-logs, -T, clean-data, -D, clean-tmp]\n'
+            f'  slpkg [{self.cyan}COMMAND{self.endc}] [-b, build, -i, install, -R, remove [packages...]]\n'
+            f'  slpkg [{self.cyan}COMMAND{self.endc}] [-d, download, -f, find, -w, view [packages...]]\n'
             f'  slpkg [{self.cyan}COMMAND{self.endc}] [-s, search, -e, dependees, -t, tracking  [packages...]]\n'
             f'  slpkg [{self.yellow}OPTIONS{self.endc}] [-y, --yes, -j, --jobs, -o, --resolve-off, -r, --reinstall]\n'
             f'  slpkg [{self.yellow}OPTIONS{self.endc}] [-k, --skip-installed, -E, --full-reverse, -S, --search]\n'
             f'  slpkg [{self.yellow}OPTIONS{self.endc}] [-n, --no-silent, -p, --pkg-version, -G, --generate-only]\n'
             f'  slpkg [{self.yellow}OPTIONS{self.endc}] [-P, --parallel, -B, --bin-repo=[REPO]]\n'
             f'  slpkg [{self.yellow}OPTIONS{self.endc}] [-z, --directory=[PATH]]\n'
             "  \nIf you need more information please try 'slpkg --help'.")
 
         print(args)
         raise SystemExit(status)
 
     def help(self, status: int) -> NoReturn:
         """ Prints the main menu. """
         args: str = (
-            f'{self.bold}USAGE:{self.endc} {self.prog_name} [{self.cyan}COMMAND{self.endc}] '
+            f'{self.prog_name} - version {Version().version}\n\n'
+            f'{self.bold}USAGE:{self.endc}\n  {self.prog_name} [{self.cyan}COMMAND{self.endc}] '
             f'[{self.yellow}OPTIONS{self.endc}] [FILELIST|PACKAGES...]\n'
-            f'\n{self.bold}DESCRIPTION:{self.endc} Package manager utility for Slackware.\n'
+            f'\n{self.bold}DESCRIPTION:{self.endc}\n  Package manager utility for Slackware.\n'
             f'\n{self.bold}COMMANDS:{self.endc}\n'
             f'  {self.red}-u, update{self.endc}                    Update the package lists.\n'
             f'  {self.cyan}-U, upgrade{self.endc}                   Upgrade all the packages.\n'
             f'  {self.cyan}-c, check-updates{self.endc}             Check for news on ChangeLog.txt.\n'
             f'  {self.cyan}-I, repo-info{self.endc}                 Prints the repositories information.\n'
             f'  {self.cyan}-g, configs{self.endc}                   Edit the configuration file.\n'
             f'  {self.cyan}-L, clean-logs{self.endc}                Clean dependencies log tracking.\n'
             f'  {self.cyan}-T, clean-data{self.endc}                Clean all the repositories data.\n'
             f'  {self.cyan}-D, clean-tmp{self.endc}                 Delete all the downloaded sources.\n'
             f'  {self.cyan}-b, build{self.endc} [packages...]       Build only the packages.\n'
             f'  {self.cyan}-i, install{self.endc} [packages...]     Build and install the packages.\n'
-            f'  {self.cyan}-d, download{self.endc} [packages...]    Download only the scripts and sources.\n'
             f'  {self.cyan}-R, remove{self.endc} [packages...]      Remove installed packages.\n'
+            f'  {self.cyan}-d, download{self.endc} [packages...]    Download only the scripts and sources.\n'
             f'  {self.cyan}-f, find{self.endc} [packages...]        Find installed packages.\n'
             f'  {self.cyan}-w, view{self.endc} [packages...]        View packages from the repository.\n'
             f'  {self.cyan}-s, search{self.endc} [packages...]      Search packages from the repository.\n'
             f'  {self.cyan}-e, dependees{self.endc} [packages...]   Show which packages depend on.\n'
             f'  {self.cyan}-t, tracking{self.endc} [packages...]    Tracking the packages dependencies.\n'
             f'\n{self.bold}OPTIONS:{self.endc}\n'
             f'  {self.yellow}-y, --yes{self.endc}                     Answer Yes to all questions.\n'
```

### Comparing `slpkg-4.8.1/slpkg/views/ascii.py` & `slpkg-4.8.2/slpkg/views/ascii.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/slpkg/views/help_commands.py` & `slpkg-4.8.2/slpkg/views/help_commands.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/slpkg/views/views.py` & `slpkg-4.8.2/slpkg/views/views.py`

 * *Files 26% similar despite different names*

```diff
@@ -24,33 +24,33 @@
         self.flags: list = flags
         self.data: dict = data
 
         self.session = Session
         self.utils = Utilities()
         self.dialogbox = DialogBox()
         self.ascii = Ascii()
-        self.upgrade = Upgrade(self.flags, self.data)
+        self.upgrade = Upgrade(flags, data)
         self.repos = Repositories()
 
         self.download_only: Path = self.tmp_slpkg
         self.installed_packages: list = []
 
         self.option_for_resolve_off: bool = self.utils.is_option(
-            ['-o', '--resolve-off'], self.flags)
+            ['-o', '--resolve-off'], flags)
 
         self.option_for_reinstall: bool = self.utils.is_option(
-            ['-r', '--reinstall'], self.flags)
+            ['-r', '--reinstall'], flags)
 
         self.option_for_yes: bool = self.utils.is_option(
-            ['-y', '--yes'], self.flags)
+            ['-y', '--yes'], flags)
 
         self.option_for_binaries: bool = self.utils.is_option(
-            ['-B', '--bin-repo='], self.flags)
+            ['-B', '--bin-repo='], flags)
 
-        self.repo: str = self.utils.repository_name(self.data)
+        self.repo: str = self.utils.repository_name(data)
 
     def view_packages(self, package: str, mode: str) -> None:
         """ Printing the main packages. """
         size: str = ''
         color: str = self.red
 
         if self.option_for_binaries:
@@ -79,15 +79,15 @@
                 and self.option_for_reinstall):
             color: str = self.violet
 
         self.ascii.draw_view_package(package, version, size, color, self.repo)
 
     def view_skipping_packages(self, package: str, version: str) -> None:
         """ Print the skipping packages. """
-        print(f'[{self.yellow}Skipping{self.endc}] {package}-{version} {self.red}(already installed){self.endc}')
+        print(f'{self.yellow}Skipping{self.endc}: {package}-{version} {self.red}(already installed){self.endc}')
 
     def build_packages(self, slackbuilds: list, dependencies: list) -> None:
         """ View packages for build only. """
         self.ascii.draw_package_title_box('The following packages will be build:', 'slpkg build packages')
 
         for sbo in slackbuilds:
             self.view_packages(sbo, mode='build')
@@ -178,15 +178,17 @@
         """ View and creates list with packages for remove. """
         installed = self.utils.is_package_installed(name)
 
         if installed:
             pkg: list = self.utils.split_binary_pkg(installed)
             self.installed_packages.append(installed)
             size: str = self.utils.get_file_size(Path(self.log_packages, installed))
-            self.ascii.draw_view_package(pkg[0], pkg[1], size, self.red, repo='')
+
+            self.ascii.draw_view_package(pkg[0], pkg[1], size, self.red,
+                                         repo=pkg[4].lower().replace('_', ''))
 
     def choose_dependencies_for_remove(self, dependencies: list) -> list:
         """ Choose packages for remove using the dialog box. """
         height: int = 10
         width: int = 70
         list_height: int = 0
         choices: list = []
@@ -207,24 +209,30 @@
 
         os.system('clear')
         return tags
 
     def summary(self, packages: list, dependencies: list, option: str) -> None:
         """ View the status of the packages action. """
         packages.extend(dependencies)
-        install = upgrade = remove = 0
+        install = upgrade = remove = size_comp = size_uncomp = size_rmv = 0
 
         for pkg in packages:
+            installed: str = self.utils.is_package_installed(pkg)
+
+            if self.option_for_binaries:
+                size_comp += int(''.join(re.findall(r'\d+', self.data[pkg][4])))
+                size_uncomp += int(''.join(re.findall(r'\d+', self.data[pkg][5])))
+
+            if installed and option == 'remove':
+                size_rmv += Path(self.log_packages, installed).stat().st_size
 
             upgradeable: bool = False
             if option != 'remove':
                 upgradeable: bool = self.upgrade.is_package_upgradeable(pkg)
 
-            installed: str = self.utils.is_package_installed(pkg)
-
             if not installed:
                 install += 1
             elif installed and self.option_for_reinstall:
                 upgrade += 1
             elif installed and upgradeable and self.option_for_reinstall:
                 upgrade += 1
             elif installed and upgradeable:
@@ -232,38 +240,44 @@
             elif installed and option == 'remove':
                 remove += 1
 
         self.ascii.draw_bottom_line()
 
         if option in ['install', 'upgrade']:
             print(f'{self.grey}Total {install} packages will be '
-                  f'installed and {upgrade} will be upgraded.{self.endc}')
+                  f'installed and {upgrade} will be upgraded, and total '
+                  f'{self.utils.convert_file_sizes(size_comp)} will be downloaded and '
+                  f'{self.utils.convert_file_sizes(size_uncomp)} will be installed.{self.endc} ')
 
         elif option == 'build':
             print(f'{self.grey}Total {len(packages)} packages '
                   f'will be build in {self.tmp_path} folder.{self.endc}')
 
         elif option == 'remove':
             print(f'{self.grey}Total {remove} packages '
-                  f'will be removed.{self.endc}')
+                  f'will be removed and {self.utils.convert_file_sizes(size_rmv)} '
+                  f'of space will be freed up.{self.endc}')
 
         elif option == 'download':
-            print(f'{self.grey}{len(packages)} packages '
+            print(f'{self.grey}Total {len(packages)} packages and {self.utils.convert_file_sizes(size_comp)} '
                   f'will be downloaded in {self.download_only} folder.{self.endc}')
 
     def logs_packages(self, dependencies: list) -> None:
         """ View the logging packages. """
         print('The following logs will be removed:\n')
 
         for dep in dependencies:
             print(f'{self.yellow}{dep[0]}{self.endc}')
             self.ascii.draw_log_package(dep[1])
 
         print('Note: After cleaning you should remove them one by one.')
 
     def question(self) -> None:
         """ Manage to proceed. """
-        if not self.option_for_yes and self.ask_question:
-            answer: str = input('\nDo you want to continue? [y/N] ')
-            if answer not in ['Y', 'y']:
-                raise SystemExit()
-        print()
+        try:
+            if not self.option_for_yes and self.ask_question:
+                answer: str = input('\nDo you want to continue? [y/N] ')
+                if answer not in ['Y', 'y']:
+                    raise SystemExit()
+            print()
+        except KeyboardInterrupt:
+            raise SystemExit()
```

### Comparing `slpkg-4.8.1/slpkg/checks.py` & `slpkg-4.8.2/slpkg/checks.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.errors = Errors()
         self.utils = Utilities()
         self.repos = Repositories()
 
         self.session = Session
 
         self.option_for_binaries: bool = self.utils.is_option(
-            ['-B', '--bin-repo='], self.flags)
+            ['-B', '--bin-repo='], flags)
 
         if self.option_for_binaries:
             self.repo_table = BinariesTable
         else:
             self.repo_table = SBoTable
             if self.repos.ponce_repo:
                 self.repo_table = PonceTable
@@ -47,46 +47,49 @@
                 if not self.data.get(pkg) and pkg != '*':
                     not_packages.append(pkg)
             else:
                 if not self.data.get(pkg) and pkg != '*':
                     not_packages.append(pkg)
 
         if not_packages:
-            self.errors.raise_error_message(f"Packages '{', '.join(not_packages)}' does not exists")
+            self.errors.raise_error_message(f"Packages '{', '.join(not_packages)}' does not exists",
+                                            exit_status=1)
 
     def is_package_unsupported(self, slackbuilds: list) -> None:
         """ Checking for unsupported slackbuilds. """
         for sbo in slackbuilds:
             if sbo != '*':
                 if self.os_arch == 'x86_64' and self.data[sbo][4]:
                     sources: list = self.data[sbo][4].split()
                 else:
                     sources: list = self.data[sbo][3].split()
 
                 if 'UNSUPPORTED' in sources:
-                    self.errors.raise_error_message(f"Package '{sbo}' unsupported by arch")
+                    self.errors.raise_error_message(f"Package '{sbo}' unsupported by arch",
+                                                    exit_status=1)
 
     def is_installed(self, packages: list) -> None:
         """ Checking for installed packages. """
         not_found: list = []
 
         for pkg in packages:
-            package: str = self.utils.is_package_installed(pkg)
-            if not package:
+            if not self.utils.is_package_installed(pkg):
                 not_found.append(pkg)
 
         if not_found:
-            self.errors.raise_error_message(f'Not found \'{", ".join(not_found)}\' installed packages')
+            self.errors.raise_error_message(f'Not found \'{", ".join(not_found)}\' installed packages',
+                                            exit_status=1)
 
     def is_empty_database(self, repo: str) -> None:
         """ Checking for empty table and database file. """
         db = Path(self.db_path, self.database_name)
 
         if self.option_for_binaries and repo != '*':
             count: int = self.session.query(self.repo_table.id).where(self.repo_table.repo == repo).count()
         else:
             count: int = self.session.query(self.repo_table.id).count()
 
         if not self.session.query(self.repo_table).first() or not db.is_file() or count == 0:
             self.errors.raise_error_message("You need to update the package lists first, run:\n\n"
-                                            "              $ 'slpkg update'\n"
-                                            "              $ 'slpkg update --bin-repo='*' for binaries")
+                                            "              $ slpkg update\n"
+                                            "              $ slpkg update --bin-repo=[repo_name] for binaries",
+                                            exit_status=1)
```

### Comparing `slpkg-4.8.1/slpkg/configs.py` & `slpkg-4.8.2/slpkg/configs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
-import os
 import tomli
 import platform
 from pathlib import Path
 from dataclasses import dataclass
 
 from slpkg.logging_config import LoggingConfig
 from slpkg.toml_error_message import TomlErrors
@@ -14,15 +13,15 @@
 @dataclass
 class Configs:
     """ Default configurations. """
     errors = TomlErrors()
 
     prog_name: str = 'slpkg'
     os_arch: str = platform.machine()
-    tmp_path: str = '/tmp/'
+    tmp_path: Path = Path('/tmp')
     tmp_slpkg: Path = Path(tmp_path, prog_name)
     build_path: Path = Path(tmp_path, prog_name, 'build')
     download_only_path: Path = Path(tmp_slpkg, '')
     lib_path: Path = Path('/var/lib', prog_name)
     etc_path: Path = Path('/etc', prog_name)
     db_path: Path = Path(lib_path, 'database')
     log_packages: Path = Path('/var', 'log', 'packages')
@@ -40,33 +39,34 @@
     lftp_get_options: str = '-c get -e'
     lftp_mirror_options: str = '-c mirror --parallel=100 --only-newer'
     silent_mode: bool = True
     ascii_characters: bool = True
     ask_question: bool = True
     parallel_downloads: bool = False
     file_pattern: str = '*'
+    spinning_bar: str = True
     progress_spinner: str = 'pixel'
     spinner_color: str = 'green'
 
     proxy_address: str = ''
     proxy_username: str = ''
     proxy_password: str = ''
 
     try:
+        # Load user configuration.
         config_path_file = Path(etc_path, f'{prog_name}.toml')
-
         if config_path_file.exists():
             with open(config_path_file, 'rb') as conf:
                 configs = tomli.load(conf)
 
         if configs:
             config = configs['CONFIGS']
 
             os_arch: str = config['OS_ARCH']
-            download_only_path: Path = config['DOWNLOAD_ONLY_PATH']
+            download_only_path: Path = Path(config['DOWNLOAD_ONLY_PATH'])
             ask_question: bool = config['ASK_QUESTION']
             installpkg: str = config['INSTALLPKG']
             reinstall: str = config['REINSTALL']
             removepkg: str = config['REMOVEPKG']
             colors: bool = config['COLORS']
             dialog: str = config['DIALOG']
             downloader: str = config['DOWNLOADER']
@@ -75,14 +75,15 @@
             lftp_get_options: str = config['LFTP_GET_OPTIONS']
             lftp_mirror_options: str = config['LFTP_MIRROR_OPTIONS']
             silent_mode: bool = config['SILENT_MODE']
             ascii_characters: bool = config['ASCII_CHARACTERS']
             file_list_suffix: str = config['FILE_LIST_SUFFIX']
             parallel_downloads: bool = config['PARALLEL_DOWNLOADS']
             file_pattern_conf: str = config['FILE_PATTERN']
+            spinning_bar: str = config['SPINNING_BAR']
             progress_spinner: str = config['PROGRESS_SPINNER']
             spinner_color: str = config['SPINNER_COLOR']
             proxy_address: str = config['PROXY_ADDRESS']
             proxy_username: str = config['PROXY_USERNAME']
             proxy_password: str = config['PROXY_PASSWORD']
 
     except (KeyError, tomli.TOMLDecodeError) as error:
@@ -125,9 +126,9 @@
         build_path,
         tmp_slpkg,
         download_only_path,
         LoggingConfig.log_path
     ]
 
     for path in paths:
-        if not os.path.isdir(path):
-            os.makedirs(path)
+        if not path.is_dir():
+            path.mkdir(parents=True, exist_ok=True)
```

### Comparing `slpkg-4.8.1/slpkg/clean_logs.py` & `slpkg-4.8.2/slpkg/logging_deps.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,44 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
-from slpkg.views.views import ViewMessage
+from slpkg.utilities import Utilities
+from slpkg.binaries.required import Required
+from slpkg.sbos.dependencies import Requires
 from slpkg.models.models import LogsDependencies
 from slpkg.models.models import session as Session
 
 
-class CleanLogsDependencies:
-    """ Cleans the logs from packages. """
+class LoggingDeps:
+    """ Logging installed dependencies. """
 
-    def __init__(self, flags: list):
-        __slots__ = 'flags'
+    def __init__(self, flags: list, data: dict):
+        __slots__ = 'flags', 'data'
         self.flags: list = flags
+        self.data: dict = data
+
+        self.utils = Utilities()
         self.session = Session
 
-    def clean(self) -> None:
-        """ Deletes the log table from the database. """
-        dependencies: list = self.session.query(
-            LogsDependencies.name, LogsDependencies.requires).all()  # type: ignore
-
-        if dependencies:
-            view = ViewMessage(self.flags)
-            view.logs_packages(dependencies)
-            view.question()
+        self.option_for_binaries: bool = self.utils.is_option(
+            ['-B', '--bin-repo='], flags)
+
+    def logging(self, name: str) -> None:
+        exist = self.session.query(LogsDependencies.name).filter(
+            LogsDependencies.name == name).first()
 
-            self.session.query(LogsDependencies).delete()
-            self.session.commit()
+        if self.option_for_binaries:
+            requires: list = Required(self.data, name).resolve()
         else:
-            print('\nNothing to clean.\n')
+            requires: list = Requires(self.data, name).resolve()
+
+        # Update the dependencies if exist else create it.
+        if exist:
+            self.session.query(
+                LogsDependencies).filter(
+                LogsDependencies.name == name).update(
+                {LogsDependencies.requires: ' '.join(requires)})
+
+        elif requires:
+            deps: list = LogsDependencies(name=name, requires=' '.join(requires))
+            self.session.add(deps)
+        self.session.commit()
```

### Comparing `slpkg-4.8.1/slpkg/utilities.py` & `slpkg-4.8.2/slpkg/utilities.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import re
 import time
 import shutil
-import logging
 import fnmatch
+import logging
 import subprocess
 from pathlib import Path
-from typing import Generator, Union
+from typing import Generator
 
 from slpkg.configs import Configs
 from slpkg.blacklist import Blacklist
 from slpkg.error_messages import Errors
 from slpkg.repositories import Repositories
 from slpkg.logging_config import LoggingConfig
 
@@ -23,41 +23,32 @@
         self.black = Blacklist()
         self.errors = Errors()
         self.repos = Repositories()
 
         self.installed_packages: dict = dict(self.all_installed())
 
         logging.basicConfig(filename=LoggingConfig.log_file,
-                            filemode='w',
-                            encoding='utf-8',
-                            level=logging.INFO)
+                            filemode=LoggingConfig.filemode,
+                            encoding=LoggingConfig.encoding,
+                            level=LoggingConfig.level)
 
     def is_package_installed(self, name: str) -> str:
         """ Returns the installed package binary. """
         try:
             return self.installed_packages[name]
         except KeyError:
             return ''
 
     def all_installed(self) -> dict:
         """ Return all installed packages from /val/log/packages folder. """
-        var_log_packages: Path = Path(self.log_packages)
-
-        try:
-            for file in var_log_packages.glob(self.file_pattern):
-                name = self.split_binary_pkg(file.name)[0]
-
-                if not name.startswith('.') and not self.blacklist_pattern(name):
-                    yield name, file.name
+        for file in self.log_packages.glob(self.file_pattern):
+            name: str = self.split_binary_pkg(file.name)[0]
 
-        except ValueError as err:
-            logger = logging.getLogger(__name__)
-            logger.info('%s: %s: %s', self.__class__.__name__,
-                        Utilities.all_installed.__name__,
-                        err)
+            if not name.startswith('.') and not self.blacklist_pattern(name):
+                yield name, file.name
 
     @staticmethod
     def remove_file_if_exists(path: Path, file: str) -> None:
         """ Clean the old files. """
         archive = Path(path, file)
         if archive.is_file():
             archive.unlink()
@@ -65,50 +56,49 @@
     @staticmethod
     def remove_folder_if_exists(folder: Path) -> None:
         """ Clean the old folders. """
         if folder.exists():
             shutil.rmtree(folder)
 
     @staticmethod
-    def create_folder(path: Path, folder: str) -> None:
-        """ Creates folder. """
-        directory = Path(path, folder)
-        if not directory.exists():
+    def create_directory(directory: Path) -> None:
+        """ Creates folder like mkdir -p. """
+        if not directory.is_dir():
             directory.mkdir(parents=True, exist_ok=True)
 
     @staticmethod
     def split_binary_pkg(package: str) -> list:
         """ Split the package by the name, version, arch, build and tag. """
         name: str = '-'.join(package.split('-')[:-3])
         version: str = ''.join(package[len(name):].split('-')[:-2])
         arch: str = ''.join(package[len(name + version) + 2:].split('-')[:-1])
         build_tag: str = package.split('-')[-1]
         build: str = ''.join(re.findall(r'\d+', build_tag[:2]))
+        pkg_tag: str = build_tag[len(build):]
 
-        return [name, version, arch, build]
+        return [name, version, arch, build, pkg_tag]
 
     def finished_time(self, elapsed_time: float) -> None:
         """ Printing the elapsed time. """
-        print(f'\n{self.yellow}Finished Successfully:{self.endc}',
+        print(f'\n{self.yellow}Finished successfully:{self.endc}',
               time.strftime(f'{self.cyan}%H:%M:%S{self.endc}',
                             time.gmtime(elapsed_time)))
 
     def read_sbo_build_tag(self, sbo: str, location: str) -> str:
         """ Returns build tag from .SlackBuild file. """
         build: str = ''
 
         sbo_script = Path(self.repos.sbo_repo_path, location, sbo, f'{sbo}.SlackBuild')
 
         if sbo_script.is_file():
-            with open(sbo_script, 'r', encoding='utf-8') as f:
-                lines = f.readlines()
+            lines = self.read_file(sbo_script)
 
-                for line in lines:
-                    if line.startswith('BUILD=$'):
-                        build = ''.join(re.findall(r'\d+', line))
+            for line in lines:
+                if line.startswith('BUILD=$'):
+                    build = ''.join(re.findall(r'\d+', line))
 
         return build
 
     @staticmethod
     def is_option(flag: list, flags: list) -> bool:
         """ Checking for flags. """
         for f in flag:
@@ -127,36 +117,45 @@
                 if package and not package.startswith('#'):
                     if '#' in package:
                         package = package.split('#')[0].strip()
 
                     yield package
 
         except FileNotFoundError:
-            self.errors.raise_error_message(f"No such file or directory: '{file}'")
+            logger = logging.getLogger(LoggingConfig.date)
+            logger.exception(f'{self.__class__.__name__}: '
+                             f'{self.__class__.read_packages_from_file.__name__}')
+            self.errors.raise_error_message(f"No such file or directory: '{file}'", exit_status=20)
 
-    @staticmethod
-    def read_file(file: Union[str, Path]) -> list:
+    def read_file(self, file: Path) -> list:
         """ Reads the text file. """
-        with open(file, 'r', encoding='utf-8', errors='replace') as f:
-            return f.readlines()
+        try:
+            with open(file, 'r', encoding='utf-8', errors='replace') as f:
+                return f.readlines()
+        except FileNotFoundError:
+            logger = logging.getLogger(LoggingConfig.date)
+            logger.exception(f'{self.__class__.__name__}: '
+                             f'{self.__class__.read_file.__name__}')
+            self.errors.raise_error_message(f"No such file or directory: '{file}'", exit_status=20)
 
-    @staticmethod
-    def process(command: str, stderr=None, stdout=None) -> None:
+    def process(self, command: str, stderr=None, stdout=None) -> None:
         """ Handle the processes. """
         try:
-            output = subprocess.call(command, shell=True, stderr=stderr, stdout=stdout)
-        except (KeyboardInterrupt, subprocess.CalledProcessError) as err:
-            raise SystemExit(err)
-
-        if output != 0:
-            raise SystemExit(output)
+            subprocess.call(command, shell=True, stderr=stderr, stdout=stdout)
+        except subprocess.CalledProcessError as error:
+            logger = logging.getLogger(LoggingConfig.date)
+            logger.exception(f'{self.__class__.__name__}'
+                             f'{self.__class__.process.__name__}')
+            self.errors.raise_error_message(str(error), exit_status=20)
+        except KeyboardInterrupt:
+            raise SystemExit(1)
 
     def get_file_size(self, file: Path) -> str:
         """ Get the local file size and converted to units. """
-        size = Path(file).stat().st_size
+        size: int = file.stat().st_size
         return self.convert_file_sizes(size)
 
     @staticmethod
     def convert_file_sizes(size: int) -> str:
         """ Convert file sizes. """
         units: list = ['KB', 'MB', 'GB']
 
@@ -172,20 +171,20 @@
 
             if pkg == '*':
                 packages.remove(pkg)
                 packages += list(data.keys())
 
         return packages
 
-    def blacklist_pattern(self, name):
+    def blacklist_pattern(self, name: str) -> bool:
         """ This module provides support for Unix shell-style wildcards. """
         if [black for black in self.black.packages() if fnmatch.fnmatch(name, black)]:
             return True
 
-    def repository_name(self, data):
+    def repository_name(self, data: dict) -> str:
         """ Get the binary repository name from the repository data. """
         try:
             # Binary repository name
             repo: list = list(data.values())[0][11]
         except (IndexError, AttributeError):
             # Slackbuilds repository name 'sbo | ponce'
             repo: str = self.repos.sbo_enabled_repo_name
```

### Comparing `slpkg-4.8.1/slpkg/dependees.py` & `slpkg-4.8.2/slpkg/dependees.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,21 @@
         self.utils = Utilities()
 
         self.llc: str = self.ascii.lower_left_corner
         self.hl: str = self.ascii.horizontal_line
         self.var: str = self.ascii.vertical_and_right
 
         self.option_for_full_reverse: bool = self.utils.is_option(
-            ['-E', '--full-reverse'], self.flags)
+            ['-E', '--full-reverse'], flags)
 
         self.option_for_pkg_version: bool = self.utils.is_option(
-            ['-p', '--pkg-version'], self.flags)
+            ['-p', '--pkg-version'], flags)
 
         self.option_for_binaries: bool = self.utils.is_option(
-            ['-B', '--bin-repo='], self.flags)
+            ['-B', '--bin-repo='], flags)
 
     def find(self) -> None:
         """ Collecting the dependees. """
         print(f"The list below shows the "
               f"packages that dependees on '{', '.join([p for p in self.packages])}':\n")
 
         self.packages: list = self.utils.apply_package_pattern(self.data, self.packages)
```

### Comparing `slpkg-4.8.1/slpkg/check_updates.py` & `slpkg-4.8.2/slpkg/check_updates.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import os
+import logging
 from pathlib import Path
 from multiprocessing import Process
 from urllib3 import PoolManager, ProxyManager, make_headers
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.progress_bar import ProgressBar
 from slpkg.repositories import Repositories
+from slpkg.logging_config import LoggingConfig
 
 
 class CheckUpdates(Configs):
     """ Check for changes in the ChangeLog file. """
 
     def __init__(self, flags: list, repo: str):
         __slots__ = 'flags', 'repo'
         super(Configs, self).__init__()
         self.flags: list = flags
         self.repo: str = repo
+
         self.utils = Utilities()
         self.progress = ProgressBar()
         self.repos = Repositories()
 
         self.compare: dict = {}
-        self.local_chg_txt = None
-        self.repo_chg_txt = None
 
         self.option_for_binaries: bool = self.utils.is_option(
-            ['-B', '--bin-repo='], self.flags)
+            ['-B', '--bin-repo='], flags)
+
+        logging.basicConfig(filename=LoggingConfig.log_file,
+                            filemode=LoggingConfig.filemode,
+                            encoding=LoggingConfig.encoding,
+                            level=LoggingConfig.level)
 
     def check(self) -> dict:
         if self.option_for_binaries:
 
             for repo in list(self.repos.repositories.keys())[2:]:
 
                 if self.repos.repositories[repo][0] and repo == self.repo:
@@ -80,27 +86,37 @@
                 http = ProxyManager(f'{self.proxy_address}', headers=proxy_default_headers)
 
             elif self.proxy_address.startswith('socks'):
                 # https://urllib3.readthedocs.io/en/stable/advanced-usage.html#socks-proxies
                 try:  # Try to import PySocks if it's installed.
                     from urllib3.contrib.socks import SOCKSProxyManager
                 except (ModuleNotFoundError, ImportError):
+                    logger = logging.getLogger(LoggingConfig.date)
+                    logger.exception(f'{self.__class__.__name__}: '
+                                     f'{self.__class__.compare_dates.__name__}')
                     raise SystemExit()
 
                 http = SOCKSProxyManager(f'{self.proxy_address}', headers=proxy_default_headers)
 
             repo = http.request('GET', repo_chg_txt)
         except KeyboardInterrupt:
             raise SystemExit(1)
 
         if local_chg_txt.is_file():
             local_size: int = int(os.stat(local_chg_txt).st_size)
 
         repo_size: int = int(repo.headers['Content-Length'])
 
+        logger = logging.getLogger(LoggingConfig.date)
+        logger.info(f'{self.__class__.__name__}: '
+                    f'{self.__class__.compare_dates.__name__}: '
+                    f'{local_chg_txt=}, {local_size=}, '
+                    f'{repo_chg_txt=}, {repo_size=}, '
+                    f'{local_size != repo_size}')
+
         return local_size != repo_size
 
     def view_message(self) -> None:
         self.check()
 
         print()
         for repo, comp in self.compare.items():
```

### Comparing `slpkg-4.8.1/slpkg/remove_packages.py` & `slpkg-4.8.2/slpkg/remove_packages.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,30 +21,30 @@
         super(Configs, self).__init__()
         self.packages: list = packages
         self.flags: list = flags
 
         self.session = Session
         self.utils = Utilities()
         self.progress = ProgressBar()
-        self.view = ViewMessage(self.flags)
+        self.view = ViewMessage(flags)
 
         self.process_message: str = ''
         self.installed_packages: list = []
         self.dependencies: list = []
         self.stderr = None
         self.stdout = None
 
         self.option_resolve_off: bool = self.utils.is_option(
-            ['-o', '--resolve-off'], self.flags)
+            ['-o', '--resolve-off'], flags)
 
         self.option_for_no_silent: bool = self.utils.is_option(
-            ['-n', '--no-silent'], self.flags)
+            ['-n', '--no-silent'], flags)
 
         self.option_for_yes: bool = self.utils.is_option(
-            ['-y', '--yes'], self.flags)
+            ['-y', '--yes'], flags)
 
     def remove(self) -> None:
         """ Removes package with dependencies. """
         self.installed_packages, self.dependencies = self.view.remove_packages(self.packages)
 
         self.view.question()
 
@@ -81,15 +81,18 @@
         if dependencies and not self.option_for_yes and self.ask_question:
             print(f"\n{self.bold}{self.violet}WARNING!{self.endc}: The package '{self.red}{name}{self.endc}' "
                   f"is a dependency for the packages:")
 
             for dep in dependencies:
                 print(f"{self.cyan:>16}-> {dep}{self.endc}")
 
-            answer: str = input('\nDo you want to remove? [y/N] ')
+            try:
+                answer: str = input('\nDo you want to remove? [y/N] ')
+            except KeyboardInterrupt:
+                raise SystemExit()
 
             if answer not in ['Y', 'y']:
                 return False
             print()
 
         return True
```

### Comparing `slpkg-4.8.1/slpkg/blacklist.py` & `slpkg-4.8.2/slpkg/blacklist.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/slpkg/download_only.py` & `slpkg-4.8.2/slpkg/download_only.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,18 @@
         self.directory: Path = directory
 
         self.repos = Repositories()
         self.utils = Utilities()
         self.session = Session
 
         self.option_for_directory: bool = self.utils.is_option(
-            ['-z', '--directory='], self.flags)
+            ['-z', '--directory='], flags)
 
         self.option_for_binaries: bool = self.utils.is_option(
-            ['-B', '--bin-repo='], self.flags)
+            ['-B', '--bin-repo='], flags)
 
     def packages(self, data: dict, packages: list) -> None:
         """ Download the package only. """
         packages: list = self.utils.apply_package_pattern(data, packages)
 
         view = ViewMessage(self.flags, data)
         view.download_packages(packages, self.directory)
```

### Comparing `slpkg-4.8.1/slpkg/tracking.py` & `slpkg-4.8.2/slpkg/tracking.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,18 @@
         self.utils = Utilities()
 
         self.llc: str = self.ascii.lower_left_corner
         self.hl: str = self.ascii.horizontal_line
         self.vl: str = self.ascii.vertical_line
 
         self.option_for_pkg_version: bool = self.utils.is_option(
-            ['-p', '--pkg-version'], self.flags)
+            ['-p', '--pkg-version'], flags)
 
         self.option_for_binaries: bool = self.utils.is_option(
-            ['-B', '--bin-repo='], self.flags)
+            ['-B', '--bin-repo='], flags)
 
     def packages(self, data: dict, packages: list) -> None:
         """ Prints the packages dependencies. """
         print(f"The list below shows the packages '{', '.join([p for p in packages])}' with dependencies:\n")
 
         packages: list = self.utils.apply_package_pattern(data, packages)
```

### Comparing `slpkg-4.8.1/slpkg/main.py` & `slpkg-4.8.2/slpkg/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,54 +9,54 @@
 from slpkg.checks import Check
 from slpkg.upgrade import Upgrade
 from slpkg.configs import Configs
 from slpkg.tracking import Tracking
 from slpkg.repo_info import RepoInfo
 from slpkg.dependees import Dependees
 from slpkg.utilities import Utilities
+from slpkg.cleanings import Cleanings
 from slpkg.search import SearchPackage
 from slpkg.views.cli_menu import Usage
 from slpkg.dialog_box import DialogBox
 from slpkg.views.version import Version
 from slpkg.download_only import Download
-from slpkg.views.views import ViewMessage
 from slpkg.sbos.queries import SBoQueries
 from slpkg.views.help_commands import Help
 from slpkg.repositories import Repositories
 from slpkg.binaries.install import Packages
 from slpkg.dialog_configs import FormConfigs
 from slpkg.check_updates import CheckUpdates
 from slpkg.sbos.slackbuild import Slackbuilds
 from slpkg.binaries.queries import BinQueries
 from slpkg.logging_config import LoggingConfig
 from slpkg.find_installed import FindInstalled
 from slpkg.views.view_package import ViewPackage
 from slpkg.remove_packages import RemovePackages
-from slpkg.clean_logs import CleanLogsDependencies
 from slpkg.update_repository import UpdateRepository
 
 
 class Argparse(Configs):
 
     def __init__(self, args: list):
         __slots__ = 'args'
         super(Configs).__init__()
         self.args: list = args
         self.flags: list = []
-
+        self.binary_repo: str = ''
         self.directory = self.tmp_slpkg
+
         self.dialogbox = DialogBox()
         self.utils = Utilities()
         self.usage = Usage()
         self.form_configs = FormConfigs()
         self.repos = Repositories()
 
         self.binary_repo: str = ''
 
-        if len(self.args) == 0 or '' in self.args:
+        if len(args) == 0 or '' in args:
             self.usage.help_short(1)
 
         self.data: dict = {}
         self.flag_yes: str = '--yes'
         self.flag_short_yes: str = '-y'
         self.flag_jobs: str = '--jobs'
         self.flag_short_jobs: str = '-j'
@@ -284,17 +284,22 @@
             self.data: dict = BinQueries(self.binary_repo).repository_data()
         else:
             self.data: dict = SBoQueries().repository_data()
 
         self.check = Check(self.flags, self.data)
 
         logging.basicConfig(filename=LoggingConfig.log_file,
-                            filemode='w',
-                            encoding='utf-8',
-                            level=logging.INFO)
+                            filemode=LoggingConfig.filemode,
+                            encoding=LoggingConfig.encoding,
+                            level=LoggingConfig.level)
+
+        logger = logging.getLogger(LoggingConfig.date)
+        logger.info(f'{self.__class__.__name__}: '
+                    f'{self.__class__.__init__.__name__}: '
+                    f'{args=}, {self.flags=}, {self.binary_repo=}')
 
     def check_for_bin_repositories(self) -> None:
         """ Checks combination for binaries use repositories only and if repository exists. """
         if self.utils.is_option(self.flag_binaries, self.flags):
 
             except_options: list = [
                 '-s', 'search',
@@ -338,14 +343,17 @@
         # Fixed for correct options by command.
         try:
             options: list = self.commands[self.args[0]]
             for opt in self.flags:
                 if opt not in options:
                     invalid.append(opt)
         except (KeyError, IndexError):
+            logger = logging.getLogger(LoggingConfig.date)
+            logger.exception(f'{self.__class__.__name__}: '
+                             f'{self.__class__.invalid_options.__name__}')
             self.usage.help_short(1)
 
         # Prints error for invalid options.
         if invalid:
             self.usage.help_minimal(f"{self.prog_name}: invalid options '{','.join(invalid)}'")
 
     def split_options(self) -> None:
@@ -379,26 +387,32 @@
                 self.directory: str = arg.split('=')[1]
                 self.args[self.args.index(arg)] = self.flag_directory
 
             if arg.startswith(self.flag_short_directory) and len(self.args) > 3:
                 try:
                     self.directory: str = self.args[self.args.index(arg) + 1]
                 except IndexError:
+                    logger = logging.getLogger(LoggingConfig.date)
+                    logger.exception(f'{self.__class__.__name__}: '
+                                     f'{self.__class__.split_options_from_args.__name__}')
                     self.directory: Path = self.tmp_slpkg
                 else:
                     self.args.remove(self.directory)
 
             if arg.startswith(self.flag_bin_repository):
                 self.binary_repo: str = arg.split('=')[1]
                 self.args[self.args.index(arg)] = self.flag_bin_repository
 
             if arg.startswith(self.flag_short_bin_repository) and len(self.args) > 2:
                 try:
                     self.binary_repo: str = self.args[self.args.index(arg) + 1]
                 except IndexError:
+                    logger = logging.getLogger(LoggingConfig.date)
+                    logger.exception(f'{self.__class__.__name__}: '
+                                     f'{self.__class__.split_options_from_args.__name__}')
                     self.binary_repo = ''
                 else:
                     self.args.remove(self.binary_repo)
 
         if self.binary_repo in self.options:
             self.binary_repo: str = ''
 
@@ -559,42 +573,30 @@
         if len(self.args) == 1:
             self.form_configs.edit()
             raise SystemExit()
         self.usage.help_short(1)
 
     def clean_logs(self) -> None:
         if len(self.args) == 1:
-            self.check.is_empty_database(self.binary_repo)
-
-            logs = CleanLogsDependencies(self.flags)
-            logs.clean()
+            clean = Cleanings(self.flags)
+            clean.logs_deps()
             raise SystemExit()
         self.usage.help_short(1)
 
     def clean_tmp(self) -> None:
         if len(self.args) == 1:
-
-            print(f"\n{self.prog_name}: {self.blink}{self.bold}{self.bred}WARNING!{self.endc}: All the files in the "
-                  f"'{self.tmp_path}{self.prog_name}' "
-                  f"folder will delete!")
-
-            views = ViewMessage(self.flags)
-            views.question()
-
-            self.utils.remove_folder_if_exists(Path(self.tmp_path, self.prog_name))
-            self.utils.create_folder(path=self.tmp_slpkg, folder='build')
-            print(f"The folder '{self.tmp_path}{self.prog_name}' was cleaned!")
-
+            clean = Cleanings(self.flags)
+            clean.tmp()
             raise SystemExit()
         self.usage.help_short(1)
 
     def clean_data(self) -> None:
         if len(self.args) == 1:
-            update = UpdateRepository(self.flags, self.binary_repo)
-            update.drop_the_tables()
+            clean = Cleanings(self.flags)
+            clean.db_tables()
             raise SystemExit()
         self.usage.help_short(1)
 
     def build(self) -> None:
         command = Argparse.build.__name__
 
         if len(self.args) >= 2:
@@ -765,24 +767,27 @@
     def help_for_commands(self) -> None:
         """ Extra help information for commands. """
         if len(self.args) == 2:
             try:
                 flags = self.commands[self.args[1]]
                 Help(self.args[1], flags).view()
             except KeyError:
+                logger = logging.getLogger(LoggingConfig.date)
+                logger.exception(f'{self.__class__.__name__}: '
+                                 f'{self.__class__.help_for_commands.__name__}')
                 self.usage.help_minimal(f"{self.prog_name}: invalid argument '{''.join(self.args[1])}'")
         else:
             self.usage.help_short(1)
 
 
-def main():
-    args = sys.argv
+def main() -> None:
+    args: list = sys.argv
     args.pop(0)
-    usage = Usage()
 
+    usage = Usage()
     argparse = Argparse(args)
 
     arguments: dict = {
         '-h': argparse.help,
         '--help': argparse.help,
         '-v': argparse.version,
         '--version': argparse.version,
@@ -821,15 +826,15 @@
         '-e': argparse.dependees,
         'tracking': argparse.tracking,
         '-t': argparse.tracking
     }
 
     try:
         arguments[args[0]]()
-    except (KeyError, IndexError) as err:
-        logger = logging.getLogger(__name__)
-        logger.info('%s: %s', main.__name__, err)
+    except (KeyError, IndexError):
+        logger = logging.getLogger(LoggingConfig.date)
+        logger.exception(f'{main.__name__}')
         usage.help_short(1)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `slpkg-4.8.1/slpkg/find_installed.py` & `slpkg-4.8.2/slpkg/find_installed.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/slpkg/upgrade.py` & `slpkg-4.8.2/slpkg/upgrade.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,20 +19,20 @@
         super(Configs, self).__init__()
         self.flags: list = flags
         self.data: dict = data
         self.utils = Utilities()
         self.repos = Repositories()
 
         self.option_for_binaries: bool = self.utils.is_option(
-            ['-B', '--bin-repo='], self.flags)
+            ['-B', '--bin-repo='], flags)
 
-        logging.basicConfig(filename=str(LoggingConfig.log_file),
-                            filemode='w',
-                            encoding='utf-8',
-                            level=logging.INFO)
+        logging.basicConfig(filename=LoggingConfig.log_file,
+                            filemode=LoggingConfig.filemode,
+                            encoding=LoggingConfig.encoding,
+                            level=LoggingConfig.level)
 
     def packages(self) -> Generator:
         """ Returns the upgradable packages. """
 
         # Returns the matched packages between two lists.
         packages: list = list(set(self.utils.installed_packages.keys()) & set(self.data.keys()))
 
@@ -71,20 +71,20 @@
             if parse(repo_pkg) > parse(inst_pkg):
                 return True
 
             if (parse(repo_pkg) == parse(inst_pkg)
                     and parse(repo_build) > parse(inst_build)):
                 return True
 
-        except InvalidVersion as err:
-            logger = logging.getLogger(__name__)
-            logger.info('%s: %s: %s: %s', self.__class__.__name__,
-                        Upgrade.is_package_upgradeable.__name__,
-                        name,
-                        err)
+        except InvalidVersion:
+            logger = logging.getLogger(LoggingConfig.date)
+            logger.exception(f'{self.__class__.__name__}: '
+                             f'{self.__class__.is_package_upgradeable.__name__}: '
+                             f'{repo_tag=}, {repo_pkg=}, {inst_pkg=}, {repo_pkg > inst_pkg}, '
+                             f'{repo_pkg == inst_pkg and repo_build > inst_build}')
 
             if repo_pkg > inst_pkg:
                 return True
 
             if repo_pkg == inst_pkg and repo_build > inst_build:
                 return True
```

### Comparing `slpkg-4.8.1/slpkg/search.py` & `slpkg-4.8.2/slpkg/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         super(Configs, self).__init__()
         self.flags: list = flags
 
         self.utils = Utilities()
         self.repos = Repositories()
 
         self.option_for_binaries: bool = self.utils.is_option(
-            ['-B', '--bin-repo='], self.flags)
+            ['-B', '--bin-repo='], flags)
 
     def package(self, data: dict, packages: list, repo: str) -> None:
         """ Searching and print the matched packages. """
         print(f'The list below shows the repo '
               f'packages that contains \'{", ".join([p for p in packages])}\':\n')
 
         matching: int = 0
```

### Comparing `slpkg-4.8.1/setup.cfg` & `slpkg-4.8.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = slpkg
-version = 4.8.1
+version = 4.8.2
 license_file = LICENSE
 author = Dimitris Zlatanidis
 author_email = d.zlatanidis@gmail.com
 description = Package manager utility for Slackware Linux.
 long_description = file:README.rst
 url = https://dslackw.gitlab.io/slpkg/
 project_urls = 
@@ -39,13 +39,18 @@
 python_requires = >= 3.9
 install_requires = 
 	SQLAlchemy >= 1.4.46
 	pythondialog >= 3.5.3
 	progress >= 1.6
 include_package_data = True
 
+[options.entry_points]
+console_scripts =
+    slpkg = slpkg.main:main
+    slpkg_new-configs = slpkg.new_configs:main
+
 [options.extras_require]
 socks =
 	PySocks >= 1.7.1
 
 [options.packages.find]
 where = .
```

### Comparing `slpkg-4.8.1/slpkg.egg-info/SOURCES.txt` & `slpkg-4.8.2/slpkg.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,39 +3,42 @@
 setup.cfg
 setup.py
 slpkg/__init__.py
 slpkg/blacklist.py
 slpkg/check_updates.py
 slpkg/checks.py
 slpkg/checksum.py
-slpkg/clean_logs.py
+slpkg/cleanings.py
 slpkg/configs.py
 slpkg/dependees.py
 slpkg/dialog_box.py
 slpkg/dialog_configs.py
 slpkg/download_only.py
 slpkg/downloader.py
 slpkg/error_messages.py
 slpkg/find_installed.py
 slpkg/install_data.py
 slpkg/logging_config.py
+slpkg/logging_deps.py
 slpkg/main.py
+slpkg/new_configs.py
 slpkg/progress_bar.py
 slpkg/remove_packages.py
 slpkg/repo_info.py
 slpkg/repositories.py
 slpkg/search.py
 slpkg/toml_error_message.py
 slpkg/tracking.py
 slpkg/update_repository.py
 slpkg/upgrade.py
 slpkg/utilities.py
 slpkg.egg-info/PKG-INFO
 slpkg.egg-info/SOURCES.txt
 slpkg.egg-info/dependency_links.txt
+slpkg.egg-info/entry_points.txt
 slpkg.egg-info/requires.txt
 slpkg.egg-info/top_level.txt
 slpkg/binaries/__init__.py
 slpkg/binaries/install.py
 slpkg/binaries/queries.py
 slpkg/binaries/required.py
 slpkg/models/__init__.py
```

### Comparing `slpkg-4.8.1/slpkg.egg-info/PKG-INFO` & `slpkg-4.8.2/slpkg.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slpkg
-Version: 4.8.1
+Version: 4.8.2
 Summary: Package manager utility for Slackware Linux.
 Home-page: https://dslackw.gitlab.io/slpkg/
 Author: Dimitris Zlatanidis
 Author-email: d.zlatanidis@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://dslackw.gitlab.io/slpkg/
 Project-URL: Documentation, https://dslackw.gitlab.io/slpkg/
```

### Comparing `slpkg-4.8.1/README.md` & `slpkg-4.8.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,25 +56,25 @@
 $ slpkg tracking --pkg-version Flask awscli pychess
 ```
 <img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_tracking.png" width="900">
 
 ### Installation
 
 ```
-$ tar xvf slpkg-4.8.1.tar.gz
-$ cd slpkg-4.8.1
+$ tar xvf slpkg-4.8.2.tar.gz
+$ cd slpkg-4.8.2
 $ ./install.sh
 ```
 
 ### Requirements
 
 ```
 SQLAlchemy >= 1.4.46
-pythondialog >= 3.5.3
-progress >= 1.6
+python3-pythondialog >= 3.5.3
+python3-progress >= 1.6
 ```
 
 ### Recommended
 
 Stay always updated, see my other project SUN [(Slackware Update Notifier)](https://gitlab.com/dslackw/sun)
 
 
@@ -82,31 +82,35 @@
 
 The majority of trials have been made in Slackware x86_64 'stable' environment.
 
 
 ### Command Line Tool Usage
 
 ```
-USAGE: slpkg [COMMAND] [OPTIONS] [FILELIST|PACKAGES...]
+slpkg - version 4.8.2
 
-DESCRIPTION: Package manager utility for Slackware.
+USAGE:
+  slpkg [COMMAND] [OPTIONS] [FILELIST|PACKAGES...]
+
+DESCRIPTION:
+  Package manager utility for Slackware.
 
 COMMANDS:
   -u, update                    Update the package lists.
   -U, upgrade                   Upgrade all the packages.
   -c, check-updates             Check for news on ChangeLog.txt.
   -I, repo-info                 Prints the repositories information.
   -g, configs                   Edit the configuration file.
   -L, clean-logs                Clean dependencies log tracking.
   -T, clean-data                Clean all the repositories data.
   -D, clean-tmp                 Delete all the downloaded sources.
   -b, build [packages...]       Build only the packages.
   -i, install [packages...]     Build and install the packages.
-  -d, download [packages...]    Download only the scripts and sources.
   -R, remove [packages...]      Remove installed packages.
+  -d, download [packages...]    Download only the scripts and sources.
   -f, find [packages...]        Find installed packages.
   -w, view [packages...]        View packages from the repository.
   -s, search [packages...]      Search packages from the repository.
   -e, dependees [packages...]   Show which packages depend on.
   -t, tracking [packages...]    Tracking the packages dependencies.
 
 OPTIONS:
@@ -235,14 +239,16 @@
 Please read the file [README](https://gitlab.com/dslackw/slpkg/-/raw/master/filelists/multilib/README) you will find in the folder [multlib](https://gitlab.com/dslackw/slpkg/-/tree/master/filelists/multilib)
 
 
 ### Issues
 
 Please report any bugs in [ISSUES](https://gitlab.com/dslackw/slpkg/issues)
 
+Note: With the issue, please reference the log file you will find in the /tmp/slpkg/logs/slpkg.log path and paste it too.
+
 
 ### Donate
 
 If you feel satisfied with this project and want to thank me, treat me to a coffee ☕ !
 
 [<img src="https://gitlab.com/dslackw/images/raw/master/donate/paypaldonate.png">](https://www.paypal.me/dslackw)
```

### Comparing `slpkg-4.8.1/tools/gen_sbo_txt.sh` & `slpkg-4.8.2/tools/gen_sbo_txt.sh`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.1/bin/slpkg_new-configs` & `slpkg-4.8.2/slpkg/new_configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import sys
 import shutil
 import difflib
 import subprocess
+from typing import Any
 from pathlib import Path
 
 
-class NewConfig:
+class NewConfigs:
 
-    def __init__(self, flags: list):
-        __slots__ = 'flags'
-        self.flags: list = flags
-        self.etc_path: str = '/etc/slpkg'
+    def __init__(self, options: list):
+        __slots__ = 'options'
+        self.options: list = options
+        self.etc_path: Path = Path('/etc/slpkg')
         self.slpkg_config: Path = Path(self.etc_path, 'slpkg.toml')
         self.repositories_config: Path = Path(self.etc_path, 'repositories.toml')
         self.blacklist_config: Path = Path(self.etc_path, 'blacklist.toml')
         self.slpkg_config_new: Path = Path(self.etc_path, 'slpkg.toml.new')
         self.repositories_config_new: Path = Path(self.etc_path, 'repositories.toml.new')
         self.blacklist_config_new: Path = Path(self.etc_path, 'blacklist.toml.new')
 
@@ -34,32 +35,32 @@
         self.violet: str = '\x1b[35m'
         self.endc: str = '\x1b[0m'
 
         self.set_no_colors()
 
         self.choice = None
 
-    def set_no_colors(self):
-        if '--no-colors' in self.flags:
+    def set_no_colors(self) -> None:
+        if '--no-colors' in self.options:
             self.bold: str = ''
             self.red: str = ''
             self.bred: str = ''
             self.green: str = ''
             self.bgreen: str = ''
             self.yellow: str = ''
             self.byellow: str = ''
             self.cyan: str = ''
             self.blue: str = ''
             self.grey: str = ''
             self.violet: str = ''
             self.endc: str = ''
 
-    def check(self):
+    def check(self) -> None:
         """ Checks for .new files. """
-        print('Checking for NEW configuration files...')
+        print('\nChecking for NEW configuration files...')
         if (self.slpkg_config_new.is_file() or self.blacklist_config_new.is_file()
                 or self.repositories_config_new.is_file()):
             print('\nThere are NEW files:\n')
 
             if self.slpkg_config_new.is_file():
                 print(f"{self.bgreen:>12}{self.slpkg_config_new}{self.endc}")
 
@@ -80,102 +81,102 @@
 
             self.menu()
 
         elif (not self.slpkg_config_new.is_file() and not self.blacklist_config_new.is_file()
               and not self.repositories_config_new.is_file()):
             print(f"\n{'No .new files found.':>23}\n")
 
-    def menu(self):
+    def menu(self) -> None:
         """ Menu of choices. """
-        choice = input('Choice: ')
+        choice: str = input('Choice: ')
 
-        choice = choice.lower()
+        choice: str = choice.lower()
 
         arguments: dict = {
             'k': self.keep,
             'o': self.overwrite,
             'r': self.remove,
             'p': self.prompt
         }
 
         try:
             arguments[choice]()
         except KeyError:
             self.keep()
 
     @staticmethod
-    def keep():
+    def keep() -> None:
         print("\nNo changes were made.\n")
 
-    def overwrite(self):
+    def overwrite(self) -> None:
         """ Copy tne .new files and rename the olds to .orig.  """
         if self.slpkg_config_new.is_file():
             self.overwrite_config_file()
 
         if self.repositories_config_new.is_file():
             self.overwrite_repositories_file()
 
         if self.blacklist_config_new.is_file():
             self.overwrite_blacklist_file()
         print()  # new line
 
-    def overwrite_config_file(self):
+    def overwrite_config_file(self) -> None:
         """ Copy tne slpkg.toml.new file and rename the old to .orig. """
         if self.slpkg_config.is_file():
             shutil.copy(self.slpkg_config, f"{self.slpkg_config}.orig")
             print(f"\ncp {self.green}{self.slpkg_config}{self.endc} -> {self.slpkg_config}.orig")
 
         shutil.move(self.slpkg_config_new, self.slpkg_config)
         print(f"mv {self.slpkg_config_new} -> {self.green}{self.slpkg_config}{self.endc}")
 
-    def overwrite_repositories_file(self):
+    def overwrite_repositories_file(self) -> None:
         """ Copy tne repositories.toml.new file and rename the old to .orig. """
         if self.slpkg_config.is_file():
             shutil.copy(self.repositories_config, f"{self.repositories_config}.orig")
             print(f"\ncp {self.green}{self.repositories_config}{self.endc} -> {self.repositories_config}.orig")
 
         shutil.move(self.repositories_config_new, self.repositories_config)
         print(f"mv {self.repositories_config_new} -> {self.green}{self.repositories_config}{self.endc}")
 
-    def overwrite_blacklist_file(self):
+    def overwrite_blacklist_file(self) -> None:
         """ Copy tne blacklist.toml.new file and rename the old to .orig. """
         if self.blacklist_config.is_file():
             shutil.copy(self.blacklist_config, f"{self.blacklist_config}.orig")
             print(f"\ncp {self.green}{self.blacklist_config}{self.endc} -> {self.blacklist_config}.orig")
 
         shutil.move(self.blacklist_config_new, self.blacklist_config)
         print(f"mv {self.blacklist_config_new} -> {self.green}{self.blacklist_config}{self.endc}")
 
-    def remove(self):
+    def remove(self) -> None:
         """ Removes the .new files. """
         print()  # new line
         self.remove_config_new_file()
         self.remove_repositories_new_file()
         self.remove_blacklist_new_file()
         print()  # new line
 
-    def remove_config_new_file(self):
+    def remove_config_new_file(self) -> None:
         """ Remove slpkg.toml.new file. """
         if self.slpkg_config_new.is_file():
             self.slpkg_config_new.unlink()
             print(f"rm {self.red}{self.slpkg_config_new}{self.endc}")
 
-    def remove_repositories_new_file(self):
+    def remove_repositories_new_file(self) -> None:
         """ Remove repositories.toml.new file. """
         if self.repositories_config_new.is_file():
             self.repositories_config_new.unlink()
             print(f"rm {self.red}{self.repositories_config_new}{self.endc}")
 
-    def remove_blacklist_new_file(self):
+    def remove_blacklist_new_file(self) -> None:
         """ Remove blacklist.toml.new file. """
         if self.blacklist_config_new.is_file():
             self.blacklist_config_new.unlink()
             print(f"rm {self.red}{self.blacklist_config_new}{self.endc}")
 
-    def prompt(self):
+    def prompt(self) -> None:
         """ Prompt K, O, R selection for every single file. """
         print(f"\n{'':>2}({self.byellow}K{self.endc})eep, ({self.byellow}O{self.endc})verwrite, "
               f"({self.byellow}R{self.endc})emove, ({self.byellow}D{self.endc})iff, "
               f"({self.byellow}V{self.endc})imdiff\n")
 
         if self.slpkg_config_new.is_file():
             make = input(f'{self.bgreen}{self.slpkg_config_new}{self.endc} - '
@@ -234,41 +235,42 @@
                 print()  # new line
             if make.lower() == 'd':
                 self.diff_files(self.blacklist_config_new, self.blacklist_config)
             if make.lower() == 'v':
                 self.vimdiff(self.blacklist_config_new, self.blacklist_config)
 
     @staticmethod
-    def diff_files(file2, file1):
+    def diff_files(file2: Any, file1: Any) -> None:
         """ Diff the .new and the current file. """
         with open(file1, 'r') as f1:
             with open(file2, 'r') as f2:
                 diff = difflib.context_diff(
                     f1.readlines(),
                     f2.readlines(),
                     fromfile=str(file1),
                     tofile=str(file2)
                 )
                 for line in diff:
                     print(line, end='')
 
     @staticmethod
-    def vimdiff(file1, file2):
+    def vimdiff(file1: Any, file2: Any) -> None:
         output = subprocess.call(f'vimdiff {file1} {file2}', shell=True)
         if output != 0:
             raise SystemExit(output)
 
 
-if __name__ == '__main__':
-    args = sys.argv
+def main() -> None:
+    args: list = sys.argv
     args.pop(0)
 
     options: list = [
         '--no-colors',
-        '-h', '--help'
+        '-h',
+        '--help'
     ]
 
     if len(args) == 1:
         if options[1] in args or options[2] in args:
             print('slpkg_new-configs [OPTIONS]\n'
                   '\n  --no-colors     Disable the output colors.\n'
                   '  -h, --help      Show this message and exit.\n')
@@ -279,11 +281,11 @@
             print('\ntry: slpkg_new-configs --help\n')
             sys.exit(1)
     elif len(args) > 1:
         print('\ntry: slpkg_new-configs --help\n')
         sys.exit(1)
 
     try:
-        config = NewConfig(args)
+        config = NewConfigs(args)
         config.check()
     except KeyboardInterrupt:
-        raise SystemExit(1)
+        raise SystemExit()
```

