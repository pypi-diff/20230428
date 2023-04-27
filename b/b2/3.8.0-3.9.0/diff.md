# Comparing `tmp/b2-3.8.0.tar.gz` & `tmp/b2-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2-3.8.0.tar", last modified: Thu Mar 23 09:19:00 2023, max compression
+gzip compressed data, was "b2-3.9.0.tar", last modified: Thu Apr 27 23:21:37 2023, max compression
```

## Comparing `b2-3.8.0.tar` & `b2-3.9.0.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:19:00.790301 b2-3.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:19:00.770301 b2-3.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-23 09:18:34.000000 b2-3.8.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-23 09:18:34.000000 b2-3.8.0/.github/no-response.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:19:00.770301 b2-3.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-03-23 09:18:34.000000 b2-3.8.0/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-03-23 09:18:34.000000 b2-3.8.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-23 09:18:34.000000 b2-3.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-23 09:18:34.000000 b2-3.8.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16299 2023-03-23 09:18:34.000000 b2-3.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-03-23 09:18:34.000000 b2-3.8.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-03-23 09:18:34.000000 b2-3.8.0/Dockerfile.template
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-03-23 09:18:34.000000 b2-3.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-23 09:18:34.000000 b2-3.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-03-23 09:19:00.790301 b2-3.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11116 2023-03-23 09:18:34.000000 b2-3.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-23 09:18:34.000000 b2-3.8.0/README.release.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:19:00.774301 b2-3.8.0/b2/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-03-23 09:18:34.000000 b2-3.8.0/b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-03-23 09:18:34.000000 b2-3.8.0/b2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-23 09:18:34.000000 b2-3.8.0/b2/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:19:00.774301 b2-3.8.0/b2/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-23 09:18:34.000000 b2-3.8.0/b2/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-03-23 09:18:34.000000 b2-3.8.0/b2/_cli/argcompleters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-03-23 09:18:34.000000 b2-3.8.0/b2/_cli/autocomplete_install.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-23 09:18:34.000000 b2-3.8.0/b2/_cli/b2api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-23 09:18:34.000000 b2-3.8.0/b2/_cli/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-23 09:18:34.000000 b2-3.8.0/b2/_cli/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-03-23 09:18:34.000000 b2-3.8.0/b2/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)   127451 2023-03-23 09:18:34.000000 b2-3.8.0/b2/console_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-23 09:18:34.000000 b2-3.8.0/b2/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)   173088 2023-03-23 09:19:00.000000 b2-3.8.0/b2/licenses_output.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-03-23 09:18:34.000000 b2-3.8.0/b2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:19:00.774301 b2-3.8.0/b2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-03-23 09:19:00.000000 b2-3.8.0/b2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-03-23 09:19:00.000000 b2-3.8.0/b2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 09:19:00.000000 b2-3.8.0/b2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-23 09:19:00.000000 b2-3.8.0/b2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-23 09:19:00.000000 b2-3.8.0/b2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-23 09:19:00.000000 b2-3.8.0/b2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-03-23 09:18:34.000000 b2-3.8.0/b2.spec
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:19:00.774301 b2-3.8.0/contrib/
--rwxr-xr-x   0 runner    (1001) docker     (123)      486 2023-03-23 09:18:34.000000 b2-3.8.0/contrib/color-b2-logs.sh
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-23 09:18:34.000000 b2-3.8.0/contrib/debug_logs.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:19:00.774301 b2-3.8.0/contrib/macos/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-23 09:18:34.000000 b2-3.8.0/contrib/macos/entitlements.plist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:19:00.774301 b2-3.8.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-23 09:18:34.000000 b2-3.8.0/doc/bash_completion.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:19:00.778301 b2-3.8.0/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/commands.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/quick_start.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/replication.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:19:00.782301 b2-3.8.0/doc/source/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/authorize_account.rst
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/cancel_all_unfinished_large_files.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/cancel_large_file.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/clear_account.rst
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/copy_file_by_id.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/create_bucket.rst
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/create_key.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/delete_bucket.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/delete_file_version.rst
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/delete_key.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/download_file_by_id.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/download_file_by_name.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/get_account_info.rst
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/get_bucket.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/get_download_auth.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/get_download_url_with_auth.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/get_file_info.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/hide_file.rst
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/install_autocomplete.rst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/list_buckets.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/list_keys.rst
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/list_parts.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/list_unfinished_large_files.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/ls.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/make_friendly_url.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/make_url.rst
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/replication-setup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/rm.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/sync.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/update_bucket.rst
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/update_file_legal_hold.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/update_file_retention.rst
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/upload_file.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-23 09:18:34.000000 b2-3.8.0/doc/source/subcommands/version.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-03-23 09:18:34.000000 b2-3.8.0/noxfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:19:00.782301 b2-3.8.0/pyinstaller-hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-23 09:18:34.000000 b2-3.8.0/pyinstaller-hooks/hook-b2.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-23 09:18:34.000000 b2-3.8.0/pyinstaller-hooks/hook-prettytable.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-23 09:18:34.000000 b2-3.8.0/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-23 09:18:34.000000 b2-3.8.0/requirements-license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-23 09:18:34.000000 b2-3.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-03-23 09:19:00.790301 b2-3.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-03-23 09:18:34.000000 b2-3.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:19:00.782301 b2-3.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-23 09:18:34.000000 b2-3.8.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:19:00.786301 b2-3.8.0/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-23 09:18:34.000000 b2-3.8.0/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-23 09:18:34.000000 b2-3.8.0/test/integration/cleanup_buckets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-03-23 09:18:34.000000 b2-3.8.0/test/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17242 2023-03-23 09:18:34.000000 b2-3.8.0/test/integration/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-03-23 09:18:34.000000 b2-3.8.0/test/integration/test_autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)    92996 2023-03-23 09:18:34.000000 b2-3.8.0/test/integration/test_b2_command_line.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:19:00.786301 b2-3.8.0/test/static/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-23 09:18:34.000000 b2-3.8.0/test/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-03-23 09:18:34.000000 b2-3.8.0/test/static/test_licenses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:19:00.786301 b2-3.8.0/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-23 09:18:34.000000 b2-3.8.0/test/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:19:00.786301 b2-3.8.0/test/unit/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-23 09:18:34.000000 b2-3.8.0/test/unit/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-03-23 09:18:34.000000 b2-3.8.0/test/unit/_cli/test_autocomplete_install.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-23 09:18:34.000000 b2-3.8.0/test/unit/_cli/test_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:19:00.786301 b2-3.8.0/test/unit/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-23 09:18:34.000000 b2-3.8.0/test/unit/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:19:00.786301 b2-3.8.0/test/unit/fixtures/test_source_mod/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-23 09:18:34.000000 b2-3.8.0/test/unit/fixtures/test_source_mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:19:00.786301 b2-3.8.0/test/unit/fixtures/test_source_mod/c/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-23 09:18:34.000000 b2-3.8.0/test/unit/fixtures/test_source_mod/c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-23 09:18:34.000000 b2-3.8.0/test/unit/fixtures/test_source_mod/c/d.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-03-23 09:18:34.000000 b2-3.8.0/test/unit/fixtures/test_source_mod/z.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:19:00.786301 b2-3.8.0/test/unit/fixtures/test_target_mod/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-23 09:18:34.000000 b2-3.8.0/test/unit/fixtures/test_target_mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:19:00.790301 b2-3.8.0/test/unit/fixtures/test_target_mod/a/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-23 09:18:34.000000 b2-3.8.0/test/unit/fixtures/test_target_mod/a/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-23 09:18:34.000000 b2-3.8.0/test/unit/fixtures/test_target_mod/a/b.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:19:00.790301 b2-3.8.0/test/unit/fixtures/test_target_mod/c/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-23 09:18:34.000000 b2-3.8.0/test/unit/fixtures/test_target_mod/c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-23 09:18:34.000000 b2-3.8.0/test/unit/fixtures/test_target_mod/z.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-23 09:18:34.000000 b2-3.8.0/test/unit/test_arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-23 09:18:34.000000 b2-3.8.0/test/unit/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)   100308 2023-03-23 09:18:34.000000 b2-3.8.0/test/unit/test_console_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-03-23 09:18:34.000000 b2-3.8.0/test/unit/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-03-23 09:18:34.000000 b2-3.8.0/test/unit/test_represent_file_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.100751 b2-3.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.088750 b2-3.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-27 23:21:13.000000 b2-3.9.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-27 23:21:13.000000 b2-3.9.0/.github/no-response.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.088750 b2-3.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-04-27 23:21:13.000000 b2-3.9.0/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-04-27 23:21:13.000000 b2-3.9.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-27 23:21:13.000000 b2-3.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-27 23:21:13.000000 b2-3.9.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16671 2023-04-27 23:21:13.000000 b2-3.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-27 23:21:13.000000 b2-3.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-27 23:21:13.000000 b2-3.9.0/Dockerfile.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-27 23:21:13.000000 b2-3.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-27 23:21:13.000000 b2-3.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-04-27 23:21:37.100751 b2-3.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-04-27 23:21:13.000000 b2-3.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-27 23:21:13.000000 b2-3.9.0/README.release.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.088750 b2-3.9.0/b2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-27 23:21:13.000000 b2-3.9.0/b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 23:21:13.000000 b2-3.9.0/b2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-27 23:21:13.000000 b2-3.9.0/b2/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.088750 b2-3.9.0/b2/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-27 23:21:13.000000 b2-3.9.0/b2/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-27 23:21:13.000000 b2-3.9.0/b2/_cli/argcompleters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-04-27 23:21:13.000000 b2-3.9.0/b2/_cli/autocomplete_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-27 23:21:13.000000 b2-3.9.0/b2/_cli/b2api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-27 23:21:13.000000 b2-3.9.0/b2/_cli/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-27 23:21:13.000000 b2-3.9.0/b2/_cli/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-27 23:21:13.000000 b2-3.9.0/b2/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)   128195 2023-04-27 23:21:13.000000 b2-3.9.0/b2/console_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-27 23:21:13.000000 b2-3.9.0/b2/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)   174088 2023-04-27 23:21:36.000000 b2-3.9.0/b2/licenses_output.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-27 23:21:13.000000 b2-3.9.0/b2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.088750 b2-3.9.0/b2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-04-27 23:21:37.000000 b2-3.9.0/b2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-27 23:21:37.000000 b2-3.9.0/b2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 23:21:37.000000 b2-3.9.0/b2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-27 23:21:37.000000 b2-3.9.0/b2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-27 23:21:37.000000 b2-3.9.0/b2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-27 23:21:37.000000 b2-3.9.0/b2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-27 23:21:13.000000 b2-3.9.0/b2.spec
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.088750 b2-3.9.0/contrib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      486 2023-04-27 23:21:13.000000 b2-3.9.0/contrib/color-b2-logs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-27 23:21:13.000000 b2-3.9.0/contrib/debug_logs.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.088750 b2-3.9.0/contrib/macos/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-27 23:21:13.000000 b2-3.9.0/contrib/macos/entitlements.plist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.088750 b2-3.9.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-27 23:21:13.000000 b2-3.9.0/doc/bash_completion.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.092750 b2-3.9.0/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/commands.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/quick_start.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/replication.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.096751 b2-3.9.0/doc/source/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/authorize_account.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/cancel_all_unfinished_large_files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/cancel_large_file.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/clear_account.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/copy_file_by_id.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/create_bucket.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/create_key.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/delete_bucket.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/delete_file_version.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/delete_key.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/download_file_by_id.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/download_file_by_name.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/get_account_info.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/get_bucket.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/get_download_auth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/get_download_url_with_auth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/get_file_info.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/hide_file.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/install_autocomplete.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/list_buckets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/list_keys.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/list_parts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/list_unfinished_large_files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/ls.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/make_friendly_url.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/make_url.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/replication-setup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/rm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/sync.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/update_bucket.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/update_file_legal_hold.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/update_file_retention.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/upload_file.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/version.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18652 2023-04-27 23:21:13.000000 b2-3.9.0/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.096751 b2-3.9.0/pyinstaller-hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-27 23:21:13.000000 b2-3.9.0/pyinstaller-hooks/hook-b2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-27 23:21:13.000000 b2-3.9.0/pyinstaller-hooks/hook-prettytable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-27 23:21:13.000000 b2-3.9.0/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-27 23:21:13.000000 b2-3.9.0/requirements-license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-27 23:21:13.000000 b2-3.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-27 23:21:37.100751 b2-3.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-04-27 23:21:13.000000 b2-3.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.096751 b2-3.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-27 23:21:13.000000 b2-3.9.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.096751 b2-3.9.0/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-27 23:21:13.000000 b2-3.9.0/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-27 23:21:13.000000 b2-3.9.0/test/integration/cleanup_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-27 23:21:13.000000 b2-3.9.0/test/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-04-27 23:21:13.000000 b2-3.9.0/test/integration/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-27 23:21:13.000000 b2-3.9.0/test/integration/test_autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94117 2023-04-27 23:21:13.000000 b2-3.9.0/test/integration/test_b2_command_line.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.096751 b2-3.9.0/test/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-27 23:21:13.000000 b2-3.9.0/test/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-27 23:21:13.000000 b2-3.9.0/test/static/test_licenses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.096751 b2-3.9.0/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.096751 b2-3.9.0/test/unit/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/_cli/test_autocomplete_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/_cli/test_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.096751 b2-3.9.0/test/unit/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.096751 b2-3.9.0/test/unit/fixtures/test_source_mod/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/fixtures/test_source_mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.096751 b2-3.9.0/test/unit/fixtures/test_source_mod/c/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/fixtures/test_source_mod/c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/fixtures/test_source_mod/c/d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/fixtures/test_source_mod/z.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.096751 b2-3.9.0/test/unit/fixtures/test_target_mod/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/fixtures/test_target_mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.100751 b2-3.9.0/test/unit/fixtures/test_target_mod/a/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/fixtures/test_target_mod/a/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/fixtures/test_target_mod/a/b.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.100751 b2-3.9.0/test/unit/fixtures/test_target_mod/c/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/fixtures/test_target_mod/c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/fixtures/test_target_mod/z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/test_arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100308 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/test_console_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/test_represent_file_metadata.py
```

### Comparing `b2-3.8.0/.github/no-response.yml` & `b2-3.9.0/.github/no-response.yml`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/.github/workflows/cd.yml` & `b2-3.9.0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/.github/workflows/ci.yml` & `b2-3.9.0/.github/workflows/ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -95,17 +95,20 @@
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: python -m pip install --upgrade nox pip setuptools
       - name: Run unit tests
         run: nox -vs unit
-      - name: Run integration tests
-        if: ${{ env.B2_TEST_APPLICATION_KEY != '' && env.B2_TEST_APPLICATION_KEY_ID != '' }}
-        run: nox -vs integration -- --cleanup
+      - name: Run integration tests (without secrets)
+        run: nox -vs integration -- -m "not require_secrets"
+      - name: Run integration tests (with secrets)
+        # Limit CI workload by running integration tests with secrets only on edge Python versions.
+        if: ${{ env.B2_TEST_APPLICATION_KEY != '' && env.B2_TEST_APPLICATION_KEY_ID != '' && contains(fromJSON('["3.7", "pypy-3.7", "3.11"]'), matrix.python-version) }}
+        run: nox -vs integration -- -m "require_secrets" --cleanup
   test-docker:
     needs: cleanup_buckets
     env:
       B2_TEST_APPLICATION_KEY: ${{ secrets.B2_TEST_APPLICATION_KEY }}
       B2_TEST_APPLICATION_KEY_ID: ${{ secrets.B2_TEST_APPLICATION_KEY_ID }}
     runs-on: ubuntu-latest
     # Running on raw machine.
@@ -144,17 +147,19 @@
           git config --global --add safe.directory '*'
       - name: Bundle the distribution
         id: bundle
         run: nox -vs bundle >> $GITHUB_OUTPUT
       - name: Generate hashes
         id: hashes
         run: nox -vs make_dist_digest
-      - name: Run integration tests
+      - name: Run integration tests (without secrets)
+        run: nox -vs integration -- -m "not require_secrets"
+      - name: Run integration tests (with secrets)
         if: ${{ env.B2_TEST_APPLICATION_KEY != '' && env.B2_TEST_APPLICATION_KEY_ID != '' }}
-        run: nox -vs integration -- --sut=${{ steps.bundle.outputs.sut_path }} --cleanup
+        run: nox -vs integration -- --sut=${{ steps.bundle.outputs.sut_path }} -m "require_secrets" --cleanup
       - name: Upload assets
         if: failure()
         uses: actions/upload-artifact@v2
         with:
           path: ${{ steps.bundle.outputs.asset_path }}
           if-no-files-found: warn
           retention-days: 7
@@ -181,17 +186,19 @@
       - name: Bundle the distribution
         id: bundle
         shell: bash
         run: nox -vs bundle >> $GITHUB_OUTPUT
       - name: Generate hashes
         id: hashes
         run: nox -vs make_dist_digest
-      - name: Run integration tests
+      - name: Run integration tests (without secrets)
+        run: nox -vs integration -- -m "not require_secrets"
+      - name: Run integration tests (with secrets)
         if: ${{ env.B2_TEST_APPLICATION_KEY != '' && env.B2_TEST_APPLICATION_KEY_ID != '' }}
-        run: nox -vs integration -- --sut=${{ steps.bundle.outputs.sut_path }} --cleanup
+        run: nox -vs integration -- --sut=${{ steps.bundle.outputs.sut_path }} -m "require_secrets" --cleanup
       - name: Upload assets
         if: failure()
         uses: actions/upload-artifact@v2
         with:
           path: ${{ steps.bundle.outputs.asset_path }}
           if-no-files-found: warn
           retention-days: 7
```

### Comparing `b2-3.8.0/.readthedocs.yml` & `b2-3.9.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/CHANGELOG.md` & `b2-3.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,27 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [3.9.0] - 2023-04-28
+
+### Added
+* Support for custom file upload timestamp
+
+### Infrastructure
+* Limit GitHub CI workload by running most integration tests only against edge versions of supported Python versions
+* Add a direct dependency from tqdm
+
 ## [3.8.0] - 2023-03-23
 
 ### Added
-* Add `install-autocomplete` command for installing shell autocompletion
+* Add `install-autocomplete` command for installing shell autocompletion (currently only `bash` is supported)
 
 ### Fixed
 * Hitting the download endpoint twice in some cases
 
 ### Infrastructure
 * GitHub CD builds and uploads an official B2 CLI image to docker hub
 * Disable changelog verification for dependabot PRs
@@ -408,15 +417,16 @@
 * More efficient uploads by sending SHA1 checksum at the end.
 
 ### Fixed
 * File modification times are set correctly when downloading.
 * Fix an off-by-one issue when downloading a range of a file (affects library, but not CLI).
 * Better handling of some errors from the B2 service.
 
-[Unreleased]: https://github.com/Backblaze/B2_Command_Line_Tool/compare/v3.8.0...HEAD
+[Unreleased]: https://github.com/Backblaze/B2_Command_Line_Tool/compare/v3.9.0...HEAD
+[3.9.0]: https://github.com/Backblaze/B2_Command_Line_Tool/compare/v3.8.0...v3.9.0
 [3.8.0]: https://github.com/Backblaze/B2_Command_Line_Tool/compare/v3.7.1...v3.8.0
 [3.7.1]: https://github.com/Backblaze/B2_Command_Line_Tool/compare/v3.7.0...v3.7.1
 [3.7.0]: https://github.com/Backblaze/B2_Command_Line_Tool/compare/v3.6.0...v3.7.0
 [3.6.0]: https://github.com/Backblaze/B2_Command_Line_Tool/compare/v3.5.0...v3.6.0
 [3.5.0]: https://github.com/Backblaze/B2_Command_Line_Tool/compare/v3.4.0...v3.5.0
 [3.4.0]: https://github.com/Backblaze/B2_Command_Line_Tool/compare/v3.3.0...v3.4.0
 [3.3.0]: https://github.com/Backblaze/B2_Command_Line_Tool/compare/v3.2.1...v3.3.0
```

### Comparing `b2-3.8.0/CONTRIBUTING.md` & `b2-3.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/Dockerfile.template` & `b2-3.9.0/Dockerfile.template`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/LICENSE` & `b2-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/PKG-INFO` & `b2-3.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b2
-Version: 3.8.0
+Version: 3.9.0
 Summary: Command Line Tool for Backblaze B2
 Home-page: https://github.com/Backblaze/B2_Command_Line_Tool
 Author: Backblaze, Inc.
 Author-email: support@backblaze.com
 License: MIT
 Keywords: backblaze b2 cloud storage
 Classifier: Development Status :: 5 - Production/Stable
@@ -67,15 +67,15 @@
 # Usage
 
     b2 authorize-account [-h]  [applicationKeyId] [applicationKey]
     b2 cancel-all-unfinished-large-files [-h] bucketName
     b2 cancel-large-file [-h] fileId
     b2 clear-account [-h]
     b2 copy-file-by-id [-h] [--fetchMetadata] [--contentType CONTENTTYPE] [--range RANGE] [--info INFO | --noInfo] [--destinationServerSideEncryption {SSE-B2,SSE-C}] [--destinationServerSideEncryptionAlgorithm {AES256}] [--sourceServerSideEncryption {SSE-C}] [--sourceServerSideEncryptionAlgorithm {AES256}] [--fileRetentionMode {compliance,governance}] [--retainUntil TIMESTAMP] [--legalHold {on,off}] sourceFileId destinationBucketName b2FileName
-    b2 create-bucket [-h] [--bucketInfo BUCKETINFO] [--corsRules CORSRULES] [--lifecycleRules LIFECYCLERULES] [--fileLockEnabled] [--replication REPLICATION] [--defaultServerSideEncryption {SSE-B2,none}] [--defaultServerSideEncryptionAlgorithm {AES256}] bucketName bucketType
+    b2 create-bucket [-h] [--bucketInfo BUCKETINFO] [--corsRules CORSRULES] [--lifecycleRules LIFECYCLERULES] [--fileLockEnabled] [--replication REPLICATION] [--defaultServerSideEncryption {SSE-B2,none}] [--defaultServerSideEncryptionAlgorithm {AES256}] bucketName {allPublic,allPrivate}
     b2 create-key [-h] [--bucket BUCKET] [--namePrefix NAMEPREFIX] [--duration DURATION] [--allCapabilities] keyName [capabilities]
     b2 delete-bucket [-h] bucketName
     b2 delete-file-version [-h] [fileName] fileId
     b2 delete-key [-h] applicationKeyId
     b2 download-file-by-id [-h] [--noProgress] [--threads THREADS] [--sourceServerSideEncryption {SSE-C}] [--sourceServerSideEncryptionAlgorithm {AES256}] [--write-buffer-size BYTES] [--skip-hash-verification] [--max-download-streams-per-file MAX_DOWNLOAD_STREAMS_PER_FILE] fileId localFileName
     b2 download-file-by-name [-h] [--noProgress] [--threads THREADS] [--sourceServerSideEncryption {SSE-C}] [--sourceServerSideEncryptionAlgorithm {AES256}] [--write-buffer-size BYTES] [--skip-hash-verification] [--max-download-streams-per-file MAX_DOWNLOAD_STREAMS_PER_FILE] bucketName b2FileName localFileName
     b2 get-account-info [-h]
@@ -89,25 +89,26 @@
     b2 list-parts [-h] largeFileId
     b2 list-unfinished-large-files [-h] bucketName
     b2 ls [-h] [--long] [--json] [--replication] [--versions] [--recursive] [--withWildcard] bucketName [folderName]
     b2 rm [-h] [--dryRun] [--threads THREADS] [--queueSize QUEUESIZE] [--noProgress] [--failFast] [--versions] [--recursive] [--withWildcard] bucketName [folderName]
     b2 make-url [-h] fileId
     b2 make-friendly-url [-h] bucketName fileName
     b2 sync [-h] [--noProgress] [--dryRun] [--allowEmptySource] [--excludeAllSymlinks] [--threads THREADS] [--syncThreads SYNCTHREADS] [--downloadThreads DOWNLOADTHREADS] [--uploadThreads UPLOADTHREADS] [--compareVersions {none,modTime,size}] [--compareThreshold MILLIS] [--excludeRegex REGEX] [--includeRegex REGEX] [--excludeDirRegex REGEX] [--excludeIfModifiedAfter TIMESTAMP] [--destinationServerSideEncryption {SSE-B2,SSE-C}] [--destinationServerSideEncryptionAlgorithm {AES256}] [--sourceServerSideEncryption {SSE-C}] [--sourceServerSideEncryptionAlgorithm {AES256}] [--write-buffer-size BYTES] [--skip-hash-verification] [--max-download-streams-per-file MAX_DOWNLOAD_STREAMS_PER_FILE] [--incrementalMode] [--skipNewer | --replaceNewer] [--delete | --keepDays DAYS] source destination
-    b2 update-bucket [-h] [--bucketInfo BUCKETINFO] [--corsRules CORSRULES] [--lifecycleRules LIFECYCLERULES] [--defaultRetentionMode {compliance,governance,none}] [--defaultRetentionPeriod period] [--replication REPLICATION] [--fileLockEnabled] [--defaultServerSideEncryption {SSE-B2,none}] [--defaultServerSideEncryptionAlgorithm {AES256}] bucketName [bucketType]
-    b2 upload-file [-h] [--noProgress] [--quiet] [--contentType CONTENTTYPE] [--minPartSize MINPARTSIZE] [--sha1 SHA1] [--threads THREADS] [--info INFO] [--destinationServerSideEncryption {SSE-B2,SSE-C}] [--destinationServerSideEncryptionAlgorithm {AES256}] [--legalHold {on,off}] [--fileRetentionMode {compliance,governance}] [--retainUntil TIMESTAMP] [--incrementalMode] bucketName localFilePath b2FileName
+    b2 update-bucket [-h] [--bucketInfo BUCKETINFO] [--corsRules CORSRULES] [--lifecycleRules LIFECYCLERULES] [--defaultRetentionMode {compliance,governance,none}] [--defaultRetentionPeriod period] [--replication REPLICATION] [--fileLockEnabled] [--defaultServerSideEncryption {SSE-B2,none}] [--defaultServerSideEncryptionAlgorithm {AES256}] bucketName [{allPublic,allPrivate}]
+    b2 upload-file [-h] [--noProgress] [--quiet] [--contentType CONTENTTYPE] [--minPartSize MINPARTSIZE] [--sha1 SHA1] [--threads THREADS] [--info INFO] [--custom-upload-timestamp CUSTOM_UPLOAD_TIMESTAMP] [--destinationServerSideEncryption {SSE-B2,SSE-C}] [--destinationServerSideEncryptionAlgorithm {AES256}] [--legalHold {on,off}] [--fileRetentionMode {compliance,governance}] [--retainUntil TIMESTAMP] [--incrementalMode] bucketName localFilePath b2FileName
     b2 update-file-legal-hold [-h] [fileName] fileId {on,off}
     b2 update-file-retention [-h] [--retainUntil TIMESTAMP] [--bypassGovernance] [fileName] fileId {governance,compliance,none}
     b2 replication-setup [-h] [--destination-profile DESTINATION_PROFILE] [--name NAME] [--priority PRIORITY] [--file-name-prefix PREFIX] [--include-existing-files] SOURCE_BUCKET_NAME DESTINATION_BUCKET_NAME
     b2 replication-delete [-h] SOURCE_BUCKET_NAME REPLICATION_RULE_NAME
     b2 replication-pause [-h] SOURCE_BUCKET_NAME REPLICATION_RULE_NAME
     b2 replication-unpause [-h] SOURCE_BUCKET_NAME REPLICATION_RULE_NAME
     b2 replication-status [-h] [--rule REPLICATION_RULE_NAME] [--destination-profile DESTINATION_PROFILE] [--dont-scan-destination] [--output-format {console,json,csv}] [--noProgress] [--columns COLUMN ONE,COLUMN TWO] SOURCE_BUCKET_NAME
     b2 version [-h]
     b2 license [-h]
+    b2 install-autocomplete [-h] [--shell {bash}]
 
 
 The environment variable `B2_ACCOUNT_INFO` specifies the sqlite
 file to use for caching authentication information.
 The default file to use is: `~/.b2_account_info`
 
 For more details on one command: `b2 <command> --help`
```

### Comparing `b2-3.8.0/README.md` & `b2-3.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 # Usage
 
     b2 authorize-account [-h]  [applicationKeyId] [applicationKey]
     b2 cancel-all-unfinished-large-files [-h] bucketName
     b2 cancel-large-file [-h] fileId
     b2 clear-account [-h]
     b2 copy-file-by-id [-h] [--fetchMetadata] [--contentType CONTENTTYPE] [--range RANGE] [--info INFO | --noInfo] [--destinationServerSideEncryption {SSE-B2,SSE-C}] [--destinationServerSideEncryptionAlgorithm {AES256}] [--sourceServerSideEncryption {SSE-C}] [--sourceServerSideEncryptionAlgorithm {AES256}] [--fileRetentionMode {compliance,governance}] [--retainUntil TIMESTAMP] [--legalHold {on,off}] sourceFileId destinationBucketName b2FileName
-    b2 create-bucket [-h] [--bucketInfo BUCKETINFO] [--corsRules CORSRULES] [--lifecycleRules LIFECYCLERULES] [--fileLockEnabled] [--replication REPLICATION] [--defaultServerSideEncryption {SSE-B2,none}] [--defaultServerSideEncryptionAlgorithm {AES256}] bucketName bucketType
+    b2 create-bucket [-h] [--bucketInfo BUCKETINFO] [--corsRules CORSRULES] [--lifecycleRules LIFECYCLERULES] [--fileLockEnabled] [--replication REPLICATION] [--defaultServerSideEncryption {SSE-B2,none}] [--defaultServerSideEncryptionAlgorithm {AES256}] bucketName {allPublic,allPrivate}
     b2 create-key [-h] [--bucket BUCKET] [--namePrefix NAMEPREFIX] [--duration DURATION] [--allCapabilities] keyName [capabilities]
     b2 delete-bucket [-h] bucketName
     b2 delete-file-version [-h] [fileName] fileId
     b2 delete-key [-h] applicationKeyId
     b2 download-file-by-id [-h] [--noProgress] [--threads THREADS] [--sourceServerSideEncryption {SSE-C}] [--sourceServerSideEncryptionAlgorithm {AES256}] [--write-buffer-size BYTES] [--skip-hash-verification] [--max-download-streams-per-file MAX_DOWNLOAD_STREAMS_PER_FILE] fileId localFileName
     b2 download-file-by-name [-h] [--noProgress] [--threads THREADS] [--sourceServerSideEncryption {SSE-C}] [--sourceServerSideEncryptionAlgorithm {AES256}] [--write-buffer-size BYTES] [--skip-hash-verification] [--max-download-streams-per-file MAX_DOWNLOAD_STREAMS_PER_FILE] bucketName b2FileName localFileName
     b2 get-account-info [-h]
@@ -66,25 +66,26 @@
     b2 list-parts [-h] largeFileId
     b2 list-unfinished-large-files [-h] bucketName
     b2 ls [-h] [--long] [--json] [--replication] [--versions] [--recursive] [--withWildcard] bucketName [folderName]
     b2 rm [-h] [--dryRun] [--threads THREADS] [--queueSize QUEUESIZE] [--noProgress] [--failFast] [--versions] [--recursive] [--withWildcard] bucketName [folderName]
     b2 make-url [-h] fileId
     b2 make-friendly-url [-h] bucketName fileName
     b2 sync [-h] [--noProgress] [--dryRun] [--allowEmptySource] [--excludeAllSymlinks] [--threads THREADS] [--syncThreads SYNCTHREADS] [--downloadThreads DOWNLOADTHREADS] [--uploadThreads UPLOADTHREADS] [--compareVersions {none,modTime,size}] [--compareThreshold MILLIS] [--excludeRegex REGEX] [--includeRegex REGEX] [--excludeDirRegex REGEX] [--excludeIfModifiedAfter TIMESTAMP] [--destinationServerSideEncryption {SSE-B2,SSE-C}] [--destinationServerSideEncryptionAlgorithm {AES256}] [--sourceServerSideEncryption {SSE-C}] [--sourceServerSideEncryptionAlgorithm {AES256}] [--write-buffer-size BYTES] [--skip-hash-verification] [--max-download-streams-per-file MAX_DOWNLOAD_STREAMS_PER_FILE] [--incrementalMode] [--skipNewer | --replaceNewer] [--delete | --keepDays DAYS] source destination
-    b2 update-bucket [-h] [--bucketInfo BUCKETINFO] [--corsRules CORSRULES] [--lifecycleRules LIFECYCLERULES] [--defaultRetentionMode {compliance,governance,none}] [--defaultRetentionPeriod period] [--replication REPLICATION] [--fileLockEnabled] [--defaultServerSideEncryption {SSE-B2,none}] [--defaultServerSideEncryptionAlgorithm {AES256}] bucketName [bucketType]
-    b2 upload-file [-h] [--noProgress] [--quiet] [--contentType CONTENTTYPE] [--minPartSize MINPARTSIZE] [--sha1 SHA1] [--threads THREADS] [--info INFO] [--destinationServerSideEncryption {SSE-B2,SSE-C}] [--destinationServerSideEncryptionAlgorithm {AES256}] [--legalHold {on,off}] [--fileRetentionMode {compliance,governance}] [--retainUntil TIMESTAMP] [--incrementalMode] bucketName localFilePath b2FileName
+    b2 update-bucket [-h] [--bucketInfo BUCKETINFO] [--corsRules CORSRULES] [--lifecycleRules LIFECYCLERULES] [--defaultRetentionMode {compliance,governance,none}] [--defaultRetentionPeriod period] [--replication REPLICATION] [--fileLockEnabled] [--defaultServerSideEncryption {SSE-B2,none}] [--defaultServerSideEncryptionAlgorithm {AES256}] bucketName [{allPublic,allPrivate}]
+    b2 upload-file [-h] [--noProgress] [--quiet] [--contentType CONTENTTYPE] [--minPartSize MINPARTSIZE] [--sha1 SHA1] [--threads THREADS] [--info INFO] [--custom-upload-timestamp CUSTOM_UPLOAD_TIMESTAMP] [--destinationServerSideEncryption {SSE-B2,SSE-C}] [--destinationServerSideEncryptionAlgorithm {AES256}] [--legalHold {on,off}] [--fileRetentionMode {compliance,governance}] [--retainUntil TIMESTAMP] [--incrementalMode] bucketName localFilePath b2FileName
     b2 update-file-legal-hold [-h] [fileName] fileId {on,off}
     b2 update-file-retention [-h] [--retainUntil TIMESTAMP] [--bypassGovernance] [fileName] fileId {governance,compliance,none}
     b2 replication-setup [-h] [--destination-profile DESTINATION_PROFILE] [--name NAME] [--priority PRIORITY] [--file-name-prefix PREFIX] [--include-existing-files] SOURCE_BUCKET_NAME DESTINATION_BUCKET_NAME
     b2 replication-delete [-h] SOURCE_BUCKET_NAME REPLICATION_RULE_NAME
     b2 replication-pause [-h] SOURCE_BUCKET_NAME REPLICATION_RULE_NAME
     b2 replication-unpause [-h] SOURCE_BUCKET_NAME REPLICATION_RULE_NAME
     b2 replication-status [-h] [--rule REPLICATION_RULE_NAME] [--destination-profile DESTINATION_PROFILE] [--dont-scan-destination] [--output-format {console,json,csv}] [--noProgress] [--columns COLUMN ONE,COLUMN TWO] SOURCE_BUCKET_NAME
     b2 version [-h]
     b2 license [-h]
+    b2 install-autocomplete [-h] [--shell {bash}]
 
 
 The environment variable `B2_ACCOUNT_INFO` specifies the sqlite
 file to use for caching authentication information.
 The default file to use is: `~/.b2_account_info`
 
 For more details on one command: `b2 <command> --help`
```

### Comparing `b2-3.8.0/README.release.md` & `b2-3.9.0/README.release.md`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/b2/LICENSE` & `b2-3.9.0/b2/LICENSE`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/b2/__init__.py` & `b2-3.9.0/b2/__init__.py`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/b2/_cli/argcompleters.py` & `b2-3.9.0/b2/_cli/argcompleters.py`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/b2/_cli/autocomplete_install.py` & `b2-3.9.0/b2/_cli/autocomplete_install.py`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/b2/_cli/b2api.py` & `b2-3.9.0/b2/_cli/b2api.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,17 +17,32 @@
 from b2sdk.v2 import B2Api
 
 from b2._cli.const import B2_USER_AGENT_APPEND_ENV_VAR
 
 
 def _get_b2api_for_profile(profile: Optional[str] = None, **kwargs) -> B2Api:
     account_info = SqliteAccountInfo(profile=profile)
-    return B2Api(
+    b2api = B2Api(
         api_config=_get_b2httpapiconfig(),
         account_info=account_info,
         cache=AuthInfoCache(account_info),
         **kwargs,
     )
 
+    if os.getenv('CI', False) and os.getenv(
+        'GITHUB_REPOSITORY',
+        '',
+    ).endswith('/B2_Command_Line_Tool'):
+        b2http = b2api.session.raw_api.b2_http
+        b2http.CONNECTION_TIMEOUT = 3 + 6 + 1
+        b2http.TIMEOUT = 12
+        b2http.TIMEOUT_FOR_COPY = 24
+        b2http.TIMEOUT_FOR_UPLOAD = 24
+        b2http.TRY_COUNT_DATA = 2
+        b2http.TRY_COUNT_DOWNLOAD = 2
+        b2http.TRY_COUNT_HEAD = 2
+        b2http.TRY_COUNT_OTHER = 2
+    return b2api
+
 
 def _get_b2httpapiconfig():
     return B2HttpApiConfig(user_agent_append=os.environ.get(B2_USER_AGENT_APPEND_ENV_VAR),)
```

### Comparing `b2-3.8.0/b2/_cli/const.py` & `b2-3.9.0/b2/_cli/const.py`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/b2/_cli/shell.py` & `b2-3.9.0/b2/_cli/shell.py`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/b2/arg_parser.py` & `b2-3.9.0/b2/arg_parser.py`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/b2/console_tool.py` & `b2-3.9.0/b2/console_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -2225,15 +2225,15 @@
     The ``--excludeDirRegex`` is a regular expression that is tested against
     the full path of each directory.  The path being matched does not have
     a trailing ``/``, so don't include on in your regular expression.
 
     Multiple regex rules can be applied by supplying them as pipe
     delimited instructions. Note that the regex for this command
     is Python regex.
-    Reference: `<https://docs.python.org/2/library/re.html>`_
+    Reference: `<https://docs.python.org/3/library/re.html>`_
 
     Regular expressions are considered a match if they match a substring
     starting at the first character.  ``.*e`` will match ``hello``.  This is
     not ideal, but we will maintain this behavior for compatibility.
     If you want to match the entire path, put a ``$`` at the end of the
     regex, such as ``.*llo$``.
 
@@ -2630,28 +2630,35 @@
     Each fileInfo is of the form ``a=b``.
 
     {DESTINATIONSSEMIXIN}
     {FILERETENTIONSETTINGMIXIN}
     {LEGALHOLDMIXIN}
     {UPLOADMODEMIXIN}
 
+    The ``--custom-upload-timestamp``, in milliseconds-since-epoch, can be used
+    to artificially change the upload timestamp of the file for the purpose
+    of preserving retention policies after migration of data from other storage.
+    The access to this feature is restricted - if you really need it, you'll
+    need to contact customer support to enable it temporarily for your account.
+
     Requires capability:
 
     - **writeFiles**
     """
 
     @classmethod
     def _setup_parser(cls, parser):
         parser.add_argument('--noProgress', action='store_true')
         parser.add_argument('--quiet', action='store_true')
         parser.add_argument('--contentType')
         parser.add_argument('--minPartSize', type=int)
         parser.add_argument('--sha1')
         parser.add_argument('--threads', type=int, default=10)
         parser.add_argument('--info', action='append', default=[])
+        parser.add_argument('--custom-upload-timestamp', type=int)
         parser.add_argument('bucketName').completer = bucket_name_completer
         parser.add_argument('localFilePath')
         parser.add_argument('b2FileName')
 
         super()._setup_parser(parser)  # add parameters from the mixins
 
     def run(self, args):
@@ -2678,14 +2685,15 @@
             sha1_sum=args.sha1,
             min_part_size=args.minPartSize,
             progress_listener=make_progress_listener(args.localFilePath, args.noProgress),
             encryption=encryption_setting,
             file_retention=file_retention,
             legal_hold=legal_hold,
             upload_mode=self._get_upload_mode_from_args(args),
+            custom_upload_timestamp=args.custom_upload_timestamp,
         )
         if not args.quiet:
             self._print("URL by file name: " + bucket.get_download_url(args.b2FileName))
             self._print("URL by fileId: " + self.api.get_download_url_for_fileid(file_info.id_))
         self._print_json(file_info)
         return 0
 
@@ -3323,23 +3331,26 @@
         parser.add_argument('--shell', choices=SUPPORTED_SHELLS, default=None)
         super()._setup_parser(parser)
 
     def run(self, args):
         shell = args.shell or detect_shell()
         if shell not in SUPPORTED_SHELLS:
             self._print_stderr(
-                f'ERROR: unsupported shell: %s. Supported shells: {SUPPORTED_SHELLS}. Use --shell to specify a target shell manually.'
+                f'ERROR: unsupported shell: {shell}. Supported shells: {SUPPORTED_SHELLS}. Use --shell to specify a target shell manually.'
             )
             return 1
 
         try:
             autocomplete_install(NAME, shell=shell)
         except AutocompleteInstallError as e:
             raise CommandError(str(e)) from e
-        self._print(f'Autocomplete installed for {shell}.')
+        self._print(f'Autocomplete successfully installed for {shell}.')
+        self._print(
+            f'Spawn a new shell instance to use it (log in again or just type `{shell}` in your current shell to start a new session inside of the existing session).'
+        )
         return 0
 
 
 class ConsoleTool(object):
     """
     Implements the commands available in the B2 command-line tool
     using the B2Api library.
```

### Comparing `b2-3.8.0/b2/json_encoder.py` & `b2-3.9.0/b2/json_encoder.py`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/b2/licenses_output.txt` & `b2-3.9.0/b2/licenses_output.txt`

 * *Files 0% similar despite different names*

```diff
@@ -10159,660 +10159,723 @@
 00027ae0: 6974 2069 6e20 6269 6e61 7279 2066 6f72  it in binary for
 00027af0: 6d3a 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  m:.+------------
 00027b00: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
 00027b10: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
 00027b20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00027b30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
 00027b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027b50: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
-00027b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00027b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00027b60: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
 00027b70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027b80: 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 2020 204d  --------+.|    M
-00027b90: 6f64 756c 6520 6e61 6d65 2020 2020 207c  odule name     |
-00027ba0: 2020 5665 7273 696f 6e20 207c 2020 2020    Version  |    
-00027bb0: 2020 2020 2020 2020 2020 2020 4c69 6365              Lice
-00027bc0: 6e73 6520 2020 2020 2020 2020 2020 2020  nse             
-00027bd0: 2020 207c 2020 2020 2020 2020 2020 2041     |           A
-00027be0: 7574 686f 7220 2020 2020 2020 2020 2020  uthor           
-00027bf0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00027c00: 2020 2020 2020 5552 4c20 2020 2020 2020        URL       
-00027c10: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00027c20: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
-00027c30: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
-00027c40: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
-00027c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00027b80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00027b90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20  ------------+.| 
+00027ba0: 2020 204d 6f64 756c 6520 6e61 6d65 2020     Module name  
+00027bb0: 2020 207c 2020 5665 7273 696f 6e20 207c     |  Version  |
+00027bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027bd0: 4c69 6365 6e73 6520 2020 2020 2020 2020  License         
+00027be0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+00027bf0: 2020 2020 2020 2020 4175 7468 6f72 2020          Author  
+00027c00: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00027c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027c20: 2020 2020 2020 2020 2055 524c 2020 2020           URL    
+00027c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027c40: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
+00027c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
 00027c60: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
 00027c70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027c80: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-00027c90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00027c80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00027c90: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
 00027ca0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027cb0: 2d2d 2d2d 2d2d 2b0a 7c20 2020 2061 7267  ------+.|    arg
-00027cc0: 636f 6d70 6c65 7465 2020 2020 207c 2020  complete     |  
-00027cd0: 2032 2e31 2e32 2020 207c 2020 2020 2020   2.1.2   |      
-00027ce0: 2020 4170 6163 6865 2053 6f66 7477 6172    Apache Softwar
-00027cf0: 6520 4c69 6365 6e73 6520 2020 2020 2020  e License       
-00027d00: 207c 2020 2020 2020 2041 6e64 7265 7920   |       Andrey 
-00027d10: 4b69 736c 7975 6b20 2020 2020 2020 7c20  Kislyuk       | 
-00027d20: 2020 2068 7474 7073 3a2f 2f67 6974 6875     https://githu
-00027d30: 622e 636f 6d2f 6b69 736c 7975 6b2f 6172  b.com/kislyuk/ar
-00027d40: 6763 6f6d 706c 6574 6520 2020 207c 0a2b  gcomplete    |.+
-00027d50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027d60: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-00027d70: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-00027d80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027d90: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00027cb0: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
+00027cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00027cd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00027ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00027cf0: 2d2d 2b0a 7c20 2020 2061 7267 636f 6d70  --+.|    argcomp
+00027d00: 6c65 7465 2020 2020 207c 2020 2033 2e30  lete     |   3.0
+00027d10: 2e38 2020 207c 2020 2020 2020 2020 4170  .8   |        Ap
+00027d20: 6163 6865 2053 6f66 7477 6172 6520 4c69  ache Software Li
+00027d30: 6365 6e73 6520 2020 2020 2020 207c 2020  cense        |  
+00027d40: 2020 2020 2020 2020 2020 416e 6472 6579            Andrey
+00027d50: 204b 6973 6c79 756b 2020 2020 2020 2020   Kislyuk        
+00027d60: 2020 2020 7c20 2020 2020 2020 2020 6874      |         ht
+00027d70: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00027d80: 2f6b 6973 6c79 756b 2f61 7267 636f 6d70  /kislyuk/argcomp
+00027d90: 6c65 7465 2020 2020 2020 2020 207c 0a2b  lete         |.+
 00027da0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027db0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
-00027dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00027db0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
+00027dc0: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
 00027dd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027de0: 2d2d 2d2d 2b0a 7c20 2020 2020 2020 6172  ----+.|       ar
-00027df0: 726f 7720 2020 2020 2020 207c 2020 2031  row        |   1
-00027e00: 2e32 2e33 2020 207c 2020 2020 2020 2020  .2.3   |        
-00027e10: 4170 6163 6865 2053 6f66 7477 6172 6520  Apache Software 
-00027e20: 4c69 6365 6e73 6520 2020 2020 2020 207c  License        |
-00027e30: 2020 2020 2020 2020 4368 7269 7320 536d          Chris Sm
-00027e40: 6974 6820 2020 2020 2020 2020 7c20 2020  ith         |   
-00027e50: 2020 2020 2020 6874 7470 733a 2f2f 6172        https://ar
-00027e60: 726f 772e 7265 6164 7468 6564 6f63 732e  row.readthedocs.
-00027e70: 696f 2020 2020 2020 2020 207c 0a2b 2d2d  io         |.+--
-00027e80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027e90: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --+-----------+-
-00027ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027eb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027ec0: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
-00027ed0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027ee0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
-00027ef0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027f00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027f10: 2d2d 2b0a 7c20 2020 2020 2020 6232 7364  --+.|       b2sd
-00027f20: 6b20 2020 2020 2020 207c 2020 2031 2e32  k        |   1.2
-00027f30: 302e 3020 207c 2020 2020 2020 2020 2020  0.0  |          
-00027f40: 2020 2020 4d49 5420 4c69 6365 6e73 6520      MIT License 
-00027f50: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00027f60: 2020 2020 4261 636b 626c 617a 652c 2049      Backblaze, I
-00027f70: 6e63 2e20 2020 2020 2020 7c20 2068 7474  nc.       |  htt
-00027f80: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00027f90: 4261 636b 626c 617a 652f 6232 2d73 646b  Backblaze/b2-sdk
-00027fa0: 2d70 7974 686f 6e20 207c 0a2b 2d2d 2d2d  -python  |.+----
-00027fb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027fc0: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  +-----------+---
-00027fd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027fe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027ff0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-00028000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028010: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-00028020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028040: 2b0a 7c20 2020 2020 2063 6572 7469 6669  +.|      certifi
-00028050: 2020 2020 2020 207c 2032 3032 322e 3132         | 2022.12
-00028060: 2e37 207c 2020 4d6f 7a69 6c6c 6120 5075  .7 |  Mozilla Pu
-00028070: 626c 6963 204c 6963 656e 7365 2032 2e30  blic License 2.0
-00028080: 2028 4d50 4c20 322e 3029 207c 2020 2020   (MPL 2.0) |    
-00028090: 2020 204b 656e 6e65 7468 2052 6569 747a     Kenneth Reitz
-000280a0: 2020 2020 2020 2020 7c20 2068 7474 7073          |  https
-000280b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6365  ://github.com/ce
-000280c0: 7274 6966 692f 7079 7468 6f6e 2d63 6572  rtifi/python-cer
-000280d0: 7469 6669 2020 207c 0a2b 2d2d 2d2d 2d2d  tifi   |.+------
-000280e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
-000280f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
-00028100: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028110: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028120: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
-00028130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00028140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028150: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028160: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a  --------------+.
-00028170: 7c20 6368 6172 7365 742d 6e6f 726d 616c  | charset-normal
-00028180: 697a 6572 207c 2020 2033 2e31 2e30 2020  izer |   3.1.0  
-00028190: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-000281a0: 4d49 5420 4c69 6365 6e73 6520 2020 2020  MIT License     
-000281b0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-000281c0: 2020 4168 6d65 6420 5441 4852 4920 2020    Ahmed TAHRI   
-000281d0: 2020 2020 2020 7c20 6874 7470 733a 2f2f        | https://
-000281e0: 6769 7468 7562 2e63 6f6d 2f4f 7573 7265  github.com/Ousre
-000281f0: 742f 6368 6172 7365 745f 6e6f 726d 616c  t/charset_normal
-00028200: 697a 6572 207c 0a2b 2d2d 2d2d 2d2d 2d2d  izer |.+--------
-00028210: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
-00028220: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00027de0: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00027df0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00027e00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+00027e10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00027e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00027e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00027e40: 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 2020 2020  --------+.|     
+00027e50: 2020 6172 726f 7720 2020 2020 2020 207c    arrow        |
+00027e60: 2020 2031 2e32 2e33 2020 207c 2020 2020     1.2.3   |    
+00027e70: 2020 2020 4170 6163 6865 2053 6f66 7477      Apache Softw
+00027e80: 6172 6520 4c69 6365 6e73 6520 2020 2020  are License     
+00027e90: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+00027ea0: 2043 6872 6973 2053 6d69 7468 2020 2020   Chris Smith    
+00027eb0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+00027ec0: 2020 2020 2020 2020 2068 7474 7073 3a2f           https:/
+00027ed0: 2f61 7272 6f77 2e72 6561 6474 6865 646f  /arrow.readthedo
+00027ee0: 6373 2e69 6f20 2020 2020 2020 2020 2020  cs.io           
+00027ef0: 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d     |.+----------
+00027f00: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
+00027f10: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+00027f20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00027f30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
+00027f40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00027f50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00027f60: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+00027f70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00027f80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00027f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a  --------------+.
+00027fa0: 7c20 2020 2020 2020 6232 7364 6b20 2020  |       b2sdk   
+00027fb0: 2020 2020 207c 2020 2031 2e32 312e 3020       |   1.21.0 
+00027fc0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+00027fd0: 4d49 5420 4c69 6365 6e73 6520 2020 2020  MIT License     
+00027fe0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+00027ff0: 2020 2020 2042 6163 6b62 6c61 7a65 2c20       Backblaze, 
+00028000: 496e 632e 2020 2020 2020 2020 2020 2020  Inc.            
+00028010: 7c20 2020 2020 2020 6874 7470 733a 2f2f  |       https://
+00028020: 6769 7468 7562 2e63 6f6d 2f42 6163 6b62  github.com/Backb
+00028030: 6c61 7a65 2f62 322d 7364 6b2d 7079 7468  laze/b2-sdk-pyth
+00028040: 6f6e 2020 2020 2020 207c 0a2b 2d2d 2d2d  on       |.+----
+00028050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028060: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  +-----------+---
+00028070: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028090: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
+000280a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000280b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+000280c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000280d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000280e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000280f0: 2d2d 2d2d 2b0a 7c20 2020 2020 2063 6572  ----+.|      cer
+00028100: 7469 6669 2020 2020 2020 207c 2032 3032  tifi       | 202
+00028110: 322e 3132 2e37 207c 2020 4d6f 7a69 6c6c  2.12.7 |  Mozill
+00028120: 6120 5075 626c 6963 204c 6963 656e 7365  a Public License
+00028130: 2032 2e30 2028 4d50 4c20 322e 3029 207c   2.0 (MPL 2.0) |
+00028140: 2020 2020 2020 2020 2020 2020 4b65 6e6e              Kenn
+00028150: 6574 6820 5265 6974 7a20 2020 2020 2020  eth Reitz       
+00028160: 2020 2020 2020 7c20 2020 2020 2020 6874        |       ht
+00028170: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00028180: 2f63 6572 7469 6669 2f70 7974 686f 6e2d  /certifi/python-
+00028190: 6365 7274 6966 6920 2020 2020 2020 207c  certifi        |
+000281a0: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
+000281b0: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+000281c0: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
+000281d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000281e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
+000281f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028200: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028210: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
+00028220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00028230: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028250: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-00028260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
-00028270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028290: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20  ------------+.| 
-000282a0: 2020 2020 2064 6f63 7574 696c 7320 2020       docutils   
-000282b0: 2020 207c 2020 2020 302e 3139 2020 207c     |    0.19   |
-000282c0: 2020 2020 2020 2020 2020 2020 2020 4253                BS
-000282d0: 4420 4c69 6365 6e73 6520 2020 2020 2020  D License       
-000282e0: 2020 2020 2020 207c 2020 2020 2020 2044         |       D
-000282f0: 6176 6964 2047 6f6f 6467 6572 2020 2020  avid Goodger    
-00028300: 2020 2020 7c20 2020 2020 2020 6874 7470      |       http
-00028310: 733a 2f2f 646f 6375 7469 6c73 2e73 6f75  s://docutils.sou
-00028320: 7263 6566 6f72 6765 2e69 6f2f 2020 2020  rceforge.io/    
-00028330: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-00028340: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00028350: 2020 2020 2020 7c20 2020 2047 4e55 2047        |    GNU G
-00028360: 656e 6572 616c 2050 7562 6c69 6320 4c69  eneral Public Li
-00028370: 6365 6e73 6520 2847 504c 2920 2020 7c20  cense (GPL)   | 
-00028380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028390: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-000283a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000283b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000283c0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
-000283d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000283e0: 207c 2020 2020 2020 2020 2020 207c 2020   |           |  
-000283f0: 2020 2020 2020 2020 2020 2020 5075 626c              Publ
-00028400: 6963 2044 6f6d 6169 6e20 2020 2020 2020  ic Domain       
-00028410: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00028420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028430: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00028440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028240: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 6368  ----------+.| ch
+00028250: 6172 7365 742d 6e6f 726d 616c 697a 6572  arset-normalizer
+00028260: 207c 2020 2033 2e31 2e30 2020 207c 2020   |   3.1.0   |  
+00028270: 2020 2020 2020 2020 2020 2020 4d49 5420              MIT 
+00028280: 4c69 6365 6e73 6520 2020 2020 2020 2020  License         
+00028290: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+000282a0: 2020 2041 686d 6564 2054 4148 5249 2020     Ahmed TAHRI  
+000282b0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+000282c0: 2020 2068 7474 7073 3a2f 2f67 6974 6875     https://githu
+000282d0: 622e 636f 6d2f 4f75 7372 6574 2f63 6861  b.com/Ousret/cha
+000282e0: 7273 6574 5f6e 6f72 6d61 6c69 7a65 7220  rset_normalizer 
+000282f0: 2020 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d       |.+--------
+00028300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+00028310: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00028320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028340: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
+00028350: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028360: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+00028370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000283a0: 2b0a 7c20 2020 2020 2064 6f63 7574 696c  +.|      docutil
+000283b0: 7320 2020 2020 207c 2020 2020 302e 3139  s      |    0.19
+000283c0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+000283d0: 2020 4253 4420 4c69 6365 6e73 6520 2020    BSD License   
+000283e0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+000283f0: 2020 2020 2020 2020 4461 7669 6420 476f          David Go
+00028400: 6f64 6765 7220 2020 2020 2020 2020 2020  odger           
+00028410: 2020 7c20 2020 2020 2020 2020 2020 2068    |            h
+00028420: 7474 7073 3a2f 2f64 6f63 7574 696c 732e  ttps://docutils.
+00028430: 736f 7572 6365 666f 7267 652e 696f 2f20  sourceforge.io/ 
+00028440: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 00028450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028460: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-00028470: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00028480: 2020 2020 7c20 2020 5079 7468 6f6e 2053      |   Python S
-00028490: 6f66 7477 6172 6520 466f 756e 6461 7469  oftware Foundati
-000284a0: 6f6e 204c 6963 656e 7365 2020 7c20 2020  on License  |   
-000284b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000284c0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+00028460: 2020 7c20 2020 2020 2020 2020 2020 7c20    |           | 
+00028470: 2020 2047 4e55 2047 656e 6572 616c 2050     GNU General P
+00028480: 7562 6c69 6320 4c69 6365 6e73 6520 2847  ublic License (G
+00028490: 504c 2920 2020 7c20 2020 2020 2020 2020  PL)   |         
+000284a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000284b0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+000284c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000284d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000284e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000284f0: 2020 2020 2020 2020 7c0a 2b2d 2d2d 2d2d          |.+-----
-00028500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00028510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
-00028520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028530: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028540: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
-00028550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028560: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-00028570: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00028590: 0a7c 2020 2020 2020 2020 6964 6e61 2020  .|        idna  
-000285a0: 2020 2020 2020 7c20 2020 2033 2e34 2020        |    3.4  
-000285b0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-000285c0: 2042 5344 204c 6963 656e 7365 2020 2020   BSD License    
-000285d0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-000285e0: 2020 2020 2055 4e4b 4e4f 574e 2020 2020       UNKNOWN    
-000285f0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00028600: 2020 2020 2020 2020 2020 2055 4e4b 4e4f             UNKNO
-00028610: 574e 2020 2020 2020 2020 2020 2020 2020  WN              
-00028620: 2020 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d        |.+-------
-00028630: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
-00028640: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
+000284f0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
+00028500: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+00028510: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+00028520: 2020 2020 2020 2020 5075 626c 6963 2044          Public D
+00028530: 6f6d 6169 6e20 2020 2020 2020 2020 2020  omain           
+00028540: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+00028550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028560: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00028570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000285a0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+000285b0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+000285c0: 2020 2020 7c20 2020 5079 7468 6f6e 2053      |   Python S
+000285d0: 6f66 7477 6172 6520 466f 756e 6461 7469  oftware Foundati
+000285e0: 6f6e 204c 6963 656e 7365 2020 7c20 2020  on License  |   
+000285f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028610: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+00028620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028640: 2020 2020 2020 2020 2020 2020 7c0a 2b2d              |.+-
 00028650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028670: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-00028680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
-00028690: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028660: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---+-----------+
+00028670: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028690: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
 000286a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000286b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c  -------------+.|
-000286c0: 2020 2020 2020 6c6f 6766 7572 7920 2020        logfury   
-000286d0: 2020 2020 7c20 2020 312e 302e 3120 2020      |   1.0.1   
-000286e0: 7c20 2020 2020 2020 2020 2020 2020 2042  |              B
-000286f0: 5344 204c 6963 656e 7365 2020 2020 2020  SD License      
-00028700: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00028710: 5061 7765 6c20 506f 6c65 7769 637a 2020  Pawel Polewicz  
-00028720: 2020 2020 207c 2068 7474 7073 3a2f 2f67       | https://g
-00028730: 6974 6875 622e 636f 6d2f 7265 6566 2d74  ithub.com/reef-t
-00028740: 6563 686e 6f6c 6f67 6965 732f 6c6f 6766  echnologies/logf
-00028750: 7572 7920 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d  ury |.+---------
-00028760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
-00028770: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-00028780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-000287a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000287b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
-000287c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000286b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
+000286c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000286d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000286e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000286f0: 2d2d 2d2d 2d2d 2d2b 0a7c 2020 2020 2020  -------+.|      
+00028700: 2020 6964 6e61 2020 2020 2020 2020 7c20    idna        | 
+00028710: 2020 2033 2e34 2020 2020 7c20 2020 2020     3.4    |     
+00028720: 2020 2020 2020 2020 2042 5344 204c 6963           BSD Lic
+00028730: 656e 7365 2020 2020 2020 2020 2020 2020  ense            
+00028740: 2020 7c20 2020 4b69 6d20 4461 7669 6573    |   Kim Davies
+00028750: 203c 6b69 6d40 6379 6e6f 7375 7265 2e63   <kim@cynosure.c
+00028760: 6f6d 2e61 753e 2020 207c 2020 2020 2020  om.au>   |      
+00028770: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
+00028780: 6769 7468 7562 2e63 6f6d 2f6b 6a64 2f69  github.com/kjd/i
+00028790: 646e 6120 2020 2020 2020 2020 2020 2020  dna             
+000287a0: 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d    |.+-----------
+000287b0: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
+000287c0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
 000287d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000287e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2070  -----------+.| p
-000287f0: 6878 2d63 6c61 7373 2d72 6567 6973 7472  hx-class-registr
-00028800: 7920 7c20 2020 342e 302e 3520 2020 7c20  y |   4.0.5   | 
-00028810: 2020 2020 2020 2020 2020 2020 204d 4954               MIT
-00028820: 204c 6963 656e 7365 2020 2020 2020 2020   License        
-00028830: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00028840: 2055 4e4b 4e4f 574e 2020 2020 2020 2020   UNKNOWN        
-00028850: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00028860: 2020 2020 2020 2055 4e4b 4e4f 574e 2020         UNKNOWN  
-00028870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028880: 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d    |.+-----------
-00028890: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
-000288a0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
-000288b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000288c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
-000288d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000288e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
-000288f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028900: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028910: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2020 2020  ---------+.|    
-00028920: 2020 2020 7069 7020 2020 2020 2020 2020      pip         
-00028930: 7c20 2020 3232 2e33 2e31 2020 7c20 2020  |   22.3.1  |   
-00028940: 2020 2020 2020 2020 2020 204d 4954 204c             MIT L
-00028950: 6963 656e 7365 2020 2020 2020 2020 2020  icense          
-00028960: 2020 2020 7c20 2020 2020 5468 6520 7069      |     The pi
-00028970: 7020 6465 7665 6c6f 7065 7273 2020 2020  p developers    
-00028980: 207c 2020 2020 2020 2020 2020 2020 2068   |             h
-00028990: 7474 7073 3a2f 2f70 6970 2e70 7970 612e  ttps://pip.pypa.
-000289a0: 696f 2f20 2020 2020 2020 2020 2020 2020  io/             
-000289b0: 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.+-------------
-000289c0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-000289d0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
-000289e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000289f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
-00028a00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028a10: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00028a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028a30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028a40: 2d2d 2d2d 2d2d 2d2b 0a7c 2020 2020 7069  -------+.|    pi
-00028a50: 702d 6c69 6365 6e73 6573 2020 2020 7c20  p-licenses    | 
-00028a60: 2020 342e 302e 3320 2020 7c20 2020 2020    4.0.3   |     
-00028a70: 2020 2020 2020 2020 204d 4954 204c 6963           MIT Lic
-00028a80: 656e 7365 2020 2020 2020 2020 2020 2020  ense            
-00028a90: 2020 7c20 2020 2020 2020 2020 2020 7261    |           ra
-00028aa0: 696d 6f6e 2020 2020 2020 2020 2020 207c  imon           |
-00028ab0: 2020 2068 7474 7073 3a2f 2f67 6974 6875     https://githu
-00028ac0: 622e 636f 6d2f 7261 696d 6f6e 3439 2f70  b.com/raimon49/p
-00028ad0: 6970 2d6c 6963 656e 7365 7320 2020 7c0a  ip-licenses   |.
-00028ae0: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-00028af0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
-00028b00: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-00028b10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028b20: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
-00028b30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028b40: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
-00028b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028b70: 2d2d 2d2d 2d2b 0a7c 2020 2020 7072 6574  -----+.|    pret
-00028b80: 7479 7461 626c 6520 2020 2020 7c20 2020  tytable     |   
-00028b90: 332e 362e 3020 2020 7c20 2020 2020 2020  3.6.0   |       
-00028ba0: 2020 2020 2020 2042 5344 204c 6963 656e         BSD Licen
-00028bb0: 7365 2020 2020 2020 2020 2020 2020 2020  se              
-00028bc0: 7c20 2020 2020 2020 2020 2055 4e4b 4e4f  |          UNKNO
-00028bd0: 574e 2020 2020 2020 2020 2020 207c 2020  WN           |  
-00028be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028bf0: 2055 4e4b 4e4f 574e 2020 2020 2020 2020   UNKNOWN        
-00028c00: 2020 2020 2020 2020 2020 2020 7c0a 2b2d              |.+-
-00028c10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028c20: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---+-----------+
+000287e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+000287f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028810: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
+00028820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c  -------------+.|
+00028850: 2020 2020 2020 6c6f 6766 7572 7920 2020        logfury   
+00028860: 2020 2020 7c20 2020 312e 302e 3120 2020      |   1.0.1   
+00028870: 7c20 2020 2020 2020 2020 2020 2020 2042  |              B
+00028880: 5344 204c 6963 656e 7365 2020 2020 2020  SD License      
+00028890: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+000288a0: 2020 2020 2050 6177 656c 2050 6f6c 6577       Pawel Polew
+000288b0: 6963 7a20 2020 2020 2020 2020 2020 207c  icz            |
+000288c0: 2020 2020 2020 6874 7470 733a 2f2f 6769        https://gi
+000288d0: 7468 7562 2e63 6f6d 2f72 6565 662d 7465  thub.com/reef-te
+000288e0: 6368 6e6f 6c6f 6769 6573 2f6c 6f67 6675  chnologies/logfu
+000288f0: 7279 2020 2020 2020 7c0a 2b2d 2d2d 2d2d  ry      |.+-----
+00028900: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+00028910: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+00028920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028940: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
+00028950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028960: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
+00028970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000289a0: 2d2d 2d2b 0a7c 2070 6878 2d63 6c61 7373  ---+.| phx-class
+000289b0: 2d72 6567 6973 7472 7920 7c20 2020 342e  -registry |   4.
+000289c0: 302e 3620 2020 7c20 2020 2020 2020 2020  0.6   |         
+000289d0: 2020 2020 204d 4954 204c 6963 656e 7365       MIT License
+000289e0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+000289f0: 2020 2020 2050 686f 656e 6978 205a 6572       Phoenix Zer
+00028a00: 696e 203c 7068 7840 7068 782e 6e7a 3e20  in <phx@phx.nz> 
+00028a10: 2020 2020 207c 2068 7474 7073 3a2f 2f67       | https://g
+00028a20: 6974 6875 622e 636f 6d2f 746f 646f 6669  ithub.com/todofi
+00028a30: 7874 6869 732f 636c 6173 732d 7265 6769  xthis/class-regi
+00028a40: 7374 7279 2f72 656c 6561 7365 7320 7c0a  stry/releases |.
+00028a50: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
+00028a60: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+00028a70: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
+00028a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028a90: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
+00028aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028ac0: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
+00028ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028af0: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2020 2020  ---------+.|    
+00028b00: 2020 2020 7069 7020 2020 2020 2020 2020      pip         
+00028b10: 7c20 2020 3232 2e33 2e31 2020 7c20 2020  |   22.3.1  |   
+00028b20: 2020 2020 2020 2020 2020 204d 4954 204c             MIT L
+00028b30: 6963 656e 7365 2020 2020 2020 2020 2020  icense          
+00028b40: 2020 2020 7c20 2020 2020 2020 2020 2054      |          T
+00028b50: 6865 2070 6970 2064 6576 656c 6f70 6572  he pip developer
+00028b60: 7320 2020 2020 2020 2020 207c 2020 2020  s          |    
+00028b70: 2020 2020 2020 2020 2020 2020 2020 6874                ht
+00028b80: 7470 733a 2f2f 7069 702e 7079 7061 2e69  tps://pip.pypa.i
+00028b90: 6f2f 2020 2020 2020 2020 2020 2020 2020  o/              
+00028ba0: 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d      |.+---------
+00028bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+00028bc0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+00028bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028be0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+00028bf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028c00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028c10: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+00028c20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00028c30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028c50: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-00028c60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028c70: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-00028c80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028c90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028ca0: 2d2d 2d2b 0a7c 2020 7079 7468 6f6e 2d64  ---+.|  python-d
-00028cb0: 6174 6575 7469 6c20 2020 7c20 2020 322e  ateutil   |   2.
-00028cc0: 382e 3220 2020 7c20 2020 2020 2020 2041  8.2   |        A
-00028cd0: 7061 6368 6520 536f 6674 7761 7265 204c  pache Software L
-00028ce0: 6963 656e 7365 2020 2020 2020 2020 7c20  icense        | 
-00028cf0: 2020 2020 2047 7573 7461 766f 204e 6965       Gustavo Nie
-00028d00: 6d65 7965 7220 2020 2020 207c 2020 2020  meyer      |    
-00028d10: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00028d20: 636f 6d2f 6461 7465 7574 696c 2f64 6174  com/dateutil/dat
-00028d30: 6575 7469 6c20 2020 2020 7c0a 7c20 2020  eutil     |.|   
-00028d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028d50: 207c 2020 2020 2020 2020 2020 207c 2020   |           |  
-00028d60: 2020 2020 2020 2020 2020 2020 2042 5344               BSD
-00028d70: 204c 6963 656e 7365 2020 2020 2020 2020   License        
-00028d80: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00028d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028da0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00028db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028dd0: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
-00028de0: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00028df0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-00028e00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028e10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
-00028e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028e30: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
-00028e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028e50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028e60: 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 2020 2020  --------+.|     
-00028e70: 2072 6571 7565 7374 7320 2020 2020 207c   requests      |
-00028e80: 2020 2032 2e32 382e 3220 207c 2020 2020     2.28.2  |    
-00028e90: 2020 2020 4170 6163 6865 2053 6f66 7477      Apache Softw
-00028ea0: 6172 6520 4c69 6365 6e73 6520 2020 2020  are License     
-00028eb0: 2020 207c 2020 2020 2020 204b 656e 6e65     |       Kenne
-00028ec0: 7468 2052 6569 747a 2020 2020 2020 2020  th Reitz        
-00028ed0: 7c20 2020 2020 2020 6874 7470 733a 2f2f  |       https://
-00028ee0: 7265 7175 6573 7473 2e72 6561 6474 6865  requests.readthe
-00028ef0: 646f 6373 2e69 6f20 2020 2020 2020 207c  docs.io        |
-00028f00: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
-00028f10: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
-00028f20: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
-00028f30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028f40: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
-00028f50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028f60: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-00028f70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028f80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028f90: 2d2d 2d2d 2d2d 2b0a 7c20 2020 2020 2072  ------+.|      r
-00028fa0: 7374 3261 6e73 6920 2020 2020 207c 2020  st2ansi      |  
-00028fb0: 2030 2e31 2e35 2020 207c 2020 2020 2020   0.1.5   |      
-00028fc0: 2020 2020 2020 2020 4d49 5420 4c69 6365          MIT Lice
-00028fd0: 6e73 6520 2020 2020 2020 2020 2020 2020  nse             
-00028fe0: 207c 2020 2020 2020 2020 2020 2053 6e61   |           Sna
-00028ff0: 6970 6520 2020 2020 2020 2020 2020 7c20  ipe           | 
-00029000: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00029010: 6f6d 2f53 6e61 6970 652f 7079 7468 6f6e  om/Snaipe/python
-00029020: 2d72 7374 2d74 6f2d 616e 7369 207c 0a2b  -rst-to-ansi |.+
-00029030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029040: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-00029050: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-00029060: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029070: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00028c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+00028c50: 0a7c 2020 2020 7069 702d 6c69 6365 6e73  .|    pip-licens
+00028c60: 6573 2020 2020 7c20 2020 342e 332e 3020  es    |   4.3.0 
+00028c70: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+00028c80: 204d 4954 204c 6963 656e 7365 2020 2020   MIT License    
+00028c90: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+00028ca0: 2020 2020 2020 2020 2020 2072 6169 6d6f             raimo
+00028cb0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00028cc0: 207c 2020 2020 2020 2020 6874 7470 733a   |        https:
+00028cd0: 2f2f 6769 7468 7562 2e63 6f6d 2f72 6169  //github.com/rai
+00028ce0: 6d6f 6e34 392f 7069 702d 6c69 6365 6e73  mon49/pip-licens
+00028cf0: 6573 2020 2020 2020 2020 7c0a 2b2d 2d2d  es        |.+---
+00028d00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028d10: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -+-----------+--
+00028d20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028d30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028d40: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+00028d50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028d60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+00028d70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028d80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028d90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028da0: 2d2d 2d2d 2d2b 0a7c 2020 2020 7072 6574  -----+.|    pret
+00028db0: 7479 7461 626c 6520 2020 2020 7c20 2020  tytable     |   
+00028dc0: 332e 372e 3020 2020 7c20 2020 2020 2020  3.7.0   |       
+00028dd0: 2020 2020 2020 2042 5344 204c 6963 656e         BSD Licen
+00028de0: 7365 2020 2020 2020 2020 2020 2020 2020  se              
+00028df0: 7c20 204c 756b 6520 4d61 7572 6974 7320  |  Luke Maurits 
+00028e00: 3c6c 756b 6540 6d61 7572 6974 732e 6964  <luke@maurits.id
+00028e10: 2e61 753e 2020 207c 2020 2020 2020 2020  .au>   |        
+00028e20: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00028e30: 6f6d 2f6a 617a 7a62 616e 642f 7072 6574  om/jazzband/pret
+00028e40: 7479 7461 626c 6520 2020 2020 2020 2020  tytable         
+00028e50: 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.+-------------
+00028e60: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+00028e70: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
+00028e80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+00028ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028eb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028ec0: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
+00028ed0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028ee0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00028ef0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2020  -----------+.|  
+00028f00: 7079 7468 6f6e 2d64 6174 6575 7469 6c20  python-dateutil 
+00028f10: 2020 7c20 2020 322e 382e 3220 2020 7c20    |   2.8.2   | 
+00028f20: 2020 2020 2020 2041 7061 6368 6520 536f         Apache So
+00028f30: 6674 7761 7265 204c 6963 656e 7365 2020  ftware License  
+00028f40: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00028f50: 2020 4775 7374 6176 6f20 4e69 656d 6579    Gustavo Niemey
+00028f60: 6572 2020 2020 2020 2020 2020 207c 2020  er           |  
+00028f70: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
+00028f80: 6769 7468 7562 2e63 6f6d 2f64 6174 6575  github.com/dateu
+00028f90: 7469 6c2f 6461 7465 7574 696c 2020 2020  til/dateutil    
+00028fa0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
+00028fb0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+00028fc0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+00028fd0: 2020 2020 2020 2020 2042 5344 204c 6963           BSD Lic
+00028fe0: 656e 7365 2020 2020 2020 2020 2020 2020  ense            
+00028ff0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+00029000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029010: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00029020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029050: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
+00029060: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00029070: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
 00029080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029090: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+00029090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
 000290a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000290b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000290c0: 2d2d 2d2d 2b0a 7c20 2020 2020 7365 7475  ----+.|     setu
-000290d0: 7074 6f6f 6c73 2020 2020 207c 2020 2036  ptools     |   6
-000290e0: 352e 352e 3020 207c 2020 2020 2020 2020  5.5.0  |        
-000290f0: 2020 2020 2020 4d49 5420 4c69 6365 6e73        MIT Licens
-00029100: 6520 2020 2020 2020 2020 2020 2020 207c  e              |
-00029110: 2050 7974 686f 6e20 5061 636b 6167 696e   Python Packagin
-00029120: 6720 4175 7468 6f72 6974 7920 7c20 2020  g Authority |   
-00029130: 2020 2068 7474 7073 3a2f 2f67 6974 6875     https://githu
-00029140: 622e 636f 6d2f 7079 7061 2f73 6574 7570  b.com/pypa/setup
-00029150: 746f 6f6c 7320 2020 2020 207c 0a2b 2d2d  tools      |.+--
-00029160: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029170: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --+-----------+-
-00029180: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000291a0: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
-000291b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000291c0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
+000290c0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
+000290d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000290e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000290f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20  ------------+.| 
+00029100: 2020 2020 2072 6571 7565 7374 7320 2020       requests   
+00029110: 2020 207c 2020 2032 2e32 392e 3020 207c     |   2.29.0  |
+00029120: 2020 2020 2020 2020 4170 6163 6865 2053          Apache S
+00029130: 6f66 7477 6172 6520 4c69 6365 6e73 6520  oftware License 
+00029140: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+00029150: 2020 2020 4b65 6e6e 6574 6820 5265 6974      Kenneth Reit
+00029160: 7a20 2020 2020 2020 2020 2020 2020 7c20  z             | 
+00029170: 2020 2020 2020 2020 2020 2068 7474 7073             https
+00029180: 3a2f 2f72 6571 7565 7374 732e 7265 6164  ://requests.read
+00029190: 7468 6564 6f63 732e 696f 2020 2020 2020  thedocs.io      
+000291a0: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
+000291b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
+000291c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
 000291d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000291e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000291f0: 2d2d 2b0a 7c20 2020 2020 2020 2073 6978  --+.|        six
-00029200: 2020 2020 2020 2020 207c 2020 2031 2e31           |   1.1
-00029210: 362e 3020 207c 2020 2020 2020 2020 2020  6.0  |          
-00029220: 2020 2020 4d49 5420 4c69 6365 6e73 6520      MIT License 
-00029230: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00029240: 2020 2042 656e 6a61 6d69 6e20 5065 7465     Benjamin Pete
-00029250: 7273 6f6e 2020 2020 2020 7c20 2020 2020  rson      |     
-00029260: 2020 6874 7470 733a 2f2f 6769 7468 7562    https://github
-00029270: 2e63 6f6d 2f62 656e 6a61 6d69 6e70 2f73  .com/benjaminp/s
-00029280: 6978 2020 2020 2020 207c 0a2b 2d2d 2d2d  ix       |.+----
-00029290: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000292a0: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  +-----------+---
-000292b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000292c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000292d0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-000292e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000292f0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
+000291f0: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
+00029200: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029210: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
+00029220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029230: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029250: 2d2d 2b0a 7c20 2020 2020 2072 7374 3261  --+.|      rst2a
+00029260: 6e73 6920 2020 2020 207c 2020 2030 2e31  nsi      |   0.1
+00029270: 2e35 2020 207c 2020 2020 2020 2020 2020  .5   |          
+00029280: 2020 2020 4d49 5420 4c69 6365 6e73 6520      MIT License 
+00029290: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+000292a0: 2020 2020 2020 2020 2020 2020 2020 536e                Sn
+000292b0: 6169 7065 2020 2020 2020 2020 2020 2020  aipe            
+000292c0: 2020 2020 7c20 2020 2020 2068 7474 7073      |      https
+000292d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 536e  ://github.com/Sn
+000292e0: 6169 7065 2f70 7974 686f 6e2d 7273 742d  aipe/python-rst-
+000292f0: 746f 2d61 6e73 6920 2020 2020 207c 0a2b  to-ansi      |.+
 00029300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029310: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029320: 2b0a 7c20 2020 2020 2074 6162 756c 6174  +.|      tabulat
-00029330: 6520 2020 2020 207c 2020 2030 2e39 2e30  e      |   0.9.0
-00029340: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00029350: 2020 4d49 5420 4c69 6365 6e73 6520 2020    MIT License   
-00029360: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00029370: 2020 2020 2020 554e 4b4e 4f57 4e20 2020        UNKNOWN   
-00029380: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00029390: 2020 2020 2020 2020 2020 2020 554e 4b4e              UNKN
-000293a0: 4f57 4e20 2020 2020 2020 2020 2020 2020  OWN             
-000293b0: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
-000293c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
-000293d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
-000293e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000293f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029400: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
-00029410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00029420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a  --------------+.
-00029450: 7c20 2020 2020 2020 2074 7164 6d20 2020  |        tqdm   
-00029460: 2020 2020 207c 2020 2034 2e36 352e 3020       |   4.65.0 
-00029470: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00029480: 4d49 5420 4c69 6365 6e73 6520 2020 2020  MIT License     
-00029490: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-000294a0: 2020 2020 554e 4b4e 4f57 4e20 2020 2020      UNKNOWN     
-000294b0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-000294c0: 2020 2068 7474 7073 3a2f 2f74 7164 6d2e     https://tqdm.
-000294d0: 6769 7468 7562 2e69 6f20 2020 2020 2020  github.io       
-000294e0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-000294f0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00029500: 2020 2020 2020 2020 7c20 204d 6f7a 696c          |  Mozil
-00029510: 6c61 2050 7562 6c69 6320 4c69 6365 6e73  la Public Licens
-00029520: 6520 322e 3020 284d 504c 2032 2e30 2920  e 2.0 (MPL 2.0) 
-00029530: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00029540: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00029550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029570: 2020 2020 2020 2020 2020 2020 7c0a 2b2d              |.+-
-00029580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029590: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---+-----------+
-000295a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029310: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
+00029320: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
+00029330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029340: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00029350: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+00029370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000293a0: 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 2020 2020  --------+.|     
+000293b0: 7365 7475 7074 6f6f 6c73 2020 2020 207c  setuptools     |
+000293c0: 2020 2036 352e 352e 3020 207c 2020 2020     65.5.0  |    
+000293d0: 2020 2020 2020 2020 2020 4d49 5420 4c69            MIT Li
+000293e0: 6365 6e73 6520 2020 2020 2020 2020 2020  cense           
+000293f0: 2020 207c 2020 2020 2020 5079 7468 6f6e     |      Python
+00029400: 2050 6163 6b61 6769 6e67 2041 7574 686f   Packaging Autho
+00029410: 7269 7479 2020 2020 2020 7c20 2020 2020  rity      |     
+00029420: 2020 2020 2020 6874 7470 733a 2f2f 6769        https://gi
+00029430: 7468 7562 2e63 6f6d 2f70 7970 612f 7365  thub.com/pypa/se
+00029440: 7475 7074 6f6f 6c73 2020 2020 2020 2020  tuptools        
+00029450: 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d     |.+----------
+00029460: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
+00029470: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+00029480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
+000294a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000294b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000294c0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+000294d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000294e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000294f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a  --------------+.
+00029500: 7c20 2020 2020 2020 2073 6978 2020 2020  |        six    
+00029510: 2020 2020 207c 2020 2031 2e31 362e 3020       |   1.16.0 
+00029520: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+00029530: 4d49 5420 4c69 6365 6e73 6520 2020 2020  MIT License     
+00029540: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+00029550: 2020 2020 4265 6e6a 616d 696e 2050 6574      Benjamin Pet
+00029560: 6572 736f 6e20 2020 2020 2020 2020 2020  erson           
+00029570: 7c20 2020 2020 2020 2020 2020 2068 7474  |            htt
+00029580: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00029590: 6265 6e6a 616d 696e 702f 7369 7820 2020  benjaminp/six   
+000295a0: 2020 2020 2020 2020 207c 0a2b 2d2d 2d2d           |.+----
 000295b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000295c0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+000295c0: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  +-----------+---
 000295d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000295e0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-000295f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000295e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000295f0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
 00029600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029610: 2d2d 2d2b 0a7c 2020 2020 2020 7572 6c6c  ---+.|      urll
-00029620: 6962 3320 2020 2020 2020 7c20 2031 2e32  ib3       |  1.2
-00029630: 362e 3135 2020 7c20 2020 2020 2020 2020  6.15  |         
-00029640: 2020 2020 204d 4954 204c 6963 656e 7365       MIT License
-00029650: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00029660: 2020 2020 2020 416e 6472 6579 2050 6574        Andrey Pet
-00029670: 726f 7620 2020 2020 2020 207c 2020 2020  rov        |    
-00029680: 2020 2068 7474 7073 3a2f 2f75 726c 6c69     https://urlli
-00029690: 6233 2e72 6561 6474 6865 646f 6373 2e69  b3.readthedocs.i
-000296a0: 6f2f 2020 2020 2020 2020 7c0a 2b2d 2d2d  o/        |.+---
-000296b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000296c0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -+-----------+--
-000296d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000296e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000296f0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
-00029700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029710: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
-00029720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+00029620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029630: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029640: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029650: 2d2d 2d2d 2b0a 7c20 2020 2020 2074 6162  ----+.|      tab
+00029660: 756c 6174 6520 2020 2020 207c 2020 2030  ulate      |   0
+00029670: 2e39 2e30 2020 207c 2020 2020 2020 2020  .9.0   |        
+00029680: 2020 2020 2020 4d49 5420 4c69 6365 6e73        MIT Licens
+00029690: 6520 2020 2020 2020 2020 2020 2020 207c  e              |
+000296a0: 2053 6572 6765 7920 4173 7461 6e69 6e20   Sergey Astanin 
+000296b0: 3c73 2e61 7374 616e 696e 4067 6d61 696c  <s.astanin@gmail
+000296c0: 2e63 6f6d 3e20 7c20 2020 2020 2020 6874  .com> |       ht
+000296d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000296e0: 2f61 7374 616e 696e 2f70 7974 686f 6e2d  /astanin/python-
+000296f0: 7461 6275 6c61 7465 2020 2020 2020 207c  tabulate       |
+00029700: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
+00029710: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+00029720: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
 00029730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029740: 2d2b 0a7c 2020 2020 2020 7763 7769 6474  -+.|      wcwidt
-00029750: 6820 2020 2020 2020 7c20 2020 302e 322e  h       |   0.2.
-00029760: 3620 2020 7c20 2020 2020 2020 2020 2020  6   |           
-00029770: 2020 204d 4954 204c 6963 656e 7365 2020     MIT License  
-00029780: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00029790: 2020 2020 2020 4a65 6666 2051 7561 7374        Jeff Quast
-000297a0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-000297b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000297c0: 6f6d 2f6a 7175 6173 742f 7763 7769 6474  om/jquast/wcwidt
-000297d0: 6820 2020 2020 2020 7c0a 2b2d 2d2d 2d2d  h       |.+-----
-000297e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-000297f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
-00029800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029820: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
-00029830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029840: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-00029850: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00029870: 0a0a 5468 6972 6420 7061 7274 7920 6c69  ..Third party li
-00029880: 6272 6172 6965 7320 6d6f 6469 6669 6564  braries modified
-00029890: 2061 6e64 2069 6e63 6c75 6465 6420 696e   and included in
-000298a0: 2062 3220 6f72 2062 3273 646b 3a0a 0a72   b2 or b2sdk:..r
-000298b0: 6571 7565 7374 730a 496e 636c 7564 6564  equests.Included
-000298c0: 2069 6e20 6120 7265 7669 7365 6420 666f   in a revised fo
-000298d0: 726d 0a46 696c 6573 2069 6e63 6c75 6465  rm.Files include
-000298e0: 6420 666f 7220 6c65 6761 6c20 636f 6d70  d for legal comp
-000298f0: 6c69 616e 6365 2072 6561 736f 6e73 3a0a  liance reasons:.
-00029900: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  +-----------+---
-00029910: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029740: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
+00029750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029770: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
+00029780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000297a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 2020  ----------+.|   
+000297b0: 2020 2020 2074 7164 6d20 2020 2020 2020       tqdm       
+000297c0: 207c 2020 2034 2e36 352e 3020 207c 2020   |   4.65.0  |  
+000297d0: 2020 2020 2020 2020 2020 2020 4d49 5420              MIT 
+000297e0: 4c69 6365 6e73 6520 2020 2020 2020 2020  License         
+000297f0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00029800: 2020 2020 2055 4e4b 4e4f 574e 2020 2020       UNKNOWN    
+00029810: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+00029820: 2020 2020 2020 2020 2020 2020 2020 6874                ht
+00029830: 7470 733a 2f2f 7471 646d 2e67 6974 6875  tps://tqdm.githu
+00029840: 622e 696f 2020 2020 2020 2020 2020 2020  b.io            
+00029850: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
+00029860: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+00029870: 2020 2020 2020 2020 7c20 204d 6f7a 696c          |  Mozil
+00029880: 6c61 2050 7562 6c69 6320 4c69 6365 6e73  la Public Licens
+00029890: 6520 322e 3020 284d 504c 2032 2e30 2920  e 2.0 (MPL 2.0) 
+000298a0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+000298b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000298c0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+000298d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000298e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000298f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029900: 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.+-------------
+00029910: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+00029920: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
 00029930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
 00029950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00029960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029980: 2d2d 2d2d 2d2b 0a7c 2046 696c 6520 6e61  -----+.| File na
-00029990: 6d65 207c 2020 2020 2020 2020 2020 2020  me |            
-000299a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000299b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000299c0: 2020 2020 2020 2020 2020 2020 436f 6e74              Cont
-000299d0: 656e 7420 2020 2020 2020 2020 2020 2020  ent             
-000299e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000299f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029a00: 2020 2020 2020 2020 2020 2020 7c0a 2b2d              |.+-
-00029a10: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
-00029a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029a30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029a40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029a50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029a60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029a70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029970: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
+00029980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000299a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2020  -----------+.|  
+000299b0: 2020 2020 7572 6c6c 6962 3320 2020 2020      urllib3     
+000299c0: 2020 7c20 2031 2e32 362e 3135 2020 7c20    |  1.26.15  | 
+000299d0: 2020 2020 2020 2020 2020 2020 204d 4954               MIT
+000299e0: 204c 6963 656e 7365 2020 2020 2020 2020   License        
+000299f0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00029a00: 2020 2041 6e64 7265 7920 5065 7472 6f76     Andrey Petrov
+00029a10: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+00029a20: 2020 2020 2020 2020 2020 6874 7470 733a            https:
+00029a30: 2f2f 7572 6c6c 6962 332e 7265 6164 7468  //urllib3.readth
+00029a40: 6564 6f63 732e 696f 2f20 2020 2020 2020  edocs.io/       
+00029a50: 2020 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d        |.+-------
+00029a60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00029a70: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
 00029a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029a90: 2d2d 2d2b 0a7c 2020 204e 4f54 4943 4520  ---+.|   NOTICE 
-00029aa0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00029ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029ad0: 2020 2020 2020 2020 2020 5265 7175 6573            Reques
-00029ae0: 7473 2020 2020 2020 2020 2020 2020 2020  ts              
-00029af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029b10: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
-00029b20: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00029b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029b50: 2020 2020 2020 2043 6f70 7972 6967 6874         Copyright
-00029b60: 2032 3031 3920 4b65 6e6e 6574 6820 5265   2019 Kenneth Re
-00029b70: 6974 7a20 2020 2020 2020 2020 2020 2020  itz             
-00029b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029ba0: 207c 0a7c 2020 2020 2020 2020 2020 207c   |.|           |
-00029bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029c20: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-00029c30: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00029c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029c60: 2020 2020 436f 7079 7269 6768 7420 3230      Copyright 20
-00029c70: 3231 2042 6163 6b62 6c61 7a65 2049 6e63  21 Backblaze Inc
-00029c80: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
-00029c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029ca0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00029cb0: 0a7c 2020 2020 2020 2020 2020 207c 2020  .|           |  
-00029cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029ce0: 2020 2020 2020 2020 4368 616e 6765 7320          Changes 
-00029cf0: 6d61 6465 2074 6f20 7468 6520 6f72 6967  made to the orig
-00029d00: 696e 616c 2073 6f75 7263 653a 2020 2020  inal source:    
-00029d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029d30: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-00029d40: 2020 2020 7c20 7265 7175 6573 7473 2e6d      | requests.m
-00029d50: 6f64 656c 732e 5265 7370 6f6e 7365 2e69  odels.Response.i
-00029d60: 7465 725f 636f 6e74 656e 7420 6861 7320  ter_content has 
-00029d70: 6265 656e 206f 7665 7272 6964 6465 6e20  been overridden 
-00029d80: 746f 2070 6173 7320 6064 6563 6f64 655f  to pass `decode_
-00029d90: 636f 6e74 656e 743d 4661 6c73 6560 2061  content=False` a
-00029da0: 7267 756d 656e 7420 746f 2060 7365 6c66  rgument to `self
-00029db0: 2e72 6177 2e73 7472 6561 6d60 207c 0a7c  .raw.stream` |.|
-00029dc0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+00029a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029aa0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
+00029ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029ac0: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00029ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029af0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029b00: 2d2b 0a7c 2020 2020 2020 7763 7769 6474  -+.|      wcwidt
+00029b10: 6820 2020 2020 2020 7c20 2020 302e 322e  h       |   0.2.
+00029b20: 3620 2020 7c20 2020 2020 2020 2020 2020  6   |           
+00029b30: 2020 204d 4954 204c 6963 656e 7365 2020     MIT License  
+00029b40: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+00029b50: 2020 2020 2020 2020 2020 204a 6566 6620             Jeff 
+00029b60: 5175 6173 7420 2020 2020 2020 2020 2020  Quast           
+00029b70: 2020 207c 2020 2020 2020 2020 2020 2068     |           h
+00029b80: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00029b90: 6d2f 6a71 7561 7374 2f77 6377 6964 7468  m/jquast/wcwidth
+00029ba0: 2020 2020 2020 2020 2020 2020 7c0a 2b2d              |.+-
+00029bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029bc0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---+-----------+
+00029bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029be0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029bf0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+00029c00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029c10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
+00029c20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029c30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029c50: 2d2d 2d2d 2d2d 2d2b 0a0a 5468 6972 6420  -------+..Third 
+00029c60: 7061 7274 7920 6c69 6272 6172 6965 7320  party libraries 
+00029c70: 6d6f 6469 6669 6564 2061 6e64 2069 6e63  modified and inc
+00029c80: 6c75 6465 6420 696e 2062 3220 6f72 2062  luded in b2 or b
+00029c90: 3273 646b 3a0a 0a72 6571 7565 7374 730a  2sdk:..requests.
+00029ca0: 496e 636c 7564 6564 2069 6e20 6120 7265  Included in a re
+00029cb0: 7669 7365 6420 666f 726d 0a46 696c 6573  vised form.Files
+00029cc0: 2069 6e63 6c75 6465 6420 666f 7220 6c65   included for le
+00029cd0: 6761 6c20 636f 6d70 6c69 616e 6365 2072  gal compliance r
+00029ce0: 6561 736f 6e73 3a0a 2b2d 2d2d 2d2d 2d2d  easons:.+-------
+00029cf0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
+00029d00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029d10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029d20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029d30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029d40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029d50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029d60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c  -------------+.|
+00029d70: 2046 696c 6520 6e61 6d65 207c 2020 2020   File name |    
+00029d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029db0: 2020 2020 436f 6e74 656e 7420 2020 2020      Content     
+00029dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00029dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029de0: 2020 2020 2020 2020 696e 206f 7264 6572          in order
-00029df0: 2074 6f20 4e4f 5420 6465 636f 6d70 7265   to NOT decompre
-00029e00: 7373 2064 6174 6120 6261 7365 6420 6f6e  ss data based on
-00029e10: 2043 6f6e 7465 6e74 2d45 6e63 6f64 696e   Content-Encodin
-00029e20: 6720 6865 6164 6572 2020 2020 2020 2020  g header        
-00029e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029e40: 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d      |.+---------
-00029e50: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
+00029de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029df0: 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d      |.+---------
+00029e00: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
+00029e10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00029e50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00029e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029e70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029e80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029eb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029ec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a0a 6232  -----------+..b2
-00029ed0: 206c 6963 656e 7365 3a0a 4261 636b 626c   license:.Backbl
-00029ee0: 617a 6520 7761 6e74 7320 6465 7665 6c6f  aze wants develo
-00029ef0: 7065 7273 2061 6e64 206f 7267 616e 697a  pers and organiz
-00029f00: 6174 696f 6e20 746f 2063 6f70 7920 616e  ation to copy an
-00029f10: 6420 7265 2d75 7365 206f 7572 0a63 6f64  d re-use our.cod
-00029f20: 6520 6578 616d 706c 6573 2c20 736f 2077  e examples, so w
-00029f30: 6520 6d61 6b65 2074 6865 2073 616d 706c  e make the sampl
-00029f40: 6573 2061 7661 696c 6162 6c65 2062 7920  es available by 
-00029f50: 7365 7665 7261 6c20 6469 6666 6572 656e  several differen
-00029f60: 740a 6c69 6365 6e73 6573 2e20 204f 6e65  t.licenses.  One
-00029f70: 206f 7074 696f 6e20 6973 2074 6865 204d   option is the M
-00029f80: 4954 206c 6963 656e 7365 2028 6265 6c6f  IT license (belo
-00029f90: 7729 2e20 204f 7468 6572 206f 7074 696f  w).  Other optio
-00029fa0: 6e73 2061 7265 0a61 7661 696c 6162 6c65  ns are.available
-00029fb0: 2068 6572 653a 0a0a 2020 2020 6874 7470   here:..    http
-00029fc0: 733a 2f2f 7777 772e 6261 636b 626c 617a  s://www.backblaz
-00029fd0: 652e 636f 6d2f 7573 696e 675f 6232 5f63  e.com/using_b2_c
-00029fe0: 6f64 652e 6874 6d6c 0a0a 0a54 6865 204d  ode.html...The M
-00029ff0: 4954 204c 6963 656e 7365 2028 4d49 5429  IT License (MIT)
-0002a000: 0a0a 436f 7079 7269 6768 7420 2863 2920  ..Copyright (c) 
-0002a010: 3230 3135 2042 6163 6b62 6c61 7a65 0a0a  2015 Backblaze..
-0002a020: 5065 726d 6973 7369 6f6e 2069 7320 6865  Permission is he
-0002a030: 7265 6279 2067 7261 6e74 6564 2c20 6672  reby granted, fr
-0002a040: 6565 206f 6620 6368 6172 6765 2c20 746f  ee of charge, to
-0002a050: 2061 6e79 2070 6572 736f 6e20 6f62 7461   any person obta
-0002a060: 696e 696e 6720 6120 636f 7079 0a6f 6620  ining a copy.of 
-0002a070: 7468 6973 2073 6f66 7477 6172 6520 616e  this software an
-0002a080: 6420 6173 736f 6369 6174 6564 2064 6f63  d associated doc
-0002a090: 756d 656e 7461 7469 6f6e 2066 696c 6573  umentation files
-0002a0a0: 2028 7468 6520 2253 6f66 7477 6172 6522   (the "Software"
-0002a0b0: 292c 2074 6f20 6465 616c 0a69 6e20 7468  ), to deal.in th
-0002a0c0: 6520 536f 6674 7761 7265 2077 6974 686f  e Software witho
-0002a0d0: 7574 2072 6573 7472 6963 7469 6f6e 2c20  ut restriction, 
-0002a0e0: 696e 636c 7564 696e 6720 7769 7468 6f75  including withou
-0002a0f0: 7420 6c69 6d69 7461 7469 6f6e 2074 6865  t limitation the
-0002a100: 2072 6967 6874 730a 746f 2075 7365 2c20   rights.to use, 
-0002a110: 636f 7079 2c20 6d6f 6469 6679 2c20 6d65  copy, modify, me
-0002a120: 7267 652c 2070 7562 6c69 7368 2c20 6469  rge, publish, di
-0002a130: 7374 7269 6275 7465 2c20 7375 626c 6963  stribute, sublic
-0002a140: 656e 7365 2c20 616e 642f 6f72 2073 656c  ense, and/or sel
-0002a150: 6c0a 636f 7069 6573 206f 6620 7468 6520  l.copies of the 
-0002a160: 536f 6674 7761 7265 2c20 616e 6420 746f  Software, and to
-0002a170: 2070 6572 6d69 7420 7065 7273 6f6e 7320   permit persons 
-0002a180: 746f 2077 686f 6d20 7468 6520 536f 6674  to whom the Soft
-0002a190: 7761 7265 2069 730a 6675 726e 6973 6865  ware is.furnishe
-0002a1a0: 6420 746f 2064 6f20 736f 2c20 7375 626a  d to do so, subj
-0002a1b0: 6563 7420 746f 2074 6865 2066 6f6c 6c6f  ect to the follo
-0002a1c0: 7769 6e67 2063 6f6e 6469 7469 6f6e 733a  wing conditions:
-0002a1d0: 0a0a 5468 6520 6162 6f76 6520 636f 7079  ..The above copy
-0002a1e0: 7269 6768 7420 6e6f 7469 6365 2061 6e64  right notice and
-0002a1f0: 2074 6869 7320 7065 726d 6973 7369 6f6e   this permission
-0002a200: 206e 6f74 6963 6520 7368 616c 6c20 6265   notice shall be
-0002a210: 2069 6e63 6c75 6465 6420 696e 2061 6c6c   included in all
-0002a220: 0a63 6f70 6965 7320 6f72 2073 7562 7374  .copies or subst
-0002a230: 616e 7469 616c 2070 6f72 7469 6f6e 7320  antial portions 
-0002a240: 6f66 2074 6865 2053 6f66 7477 6172 652e  of the Software.
-0002a250: 0a0a 5448 4520 534f 4654 5741 5245 2049  ..THE SOFTWARE I
-0002a260: 5320 5052 4f56 4944 4544 2022 4153 2049  S PROVIDED "AS I
-0002a270: 5322 2c20 5749 5448 4f55 5420 5741 5252  S", WITHOUT WARR
-0002a280: 414e 5459 204f 4620 414e 5920 4b49 4e44  ANTY OF ANY KIND
-0002a290: 2c20 4558 5052 4553 5320 4f52 0a49 4d50  , EXPRESS OR.IMP
-0002a2a0: 4c49 4544 2c20 494e 434c 5544 494e 4720  LIED, INCLUDING 
-0002a2b0: 4255 5420 4e4f 5420 4c49 4d49 5445 4420  BUT NOT LIMITED 
-0002a2c0: 544f 2054 4845 2057 4152 5241 4e54 4945  TO THE WARRANTIE
-0002a2d0: 5320 4f46 204d 4552 4348 414e 5441 4249  S OF MERCHANTABI
-0002a2e0: 4c49 5459 2c0a 4649 544e 4553 5320 464f  LITY,.FITNESS FO
-0002a2f0: 5220 4120 5041 5254 4943 554c 4152 2050  R A PARTICULAR P
-0002a300: 5552 504f 5345 2041 4e44 204e 4f4e 494e  URPOSE AND NONIN
-0002a310: 4652 494e 4745 4d45 4e54 2e20 494e 204e  FRINGEMENT. IN N
-0002a320: 4f20 4556 454e 5420 5348 414c 4c20 5448  O EVENT SHALL TH
-0002a330: 450a 4155 5448 4f52 5320 4f52 2043 4f50  E.AUTHORS OR COP
-0002a340: 5952 4947 4854 2048 4f4c 4445 5253 2042  YRIGHT HOLDERS B
-0002a350: 4520 4c49 4142 4c45 2046 4f52 2041 4e59  E LIABLE FOR ANY
-0002a360: 2043 4c41 494d 2c20 4441 4d41 4745 5320   CLAIM, DAMAGES 
-0002a370: 4f52 204f 5448 4552 0a4c 4941 4249 4c49  OR OTHER.LIABILI
-0002a380: 5459 2c20 5748 4554 4845 5220 494e 2041  TY, WHETHER IN A
-0002a390: 4e20 4143 5449 4f4e 204f 4620 434f 4e54  N ACTION OF CONT
-0002a3a0: 5241 4354 2c20 544f 5254 204f 5220 4f54  RACT, TORT OR OT
-0002a3b0: 4845 5257 4953 452c 2041 5249 5349 4e47  HERWISE, ARISING
-0002a3c0: 2046 524f 4d2c 0a4f 5554 204f 4620 4f52   FROM,.OUT OF OR
-0002a3d0: 2049 4e20 434f 4e4e 4543 5449 4f4e 2057   IN CONNECTION W
-0002a3e0: 4954 4820 5448 4520 534f 4654 5741 5245  ITH THE SOFTWARE
-0002a3f0: 204f 5220 5448 4520 5553 4520 4f52 204f   OR THE USE OR O
-0002a400: 5448 4552 2044 4541 4c49 4e47 5320 494e  THER DEALINGS IN
-0002a410: 2054 4845 0a53 4f46 5457 4152 452e 0a0a   THE.SOFTWARE...
+00029e70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2020  -----------+.|  
+00029e80: 204e 4f54 4943 4520 207c 2020 2020 2020   NOTICE  |      
+00029e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029ec0: 2020 5265 7175 6573 7473 2020 2020 2020    Requests      
+00029ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029f00: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
+00029f10: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00029f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029f30: 2020 2020 2020 2020 2020 2020 2020 2043                 C
+00029f40: 6f70 7972 6967 6874 2032 3031 3920 4b65  opyright 2019 Ke
+00029f50: 6e6e 6574 6820 5265 6974 7a20 2020 2020  nneth Reitz     
+00029f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029f80: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
+00029f90: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+00029fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a010: 7c0a 7c20 2020 2020 2020 2020 2020 7c20  |.|           | 
+0002a020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a040: 2020 2020 2020 2020 2020 2020 436f 7079              Copy
+0002a050: 7269 6768 7420 3230 3231 2042 6163 6b62  right 2021 Backb
+0002a060: 6c61 7a65 2049 6e63 2e20 2020 2020 2020  laze Inc.       
+0002a070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a090: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0002a0a0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+0002a0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a0d0: 4368 616e 6765 7320 6d61 6465 2074 6f20  Changes made to 
+0002a0e0: 7468 6520 6f72 6967 696e 616c 2073 6f75  the original sou
+0002a0f0: 7263 653a 2020 2020 2020 2020 2020 2020  rce:            
+0002a100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a110: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+0002a120: 7c20 2020 2020 2020 2020 2020 7c20 7265  |           | re
+0002a130: 7175 6573 7473 2e6d 6f64 656c 732e 5265  quests.models.Re
+0002a140: 7370 6f6e 7365 2e69 7465 725f 636f 6e74  sponse.iter_cont
+0002a150: 656e 7420 6861 7320 6265 656e 206f 7665  ent has been ove
+0002a160: 7272 6964 6465 6e20 746f 2070 6173 7320  rridden to pass 
+0002a170: 6064 6563 6f64 655f 636f 6e74 656e 743d  `decode_content=
+0002a180: 4661 6c73 6560 2061 7267 756d 656e 7420  False` argument 
+0002a190: 746f 2060 7365 6c66 2e72 6177 2e73 7472  to `self.raw.str
+0002a1a0: 6561 6d60 207c 0a7c 2020 2020 2020 2020  eam` |.|        
+0002a1b0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+0002a1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a1d0: 696e 206f 7264 6572 2074 6f20 4e4f 5420  in order to NOT 
+0002a1e0: 6465 636f 6d70 7265 7373 2064 6174 6120  decompress data 
+0002a1f0: 6261 7365 6420 6f6e 2043 6f6e 7465 6e74  based on Content
+0002a200: 2d45 6e63 6f64 696e 6720 6865 6164 6572  -Encoding header
+0002a210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a220: 2020 2020 2020 2020 2020 2020 7c0a 2b2d              |.+-
+0002a230: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
+0002a240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0002a250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0002a260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0002a270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0002a280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0002a290: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0002a2a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0002a2b0: 2d2d 2d2b 0a0a 6232 206c 6963 656e 7365  ---+..b2 license
+0002a2c0: 3a0a 4261 636b 626c 617a 6520 7761 6e74  :.Backblaze want
+0002a2d0: 7320 6465 7665 6c6f 7065 7273 2061 6e64  s developers and
+0002a2e0: 206f 7267 616e 697a 6174 696f 6e20 746f   organization to
+0002a2f0: 2063 6f70 7920 616e 6420 7265 2d75 7365   copy and re-use
+0002a300: 206f 7572 0a63 6f64 6520 6578 616d 706c   our.code exampl
+0002a310: 6573 2c20 736f 2077 6520 6d61 6b65 2074  es, so we make t
+0002a320: 6865 2073 616d 706c 6573 2061 7661 696c  he samples avail
+0002a330: 6162 6c65 2062 7920 7365 7665 7261 6c20  able by several 
+0002a340: 6469 6666 6572 656e 740a 6c69 6365 6e73  different.licens
+0002a350: 6573 2e20 204f 6e65 206f 7074 696f 6e20  es.  One option 
+0002a360: 6973 2074 6865 204d 4954 206c 6963 656e  is the MIT licen
+0002a370: 7365 2028 6265 6c6f 7729 2e20 204f 7468  se (below).  Oth
+0002a380: 6572 206f 7074 696f 6e73 2061 7265 0a61  er options are.a
+0002a390: 7661 696c 6162 6c65 2068 6572 653a 0a0a  vailable here:..
+0002a3a0: 2020 2020 6874 7470 733a 2f2f 7777 772e      https://www.
+0002a3b0: 6261 636b 626c 617a 652e 636f 6d2f 7573  backblaze.com/us
+0002a3c0: 696e 675f 6232 5f63 6f64 652e 6874 6d6c  ing_b2_code.html
+0002a3d0: 0a0a 0a54 6865 204d 4954 204c 6963 656e  ...The MIT Licen
+0002a3e0: 7365 2028 4d49 5429 0a0a 436f 7079 7269  se (MIT)..Copyri
+0002a3f0: 6768 7420 2863 2920 3230 3135 2042 6163  ght (c) 2015 Bac
+0002a400: 6b62 6c61 7a65 0a0a 5065 726d 6973 7369  kblaze..Permissi
+0002a410: 6f6e 2069 7320 6865 7265 6279 2067 7261  on is hereby gra
+0002a420: 6e74 6564 2c20 6672 6565 206f 6620 6368  nted, free of ch
+0002a430: 6172 6765 2c20 746f 2061 6e79 2070 6572  arge, to any per
+0002a440: 736f 6e20 6f62 7461 696e 696e 6720 6120  son obtaining a 
+0002a450: 636f 7079 0a6f 6620 7468 6973 2073 6f66  copy.of this sof
+0002a460: 7477 6172 6520 616e 6420 6173 736f 6369  tware and associ
+0002a470: 6174 6564 2064 6f63 756d 656e 7461 7469  ated documentati
+0002a480: 6f6e 2066 696c 6573 2028 7468 6520 2253  on files (the "S
+0002a490: 6f66 7477 6172 6522 292c 2074 6f20 6465  oftware"), to de
+0002a4a0: 616c 0a69 6e20 7468 6520 536f 6674 7761  al.in the Softwa
+0002a4b0: 7265 2077 6974 686f 7574 2072 6573 7472  re without restr
+0002a4c0: 6963 7469 6f6e 2c20 696e 636c 7564 696e  iction, includin
+0002a4d0: 6720 7769 7468 6f75 7420 6c69 6d69 7461  g without limita
+0002a4e0: 7469 6f6e 2074 6865 2072 6967 6874 730a  tion the rights.
+0002a4f0: 746f 2075 7365 2c20 636f 7079 2c20 6d6f  to use, copy, mo
+0002a500: 6469 6679 2c20 6d65 7267 652c 2070 7562  dify, merge, pub
+0002a510: 6c69 7368 2c20 6469 7374 7269 6275 7465  lish, distribute
+0002a520: 2c20 7375 626c 6963 656e 7365 2c20 616e  , sublicense, an
+0002a530: 642f 6f72 2073 656c 6c0a 636f 7069 6573  d/or sell.copies
+0002a540: 206f 6620 7468 6520 536f 6674 7761 7265   of the Software
+0002a550: 2c20 616e 6420 746f 2070 6572 6d69 7420  , and to permit 
+0002a560: 7065 7273 6f6e 7320 746f 2077 686f 6d20  persons to whom 
+0002a570: 7468 6520 536f 6674 7761 7265 2069 730a  the Software is.
+0002a580: 6675 726e 6973 6865 6420 746f 2064 6f20  furnished to do 
+0002a590: 736f 2c20 7375 626a 6563 7420 746f 2074  so, subject to t
+0002a5a0: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6e  he following con
+0002a5b0: 6469 7469 6f6e 733a 0a0a 5468 6520 6162  ditions:..The ab
+0002a5c0: 6f76 6520 636f 7079 7269 6768 7420 6e6f  ove copyright no
+0002a5d0: 7469 6365 2061 6e64 2074 6869 7320 7065  tice and this pe
+0002a5e0: 726d 6973 7369 6f6e 206e 6f74 6963 6520  rmission notice 
+0002a5f0: 7368 616c 6c20 6265 2069 6e63 6c75 6465  shall be include
+0002a600: 6420 696e 2061 6c6c 0a63 6f70 6965 7320  d in all.copies 
+0002a610: 6f72 2073 7562 7374 616e 7469 616c 2070  or substantial p
+0002a620: 6f72 7469 6f6e 7320 6f66 2074 6865 2053  ortions of the S
+0002a630: 6f66 7477 6172 652e 0a0a 5448 4520 534f  oftware...THE SO
+0002a640: 4654 5741 5245 2049 5320 5052 4f56 4944  FTWARE IS PROVID
+0002a650: 4544 2022 4153 2049 5322 2c20 5749 5448  ED "AS IS", WITH
+0002a660: 4f55 5420 5741 5252 414e 5459 204f 4620  OUT WARRANTY OF 
+0002a670: 414e 5920 4b49 4e44 2c20 4558 5052 4553  ANY KIND, EXPRES
+0002a680: 5320 4f52 0a49 4d50 4c49 4544 2c20 494e  S OR.IMPLIED, IN
+0002a690: 434c 5544 494e 4720 4255 5420 4e4f 5420  CLUDING BUT NOT 
+0002a6a0: 4c49 4d49 5445 4420 544f 2054 4845 2057  LIMITED TO THE W
+0002a6b0: 4152 5241 4e54 4945 5320 4f46 204d 4552  ARRANTIES OF MER
+0002a6c0: 4348 414e 5441 4249 4c49 5459 2c0a 4649  CHANTABILITY,.FI
+0002a6d0: 544e 4553 5320 464f 5220 4120 5041 5254  TNESS FOR A PART
+0002a6e0: 4943 554c 4152 2050 5552 504f 5345 2041  ICULAR PURPOSE A
+0002a6f0: 4e44 204e 4f4e 494e 4652 494e 4745 4d45  ND NONINFRINGEME
+0002a700: 4e54 2e20 494e 204e 4f20 4556 454e 5420  NT. IN NO EVENT 
+0002a710: 5348 414c 4c20 5448 450a 4155 5448 4f52  SHALL THE.AUTHOR
+0002a720: 5320 4f52 2043 4f50 5952 4947 4854 2048  S OR COPYRIGHT H
+0002a730: 4f4c 4445 5253 2042 4520 4c49 4142 4c45  OLDERS BE LIABLE
+0002a740: 2046 4f52 2041 4e59 2043 4c41 494d 2c20   FOR ANY CLAIM, 
+0002a750: 4441 4d41 4745 5320 4f52 204f 5448 4552  DAMAGES OR OTHER
+0002a760: 0a4c 4941 4249 4c49 5459 2c20 5748 4554  .LIABILITY, WHET
+0002a770: 4845 5220 494e 2041 4e20 4143 5449 4f4e  HER IN AN ACTION
+0002a780: 204f 4620 434f 4e54 5241 4354 2c20 544f   OF CONTRACT, TO
+0002a790: 5254 204f 5220 4f54 4845 5257 4953 452c  RT OR OTHERWISE,
+0002a7a0: 2041 5249 5349 4e47 2046 524f 4d2c 0a4f   ARISING FROM,.O
+0002a7b0: 5554 204f 4620 4f52 2049 4e20 434f 4e4e  UT OF OR IN CONN
+0002a7c0: 4543 5449 4f4e 2057 4954 4820 5448 4520  ECTION WITH THE 
+0002a7d0: 534f 4654 5741 5245 204f 5220 5448 4520  SOFTWARE OR THE 
+0002a7e0: 5553 4520 4f52 204f 5448 4552 2044 4541  USE OR OTHER DEA
+0002a7f0: 4c49 4e47 5320 494e 2054 4845 0a53 4f46  LINGS IN THE.SOF
+0002a800: 5457 4152 452e 0a0a                      TWARE...
```

### Comparing `b2-3.8.0/b2.egg-info/PKG-INFO` & `b2-3.9.0/b2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b2
-Version: 3.8.0
+Version: 3.9.0
 Summary: Command Line Tool for Backblaze B2
 Home-page: https://github.com/Backblaze/B2_Command_Line_Tool
 Author: Backblaze, Inc.
 Author-email: support@backblaze.com
 License: MIT
 Keywords: backblaze b2 cloud storage
 Classifier: Development Status :: 5 - Production/Stable
@@ -67,15 +67,15 @@
 # Usage
 
     b2 authorize-account [-h]  [applicationKeyId] [applicationKey]
     b2 cancel-all-unfinished-large-files [-h] bucketName
     b2 cancel-large-file [-h] fileId
     b2 clear-account [-h]
     b2 copy-file-by-id [-h] [--fetchMetadata] [--contentType CONTENTTYPE] [--range RANGE] [--info INFO | --noInfo] [--destinationServerSideEncryption {SSE-B2,SSE-C}] [--destinationServerSideEncryptionAlgorithm {AES256}] [--sourceServerSideEncryption {SSE-C}] [--sourceServerSideEncryptionAlgorithm {AES256}] [--fileRetentionMode {compliance,governance}] [--retainUntil TIMESTAMP] [--legalHold {on,off}] sourceFileId destinationBucketName b2FileName
-    b2 create-bucket [-h] [--bucketInfo BUCKETINFO] [--corsRules CORSRULES] [--lifecycleRules LIFECYCLERULES] [--fileLockEnabled] [--replication REPLICATION] [--defaultServerSideEncryption {SSE-B2,none}] [--defaultServerSideEncryptionAlgorithm {AES256}] bucketName bucketType
+    b2 create-bucket [-h] [--bucketInfo BUCKETINFO] [--corsRules CORSRULES] [--lifecycleRules LIFECYCLERULES] [--fileLockEnabled] [--replication REPLICATION] [--defaultServerSideEncryption {SSE-B2,none}] [--defaultServerSideEncryptionAlgorithm {AES256}] bucketName {allPublic,allPrivate}
     b2 create-key [-h] [--bucket BUCKET] [--namePrefix NAMEPREFIX] [--duration DURATION] [--allCapabilities] keyName [capabilities]
     b2 delete-bucket [-h] bucketName
     b2 delete-file-version [-h] [fileName] fileId
     b2 delete-key [-h] applicationKeyId
     b2 download-file-by-id [-h] [--noProgress] [--threads THREADS] [--sourceServerSideEncryption {SSE-C}] [--sourceServerSideEncryptionAlgorithm {AES256}] [--write-buffer-size BYTES] [--skip-hash-verification] [--max-download-streams-per-file MAX_DOWNLOAD_STREAMS_PER_FILE] fileId localFileName
     b2 download-file-by-name [-h] [--noProgress] [--threads THREADS] [--sourceServerSideEncryption {SSE-C}] [--sourceServerSideEncryptionAlgorithm {AES256}] [--write-buffer-size BYTES] [--skip-hash-verification] [--max-download-streams-per-file MAX_DOWNLOAD_STREAMS_PER_FILE] bucketName b2FileName localFileName
     b2 get-account-info [-h]
@@ -89,25 +89,26 @@
     b2 list-parts [-h] largeFileId
     b2 list-unfinished-large-files [-h] bucketName
     b2 ls [-h] [--long] [--json] [--replication] [--versions] [--recursive] [--withWildcard] bucketName [folderName]
     b2 rm [-h] [--dryRun] [--threads THREADS] [--queueSize QUEUESIZE] [--noProgress] [--failFast] [--versions] [--recursive] [--withWildcard] bucketName [folderName]
     b2 make-url [-h] fileId
     b2 make-friendly-url [-h] bucketName fileName
     b2 sync [-h] [--noProgress] [--dryRun] [--allowEmptySource] [--excludeAllSymlinks] [--threads THREADS] [--syncThreads SYNCTHREADS] [--downloadThreads DOWNLOADTHREADS] [--uploadThreads UPLOADTHREADS] [--compareVersions {none,modTime,size}] [--compareThreshold MILLIS] [--excludeRegex REGEX] [--includeRegex REGEX] [--excludeDirRegex REGEX] [--excludeIfModifiedAfter TIMESTAMP] [--destinationServerSideEncryption {SSE-B2,SSE-C}] [--destinationServerSideEncryptionAlgorithm {AES256}] [--sourceServerSideEncryption {SSE-C}] [--sourceServerSideEncryptionAlgorithm {AES256}] [--write-buffer-size BYTES] [--skip-hash-verification] [--max-download-streams-per-file MAX_DOWNLOAD_STREAMS_PER_FILE] [--incrementalMode] [--skipNewer | --replaceNewer] [--delete | --keepDays DAYS] source destination
-    b2 update-bucket [-h] [--bucketInfo BUCKETINFO] [--corsRules CORSRULES] [--lifecycleRules LIFECYCLERULES] [--defaultRetentionMode {compliance,governance,none}] [--defaultRetentionPeriod period] [--replication REPLICATION] [--fileLockEnabled] [--defaultServerSideEncryption {SSE-B2,none}] [--defaultServerSideEncryptionAlgorithm {AES256}] bucketName [bucketType]
-    b2 upload-file [-h] [--noProgress] [--quiet] [--contentType CONTENTTYPE] [--minPartSize MINPARTSIZE] [--sha1 SHA1] [--threads THREADS] [--info INFO] [--destinationServerSideEncryption {SSE-B2,SSE-C}] [--destinationServerSideEncryptionAlgorithm {AES256}] [--legalHold {on,off}] [--fileRetentionMode {compliance,governance}] [--retainUntil TIMESTAMP] [--incrementalMode] bucketName localFilePath b2FileName
+    b2 update-bucket [-h] [--bucketInfo BUCKETINFO] [--corsRules CORSRULES] [--lifecycleRules LIFECYCLERULES] [--defaultRetentionMode {compliance,governance,none}] [--defaultRetentionPeriod period] [--replication REPLICATION] [--fileLockEnabled] [--defaultServerSideEncryption {SSE-B2,none}] [--defaultServerSideEncryptionAlgorithm {AES256}] bucketName [{allPublic,allPrivate}]
+    b2 upload-file [-h] [--noProgress] [--quiet] [--contentType CONTENTTYPE] [--minPartSize MINPARTSIZE] [--sha1 SHA1] [--threads THREADS] [--info INFO] [--custom-upload-timestamp CUSTOM_UPLOAD_TIMESTAMP] [--destinationServerSideEncryption {SSE-B2,SSE-C}] [--destinationServerSideEncryptionAlgorithm {AES256}] [--legalHold {on,off}] [--fileRetentionMode {compliance,governance}] [--retainUntil TIMESTAMP] [--incrementalMode] bucketName localFilePath b2FileName
     b2 update-file-legal-hold [-h] [fileName] fileId {on,off}
     b2 update-file-retention [-h] [--retainUntil TIMESTAMP] [--bypassGovernance] [fileName] fileId {governance,compliance,none}
     b2 replication-setup [-h] [--destination-profile DESTINATION_PROFILE] [--name NAME] [--priority PRIORITY] [--file-name-prefix PREFIX] [--include-existing-files] SOURCE_BUCKET_NAME DESTINATION_BUCKET_NAME
     b2 replication-delete [-h] SOURCE_BUCKET_NAME REPLICATION_RULE_NAME
     b2 replication-pause [-h] SOURCE_BUCKET_NAME REPLICATION_RULE_NAME
     b2 replication-unpause [-h] SOURCE_BUCKET_NAME REPLICATION_RULE_NAME
     b2 replication-status [-h] [--rule REPLICATION_RULE_NAME] [--destination-profile DESTINATION_PROFILE] [--dont-scan-destination] [--output-format {console,json,csv}] [--noProgress] [--columns COLUMN ONE,COLUMN TWO] SOURCE_BUCKET_NAME
     b2 version [-h]
     b2 license [-h]
+    b2 install-autocomplete [-h] [--shell {bash}]
 
 
 The environment variable `B2_ACCOUNT_INFO` specifies the sqlite
 file to use for caching authentication information.
 The default file to use is: `~/.b2_account_info`
 
 For more details on one command: `b2 <command> --help`
```

### Comparing `b2-3.8.0/b2.egg-info/SOURCES.txt` & `b2-3.9.0/b2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/b2.spec` & `b2-3.9.0/b2.spec`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/contrib/debug_logs.ini` & `b2-3.9.0/contrib/debug_logs.ini`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/doc/source/conf.py` & `b2-3.9.0/doc/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,15 +196,15 @@
     (
         master_doc, 'B2_Command_Line_Tool', u'B2_Command_Line_Tool Documentation', author,
         'B2_Command_Line_Tool', 'One line description of project.', 'Miscellaneous'
     ),
 ]
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {'https://docs.python.org/': None}
+intersphinx_mapping = {'python3': ('https://docs.python.org/3', None)}
 
 
 white_spaces_start = re.compile(r'^\s*')
 
 
 def setup(_):
     """
```

### Comparing `b2-3.8.0/doc/source/quick_start.rst` & `b2-3.9.0/doc/source/quick_start.rst`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/doc/source/replication.rst` & `b2-3.9.0/doc/source/replication.rst`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/noxfile.py` & `b2-3.9.0/noxfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,14 +205,16 @@
     install_myself(session, ['license'])
     session.run('pip', 'install', *REQUIREMENTS_TEST)
     session.run(
         'pytest',
         '-s',
         '-n',
         'auto',
+        '--log-level',
+        'INFO',
         '-W',
         'ignore::DeprecationWarning:rst2ansi.visitor:',
         *session.posargs,
         'test/integration',
     )
```

### Comparing `b2-3.8.0/pyinstaller-hooks/hook-prettytable.py` & `b2-3.9.0/pyinstaller-hooks/hook-prettytable.py`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/setup.py` & `b2-3.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/test/integration/conftest.py` & `b2-3.9.0/test/integration/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
 
+import base64
 import contextlib
 import sys
 
 from os import environ, path
 from tempfile import TemporaryDirectory
 
 import pytest
 
 from b2sdk.v2 import B2_ACCOUNT_INFO_ENV_VAR, XDG_CONFIG_HOME_ENV_VAR
-from b2sdk.exception import BucketIdNotFound
+from b2sdk.exception import BadRequest, BucketIdNotFound
 
 from .helpers import Api, CommandLine, bucket_name_part
 
 GENERAL_BUCKET_NAME_PREFIX = 'clitst'
 
 
 @pytest.hookimpl
@@ -49,15 +50,22 @@
 @pytest.fixture(scope='session')
 def realm() -> str:
     yield environ.get('B2_TEST_ENVIRONMENT', 'production')
 
 
 @pytest.fixture(scope='function')
 def bucket(b2_api) -> str:
-    bucket = b2_api.create_bucket()
+    try:
+        bucket = b2_api.create_bucket()
+    except BadRequest as e:
+        if e.code != 'too_many_buckets':
+            raise
+        num_buckets = b2_api.count_and_print_buckets()
+        print('current number of buckets:', num_buckets)
+        raise
     yield bucket
     with contextlib.suppress(BucketIdNotFound):
         b2_api.clean_bucket(bucket)
 
 
 @pytest.fixture(scope='function')
 def bucket_name(bucket) -> str:
@@ -123,25 +131,38 @@
     yield Api(
         application_key_id, application_key, realm, GENERAL_BUCKET_NAME_PREFIX,
         this_run_bucket_name_prefix
     )
 
 
 @pytest.fixture(scope='module')
-def b2_tool(
+def global_b2_tool(
     request, application_key_id, application_key, realm, this_run_bucket_name_prefix
 ) -> CommandLine:
     tool = CommandLine(
         request.config.getoption('--sut'),
         application_key_id,
         application_key,
         realm,
         this_run_bucket_name_prefix,
     )
     tool.reauthorize(check_key_capabilities=True)  # reauthorize for the first time (with check)
     return tool
 
 
-@pytest.fixture(scope='function', autouse=True)
-def auto_reauthorize(request, b2_tool):
-    """ Automatically reauthorize for each test (without check) """
-    b2_tool.reauthorize(check_key_capabilities=False)
+@pytest.fixture(scope='function')
+def b2_tool(global_b2_tool):
+    """Automatically reauthorized b2_tool for each test (without check)"""
+    global_b2_tool.reauthorize(check_key_capabilities=False)
+    return global_b2_tool
+
+
+SECRET_FIXTURES = {'application_key', 'application_key_id'}
+
+
+def pytest_collection_modifyitems(items):
+    """
+    Add 'require_secrets' marker to all tests that use secrets.
+    """
+    for item in items:
+        if SECRET_FIXTURES & set(getattr(item, 'fixturenames', ())):
+            item.add_marker('require_secrets')
```

### Comparing `b2-3.8.0/test/integration/helpers.py` & `b2-3.9.0/test/integration/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,39 +5,44 @@
 # Copyright 2022 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
 
 import json
+import logging
 import os
 import platform
 import random
 import re
 import shutil
 import string
 import subprocess
 import sys
 import threading
+import time
 
 from dataclasses import dataclass
 from datetime import datetime
 from os import environ, linesep, path
 from pathlib import Path
 from tempfile import gettempdir, mkdtemp
 from typing import List, Optional, Union
 
 import backoff
+import pytest
 
 from b2sdk._v3.exception import BucketIdNotFound as v3BucketIdNotFound
 from b2sdk.v2 import ALL_CAPABILITIES, NO_RETENTION_FILE_SETTING, B2Api, Bucket, EncryptionAlgorithm, EncryptionKey, EncryptionMode, EncryptionSetting, InMemoryAccountInfo, InMemoryCache, LegalHold, RetentionMode, SqliteAccountInfo, fix_windows_path_limit
 from b2sdk.v2.exception import BucketIdNotFound, DuplicateBucketName, FileNotPresent, TooManyRequests
 
 from b2.console_tool import Command, current_time_millis
 
+logger = logging.getLogger(__name__)
+
 BUCKET_CLEANUP_PERIOD_MILLIS = 0
 ONE_HOUR_MILLIS = 60 * 60 * 1000
 ONE_DAY_MILLIS = ONE_HOUR_MILLIS * 24
 
 BUCKET_NAME_LENGTH = 50
 BUCKET_NAME_CHARS = string.ascii_letters + string.digits + '-'
 BUCKET_CREATED_AT_MILLIS = 'created_at_millis'
@@ -54,17 +59,41 @@
 )
 SSE_C_AES_2 = EncryptionSetting(
     mode=EncryptionMode.SSE_C,
     algorithm=EncryptionAlgorithm.AES256,
     key=EncryptionKey(secret=os.urandom(32), key_id='another-user-generated-key-id')
 )
 
+RNG_SEED = '_'.join(
+    [
+        os.getenv('GITHUB_REPOSITORY', ''),
+        os.getenv('GITHUB_SHA', ''),
+        os.getenv('GITHUB_RUN_ID', ''),
+        os.getenv('GITHUB_RUN_ATTEMPT', ''),
+        os.getenv('GITHUB_JOB', ''),
+        os.getenv('GITHUB_ACTION', ''),
+        str(os.getpid()),  # for local runs with xdist
+        str(time.time()),
+    ]
+)
+
+RNG = random.Random(RNG_SEED)
+
+RNG_COUNTER = 0
+
 
 def bucket_name_part(length: int) -> str:
-    return ''.join(random.choice(BUCKET_NAME_CHARS) for _ in range(length))
+    assert length >= 1
+    global RNG_COUNTER
+    RNG_COUNTER += 1
+    name_part = ''.join(RNG.choice(BUCKET_NAME_CHARS) for _ in range(length))
+    logger.info('RNG_SEED: %s', RNG_SEED)
+    logger.info('RNG_COUNTER: %i, length: %i', RNG_COUNTER, length)
+    logger.info('name_part: %s', name_part)
+    return name_part
 
 
 @dataclass
 class Api:
     account_id: str
     application_key: str
     realm: str
@@ -74,14 +103,17 @@
     api: B2Api = None
 
     def __post_init__(self):
         info = InMemoryAccountInfo()
         cache = InMemoryCache()
         self.api = B2Api(info, cache=cache)
         self.api.authorize_account(self.realm, self.account_id, self.application_key)
+        assert BUCKET_NAME_LENGTH - len(
+            self.this_run_bucket_name_prefix
+        ) > 5, self.this_run_bucket_name_prefix
 
     def create_bucket(self) -> Bucket:
         for _ in range(10):
             bucket_name = self.this_run_bucket_name_prefix + bucket_name_part(
                 BUCKET_NAME_LENGTH - len(self.this_run_bucket_name_prefix)
             )
             print('Creating bucket:', bucket_name)
@@ -304,27 +336,28 @@
     Establish config for environment variable test.
     Copy the B2 credential file and rename the existing copy
     """
     ENV_VAR = 'B2_ACCOUNT_INFO'
 
     def __init__(self, account_info_file_name: str):
         self.account_info_file_name = account_info_file_name
+        self.suffix = ''.join(RNG.choice('abcdefghijklmnopqrstuvwxyz0123456789') for _ in range(7))
 
     def __enter__(self):
         src = self.account_info_file_name
         dst = path.join(gettempdir(), 'b2_account_info')
         shutil.copyfile(src, dst)
-        shutil.move(src, src + '.bkup')
+        shutil.move(src, src + self.suffix)
         environ[self.ENV_VAR] = dst
         return dst
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         os.remove(environ.get(self.ENV_VAR))
         fname = self.account_info_file_name
-        shutil.move(fname + '.bkup', fname)
+        shutil.move(fname + self.suffix, fname)
         if environ.get(self.ENV_VAR) is not None:
             del environ[self.ENV_VAR]
 
 
 def should_equal(expected, actual):
     print('  expected:')
     print_json_indented(expected)
@@ -479,7 +512,14 @@
     if isinstance(path, Path):
         path = str(path)
     os.utime(path, (os.path.getatime(path), time / 1000))
 
 
 def random_hex(length):
     return ''.join(random.choice('0123456789abcdef') for _ in range(length))
+
+
+def skip_on_windows(*args, reason='Not supported on Windows', **kwargs):
+    return pytest.mark.skipif(
+        platform.system() == 'Windows',
+        reason=reason,
+    )(*args, **kwargs)
```

### Comparing `b2-3.8.0/test/integration/test_autocomplete.py` & `b2-3.9.0/test/integration/test_autocomplete.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,38 +5,32 @@
 # Copyright 2023 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
 
 import os
-import platform
 
 import pexpect
 import pytest
 
-TIMEOUT = 10
+from test.integration.helpers import skip_on_windows
+
+TIMEOUT = 20  # CI can be slow at times
 
 BASHRC_CONTENT = """\
 # ~/.bashrc dummy file
 
 echo "Just testing if we don't replace existing script" > /dev/null
 # >>> just a test section >>>
 # regardless what is in there already
 # <<< just a test section <<<
 """
 
 
-def skip_on_windows(f):
-    return pytest.mark.skipif(
-        platform.system() == 'Windows',
-        reason='Autocomplete is not supported on Windows',
-    )(f)
-
-
 @pytest.fixture(scope="session")
 def homedir(tmp_path_factory):
     yield tmp_path_factory.mktemp("test_homedir")
 
 
 @pytest.fixture(scope="session")
 def bashrc(homedir):
@@ -44,22 +38,23 @@
     bashrc_path.write_text(BASHRC_CONTENT)
     yield bashrc_path
 
 
 @pytest.fixture(scope="module")
 def env(homedir, monkey_patch):
     monkey_patch.setenv('HOME', str(homedir))
+    monkey_patch.setenv('SHELL', "/bin/bash")  # fix for running under github actions
     yield os.environ
 
 
 @pytest.fixture(scope="module")
 def autocomplete_installed(env, homedir, bashrc):
     shell = pexpect.spawn('bash -i -c "b2 install-autocomplete"', env=env)
     try:
-        shell.expect_exact('Autocomplete installed for bash', timeout=TIMEOUT)
+        shell.expect_exact('Autocomplete successfully installed for bash', timeout=TIMEOUT)
     finally:
         shell.close()
     shell.wait()
     assert (homedir / '.bash_completion.d' / 'b2').is_file()
     assert bashrc.read_text().startswith(BASHRC_CONTENT)
```

### Comparing `b2-3.8.0/test/integration/test_b2_command_line.py` & `b2-3.9.0/test/integration/test_b2_command_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -1461,43 +1461,43 @@
 def test_license(b2_tool, with_packages):
     license_text = b2_tool.should_succeed(
         ['license'] + (['--with-packages'] if with_packages else [])
     )
 
     if with_packages:
         full_license_re = re.compile(
-            r'Licenses of all modules used by b2, shipped with it in binary form:\r?\n'
+            r'Licenses of all modules used by b2(\.EXE)?, shipped with it in binary form:\r?\n'
             r'\+-*\+-*\+\r?\n'
             r'\|\s*Module name\s*\|\s*License text\s*\|\r?\n'
             r'.*'
             r'\+-*\+-*\+\r?\n', re.MULTILINE + re.DOTALL
         )
         full_license_text = next(full_license_re.finditer(license_text), None)
-        assert full_license_text
+        assert full_license_text, license_text
         assert len(
             full_license_text.group(0)
         ) > 140_000  # we should know if the length of this block changes dramatically
         # Note that GitHub CI adds additional packages:
         # 'colorlog', 'virtualenv', 'nox', 'packaging', 'argcomplete', 'filelock'
         # that sum up to around 50k characters. Tests ran from docker image are unaffected.
 
         license_summary_re = re.compile(
-            r'Summary of all modules used by b2, shipped with it in binary form:\r?\n'
+            r'Summary of all modules used by b2(\.EXE)?, shipped with it in binary form:\r?\n'
             r'\+-*\+-*\+-*\+-*\+-*\+\r?\n'
             r'\|\s*Module name\s*\|\s*Version\s*\|\s*License\s*\|\s*Author\s*\|\s*URL\s*\|\r?\n'
             r'.*'
             r'\+-*\+-*\+-*\+-*\+-*\+\r?\n', re.MULTILINE + re.DOTALL
         )
         license_summary_text = next(license_summary_re.finditer(license_text), None)
-        assert license_summary_text
+        assert license_summary_text, license_text
         assert len(
             license_summary_text.group(0)
         ) > 6_500  # we should know if the length of this block changes dramatically
 
-    assert """b2 license:
+    assert """ license:
 Backblaze wants developers and organization to copy and re-use our
 code examples, so we make the samples available by several different
 licenses.  One option is the MIT license (below).  Other options are
 available here:
 
     https://www.backblaze.com/using_b2_code.html
 
@@ -1518,15 +1518,15 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.""" in license_text.replace(os.linesep, '\n')
+SOFTWARE.""" in license_text.replace(os.linesep, '\n'), repr(license_text[-2000:])
 
 
 def test_file_lock(b2_tool, application_key_id, application_key, b2_api):
     lock_disabled_bucket_name = b2_tool.generate_bucket_name()
     b2_tool.should_succeed(
         [
             'create-bucket',
@@ -2508,7 +2508,42 @@
         assert expected_file_retention == actual_file_retention
     if legal_hold is not None:
         if file_version['legalHold'] == 'unknown':
             actual_legal_hold = LegalHold.UNKNOWN
         else:
             actual_legal_hold = LegalHold.from_string_or_none(file_version['legalHold'])
         assert legal_hold == actual_legal_hold
+
+
+def test_cut(b2_tool, bucket_name):
+    file_to_upload = 'README.md'
+    file_data = read_file(file_to_upload)
+    cut = 12345
+    cut_printable = '1970-01-01  00:00:12'
+    args = [
+        'upload-file',
+        '--noProgress',
+        '--custom-upload-time',
+        str(cut),
+        '--quiet',
+        bucket_name,
+        file_to_upload,
+        'a',
+    ]
+    succeeded, stdout = b2_tool.run_command(args)
+    if not succeeded:
+        b2_tool.should_fail(args, 'custom_timestamp_not_allowed')
+    else:
+        # file_id, action, date, time, size(, replication), name
+        b2_tool.should_succeed(
+            ['ls', '--long', bucket_name], '^4_z.*  upload  %s +%s  a' % (
+                cut_printable,
+                len(file_data),
+            )
+        )
+        # file_id, action, date, time, size(, replication), name
+        b2_tool.should_succeed(
+            ['ls', '--long', '--replication', bucket_name], '^4_z.*  upload  %s +%s  -  a' % (
+                cut_printable,
+                len(file_data),
+            )
+        )
```

### Comparing `b2-3.8.0/test/static/test_licenses.py` & `b2-3.9.0/test/static/test_licenses.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 from itertools import islice
 
 import pytest
 
 
 def test_files_headers():
     for file in glob('**/*.py', recursive=True):
+        if file.startswith('build/'):
+            # built files naturally have a different file path than source files
+            continue
         with open(file) as fd:
             file = file.replace(
                 '\\', '/'
             )  # glob('**/*.py') on Windows returns "b2\console_tool.py" (wrong slash)
             head = ''.join(islice(fd, 9))
             if 'All Rights Reserved' not in head:
                 pytest.fail('Missing "All Rights Reserved" in the header in: {}'.format(file))
```

### Comparing `b2-3.8.0/test/unit/_cli/test_autocomplete_install.py` & `b2-3.9.0/test/unit/_cli/test_autocomplete_install.py`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/test/unit/test_arg_parser.py` & `b2-3.9.0/test/unit/test_arg_parser.py`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/test/unit/test_base.py` & `b2-3.9.0/test/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/test/unit/test_console_tool.py` & `b2-3.9.0/test/unit/test_console_tool.py`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/test/unit/test_copy.py` & `b2-3.9.0/test/unit/test_copy.py`

 * *Files identical despite different names*

### Comparing `b2-3.8.0/test/unit/test_represent_file_metadata.py` & `b2-3.9.0/test/unit/test_represent_file_metadata.py`

 * *Files identical despite different names*

